---
title: "Percepatan Sentripetal dan Dinamika Melingkar SMA"
type: materi
subject: Physics
level: sma
target_audience: "SMA Kelas XI"
created: 2026-09-09
sources:
  - "[[Gerak Melingkar Beraturan SMA]]"
  - "[[Besaran Sudut dan Karakteristik GMB SMA]]"
  - "[[Gaya Sentripetal SMA]]"
  - "[[Dinamika Gerak SMA]]"
tags:
  - fisika
  - sma_kelas_11
  - kurikulum_merdeka
  - materi_ajar
  - gerak_melingkar
  - percepatan_sentripetal
  - gaya_sentripetal
  - vektor_percepatan
  - dinamika_rotasi
---

> [!info] Navigasi Pembelajaran Terpadu
> [[Gerak Melingkar Beraturan SMA|🏠 Master Dashboard]] | [[Besaran Sudut dan Karakteristik GMB SMA|⏱️ Modul 1: Besaran Sudut & GMB]] | **🎯 Modul 2: Percepatan Sentripetal** | [[Hubungan Roda Roda dan Transmisi Gerak SMA|⚙️ Modul 3: Hubungan Roda-Roda]] | [[LKPD Gerak Melingkar Beraturan SMA|📝 LKPD Inkuiri]] | [[Soal Gerak Melingkar Beraturan SMA|🎯 Soal Evaluasi]]

---

# Percepatan Sentripetal dan Dinamika Melingkar — Menyingkap Misteri Pembelokan Gerak 🎯⚡

Percepatan sentripetal adalah percepatan fisis yang timbul pada suatu objek yang menempuh lintasan melengkung akibat perubahan arah vektor kecepatan secara kontinu terhadap waktu, meskipun kelajuan linier objek tersebut bernilai konstan. Nama *sentripetal* berakar dari bahasa Latin (*centrum* = pusat, *petere* = menuju), yang secara harfiah menggambarkan karakteristik vektor percepatan ini yang senantiasa mengarah tegak lurus menuju titik pusat kelengkungan lintasan lingkaran. Tanpa adanya percepatan sentripetal—dan gaya penyebabnya—Hukum Kelembaman Newton menuntut setiap benda bergerak lurus beraturan tanpa berbelok. Modul ini menyajikan penurunan geometris rigor persamaan percepatan sentripetal ($a_s = \frac{v^2}{r} = \omega^2 r$), menganalisis sifat ortogonalitas arah vektor yang tidak melakukan usaha mekanik, serta membangun jembatan konseptual menuju dinamika gaya sentripetal pada fenomena tikungan jalan, wahana putar, hingga orbit gravitasi kosmik.

---

## 1. Paradoks Kelajuan Tetap vs Percepatan Fisis

Pada pembahasan [[Kinematika Gerak Lurus SMA]], kita mendefinisikan percepatan sebagai laju perubahan kecepatan terhadap waktu:

$$
\vec{a} = \frac{d\vec{v}}{dt}
$$

Karena kecepatan ($\vec{v}$) adalah besaran **vektor**, perubahan kecepatan ($d\vec{v}$) dapat terjadi melalui dua mekanisme yang berbeda:
1. **Perubahan Magnitudo (Besar/Kelajuan):** Kecepatan bertambah cepat atau lambat pada lintasan lurus. Komponen perubahan ini disebut **percepatan tangensial** ($a_t$). Pada GMB, $a_t = 0$ karena kelajuannya konstan.
2. **Perubahan Arah Vektor:** Partikel mempertahankan kelajuan yang sama, namun orientasi arah panah kecepatannya dibelokkan setiap detik. Komponen perubahan arah ini disebut **percepatan radial / percepatan sentripetal** ($a_s$).

![[diagram_physics_gmb_percepatan_sentripetal.webp]]

Pada Gerak Melingkar Beraturan:
- Kelajuan skalar konstan: $|\vec{v}| = v = \text{konstan}$.
- Arah vektor kecepatan $\vec{v}$ terus berotasi: $\frac{d\vec{v}}{dt} \neq 0$.
- **Kesimpulan Fisis:** Benda yang bergerak melingkar beraturan **tidak pernah berada dalam kesetimbangan percepatan nol**; benda tersebut selalu dipercepat ke arah pusat lingkaran!

---

## 2. Penurunan Matematis Geometris Formula $a_s$

Secara historis, Christian Huygens dan Isaac Newton menurunkan formulasi percepatan sentripetal menggunakan kesebangunan segitiga geometris.

### Langkah Pembuktian Geometris:
Tinjau sebuah partikel yang bergerak melingkar beraturan dengan jari-jari $r$ dan kelajuan tetap $v$.
1. Pada waktu $t_1$, posisi partikel adalah $\vec{r}_1$ dan kecepatannya $\vec{v}_1$.
2. Pada waktu $t_2 = t_1 + \Delta t$, posisi partikel berpindah ke $\vec{r}_2$ dan kecepatannya menjadi $\vec{v}_2$.
3. Perpindahan posisi partikel dinyatakan oleh vektor $\Delta \vec{r} = \vec{r}_2 - \vec{r}_1$, yang membentuk segitiga posisi sama kaki dengan sudut puncak $\Delta \theta$. Untuk selang waktu yang sangat kecil ($\Delta t \to 0$), panjang busur lintasan mendekati panjang tali busur: $|\Delta \vec{r}| \approx \Delta s = v \Delta t$.
4. Perubahan kecepatan partikel dinyatakan oleh vektor $\Delta \vec{v} = \vec{v}_2 - \vec{v}_1$. Karena magnitudo kecepatan tetap ($|\vec{v}_1| = |\vec{v}_2| = v$) dan vektor kecepatan selalu tegak lurus terhadap vektor posisi masing-masing ($\vec{v} \perp \vec{r}$), maka segitiga vektor kecepatan juga merupakan segitiga sama kaki dengan sudut puncak yang persis sama, yaitu $\Delta \theta$.

Karena kedua segitiga tersebut **sebangun** (*similar triangles*), perbandingan sisi-sisi yang bersesuaian harus bernilai sama:

$$
\frac{|\Delta \vec{v}|}{v} = \frac{|\Delta \vec{r}|}{r}
$$

Kalikan kedua ruas dengan $v$ dan bagi dengan selang waktu $\Delta t$:

$$
\frac{|\Delta \vec{v}|}{\Delta t} = \frac{v}{r} \cdot \frac{|\Delta \vec{r}|}{\Delta t}
$$

Ambil limit untuk $\Delta t \to 0$:
- Ruas kiri menjadi definisi percepatan sesaat: $\lim_{\Delta t \to 0} \frac{|\Delta \vec{v}|}{\Delta t} = a_s$.
- Suku $\lim_{\Delta t \to 0} \frac{|\Delta \vec{r}|}{\Delta t}$ di ruas kanan adalah kelajuan linier partikel $v$.

Maka diperoleh perumusan percepatan sentripetal yang elegan:

$$
a_s = \frac{v \cdot v}{r} = \frac{v^2}{r}
$$

### Bentuk Alternatif Melalui Relasi Sudut ($\omega$ dan $f$):
Dengan menyubstitusikan hubungan $v = \omega r$ dari [[Besaran Sudut dan Karakteristik GMB SMA]]:

$$
a_s = \frac{(\omega r)^2}{r} = \frac{\omega^2 r^2}{r} = \omega^2 \cdot r
$$

Dan karena $\omega = \frac{2\pi}{T} = 2\pi f$, maka percepatan sentripetal juga dapat diekspresikan dalam bentuk:

$$
a_s = \left(\frac{2\pi}{T}\right)^2 r = \frac{4\pi^2 r}{T^2}
$$

$$
a_s = (2\pi f)^2 r = 4\pi^2 f^2 r
$$

**Legenda Variabel:**
- $a_s$ = Percepatan sentripetal ($\text{m/s}^2$)
- $v$ = Kelajuan linier / tangensial ($\text{m/s}$)
- $\omega$ = Kecepatan sudut ($\text{rad/s}$)
- $r$ = Jari-jari lingkaran ($\text{m}$)
- $T$ = Periode putaran ($\text{s}$)
- $f$ = Frekuensi putaran ($\text{Hz}$)

---

## 3. Sifat Vektor dan Konsep Kerja (Usaha Mekanik) Nol

Dua karakteristik fundamental dari vektor percepatan sentripetal $\vec{a}_s$:

### A. Arah Selalu Radial Menuju Pusat Putaran
Pada setiap titik di sepanjang lingkaran, vektor percepatan sentripetal $\vec{a}_s$ selalu berarah tegak lurus terhadap vektor kecepatan sesaat $\vec{v}$ ($\vec{a}_s \cdot \vec{v} = 0$). Vektor kecepatan menunjuk ke arah garis singgung (tangensial), sementara vektor percepatan sentripetal menunjuk tepat ke titik pusat poros lingkaran.

### B. Percepatan Sentripetal Tidak Mengubah Energi Kinetik (Usaha Nol)
Usaha mekanik ($W$) didefinisikan sebagai perkalian titik antara vektor gaya dan vektor perpindahan elemen lintasan ($d\vec{s}$):

$$
dW = \vec{F}_s \cdot d\vec{s} = (m \vec{a}_s) \cdot (\vec{v} \, dt)
$$

Karena $\vec{a}_s$ tegak lurus terhadap $\vec{v}$ ($\cos 90^\circ = 0$), maka:

$$
dW = 0 \quad \Longrightarrow \quad W = \Delta E_k = 0
$$

> [!NOTE]
> **Implikasi Fisis:** Percepatan sentripetal **murni berfungsi mengubah orientasi arah gerak benda**, dan **tidak pernah mengubah besar kelajuan maupun energi kinetik** partikel. Oleh karena itu, satelit yang mengorbit bumi dalam lintasan melingkar beraturan tidak membutuhkan bahan bakar pendorong untuk mempertahankan kelajuannya!

---

## 4. Jembatan Menuju Dinamika: Peran Gaya Sentripetal ($F_s$)

Menurut Hukum II Newton pada [[Dinamika Gerak SMA]], setiap percepatan harus dihasilkan oleh suatu resultan gaya netto yang searah dengan percepatan tersebut. Gaya yang menyebabkan timbulnya percepatan sentripetal disebut **Gaya Sentripetal** ($F_s$):

$$
\Sigma F_s = m \cdot a_s = m \frac{v^2}{r} = m \omega^2 r
$$

**Legenda Variabel:**
- $F_s$ = Gaya sentripetal netto ($\text{Newton, N}$)
- $m$ = Massa partikel ($\text{kg}$)
- $a_s$ = Percepatan sentripetal ($\text{m/s}^2$)
- $v$ = Kelajuan linier ($\text{m/s}$)
- $r$ = Jari-jari lintasan ($\text{m}$)

### Siapa yang Bertindak sebagai Gaya Sentripetal?
Penting dipahami bahwa *gaya sentripetal bukanlah jenis gaya baru yang misterius*, melainkan **peran/pekerjaan fisis** yang diambil oleh gaya-gaya nyata yang telah ada di alam:

| Fenomena Fisika | Sumber Gaya Nyata yang Berperan sebagai $F_s$ | Persamaan Dinamika |
| :--- | :--- | :--- |
| **Batu diputar dengan tali** | Tegangan tali ($T$) | $$T = m \frac{v^2}{r}$$ |
| **Mobil berbelok di tikungan mendatar** | Gaya gesek statis ban mobil dengan aspal ($f_s$) | $$f_s = \mu_s N = m \frac{v^2}{r}$$ |
| **Bulan / Satelit mengorbit Bumi** | Gaya gravitasi universal Newton ($F_g$) | $$G \frac{M m}{r^2} = m \frac{v^2}{r}$$ |
| **Elektron mengitari inti atom** | Gaya tarik elektrostatik Coulomb ($F_e$) | $$k \frac{|q_1 q_2|}{r^2} = m \frac{v^2}{r}$$ |

Rincian analitis lengkap mengenai penguraian diagram benda bebas gaya sentripetal dapat dipelajari pada modul rujukan [[Gaya Sentripetal SMA]].

---

## 5. Studi Kasus Kontekstual & Rekayasa Nyata

### Kasus 1: Tikungan Aspal Mendatar & Batas Kelajuan Aman
Ketika mobil melintasi tikungan lingkaran mendatar dengan jari-jari $r$, gaya yang mencegah mobil tergelincir keluar adalah gaya gesek statis ($f_s$) antara permukaan ban dan aspal.

Karena pada sumbu vertikal mobil diam ($N = m g$), maka gaya gesek statis maksimum adalah:
$$
f_{s,\max} = \mu_s N = \mu_s m g
$$

Agar mobil dapat membelok stabil tanpa tergelincir (*skidding*), gaya gesek statis maksimum harus mampu mencukupi kebutuhan gaya sentripetal:
$$
f_{s,\max} \ge m \frac{v^2}{r} \quad \Longrightarrow \quad \mu_s m g \ge m \frac{v^2}{r}
$$

Massa mobil $m$ saling meniadakan di kedua ruas, sehingga diperoleh batas kelajuan maksimum aman:

$$
v_{\max} = \sqrt{\mu_s \cdot g \cdot r}
$$

**Legenda Variabel:**
- $v_{\max}$ = Kelajuan maksimum aman sebelum tergelincir ($\text{m/s}$)
- $\mu_s$ = Koefisien gesekan statis antara ban dan jalan
- $g$ = Percepatan gravitasi bumi ($\approx 9{,}8\text{ m/s}^2$ atau $10\text{ m/s}^2$)
- $r$ = Jari-jari kelengkungan tikungan jalan ($\text{m}$)

> [!WARNING]
> Perhatikan bahwa batas kecepatan $v_{\max}$ **sama sekali tidak bergantung pada massa kendaraan ($m$)**. Sebuah truk tronton bermassa 20 ton dan sepeda motor bermassa 100 kg memiliki batas kelajuan aman yang sama persis saat melintasi tikungan yang licin!

---

### Kasus 2: Fenomena Saat Tali Pemutar Terputus
Bayangkan kamu memutar bola di ujung tali pada bidang horizontal licin. Jika tiba-tiba tali pemutar tersebut putus:
- Seketika tali terputus, tegangan tali lenyap ($T = 0$).
- Dengan lenyapnya tegangan tali, tidak ada lagi resultan gaya netto yang mengarah ke pusat ($\Sigma F = 0$).
- Berdasarkan **Hukum I Newton (Inersia)**, partikel akan mempertahankan kecepatannya saat itu dan bergerak lurus beraturan menempuh **garis singgung lingkaran (tangensial)**, bukan terdorong radial ke luar!

---

## ✍️ Worked Examples: Contoh Soal & Analisis Terpandu

### Contoh Soal 1: Analisis Kuantitatif Percepatan Sentripetal Centrifuge Medis
Di sebuah laboratorium klinis, sebuah tabung reaksi dalam alat sentrifugasi (*centrifuge*) berputar pada jarak $12\text{ cm}$ dari poros putaran dengan kecepatan rotasi $3000\text{ rpm}$. Jika percepatan gravitasi bumi adalah $g = 9{,}8\text{ m/s}^2$, hitunglah:
a) Kecepatan sudut alat sentrifugasi dalam $\text{rad/s}$.  
b) Besar percepatan sentripetal yang dialami oleh endapan darah di dasar tabung.  
c) Nilai percepatan sentripetal tersebut dalam kelipatan gaya gravitasi ($g\text{-force}$).

#### Pembahasan:
**Identifikasi Data:**
- Jari-jari $r = 12\text{ cm} = 0{,}12\text{ m}$.
- Frekuensi putaran: $f = \frac{3000\text{ rpm}}{60\text{ s}} = 50\text{ Hz}$.
- Percepatan gravitasi: $g = 9{,}8\text{ m/s}^2$.

**Penyelesaian Bagian (a):**
$$
\omega = 2\pi f = 2\pi (50) = 100\pi \text{ rad/s} \approx 314{,}16 \text{ rad/s}
$$

**Penyelesaian Bagian (b):**
Gunakan formula $a_s = \omega^2 r$:
$$
a_s = (100\pi)^2 \times 0{,}12 = 10.000\pi^2 \times 0{,}12 = 1.200\pi^2 \text{ m/s}^2
$$
Dengan mengasumsikan $\pi^2 \approx 9{,}8696$:
$$
a_s = 1.200 \times 9{,}8696 \approx 11.843{,}5 \text{ m/s}^2
$$

**Penyelesaian Bagian (c):**
Beban percepatan dalam satuan $g$:
$$
\text{Beban } g = \frac{a_s}{g} = \frac{11.843{,}5}{9{,}8} \approx 1.208{,}5 \, g
$$
*Interpretasi Fisis:* Partikel darah di dalam tabung mengalami percepatan sebesar lebih dari $1.200$ kali percepatan gravitasi bumi! Percepatan radial raksasa inilah yang memisahkan sel-sel darah merah padat dari plasma darah cair dalam hitungan menit.

---

### Contoh Soal 2: Tikungan Sirkuit Balap Mendatar
Sebuah mobil balap Formula melaju di tikungan sirkuit mendatar dengan radius kelengkungan $r = 50\text{ meter}$. Koefisien gesekan statis antara ban mobil dan aspal kering adalah $\mu_s = 0{,}8$. Dengan asumsi $g = 10\text{ m/s}^2$, tentukan:
a) Kelajuan maksimum mobil agar tidak melorot tergelincir ke luar lintasan.  
b) Percepatan sentripetal mobil pada kelajuan batas maksimum tersebut.

#### Pembahasan:
**Penyelesaian Bagian (a):**
Gunakan persamaan batas kecepatan tikungan mendatar:
$$
v_{\max} = \sqrt{\mu_s \cdot g \cdot r} = \sqrt{0{,}8 \times 10 \times 50} = \sqrt{400} = 20 \text{ m/s}
$$
Konversi ke satuan umum:
$$
v_{\max} = 20 \times 3{,}6 = 72 \text{ km/jam}
$$

**Penyelesaian Bagian (b):**
Percepatan sentripetal pada kelajuan $v_{\max} = 20\text{ m/s}$:
$$
a_s = \frac{v_{\max}^2}{r} = \frac{20^2}{50} = \frac{400}{50} = 8 \text{ m/s}^2
$$
*Verifikasi Fisis:* Karena $a_s = \mu_s g = 0{,}8 \times 10 = 8\text{ m/s}^2$, nilai percepatan sentripetal tepat sama dengan batas kapasitas gaya gesek statis per satuan massa.

---

> [!info] Navigasi Pembelajaran Terpadu
> [[Gerak Melingkar Beraturan SMA|🏠 Master Dashboard]] | [[Besaran Sudut dan Karakteristik GMB SMA|⏱️ Modul 1: Besaran Sudut & GMB]] | **🎯 Modul 2: Percepatan Sentripetal** | [[Hubungan Roda Roda dan Transmisi Gerak SMA|⚙️ Modul 3: Hubungan Roda-Roda]] | [[LKPD Gerak Melingkar Beraturan SMA|📝 LKPD Inkuiri]] | [[Soal Gerak Melingkar Beraturan SMA|🎯 Soal Evaluasi]]
