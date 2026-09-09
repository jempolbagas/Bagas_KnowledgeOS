---
title: "Besaran Sudut dan Karakteristik GMB SMA"
type: materi
subject: Physics
level: sma
target_audience: "SMA Kelas XI"
created: 2026-09-09
sources:
  - "[[Gerak Melingkar Beraturan SMA]]"
  - "[[Kinematika Gerak Lurus SMA]]"
tags:
  - fisika
  - sma_kelas_11
  - kurikulum_merdeka
  - materi_ajar
  - gerak_melingkar
  - besaran_sudut
  - kecepatan_sudut
  - periode_frekuensi
  - radian
---

> [!info] Navigasi Pembelajaran Terpadu
> [[Gerak Melingkar Beraturan SMA|🏠 Master Dashboard]] | **⏱️ Modul 1: Besaran Sudut & GMB** | [[Percepatan Sentripetal dan Dinamika Melingkar SMA|🎯 Modul 2: Percepatan Sentripetal]] | [[Hubungan Roda Roda dan Transmisi Gerak SMA|⚙️ Modul 3: Hubungan Roda-Roda]] | [[LKPD Gerak Melingkar Beraturan SMA|📝 LKPD Inkuiri]] | [[Soal Gerak Melingkar Beraturan SMA|🎯 Soal Evaluasi]]

---

# Besaran Sudut dan Karakteristik GMB — Memetakan Ruang & Waktu Rotasi ⏱️🔄

Besaran sudut dan karakteristik kinematika gerak melingkar beraturan merupakan fondasi matematis untuk mendeskripsikan setiap gerak melengkung pada bidang dua dimensi dengan jari-jari kelengkungan tetap. Berbeda dengan kinematika translasi pada [[Kinematika Gerak Lurus SMA]] yang mengukur posisi dalam meter, gerak melingkar memetakan perpindahan berdasarkan sapuan sudut dalam satuan radian yang ditempuh per satuan waktu. Dalam Gerak Melingkar Beraturan (GMB), laju perubahan sudut atau kecepatan sudut ($\omega$) bernilai konstan sepanjang waktu, yang berimplikasi bahwa kelajuan linier partikel pada jarak tertentu dari pusat rotasi juga bernilai konstan, meskipun arah geraknya selalu berbelok secara kontinu. Modul ini membedah secara runtut konsep radian, hubungan periode-frekuensi, formulasi kecepatan sudut, relasi kelajuan tangensial ($v = \omega r$), serta karakteristik hakiki yang membedakan GMB dari gerak lurus lainnya.

---

## 1. Transformasi Spasial: Dari Lintasan Lurus ke Koordinat Polar

Ketika sebuah benda bergerak pada garis lurus, posisinya cukup dinyatakan dengan satu koordinat spasial $x$ atau $y$. Namun, ketika partikel bergerak melingkar di sekeliling suatu titik poros (misalnya ujung baling-baling helikopter atau jarum jam dinding), posisi partikel tersebut jauh lebih efisien dinyatakan dalam **sistem koordinat polar** $(r, \theta)$:
- $r$ adalah jarak radial partikel dari titik poros (pusat lingkaran).
- $\theta$ adalah posisi sudut partikel terhadap sumbu acuan horizontal (biasanya sumbu $+X$).

Bila partikel bergerak sepanjang keliling lingkaran sejauh busur lintasan $s$, partikel tersebut menyapu sudut sebesar $\Delta \theta$ pada titik pusat:

$$
s = r \cdot \Delta \theta
$$

**Legenda Variabel:**
- $s$ = Panjang busur lingkaran yang ditempuh partikel ($\text{m}$)
- $r$ = Jari-jari lingkaran / jarak radial dari titik pusat ($\text{m}$)
- $\Delta \theta$ = Perpindahan sudut partikel ($\text{rad}$)

Persamaan di atas secara gamblang menunjukkan bahwa panjang lintasan fisik ($s$) yang ditempuh suatu objek sebanding langsung dengan seberapa jauh jaraknya dari pusat putaran ($r$).

---

## 2. Satuan Sudut: Radian, Derajat, dan Revolusi (RPM)

Dalam fisika dan kalkulus lanjut, sudut tidak diukur dalam satuan sembarang derajat ($^\circ$), melainkan dalam satuan murni tanpa dimensi yang disebut **Radian** ($\text{rad}$).

### Mengapa Radian Bersifat Alami?
Satu radian didefinisikan sebagai besar sudut pusat yang menghadap busur lingkaran yang panjangnya **tepat sama dengan jari-jari lingkaran tersebut** ($s = r$). Karena keliling satu lingkaran penuh adalah $K = 2\pi r$, maka dalam satu putaran penuh ($1\text{ rotasi} = 360^\circ$) sudut yang disapu adalah:

$$
\theta_{\text{1 putaran}} = \frac{K}{r} = \frac{2\pi r}{r} = 2\pi \text{ rad}
$$

Dari relasi fundamental ini diperoleh faktor konversi matematis:

$$
2\pi \text{ rad} = 360^\circ \quad \Longleftrightarrow \quad 1 \text{ rad} = \frac{360^\circ}{2\pi} \approx 57{,}2958^\circ
$$

$$
1^\circ = \frac{2\pi}{360} \text{ rad} = \frac{\pi}{180} \text{ rad} \approx 0{,}01745 \text{ rad}
$$

### Konversi Satuan Industri: Rotasi per Menit (RPM)
Pada mesin kendaraan, motor listrik, dan cakram komputer, laju rotasi sering dinyatakan dalam $\text{rpm}$ (*revolutions per minute* atau putaran per menit). Karena $1\text{ putaran} = 2\pi\text{ rad}$ dan $1\text{ menit} = 60\text{ sekon}$, maka konversi dari $\text{rpm}$ ke satuan baku SI ($\text{rad/s}$) dirumuskan:

$$
1 \text{ rpm} = \frac{1 \times 2\pi \text{ rad}}{60 \text{ s}} = \frac{\pi}{30} \text{ rad/s} \approx 0{,}1047 \text{ rad/s}
$$

---

## 3. Parameter Temporal: Periode ($T$) dan Frekuensi ($f$)

Gerak melingkar beraturan merupakan gerak periodik, yaitu gerak yang berulang secara teratur dalam selang waktu yang sama. Dua besaran temporal yang mendeskripsikan keteraturan ini adalah **Periode** dan **Frekuensi**.

### A. Periode ($T$)
Periode adalah selang waktu yang dibutuhkan oleh suatu partikel untuk menempuh **satu kali putaran penuh** ($1\text{ siklus} = 2\pi\text{ rad}$).

$$
T = \frac{t}{n}
$$

**Legenda Variabel:**
- $T$ = Periode putaran ($\text{sekon, s}$)
- $t$ = Total waktu yang diamati ($\text{sekon, s}$)
- $n$ = Jumlah putaran yang berhasil diselesaikan ($\text{tanpa satuan}$)

### B. Frekuensi ($f$)
Frekuensi adalah banyaknya putaran lengkap yang dapat dihasilkan oleh suatu benda dalam **satu satuan waktu** (satu sekon).

$$
f = \frac{n}{t}
$$

**Legenda Variabel:**
- $f$ = Frekuensi putaran ($\text{Hertz, Hz}$ atau $\text{sekon}^{-1}$)
- $n$ = Jumlah putaran lengkap
- $t$ = Selang waktu pengamatan ($\text{s}$)

### Relasi Timbal-Balik:
Periode dan frekuensi memiliki relasi timbal-balik (*inversely proportional*):

$$
T = \frac{1}{f} \quad \Longleftrightarrow \quad f = \frac{1}{T} \quad \Longleftrightarrow \quad T \cdot f = 1
$$

> [!TIP]
> **Aplikasi Cepat pada Jarum Jam:**
> - Jarum detik: Melakukan 1 putaran penuh dalam 60 detik $\rightarrow T_{\text{detik}} = 60\text{ s}$ ($f = \frac{1}{60}\text{ Hz}$).
> - Jarum menit: Melakukan 1 putaran penuh dalam 1 jam $\rightarrow T_{\text{menit}} = 3600\text{ s}$.
> - Jarum jam (pendek): Melakukan 1 putaran penuh dalam 12 jam (bukan 24 jam!) $\rightarrow T_{\text{jam}} = 12 \times 3600 = 43.200\text{ s}$.

---

## 4. Kecepatan Sudut / Frekuensi Sudut ($\omega$)

Kecepatan sudut ($\omega$, dibaca *omega*) mendeskripsikan seberapa cepat sudut pusat disapu oleh garis hubung partikel terhadap waktu.

### A. Kecepatan Sudut Rata-rata ($\bar{\omega}$) dan Sesaat ($\omega$)
$$
\bar{\omega} = \frac{\Delta \theta}{\Delta t} = \frac{\theta_2 - \theta_1}{t_2 - t_1}
$$

$$
\omega = \lim_{\Delta t \to 0} \frac{\Delta \theta}{\Delta t} = \frac{d\theta}{dt}
$$

Pada Gerak Melingkar Beraturan (GMB), kecepatan sudut bernilai **konstan setiap saat**, sehingga $\bar{\omega} = \omega$.

### B. Formulasi $\omega$ Berdasarkan $T$ dan $f$
Untuk satu putaran penuh, sudut yang disapu adalah $\Delta \theta = 2\pi\text{ rad}$ dalam waktu $\Delta t = T\text{ sekon}$. Oleh karena itu:

$$
\omega = \frac{2\pi}{T} = 2\pi f
$$

**Legenda Variabel:**
- $\omega$ = Kecepatan sudut / kelajuan sudut ($\text{rad/s}$)
- $T$ = Periode putaran ($\text{s}$)
- $f$ = Frekuensi putaran ($\text{Hz}$)
- $\pi \approx 3{,}14159$

> [!NOTE]
> **Vektor Kecepatan Sudut ($\vec{\omega}$):** Kecepatan sudut secara ketat merupakan besaran vektor semu (*pseudovector*). Arah vektor $\vec{\omega}$ ditentukan menggunakan **Kaidah Tangan Kanan**: lipat empat jari tangan kanan searah dengan arah putaran benda, maka arah jempol yang tegak lurus menunjukkan arah vektor $\vec{\omega}$ (keluar bidang atau masuk bidang rotasi).

---

## 5. Hubungan Kecepatan Linier / Tangensial dengan Kecepatan Sudut

Meskipun semua titik pada sebuah benda tegar yang berputar memiliki kecepatan sudut $\omega$ yang persis sama, titik-titik yang terletak pada jarak radial ($r$) yang berbeda menempuh panjang lintasan busur yang berbeda dalam waktu yang sama.

Kecepatan linier partikel yang menyinggung garis tepi lingkaran disebut **kecepatan tangensial** ($\vec{v}$). Kelajuannya diturunkan langsung dari definisi laju lintasan:

$$
v = \frac{s}{t} = \frac{r \cdot \theta}{t} = r \cdot \left(\frac{\theta}{t}\right) = \omega \cdot r
$$

Atau bila dinyatakan melalui periode dan frekuensi:

$$
v = \frac{2\pi r}{T} = 2\pi f r = \omega \cdot r
$$

**Legenda Variabel:**
- $v$ = Kelajuan linier / tangensial ($\text{m/s}$)
- $\omega$ = Kecepatan sudut ($\text{rad/s}$)
- $r$ = Jari-jari lingkaran / jarak titik ke poros putar ($\text{m}$)
- $T$ = Periode putaran ($\text{s}$)
- $f$ = Frekuensi putaran ($\text{Hz}$)

### Intisari Fisis $v = \omega r$:
Jika kamu berada di atas wahana komidi putar (*merry-go-round*), duduk di dekat titik pusat poros terasa bergerak lambat, sedangkan jika kamu berdiri di tepi terluar wahana, kamu akan merasakan laju linier yang sangat kencang. Hal ini membuktikan bahwa **kelajuan linier berbanding lurus dengan jarak radial ($r$)**, walaupun waktu tempuh satu putarannya ($T$) dan laju sudutnya ($\omega$) sama persis.

---

## 6. Karakteristik Mutlak Gerak Melingkar Beraturan (GMB)

Secara ringkas dan tegas, suatu benda dikatakan berada dalam kondisi **Gerak Melingkar Beraturan (GMB)** apabila memenuhi parameter-parameter fisis berikut:

1. **Jari-jari Lintasan Konstan ($r = \text{konstan}$):** Lintasan berbentuk lingkaran sempurna.
2. **Kelajuan Sudut Konstan ($\omega = \text{konstan}$):** Partikel menyapu sudut yang sama dalam selang waktu yang sama.
3. **Percepatan Sudut Nol ($\alpha = \frac{d\omega}{dt} = 0$):** Tidak ada percepatan sudut yang mempercepat atau memperlambat rotasi.
4. **Kelajuan Linier Konstan ($v = |\vec{v}| = \text{konstan}$):** Nilai skalar kelajuan tidak berubah.
5. **Percepatan Tangensial Nol ($a_t = \frac{dv}{dt} = 0$):** Karena besar kelajuan tidak bertambah maupun berkurang.
6. **Vektor Kecepatan Linier Berubah Secara Kontinu ($\frac{d\vec{v}}{dt} \neq 0$):** Walaupun magnitudo $v$ konstan, arah vektornya senantiasa berubah searah garis singgung lingkaran. Perubahan arah vektor inilah yang melahirkan percepatan sentripetal ($a_s$), yang dibedah mendalam pada [[Percepatan Sentripetal dan Dinamika Melingkar SMA|Modul 2]].

---

## ✍️ Worked Examples: Contoh Soal & Analisis Terpandu

### Contoh Soal 1: Konversi Mesin Gerinda & Kecepatan Tepi Cakram
Sebuah piringan batu gerinda pemotong logam memiliki diameter $20\text{ cm}$. Piringan tersebut berputar dengan laju rotasi konstan sebesar $1200\text{ rpm}$.  
Tentukan:
a) Frekuensi dan periode putaran gerinda.  
b) Kecepatan sudut piringan gerinda dalam satuan baku $\text{rad/s}$.  
c) Kelajuan linier sebuah titik pada tepi terluar piringan gerinda.

#### Pembahasan:
**Identifikasi Variabel yang Diketahui:**
- Diameter $D = 20\text{ cm} \rightarrow r = \frac{D}{2} = 10\text{ cm} = 0{,}1\text{ m}$.
- Putaran per menit $\text{RPM} = 1200\text{ putaran/menit}$.

**Penyelesaian Bagian (a):**  
Frekuensi adalah jumlah putaran tiap sekon:
$$
f = \frac{1200\text{ putaran}}{60\text{ s}} = 20\text{ Hz}
$$

Periode adalah kebalikan dari frekuensi:
$$
T = \frac{1}{f} = \frac{1}{20} = 0{,}05\text{ sekon}
$$

**Penyelesaian Bagian (b):**  
Kecepatan sudut dihitung melalui $\omega = 2\pi f$:
$$
\omega = 2\pi (20) = 40\pi \text{ rad/s} \approx 40 \times 3{,}1416 = 125{,}66 \text{ rad/s}
$$

**Penyelesaian Bagian (c):**  
Kelajuan linier titik tepi menggunakan relasi $v = \omega r$:
$$
v = \omega \cdot r = (40\pi \text{ rad/s}) \times (0{,}1 \text{ m}) = 4\pi \text{ m/s} \approx 12{,}57 \text{ m/s}
$$
*Kesimpulan:* Dalam satu sekon, serpihan percikan api dari tepi gerinda melesat dengan kelajuan sekitar $12{,}57\text{ m/s}$ (atau setara dengan $45{,}25\text{ km/jam}$).

---

### Contoh Soal 2: Komparasi Kecepatan Sudut Jarum Jam
Hitunglah perbandingan kecepatan sudut jarum detik ($\omega_d$), jarum menit ($\omega_m$), dan jarum jam ($\omega_j$) pada sebuah jam dinding analog standar!

#### Pembahasan:
**Identifikasi Periode Masing-Masing Jarum:**
- Jarum detik: $T_d = 60\text{ s}$.
- Jarum menit: $T_m = 60\text{ menit} = 3600\text{ s}$.
- Jarum jam: $T_j = 12\text{ jam} = 12 \times 3600\text{ s} = 43200\text{ s}$.

**Perumusan Kecepatan Sudut:**
Karena $\omega = \frac{2\pi}{T}$, maka $\omega$ berbanding terbalik dengan periode $T$:

$$
\omega_d : \omega_m : \omega_j = \frac{2\pi}{T_d} : \frac{2\pi}{T_m} : \frac{2\pi}{T_j} = \frac{1}{60} : \frac{1}{3600} : \frac{1}{43200}
$$

Kalikan seluruh ruas perbandingan dengan angka $43200$:
$$
\omega_d : \omega_m : \omega_j = \frac{43200}{60} : \frac{43200}{3600} : \frac{43200}{43200} = 720 : 12 : 1
$$

*Kesimpulan Fisis:* Jarum detik berputar $12$ kali lebih cepat daripada jarum menit, dan $720$ kali lebih cepat daripada jarum jam.

---

> [!info] Navigasi Pembelajaran Terpadu
> [[Gerak Melingkar Beraturan SMA|🏠 Master Dashboard]] | **⏱️ Modul 1: Besaran Sudut & GMB** | [[Percepatan Sentripetal dan Dinamika Melingkar SMA|🎯 Modul 2: Percepatan Sentripetal]] | [[Hubungan Roda Roda dan Transmisi Gerak SMA|⚙️ Modul 3: Hubungan Roda-Roda]] | [[LKPD Gerak Melingkar Beraturan SMA|📝 LKPD Inkuiri]] | [[Soal Gerak Melingkar Beraturan SMA|🎯 Soal Evaluasi]]
