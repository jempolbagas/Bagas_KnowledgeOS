---
title: "Gerak Melingkar Beraturan — Master Guide & Navigasi Modul"
type: master-dashboard
subject: Physics
level: sma
target_audience: "SMA Kelas XI"
created: 2026-09-09
sources:
  - "[[Besaran Sudut dan Karakteristik GMB SMA]]"
  - "[[Percepatan Sentripetal dan Dinamika Melingkar SMA]]"
  - "[[Hubungan Roda Roda dan Transmisi Gerak SMA]]"
  - "[[Gaya Sentripetal SMA]]"
  - "[[Kinematika Gerak Lurus SMA]]"
tags:
  - fisika
  - sma_kelas_11
  - kurikulum_merdeka
  - materi_ajar
  - gerak_melingkar
  - kinematika_rotasi
  - percepatan_sentripetal
  - hubungan_roda_roda
  - master-dashboard
---

# Gerak Melingkar Beraturan — Harmoni Putaran & Dinamika Lintas Melengkung! 🎡🔄

Gerak Melingkar Beraturan (GMB) adalah gerak suatu benda pada lintasan melingkar dengan jari-jari tetap serta kelajuan linier dan kelajuan sudut yang konstan, namun senantiasa mengalami perubahan arah vektor kecepatan di setiap titik lintasannya. Konsekuensi fundamental dari pembelokan arah vektor kecepatan yang terus-menerus ini adalah lahirnya percepatan yang selalu mengarah tegak lurus menuju pusat lingkaran, yakni percepatan sentripetal ($a_s$). Pemahaman mendalam mengenai GMB merupakan jembatan analitis yang menghubungkan kinematika satu dimensi pada [[Kinematika Gerak Lurus SMA]] dengan konsep dinamika rotasi, orbit wahana antariksa, mekanika fluida pada sentrifugasi medis, hingga rekayasa transmisi mekanis roda-roda gigi pada kendaraan bermotor. Modul Master Guide ini dirancang khusus bagi peserta didik SMA Kelas XI (Fase F — Fisika Pilihan Kurikulum Merdeka) untuk memberikan peta navigasi komprehensif, cheatsheet formula terpadu, dan integrasi kurikulum dari teori dasar hingga aplikasi rekayasa nyata.

---

## 📊 Overview Bab & Peta Konsep Makro

Dalam fisika klasik, gerak partikel pada lintasan melingkar mengharuskan pemisahan tegas antara **besaran skalar** (kelajuan linier $v$ dan kelajuan sudut $\omega$ yang bernilai tetap pada GMB) dan **besaran vektor** (vektor kecepatan $\vec{v}$ yang arahnya selalu menyinggung lintasan/tangensial dan berubah secara kontinu).

![[infographic_physics_gmb_master_dashboard.webp]]

### Tiga Pilar Konseptual Utama:
1. **Kinematika Sudut & Relasi Linier:** Mentranslasikan konsep gerak garis lurus ke dalam ruang koordinat polar: posisi sudut ($\theta$), periode ($T$), frekuensi ($f$), dan kecepatan sudut ($\omega$), serta menjembataninya ke ranah gerak linier lewat parameter jari-jari lintasan ($r$).
2. **Geometri Vektor Percepatan Sentripetal:** Membedah paradoks bahwa kelajuan konstan pada lintasan lengkung tetap menghasilkan percepatan ($a_s \neq 0$), membuktikan penurunan formula geometris $a_s = \frac{v^2}{r} = \omega^2 r$, serta mengaitkannya dengan gaya pemaksa menuju pusat lintasan sebagai prasyarat eksistensi gerak melingkar.
3. **Mekanika Transmisi & Hubungan Roda-Roda:** Menganalisis interaksi kinematika pada tiga model hubungan gerak: roda sesumbu/seporos, roda bersinggungan langsung, dan roda terhubung sabuk/rantai, yang menjadi fondasi dasar transmisi gir sepeda, puli mesin, hingga sistem persneling otomotif.

---

## ⚖️ Matriks Komparasi: Kinematika Linier vs Kinematika Sudut

Untuk memudahkan pemahaman analogi fisis, seluruh besaran dalam gerak lurus memiliki padanan langsung dalam gerak melingkar beraturan:

| Besaran Kinematika | Dimensi Linier (Translasi) | Dimensi Sudut (Rotasi) | Persamaan Penghubung ($s = r \cdot \text{Sudut}$) | Satuan SI |
| :--- | :--- | :--- | :--- | :--- |
| **Posisi / Perpindahan** | Jarak/Perpindahan linier ($s$) | Sudut tempuh ($\theta$) | $$s = \theta \cdot r$$ | $\text{meter (m)}$ vs $\text{radian (rad)}$ |
| **Kecepatan / Laju** | Kecepatan linier / tangensial ($v$) | Kecepatan sudut ($\omega$) | $$v = \omega \cdot r$$ | $\text{m/s}$ vs $\text{rad/s}$ |
| **Percepatan** | Percepatan tangensial ($a_t = 0\text{ pada GMB}$) | Percepatan sudut ($\alpha = 0\text{ pada GMB}$) | $$a_t = \alpha \cdot r = 0$$ | $\text{m/s}^2$ vs $\text{rad/s}^2$ |
| **Percepatan Sentripetal** | Percepatan radial ($a_s$) | Relasi laju sudut | $$a_s = \frac{v^2}{r} = \omega^2 \cdot r$$ | $\text{m/s}^2$ |
| **Inersia / Ukuran Gerak** | Massa benda ($m$) | Momen Inersia ($I$) | $$I = m \cdot r^2\text{ (partikel)}$$ | $\text{kg}$ vs $\text{kg}\cdot\text{m}^2$ |

> [!NOTE]
> **Catatan Kritis Sudut Radian:** Hubungan linier-sudut ($s = \theta r$ dan $v = \omega r$) hanya sah berlaku jika nilai sudut $\theta$ dinyatakan dalam satuan **radian** ($\text{rad}$), bukan derajat ($\text{deg}$). Dalam $1\text{ putaran penuh}$ berlaku $360^\circ = 2\pi\text{ rad}$.

---

## 🧭 Navigasi Modul Pembelajaran Terpadu

Paket pembelajaran Gerak Melingkar Beraturan SMA Kelas XI ini disusun dalam tiga sub-modul terstruktur dan dua instrumen praktik-asesmen:

### ⏱️ [[Besaran Sudut dan Karakteristik GMB SMA | Modul 1: Besaran Sudut & Karakteristik Kinematika GMB]]
> *Fokus Pembahasan:*
> - Definisi radian, derajat, dan konversi revolusi per menit ($\text{rpm}$).
> - Karakteristik waktu: Periode ($T$) dan Frekuensi ($f$) serta formulasinya.
> - Kecepatan sudut rata-rata dan sesaat ($\omega$).
> - Hubungan kecepatan tangensial dengan kecepatan sudut ($v = \omega r$).
> - Ciri esensial GMB: $\omega = \text{konstan}$, $v = \text{konstan}$, $\alpha = 0$, namun vektor $\vec{v}$ berubah arah.
> - Contoh soal langkah demi langkah dan analisis jarum jam analitik.

### 🎯 [[Percepatan Sentripetal dan Dinamika Melingkar SMA | Modul 2: Geometri Vektor Percepatan Sentripetal & Aspek Fisis Dinamika]]
> *Fokus Pembahasan:*
> - Mengapa partikel dengan kelajuan tetap tetap mengalami percepatan fisis.
> - Penurunan matematis vektor percepatan sentripetal ($a_s = \frac{v^2}{r} = \omega^2 r$).
> - Arah vektor percepatan sentripetal $\vec{a}_s$ yang selalu tegak lurus terhadap $\vec{v}$ dan mengarah ke pusat putaran.
> - Pengantar jembatan menuju gaya sentripetal ($F_s = m a_s$) dan kaitannya dengan [[Gaya Sentripetal SMA]].
> - Studi fenomena: Tegangan tali pemutar batu, gaya gesek roda kendaraan di tikungan mendatar, dan wahana gravitasi buatan (*artificial gravity*).

### ⚙️ [[Hubungan Roda Roda dan Transmisi Gerak SMA | Modul 3: Sistem Transmisi Mekanis & Hubungan Roda-Roda]]
> *Fokus Pembahasan:*
> - Roda-roda seporos / sesumbu (*coaxial*): Kesamaan kecepatan sudut ($\omega_A = \omega_B$).
> - Roda-roda bersinggungan langsung (*direct contact gears*): Kesamaan kelajuan linier ($v_A = v_B$) dengan pembalikan arah putar.
> - Roda-roda terhubung sabuk atau rantai (*belt/chain drive*): Kesamaan kelajuan linier ($v_A = v_B$) dengan arah putar searah.
> - Rasio transmisi roda gigi ($N_A \cdot \omega_A = N_B \cdot \omega_B$).
> - Dekonstruksi sistem gir sepeda balap (*chainring* vs *sprocket cassette*) dan pengatur kecepatan *gearbox*.

### 📝 [[LKPD Gerak Melingkar Beraturan SMA | Instrumen Praktik: Lembar Kerja Peserta Didik (LKPD Inkuiri)]]
> *Format Kegiatan:*
> - **Aktivitas 1:** Eksperimen Sederhana Putaran Benda Bertali & Stopwatch (Pengukuran empiris $T, f, \omega, v$).
> - **Aktivitas 2:** Investigasi Vektor Tangensial saat Tali Pemutar Terputus (*Inertial Trajectory*).
> - **Aktivitas 3:** Proyek Analisis Rasio Transmisi Gir Sepeda Nyata (Eksplorasi kayuhan pedal terhadap kecepatan laju).

### 🎯 [[Soal Gerak Melingkar Beraturan SMA | Instrumen Evaluasi: Paket Soal Asesmen Standar HOTS]]
> *Struktur Asesmen:*
> - **15 Soal Pilihan Ganda Berjenjang:** Level 1 Fondasi Konseptual (C2–C3), Level 2 Aplikasi Matematis (C3–C4), dan Level 3 Penalaran Analitis Rekayasa (C4–C5).
> - **5 Soal Uraian Ilmiah & Studi Kasus Rekayasa.**
> - Kunci jawaban analitis komprehensif langkah demi langkah disertai legenda variabel lengkap dan rubrik penilaian.

---

## 📋 Master Formula Cheatsheet

Kumpulan formula inti yang digunakan di seluruh unit pembelajaran Gerak Melingkar Beraturan:

### 1. Hubungan Periode dan Frekuensi
$$
T = \frac{t}{n} = \frac{1}{f} \quad \Longleftrightarrow \quad f = \frac{n}{t} = \frac{1}{T}
$$

**Legenda Variabel:**
- $T$ = Periode putaran ($\text{s}$)
- $f$ = Frekuensi putaran ($\text{Hz}$ atau $\text{s}^{-1}$)
- $t$ = Total waktu putaran ($\text{s}$)
- $n$ = Jumlah putaran lengkap ($\text{tanpa satuan}$)

---

### 2. Kecepatan Sudut ($\omega$)
$$
\omega = \frac{\Delta \theta}{\Delta t} = \frac{2\pi}{T} = 2\pi f
$$

**Legenda Variabel:**
- $\omega$ = Kecepatan sudut / frekuensi sudut ($\text{rad/s}$)
- $\Delta \theta$ = Perpindahan sudut ($\text{rad}$)
- $\Delta t$ = Selang waktu ($\text{s}$)
- $\pi$ = Konstanta lingkaran ($\approx 3{,}14159$ atau $\frac{22}{7}$)

---

### 3. Hubungan Kecepatan Linier / Tangensial ($v$)
$$
v = \frac{2\pi r}{T} = 2\pi f r = \omega \cdot r
$$

**Legenda Variabel:**
- $v$ = Kelajuan linier / tangensial ($\text{m/s}$)
- $r$ = Jari-jari lintasan lingkaran ($\text{m}$)
- $\omega$ = Kecepatan sudut ($\text{rad/s}$)

---

### 4. Percepatan Sentripetal ($a_s$)
$$
a_s = \frac{v^2}{r} = \omega^2 \cdot r = \left(\frac{2\pi}{T}\right)^2 r = 4\pi^2 f^2 r
$$

**Legenda Variabel:**
- $a_s$ = Percepatan sentripetal ($\text{m/s}^2$)
- $v$ = Kelajuan linier ($\text{m/s}$)
- $\omega$ = Kecepatan sudut ($\text{rad/s}$)
- $r$ = Jari-jari lintasan lingkaran ($\text{m}$)

---

### 5. Sintesis Hubungan Roda-Roda
$$
\begin{aligned}
\text{Seporos (Sesumbu):} \quad &\omega_A = \omega_B \quad \Longrightarrow \quad \frac{v_A}{r_A} = \frac{v_B}{r_B} \\
\text{Bersinggungan Langsung:} \quad &v_A = v_B \quad \Longrightarrow \quad \omega_A r_A = \omega_B r_B \quad (\text{Arah putar berlawanan}) \\
\text{Dihubungkan Sabuk / Rantai:} \quad &v_A = v_B \quad \Longrightarrow \quad \omega_A r_A = \omega_B r_B \quad (\text{Arah putar searah}) \\
\text{Transmisi Roda Gigi (Gigi } N\text{):} \quad &N_A \cdot \omega_A = N_B \cdot \omega_B \quad \Longleftrightarrow \quad N_A \cdot f_A = N_B \cdot f_B
\end{aligned}
$$

**Legenda Variabel:**
- $\omega_A, \omega_B$ = Kecepatan sudut roda $A$ dan roda $B$ ($\text{rad/s}$)
- $v_A, v_B$ = Kelajuan linier tepi roda $A$ dan roda $B$ ($\text{m/s}$)
- $r_A, r_B$ = Jari-jari roda $A$ dan roda $B$ ($\text{m}$)
- $N_A, N_B$ = Jumlah mata gerigi roda $A$ dan roda $B$ ($\text{buah}$)

---

## ⚠️ Analisis Miskonsepsi Kritis Peserta Didik

Dalam pembelajaran GMB, sering kali muncul miskonsepsi mendasar yang wajib diurai secara pedagogis:

1. **Miskonsepsi "Kecepatan Konstan":**  
   *Kekeliruan:* Banyak siswa mengira bahwa karena kelajuan partikel tetap, maka percepatannya nol ($a = 0$) seperti pada GLB.  
   *Klarifikasi Fisis:* Kelajuan ($v$, besaran skalar) memang konstan, namun vektor kecepatan ($\vec{v}$) arahnya selalu berubah setiap saat. Perubahan arah vektor inilah yang meniscayakan timbulnya percepatan sentripetal ($a_s \neq 0$).

2. **Miskonsepsi "Gaya Sentrifugal sebagai Gaya Nyata":**  
   *Kekeliruan:* Siswa sering mengira bahwa ada gaya riil yang "mendorong benda keluar" dari lingkaran.  
   *Klarifikasi Fisis:* Gaya sentrifugal adalah gaya inersial fiktif (semu) yang hanya muncul saat kita meninjau dari kerangka acuan non-inersia yang berputar. Dari kerangka acuan inersia di bumi, partikel hanya berusaha mempertahankan lintasan lurusnya (inersia Hukum I Newton), sementara gaya riil yang bekerja hanyalah gaya sentripetal menuju ke pusat.

3. **Miskonsepsi Lintasan Lepas:**  
   *Kekeliruan:* Jika tali pemutar batu tiba-tiba putus, batu dianggap akan terlempar radial lurus menjauhi pusat lingkaran.  
   *Klarifikasi Fisis:* Berdasarkan Hukum Kelembaman I Newton, saat tali putus gaya sentripetal seketika lenyap, sehingga batu akan melesat lurus sesuai arah kecepatan tangensial sesaatnya ($\vec{v}$) yang tegak lurus terhadap garis radial jari-jari.

---

## 🎯 Panduan Alur Belajar yang Disarankan

Untuk mencapai ketuntasan kompetensi kognitif dan keterampilan analitis, alur pembelajaran direkomendasikan mengikuti tahapan berikut:

```
[1. Modul 1: Besaran Sudut & Karakteristik GMB]
       │
       ▼
[2. Modul 2: Geometri Percepatan Sentripetal]
       │
       ▼
[3. Modul 3: Sistem Hubungan Roda-Roda]
       │
       ▼
[4. Praktik LKPD Inkuiri: Eksperimen Benda Bertali & Gir Sepeda]
       │
       ▼
[5. Asesmen Sumatif HOTS: Paket Soal Evaluasi]
```
