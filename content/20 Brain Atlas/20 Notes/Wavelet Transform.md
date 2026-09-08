---
type: note
title: "Wavelet Transform"
subject: "Computer Vision"
created: 2026-09-07
prerequisites:
  - "[[Convolution]]"
  - "[[Calculus for Machine Learning]]"
tags:
  - computer-vision
  - image-processing
  - signal-processing
  - mathematics
---

Transformasi Wavelet (*Wavelet Transform*) adalah teknik analisis sinyal dan citra yang mendekomposisi data ke dalam komponen skala dan frekuensi yang terlokalisasi secara spasial secara simultan. Berbeda dengan Transformasi Fourier yang memetakan citra murni ke dalam fungsi sinus/kosinus dengan bentangan spasial tak hingga (sehingga kehilangan informasi lokasi pasti), wavelet menggunakan fungsi gelombang mini (*wavelet*) berdurasi terbatas yang dapat digeser (*translated*) dan diskalakan (*scaled*). Dalam *image processing* dan *computer vision*, sifat pelokalan ruang-frekuensi (*spatial-frequency localization*) dan analisis multi-resolusi (*multi-resolution analysis*) ini menjadikannya fondasi esensial untuk kompresi citra berbasis subband (JPEG 2000), penghilangan derau adaptif (*wavelet denoising*), deteksi tepi multi-arah, hingga ekstraksi fitur klasik (Haar cascades) dan modern (Wavelet CNNs).

## Masalah Mendasar: Mengapa Fourier Gagal Melokalisasi Fitur Citra?

Citra dunia nyata bersifat **non-stasioner**: informasi penting seperti tepi objek (*edges*), sudut (*corners*), dan tekstur adalah fenomena frekuensi tinggi yang terlokalisasi secara ketat pada koordinat $(x, y)$ tertentu, sementara area latar belakang langit atau dinding datar didominasi oleh variasi frekuensi rendah yang tersebar luas.

Ketika Transformasi Fourier 2D diaplikasikan pada citra:
1. Basis Fourier adalah fungsi sinusoidal $e^{j(u x + v y)}$ yang memiliki bentangan spasial tak berhingga ($-\infty$ hingga $+\infty$).
2. Koefisien Fourier memberi tahu **seberapa banyak** frekuensi $(u, v)$ hadir di dalam citra, namun **kehilangan total informasi di mana** frekuensi tersebut berada dalam ruang piksel.
3. Mengubah satu piksel saja pada koordinat $(x_0, y_0)$ akan mengubah nilai seluruh spektrum Fourier citra.

```
Domain Spasial (Piksel): Tahu LOKASI (x, y) presisi, tapi TIDAK TAHU frekuensi.
Domain Fourier (FFT):    Tahu FREKUENSI (u, v) presisi, tapi HILANG informasi lokasi.
Domain Wavelet (DWT):    Tahu FREKUENSI sekaligus LOKASI SPASIAL secara simultan.
```

Pendekatan *Short-Time Fourier Transform* (STFT) mencoba memotong citra dengan jendela (*window*) spasial berukuran tetap. Namun, teorema ketidakpastian Heisenberg-Gabor menetapkan batas fundamental: jendela tetap menghasilkan trade-off kaku yang tidak efisien—jika jendela sempit, resolusi frekuensi buruk; jika jendela lebar, resolusi lokasi spasial hilang.

---

## Anatomi Wavelet: Gelombang Mini Terdilatasi dan Tertranslasi

Kata *wavelet* secara harfiah berarti "gelombang kecil". Secara matematis, suatu fungsi $\psi(t)$ disebut *mother wavelet* jika memenuhi syarat keterbagian (*admissibility condition*), yang mensyaratkan rata-rata fungsi bernilai nol (osilasi teredam):

$$
\int_{-\infty}^{\infty} \psi(t) \, dt = 0
$$

Di mana:
- $\psi(t)$ adalah fungsi *mother wavelet* kontinu dalam domain waktu/ruang.

Keluarga basis wavelet dibentuk melalui dua operasi geometri:
1. **Skalasi / Dilatasi ($a$):** Melebarkan atau menyempitkan gelombang untuk mengukur frekuensi rendah vs frekuensi tinggi.
2. **Translasi / Pergeseran ($b$):** Menggeser posisi pusat gelombang ke koordinat spasial tertentu.

$$
\psi_{a, b}(t) = \frac{1}{\sqrt{|a|}} \psi\left(\frac{t - b}{a}\right)
$$

Di mana:
- $a \in \mathbb{R}^+$ adalah parameter skala (*dilation factor*). Nilai $a$ kecil merepresentasikan frekuensi tinggi (gelombang mengkerut/sempit), sedangkan nilai $a$ besar merepresentasikan frekuensi rendah (gelombang melebar).
- $b \in \mathbb{R}$ adalah parameter posisi translasi (*shift factor*).
- $\frac{1}{\sqrt{|a|}}$ adalah faktor normalisasi energi agar energi fungsi wavelet tetap konstan di setiap skala.

### Analisis Multi-Resolusi (MRA): Resolusi Fleksibel
Prinsip kunci wavelet adalah adaptasi dinamis:
- **Frekuensi Tinggi (Tepi/Transisi Tajam):** Wavelet menyempit secara spasial $\rightarrow$ resolusi spasial sangat tinggi, resolusi frekuensi rendah. Ini ideal karena kita ingin tahu *koordinat pasti* di mana sebuah tepi terjadi.
- **Frekuensi Rendah (Gradien Halus/Latar Belakang):** Wavelet melebar secara spasial $\rightarrow$ resolusi frekuensi tinggi, resolusi spasial rendah. Kita peduli pola warna umum, bukan lokasi presisi piksel per piksel.

---

## Transformasi Wavelet Diskrit 2D (2D-DWT) pada Citra

Pada citra digital berukuran $M \times N$, operasi dilakukan menggunakan *Discrete Wavelet Transform* (DWT) dyadik, di mana skala berubah dalam kelipatan pangkat dua ($a = 2^j$) dan translasi dalam langkah integer ($b = k \cdot 2^j$).

Dekomposisi citra 2D bersifat *separable* dan diimplementasikan melalui pasangan filter komplementer (*filter banks*):
- **Filter Lolos-Rendah (*Low-pass Filter*, $L$ atau $\phi$ / scaling function):** Mengambil rata-rata lokal (informasi aproksimasi kasar).
- **Filter Lolos-Tinggi (*High-pass Filter*, $H$ atau $\psi$ / wavelet function):** Mengambil perbedaan lokal (informasi detail/tepi).

### Mekanisme 1-Level Dekomposisi 2D
Proses filtering dilakukan bergantian pada baris dan kolom citra, diikuti dengan *downsampling* faktor 2 ($\downarrow 2$):

```
Citra Input I(x,y)
    ├── Filter Baris Low-Pass (L) ──> [Downsample Kolom ↓2]
    │       ├── Filter Kolom Low-Pass (L)  ──> [Downsample Baris ↓2] ──> Subband LL (Aproksimasi)
    │       └── Filter Kolom High-Pass (H) ──> [Downsample Baris ↓2] ──> Subband LH (Tepi Horisontal)
    │
    └── Filter Baris High-Pass (H) ──> [Downsample Kolom ↓2]
            ├── Filter Kolom Low-Pass (L)  ──> [Downsample Baris ↓2] ──> Subband HL (Tepi Vertikal)
            └── Filter Kolom High-Pass (H) ──> [Downsample Baris ↓2] ──> Subband HH (Tepi Diagonal)
```

Hasil satu tingkat dekomposisi menghasilkan 4 subband berukuran seperempat dari citra asli:

| Subband | Pasangan Filter (Baris $\times$ Kolom) | Karakteristik Informasi |
| :--- | :--- | :--- |
| **$LL$** | Low-Pass $\times$ Low-Pass | **Approximation:** Versi thumbnail halus dari citra asli. Mengandung sebagian besar energi visual sinyal. |
| **$LH$** | Low-Pass $\times$ High-Pass | **Horizontal Detail:** Menyorot perubahan intensitas tajam pada arah vertikal (mendeteksi garis/tepi horizontal). |
| **$HL$** | High-Pass $\times$ Low-Pass | **Vertical Detail:** Menyorot perubahan intensitas tajam pada arah horizontal (mendeteksi garis/tepi vertikal). |
| **$HH$** | High-Pass $\times$ High-Pass | **Diagonal Detail:** Menyorot sudut (*corners*), tekstur tajam, dan struktur miring $45^\circ$. |

```
+---------------+---------------+
|               |               |
|      LL       |      HL       |
| (Aproksimasi) | (Tepi Vertikal|
|               |               |
+---------------+---------------+
|               |               |
|      LH       |      HH       |
| (Tepi Horiz.) | (Tepi Diag.)  |
|               |               |
+---------------+---------------+
```

### Dekomposisi Piramida Mallat (Multi-Level)
Untuk analisis skala yang lebih dalam, subband $LL$ didekomposisi kembali secara rekursif menjadi 4 subband tingkat berikutnya ($LL_2, LH_2, HL_2, HH_2$), membentuk representasi piramida resolusi bertingkat (*Mallat's pyramidal algorithm*).

---

## Contoh Perhitungan Nyata: Dekomposisi Haar Wavelet 2D

Haar Wavelet adalah wavelet paling sederhana dan ortogonal. 
Filter 1D Haar untuk input diskret dua titik $\begin{bmatrix} x_1 & x_2 \end{bmatrix}$ adalah:
- Nilai rata-rata (*scaling/low-pass*): $s = \frac{x_1 + x_2}{\sqrt{2}}$ (atau $\frac{x_1 + x_2}{2}$ tanpa normalisasi energi ortonormal).
- Nilai selisih (*wavelet/high-pass*): $d = \frac{x_1 - x_2}{\sqrt{2}}$ (atau $\frac{x_1 - x_2}{2}$).

Misalkan terdapat blok citra berukuran $2 \times 2$:

$$
I = \begin{bmatrix} 120 & 140 \\ 40 & 60 \end{bmatrix}
$$

Kita terapkan dekomposisi Haar standar (menggunakan skala pembagi 2 untuk kemudahan perhitungan mental):

1. **Transformasi pada setiap baris:**
   - Baris 1: $\begin{bmatrix} 120 & 140 \end{bmatrix}$
     - Rata-rata $L$: $\frac{120 + 140}{2} = 130$
     - Selisih $H$: $\frac{120 - 140}{2} = -10$
   - Baris 2: $\begin{bmatrix} 40 & 60 \end{bmatrix}$
     - Rata-rata $L$: $\frac{40 + 60}{2} = 50$
     - Selisih $H$: $\frac{40 - 60}{2} = -10$

   Matriks sementara setelah filter baris:
   $$
   I_{row} = \begin{bmatrix} 130 & -10 \\ 50 & -10 \end{bmatrix}
   $$

2. **Transformasi pada setiap kolom dari $I_{row}$:**
   - Kolom 1 (Kolom $L$): $\begin{bmatrix} 130 \\ 50 \end{bmatrix}$
     - Rata-rata kolom $\rightarrow LL$: $\frac{130 + 50}{2} = 90$
     - Selisih kolom $\rightarrow LH$: $\frac{130 - 50}{2} = 40$
   - Kolom 2 (Kolom $H$): $\begin{bmatrix} -10 \\ -10 \end{bmatrix}$
     - Rata-rata kolom $\rightarrow HL$: $\frac{-10 + (-10)}{2} = -10$
     - Selisih kolom $\rightarrow HH$: $\frac{-10 - (-10)}{2} = 0$

Matriks koefisien subband 2D-DWT:

$$
\text{DWT}(I) = \begin{bmatrix} LL & HL \\ LH & HH \end{bmatrix} = \begin{bmatrix} 90 & -10 \\ 40 & 0 \end{bmatrix}
$$

**Interpretasi Hasil:**
- $LL = 90$: Intensitas rata-rata keseluruhan patch citra.
- $LH = 40$: Nilai besar positif menunjukkan adanya transisi tajam intensitas dari atas ke bawah (garis tepi horizontal kuat antara baris atas bernilai ~130 dan baris bawah bernilai ~50).
- $HL = -10$: Kontras kiri-kanan yang moderat.
- $HH = 0$: Tidak ada komponen diagonal karena perubahan intensitas horizontal di baris atas sama persis dengan baris bawah.

---

## Aplikasi Inti dalam Image Processing & Computer Vision

### 1. Kompresi Citra: Mengapa JPEG 2000 Memilih Wavelet Menggantikan DCT?
Format JPEG standar menggunakan *Discrete Cosine Transform* (DCT) berbasis blok $8 \times 8$ piksel. Pada rasio kompresi tinggi, batas antar-blok patah, memunculkan distorsi kotak-kotak (*blocking artifacts*).

JPEG 2000 menggunakan 2D-DWT (filter biorthogonal Daubechies 9/7 untuk *lossy* dan Le Gall 5/3 untuk *lossless*):
- Transformasi diterapkan pada seluruh citra secara utuh (*tile-less/full image*), sehingga **tidak pernah muncul blocking artifacts**.
- Mayoritas koefisien di subband detail ($LH, HL, HH$) bernilai mendekati nol (*energy compaction* tinggi), sehingga dapat dikompresi sangat padat via EBCOT (*Embedded Block Coding with Optimal Truncation*).
- Mendukung *progressive transmission*: klien dapat mengunduh subband resolusi rendah ($LL$) terlebih dahulu untuk preview instan, lalu memuat subband detail seiring waktu.

### 2. Denoising Citra: Wavelet Shrinkage (Thresholding)
Derau putih Gaussian (*additive white Gaussian noise*) tersebar secara acak di seluruh piksel citra. Dalam domain wavelet:
- Sinyal citra terorganisir menghasilkan koefisien bernilai **sangat besar** pada lokasi tepi di subband detail.
- Derau tersebar merata sebagai koefisien beramplitudo **sangat kecil**.

Algoritma Donoho-Johnstone (VisuShrink/BayesShrink) melakukan pembersihan dengan menetapkan ambang batas $\lambda$:
1. Hitung ambang batas universal:
   $$
   \lambda = \sigma \sqrt{2 \ln N}
   $$
   Di mana:
   - $\lambda$ adalah nilai ambang batas (*threshold*).
   - $\sigma$ adalah estimasi deviasi standar derau (biasanya diestimasi dari median mutlak subband $HH_1$: $\sigma = \frac{\text{median}(|HH_1|)}{0.6745}$).
   - $N$ adalah jumlah total piksel citra.
2. Terapkan fungsi *soft-thresholding*:
   $$
   \eta_\lambda(w) = \text{sign}(w) \cdot \max(0, |w| - \lambda)
   $$
   Di mana:
   - $\eta_\lambda(w)$ adalah koefisien wavelet setelah ambang batas.
   - $w$ adalah koefisien wavelet asli sebelum ambang batas.
   - $\text{sign}(w)$ adalah tanda aljabar ($+1, -1,$ atau $0$) dari koefisien.
3. Rekonstruksi citra via Inverse DWT (IDWT). Hasilnya: derau tereduksi signifikan dengan struktur ketajaman tepi yang tetap utuh (*edge-preserving denoising*).

### 3. Ekstraksi Fitur & Deteksi Objek Klasik
- **Haar-like Features & Viola-Jones Face Detector:**
  Detektor wajah legendaris Viola-Jones (2001) menggunakan rectangular filters yang merupakan aproksimasi langsung dari fungsi basis Haar wavelet. Dengan memanfaatkan *Integral Image*, fitur Haar dapat dihitung dalam waktu konstan $\mathcal{O}(1)$ per jendela, memungkinkan deteksi wajah *real-time* pertama di dunia komputasi visual.
- **Gabor Wavelets (Gabor Filters):**
  Fungsi sinus yang dimodulasi oleh amplop Gaussian. Gabor wavelet secara matematis memodelkan fungsi transfer sel sederhana (*simple cells*) pada korteks visual primer (area V1) mamalia. Digunakan secara luas untuk analisis tekstur, segmentasi sidik jari, dan verifikasi biometrik iris mata.

### 4. Era Modern: Wavelet dalam Deep Learning & Computer Vision
Dalam era *Deep Learning*, wavelet kembali menjadi topik riset penting untuk mengatasi kelemahan operasi standar CNN:
- **Wavelet Pooling / Wavelet Downsampling:** Operasi *Max-Pooling* atau *Strided Convolution* konvensional sering membuang informasi detail dan memicu fenomena *aliasing* frekuensi tinggi (pelanggaran teorema Nyquist-Shannon). Mengganti pooling dengan DWT memisahkan fitur aproksimasi dan detail tanpa membuang informasi (operasi DWT bersifat bijektif dan *lossless*).
- **Invertible Neural Networks (INNs):** Arsitektur pemulihan citra (*super-resolution*, *image inpainting*, *deraining*) seperti MWCNN (*Multi-level Wavelet CNN*) menggunakan DWT pada *encoder* untuk menjaga aliran informasi gradien dan IDWT pada *decoder* untuk sintesis citra beresolusi tinggi tanpa artifak blur.

---

## Perbandingan Ringkas: Spasial vs. Fourier vs. Wavelet

| Dimensi Evaluasi | Domain Spasial (Piksel) | Transformasi Fourier (FFT) | Transformasi Wavelet (DWT) |
| :--- | :--- | :--- | :--- |
| **Fungsi Basis** | Titik diskret Delta Dirac $\delta(x, y)$ | Sinusoidal murni $e^{j(ux + vy)}$ | Wavelet terlokalisasi $\psi_{a,b}(x, y)$ |
| **Bentangan Basis** | Sangat sempit (1 piksel) | Tak berhingga ($-\infty \dots \infty$) | Kompak (*compact support*) |
| **Lokasi Spasial** | Presisi mutlak | Hilang sama sekali | Terjaga di semua level skala |
| **Lokasi Frekuensi** | Hilang sama sekali | Presisi mutlak | Terbagi adaptif per pita oktaf |
| **Penanganan Fitur Tepi** | Terbaca lokal, rentan derau | Tersebar ke seluruh fase | Terisolasi rapi di subband $LH, HL, HH$ |
| **Kompleksitas Komputasi** | $\mathcal{O}(1)$ (akses langsung) | $\mathcal{O}(N \log N)$ (FFT) | $\mathcal{O}(N)$ (Filter bank piramida) |

---

> [!abstract]- Quick Reference
> 
> ### Formula & Definisi Utama
> 
> 1. **Kondisi Admisibilitas Mother Wavelet:**
>    $$
>    \int_{-\infty}^{\infty} \psi(t) \, dt = 0
>    $$
>    Di mana $\psi(t)$ adalah fungsi *mother wavelet*.
> 
> 2. **Fungsi Wavelet Terdilatasi & Tertranslasi:**
>    $$
>    \psi_{a, b}(t) = \frac{1}{\sqrt{|a|}} \psi\left(\frac{t - b}{a}\right)
>    $$
>    Di mana $a$ adalah skala dilatasi, $b$ adalah posisi pergeseran translasi.
> 
> 3. **Subband 2D-DWT:**
>    - $LL = \text{Low-pass Row} \times \text{Low-pass Column}$ (Aproksimasi / Thumbnail)
>    - $LH = \text{Low-pass Row} \times \text{High-pass Column}$ (Tepi Horizontal)
>    - $HL = \text{High-pass Row} \times \text{Low-pass Column}$ (Tepi Vertikal)
>    - $HH = \text{High-pass Row} \times \text{High-pass Column}$ (Sudut & Diagonal)
> 
> 4. **Kompleksitas Algoritma:**
>    - Dekomposisi DWT Piramida Mallat: $\mathcal{O}(N)$, lebih cepat dari FFT ($\mathcal{O}(N \log N)$).

---

> [!question]- Practice
> 
> **Pertanyaan 1:** Diberikan citra biner hitam-putih ukuran $4 \times 4$ berikut, di mana angka 0 adalah hitam dan 100 adalah putih:
> $$
> I = \begin{bmatrix} 0 & 0 & 100 & 100 \\ 0 & 0 & 100 & 100 \\ 0 & 0 & 100 & 100 \\ 0 & 0 & 100 & 100 \end{bmatrix}
> $$
> Citra ini memiliki tepi vertikal tajam persis di tengah. Jika kita melakukan dekomposisi Haar DWT 1-level, subband manakah ($LL, LH, HL, HH$) yang koefisien detailnya akan memiliki nilai absolut non-nol paling dominan?
> 
> > [!check]- Answer
> > **Subband $HL$ (High-pass Baris $\times$ Low-pass Kolom).**
> > 
> > **Penjelasan:**
> > Tepi vertikal menunjukkan bahwa intensitas konstan sepanjang kolom (vertikal), namun berubah drastis sepanjang baris (horizontal):
> > 1. Filter baris *High-pass* ($H$) menghitung selisih horizontal: $\frac{0 - 0}{2} = 0$, tetapi pada transisi tengah $\frac{0 - 100}{2} = -50$. Ini menghasilkan respons selisih yang kuat.
> > 2. Filter kolom *Low-pass* ($L$) menghitung rata-rata vertikal yang mempertahankan nilai respons tersebut karena piksel di atas dan di bawahnya identik.
> > 3. Sebaliknya, subband $LH$ (perbedaan vertikal) akan bernilai 0 di seluruh elemen karena tidak ada perubahan intensitas pada arah vertikal sama sekali. Begitu pula $HH$ akan bernilai 0.
> 
> ---
> 
> **Pertanyaan 2:** Mengapa *downsampling* ($\downarrow 2$) aman dilakukan setelah filtering tanpa melanggar batas aliasing Nyquist?
> 
> > [!check]- Answer
> > Karena filter *Low-pass* ($L$) dan *High-pass* ($H$) bertindak sebagai *half-band filter*. Filter *low-pass* telah memotong frekuensi di atas setengah pita Nyquist (sehingga bandwidth sinyal berkurang menjadi setengahnya). Sementara itu, filter *high-pass* menggeser dan mengisolasi setengah spektrum frekuensi atas ke pita dasar. Sinyal yang telah dibatasi bandwidthnya menjadi $\frac{B}{2}$ dapat disampling dengan separuh frekuensi awal tanpa kehilangan informasi (*lossless critical sampling*).

---

> [!info]- Going Deeper
> 
> - **Wavelet Biorthogonal (Daubechies 9/7):** Pelajari bagaimana simetri fase linear dipertahankan dalam kompresi citra tanpa distorsi fase rekursif melalui *biorthogonal filter banks*.
> - **Stationary Wavelet Transform (SWT / Undecimated DWT):** Menghilangkan tahap *downsampling* untuk menghasilkan representasi yang invarian terhadap pergeseran (*shift-invariant*), sangat berguna dalam segmentasi citra medis dan restorasi citra seismik.
> - **Scattering Transforms (Stéphane Mallat):** Menghubungkan wavelet dengan arsitektur *deep learning* convolutional secara matematis formal, di mana filter bank wavelet dikombinasikan dengan fungsi non-linearitas modulus ($|\cdot|$) untuk membentuk ekstraktor fitur citra yang terbukti invarian terhadap translasi dan stabil terhadap deformasi difeomorfisme.
