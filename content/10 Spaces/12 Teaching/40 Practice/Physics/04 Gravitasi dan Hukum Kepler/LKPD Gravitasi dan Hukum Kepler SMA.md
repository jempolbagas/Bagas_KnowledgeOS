---
title: "LKPD: Hukum Gravitasi Newton dan Hukum Kepler"
type: lkpd
subject: Physics
level: sma
target_audience: "SMA Kelas XI"
created: 2026-09-08
sources:
  - "[[Gravitasi dan Hukum Kepler SMA]]"
  - "[[Gaya dan Medan Gravitasi SMA]]"
  - "[[Energi Potensial dan Kecepatan Lepas SMA]]"
  - "[[Hukum Kepler dan Gerak Satelit SMA]]"
tags:
  - lkpd
  - lembar_kerja
  - fisika
  - sma_kelas_11
  - kurikulum_merdeka
  - gravitasi
  - hukum_kepler
  - phet
  - inkuiri
---

# Lembar Kerja Peserta Didik (LKPD): Gravitasi Newton dan Hukum Kepler 📝🪐

> [!info] Informasi Dokumen & Navigasi Cepat
> **Modul Induk:** [[Gravitasi dan Hukum Kepler SMA|🏠 Master Dashboard]] | **Materi Pendukung:** [[Gaya dan Medan Gravitasi SMA|⚡ Modul 1: Gaya & Medan]], [[Energi Potensial dan Kecepatan Lepas SMA|🚀 Modul 2: Energi & Kecepatan Lepas]], & [[Hukum Kepler dan Gerak Satelit SMA|🪐 Modul 3: Hukum Kepler & Satelit]] | **Instrumen Evaluasi:** [[Soal Gravitasi dan Hukum Kepler SMA|🎯 Paket Soal HOTS]]  
> **Jenjang / Kelas:** SMA Kelas XI (Fase F - Kurikulum Merdeka)  
> **Model Pembelajaran:** *Inquiry-Based Digital Physics Lab & Real Astronomy Data Analysis*  
> **Alokasi Waktu:** 2 Pertemuan Pembelajaran ($4 \times 45\text{ Menit}$)

---

## 👥 Identitas Peserta Didik / Kelompok
- **Nama Anggota Kelompok:**
  1. ..................................................................... (Ketua)
  2. .....................................................................
  3. .....................................................................
  4. .....................................................................
- **Kelas / No. Presensi :** XI - ....... / ............................
- **Hari / Tanggal       :** ............................................

---

## 🎯 Tujuan Pembelajaran Inkuiri
Setelah menyelesaikan rangkaian kegiatan pembelajaran ini, peserta didik mampu:
1. **Menyelidiki secara kuantitatif** hubungan ketergantungan gaya gravitasi terhadap besaran massa dan kuadrat jarak pisah antarbenda melalui laboratorium virtual *PhET Interactive Simulations*.
2. **Membuktikan Hukum Kuadrat Terbalik (*Inverse-Square Law*)** melalui analisis grafik linearisasi $F$ versus $1/r^2$ serta mengestimasi nilai konstanta gravitasi universal ($G$).
3. **Menganalisis fenomena mekanika orbit** planet dan satelit, termasuk perubahan vektor kelajuan linier di perihelion dan aphelion sesuai Hukum II Kepler.
4. **Memvalidasi Hukum III Kepler secara empiris** menggunakan data astronomi riil delapan planet di Tata Surya serta menghitung perkiraan massa Matahari ($M_{\odot}$).

---

## 💻 AKTIVITAS 1: Eksperimen Virtual — Uji Hukum Gravitasi Newton (PhET Gravity Force Lab)

### A. Persiapan dan Akses Simulasi:
1. Buka peramban (browser) di laptop atau gawai masing-masing.
2. Akses simulasi interaktif **PhET: Gravity Force Lab** melalui tautan resmi:  
   `https://phet.colorado.edu/sims/html/gravity-force-lab/latest/gravity-force-lab_all.html`
3. Pastikan fitur penampil nilai gaya (*Force Values*) dan penggaris (*Ruler*) dalam posisi aktif.

---

### B. Investigasi Bagian 1: Pengaruh Variasi Massa terhadap Gaya Gravitasi
**Langkah Kerja:**
1. Atur jarak antar-pusat massa bola ($r$) konstan pada nilai $r = 4{,}0\text{ meter}$.
2. Tetapkan massa bola 2 ($m_2$) konstan pada nilai $m_2 = 100\text{ kg}$.
3. Ubah nilai massa bola 1 ($m_1$) secara bertahap sesuai tabel berikut, lalu catat besar gaya gravitasi ($F$) yang terukur pada layar.

| Percobaan | Massa Benda 1 ($m_1$) | Massa Benda 2 ($m_2$) | Jarak Pisah ($r$) | Gaya Gravitasi ($F$) |
|:---:|:---:|:---:|:---:|:---:|
| 1 | $100\text{ kg}$ | $100\text{ kg}$ | $4{,}0\text{ m}$ | ........................ $\times 10^{-9}\text{ N}$ |
| 2 | $200\text{ kg}$ | $100\text{ kg}$ | $4{,}0\text{ m}$ | ........................ $\times 10^{-9}\text{ N}$ |
| 3 | $300\text{ kg}$ | $100\text{ kg}$ | $4{,}0\text{ m}$ | ........................ $\times 10^{-9}\text{ N}$ |
| 4 | $400\text{ kg}$ | $100\text{ kg}$ | $4{,}0\text{ m}$ | ........................ $\times 10^{-9}\text{ N}$ |
| 5 | $500\text{ kg}$ | $100\text{ kg}$ | $4{,}0\text{ m}$ | ........................ $\times 10^{-9}\text{ N}$ |

**Pertanyaan Analisis Bagian 1:**
- Bagaimana tren perubahan nilai gaya gravitasi ($F$) ketika massa $m_1$ dilipatgandakan menjadi 2 kali dan 3 kali semula?  
  *Jawaban:* .............................................................................................................................................
- Buat kesimpulan hubungan matematis antara $F$ dengan $m_1$ dan $m_2$:  
  *Kesimpulan:* $F \propto$ .............................................................................................................................

---

### C. Investigasi Bagian 2: Pengaruh Jarak Pisah terhadap Gaya Gravitasi & Linearisasi Grafik
**Langkah Kerja:**
1. Tetapkan massa kedua bola konstan: $m_1 = 400\text{ kg}$ dan $m_2 = 400\text{ kg}$.
2. Ubah jarak pisah kedua pusat massa bola ($r$) secara bertahap mulai dari $2{,}0\text{ m}$ hingga $10{,}0\text{ m}$.
3. Catat besar gaya gravitasi ($F$), lalu hitung nilai kuadrat terbalik jarak ($\frac{1}{r^2}$).

| Percobaan | Jarak Pisah ($r$) | Jarak Kuadrat ($r^2$) | Nilai $\frac{1}{r^2}$ ($\text{m}^{-2}$) | Gaya Gravitasi Terukur ($F$) |
|:---:|:---:|:---:|:---:|:---:|
| 1 | $2{,}0\text{ m}$ | $4{,}0\text{ m}^2$ | $0{,}250\text{ m}^{-2}$ | ........................ $\text{N}$ |
| 2 | $4{,}0\text{ m}$ | $16{,}0\text{ m}^2$ | $0{,}0625\text{ m}^{-2}$ | ........................ $\text{N}$ |
| 3 | $6{,}0\text{ m}$ | $36{,}0\text{ m}^2$ | $0{,}0278\text{ m}^{-2}$ | ........................ $\text{N}$ |
| 4 | $8{,}0\text{ m}$ | $64{,}0\text{ m}^2$ | $0{,}0156\text{ m}^{-2}$ | ........................ $\text{N}$ |
| 5 | $10{,}0\text{ m}$ | $100{,}0\text{ m}^2$ | $0{,}0100\text{ m}^{-2}$ | ........................ $\text{N}$ |

**Tugas Pengolahan Data & Grafik:**
1. Gambarkan grafik hubungan antara **Gaya Gravitasi ($F$) pada sumbu-Y** terhadap **$\frac{1}{r^2}$ pada sumbu-X** pada kertas milimeter blok atau aplikasi spreadsheet!
2. Apakah grafik membentuk garis lurus linier yang memotong titik pusat $(0,0)$? Jelaskan maknanya!  
   *Penjelasan:* ........................................................................................................................................
3. Hitung gradien kemiringan garis ($k = \frac{\Delta F}{\Delta (1/r^2)}$) dari grafikmu:  
   $k = \frac{\dots\dots\dots\dots - \dots\dots\dots\dots}{\dots\dots\dots\dots - \dots\dots\dots\dots} = \dots\dots\dots\dots\dots\dots\dots\dots\dots\text{ N}\cdot\text{m}^2$
4. Karena berdasarkan Hukum Newton $F = \left(G \cdot m_1 \cdot m_2\right) \cdot \frac{1}{r^2}$, maka gradien $k = G \cdot m_1 \cdot m_2$. Hitung nilai konstanta gravitasi $G$ dari hasil eksperimenmu:  
   $$
   G_{\text{eksperimen}} = \frac{k}{m_1 \cdot m_2} = \frac{k}{400 \times 400} = \dots\dots\dots\dots\dots\dots\dots\dots\dots\text{ N}\cdot\text{m}^2/\text{kg}^2
   $$
   Bandingkan nilai $G$ eksperimenmu dengan konstanta baku Cavendish ($6{,}674 \times 10^{-11}\text{ N}\cdot\text{m}^2/\text{kg}^2$). Berapa persen galat (*error*)-nya?  
   *Persentase Error:* ..............................................................................................................................

---

## 🪐 AKTIVITAS 2: Eksplorasi Mekanika Orbit Planet & Satelit (PhET Gravity and Orbits)

### A. Akses Simulasi:
Buka simulasi **PhET: Gravity and Orbits** melalui tautan:  
`https://phet.colorado.edu/sims/html/gravity-and-orbits/latest/gravity-and-orbits_all.html`  
Pilih mode **Model** atau **To Scale**. Centang kotak: *Gravity Force*, *Velocity*, *Path*, dan *Grid*.

---

### B. Investigasi Eksperimen & Analisis Konseptual:

#### 1. Eksperimen Skenario "Mematikan Gravitasi" (Hukum Inersia Newton)
- Jalankan simulasi orbit Bumi mengelilingi Matahari.
- Saat Bumi berada pada posisi tertentu, klik tombol **"Gravity: OFF"**.
- Amati apa yang terjadi pada lintasan gerak Bumi selanjutnya!
- *Analisis:* Mengapa Bumi bergerak lurus beraturan menjauhi Matahari sesaat setelah gravitasi dimatikan? Prinsip hukum fisika apa yang mendasarinya?  
  *Jawaban:* .............................................................................................................................................

#### 2. Investigasi Hukum II Kepler pada Orbit Elips
- Pilih mode orbit komet atau perbesar eksentrisitas orbit planet.
- Amati panjang panah vektor kecepatan ($\vec{v}$) dan vektor gaya gravitasi ($\vec{F}$) saat planet bergerak mendekati Matahari (menuju perihelion) dan saat menjauhi Matahari (menuju aphelion).
- *Analisis:*  
  a. Di titik manakah panah vektor kecepatan ($\vec{v}$) berukuran paling panjang? Mengapa demikian?  
  *Jawaban:* ..........................................................................................................................................  
  b. Bagaimana arah vektor gaya tarik gravitasi terhadap arah gerak komet saat ia bergerak dari aphelion menuju perihelion? Apakah gaya tersebut mempercepat atau memperlambat komet?  
  *Jawaban:* ..........................................................................................................................................

---

## 📊 AKTIVITAS 3: Validasi Empiris Hukum III Kepler pada Delapan Planet Tata Surya

Para astronom telah mengukur jarak rata-rata ($r$) dan periode revolusi ($T$) dari seluruh planet anggota tata surya kita. Pada aktivitas ini, kelompokmu akan menguji apakah rasio $\frac{T^2}{r^3}$ benar-benar bernilai konstan bagi seluruh planet, sekaligus menghitung massa Matahari ($M_{\odot}$)!

### A. Tabel Data Observasi Astronomis Planet:
> **Catatan Konversi Satuan:**
> - $1\text{ AU (Astronomical Unit)} = 1{,}496 \times 10^{11}\text{ meter}$
> - $1\text{ Tahun Bumi} = 365{,}25\text{ Hari} = 3{,}156 \times 10^7\text{ sekon}$

Lengkapilah kolom perhitungan berikut:

| Nama Planet | Jarak Sumbu Semi-Mayor ($r$ dlm $\text{AU}$) | Periode Revolusi ($T$ dlm Tahun) | Nilai $r^3$ ($\text{AU}^3$) | Nilai $T^2$ ($\text{Tahun}^2$) | Rasio $\frac{T^2}{r^3}$ ($\text{Tahun}^2/\text{AU}^3$) |
|:---|:---:|:---:|:---:|:---:|:---:|
| **Merkurius** | $0{,}387$ | $0{,}241$ | $0{,}058$ | $0{,}058$ | ........................ |
| **Venus** | $0{,}723$ | $0{,}615$ | $0{,}378$ | $0{,}378$ | ........................ |
| **Bumi** | $1{,}000$ | $1{,}000$ | $1{,}000$ | $1{,}000$ | ........................ |
| **Mars** | $1{,}524$ | $1{,}881$ | $3{,}540$ | $3{,}538$ | ........................ |
| **Jupiter** | $5{,}204$ | $11{,}862$ | $140{,}9$ | $140{,}7$ | ........................ |
| **Saturnus** | $9{,}582$ | $29{,}457$ | $879{,}8$ | $867{,}7$ | ........................ |
| **Uranus** | $19{,}201$ | $84{,}011$ | $7.079{,}4$ | $7.057{,}8$ | ........................ |
| **Neptunus** | $30{,}047$ | $164{,}79$ | $27.127{,}1$ | $27.155{,}7$ | ........................ |

---

### B. Menghitung Massa Matahari ($M_{\odot}$) Menggunakan Sintesis Newton:
1. Hitung nilai rata-rata rasio $\frac{T^2}{r^3}$ dalam satuan $\text{Tahun}^2/\text{AU}^3$:  
   $$
   \left(\frac{T^2}{r^3}\right)_{\text{rata-rata}} = \dots\dots\dots\dots\dots\dots\dots\dots\dots\text{ Tahun}^2/\text{AU}^3
   $$
2. Sekarang, kita gunakan data planet Bumi dalam satuan Internasional (SI):
   - $r_{\oplus} = 1{,}496 \times 10^{11}\text{ m}$
   - $T_{\oplus} = 3{,}156 \times 10^7\text{ s}$
   - $G = 6{,}674 \times 10^{-11}\text{ N}\cdot\text{m}^2/\text{kg}^2$

   Berdasarkan sintesis analitik Newton pada gerak melingkar melingari matahari:
   $$
   \frac{T^2}{r^3} = \frac{4\pi^2}{G M_{\odot}} \implies M_{\odot} = \frac{4\pi^2 r^3}{G T^2}
   $$

   Hitunglah nilai $M_{\odot}$:
   $$
   M_{\odot} = \frac{4 \times (3{,}14159)^2 \times (1{,}496 \times 10^{11})^3}{(6{,}674 \times 10^{-11}) \times (3{,}156 \times 10^7)^2}
   $$
   $$
   M_{\odot} = \dots\dots\dots\dots\dots\dots\dots\dots\dots\dots\dots\dots\dots\dots\dots\dots\dots\text{ kg}
   $$
3. Apakah hasil perhitunganmu mendekati nilai massa Matahari referensi ($M_{\odot} \approx 1{,}989 \times 10^{30}\text{ kg}$)? Tuliskan analisismu!  
   *Refleksi:* .........................................................................................................................................

---

## 💡 PERTANYAAN DISKUSI & PENALARAN KRITIS (HOTS)

Diskusikan pertanyaan-pertanyaan berikut bersama teman kelompokmu:

1. **Studi Kasus Satelit Komunikasi:**  
   Indonesia mengoperasikan Satelit SATRIA-1 di orbit geostasioner pada bujur $146^\circ\text{ BT}$. Mengapa satelit geostasioner tersebut harus diposisikan tepat di atas garis khatulistiwa (*equator*) dan tidak boleh diletakkan di atas kutub utara/selatan? Jelaskan konsekuensinya terhadap penerimaan sinyal antena parabola di bumi jika satelit tersebut diletakkan di atas kutub!  
   *Jawaban:* .............................................................................................................................................

2. **Dilema Tabrakan Dua Bintang:**  
   Dua buah bintang bermassa masing-masing $M$ mula-mula diam terpisah pada jarak $D$ di ruang angkasa yang hampa tanpa pengaruh gravitasi benda langit lain. Akibat tarikan gravitasi timbal balik, kedua bintang perlahan mulai bergerak saling mendekat. Mengapa kelajuan kedua bintang semakin lama semakin cepat hingga akhirnya bertumbukan? Apakah titik tumbukan tepat berada di tengah-tengah jarak $D$? Jelaskan menggunakan Hukum Kekekalan Energi dan Momentum!  
   *Jawaban:* .............................................................................................................................................

3. **Misteri Pasang Surut Air Laut:**  
   Gaya gravitasi matahari terhadap bumi jauh lebih besar daripada gaya gravitasi bulan terhadap bumi karena massa matahari teramat masif. Namun, mengapa fenomena pasang surut air laut di permukaan bumi justru didominasi oleh gravitasi Bulan, bukan gravitasi Matahari? (*Petunjuk: Pikirkan konsep gradien medan gravitasi / gaya pasang surut $\Delta F \propto 1/r^3$*).  
   *Jawaban:* .............................................................................................................................................

---

## 📝 Kesimpulan Akhir Eksperimen

Tuliskan kesimpulan ilmiah menyeluruh kelompokmu mengenai:
1. Hubungan antara massa, jarak, dan gaya gravitasi:  
   ...................................................................................................................................................................
2. Validitas dan keakuratan Tiga Hukum Kepler dalam menjelaskan peredaran benda langit:  
   ...................................................................................................................................................................
3. Bagaimana sintesis Newton memungkinkan kita menentukan massa benda langit yang tak terjangkau:  
   ...................................................................................................................................................................

---

## 📋 Rubrik Penilaian Kinerja Inkuiri & Portofolio Siswa

| Aspek Penilaian | Kriteria Sangat Baik (4) | Kriteria Baik (3) | Kriteria Cukup (2) | Kriteria Perlu Bimbingan (1) |
|:---|:---|:---|:---|:---|
| **Keterampilan Eksperimen PhET** | Mengambil data simulasi secara runtut, presisi, dan mengisi seluruh tabel tanpa kesalahan. | Data simulasi lengkap dengan 1–2 kesalahan pembacaan minor. | Data simulasi terisi sebagian (>60%), ada beberapa ketidaksesuaian nilai. | Data simulasi tidak lengkap (<50%) dan tidak memahami kontrol instrumen. |
| **Pengolahan Data & Grafik** | Grafik digambar presisi dengan skala proporsional, gradien garis dan nilai $G$ dihitung akurat. | Grafik rapi, perhitungan gradien benar dengan kesalahan pembulatan angka kecil. | Grafik dibuat namun skala kurang proporsional, perhitungan gradien kurang tepat. | Tidak membuat grafik atau perhitungan gradien tidak dikerjakan. |
| **Analisis Data Tata Surya** | Perhitungan rasio $T^2/r^3$ dan estimasi massa Matahari akurat dengan penalaran ilmiah kuat. | Perhitungan rasio benar, kalkulasi massa Matahari benar dengan sedikit bantuan. | Sebagian perhitungan rasio selesai, kalkulasi massa matahari belum tuntas. | Perhitungan data tabel tidak tuntas dan tidak memahami korelasi rumus. |
| **Penalaran Soal HOTS & Diskusi** | Jawaban soal diskusi mendalam, argumentatif, mengaitkan konsep fisika dengan realitas teknologi. | Jawaban soal diskusi benar dan runtut secara konsep dasar fisika. | Jawaban soal diskusi bersifat hafalan rumus tanpa penjelasan fisis yang memadai. | Jawaban soal diskusi keliru atau tidak diisi. |
