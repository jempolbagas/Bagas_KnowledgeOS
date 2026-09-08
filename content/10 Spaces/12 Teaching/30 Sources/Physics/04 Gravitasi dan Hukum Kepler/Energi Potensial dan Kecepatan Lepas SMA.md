---
title: "Energi Potensial Gravitasi dan Kecepatan Lepas — Mekanika Energi Kosmik & Peluncuran Roket"
type: materi
subject: physics
level: sma
target_audience: "SMA Kelas XI"
created: 2026-09-08
sources:
  - "[[Gravitasi dan Hukum Kepler SMA]]"
  - "[[Gaya dan Medan Gravitasi SMA]]"
  - "[[Hukum Kepler dan Gerak Satelit SMA]]"
  - "[[Dinamika Gerak SMA]]"
tags:
  - fisika
  - energi-potensial-gravitasi
  - kecepatan-lepas
  - potensial-gravitasi
  - roket
  - kelas-11
  - kurikulum-merdeka
---

# Energi Potensial Gravitasi dan Kecepatan Lepas — Mekanika Energi Kosmik & Peluncuran Roket 🚀🌌

> 📍 **Navigasi Terpadu Unit Gravitasi & Kepler:**  
> [[Gravitasi dan Hukum Kepler SMA|🏠 Master Dashboard]] | [[Gaya dan Medan Gravitasi SMA|⏪ Modul 1: Gaya & Medan Gravitasi]] | **[Modul 2: Energi & Kecepatan Lepas]** | [[Hukum Kepler dan Gerak Satelit SMA|Modul 3: Hukum Kepler 🪐 ⏩]] | 📝 [[LKPD Gravitasi dan Hukum Kepler SMA|LKPD Inkuiri]] | 🎯 [[Soal Gravitasi dan Hukum Kepler SMA|Paket Soal HOTS]]

Energi potensial gravitasi pada skala kosmik merepresentasikan usaha yang diperlukan untuk memindahkan massa uji dari jarak tak hingga menuju suatu titik di dalam medan gravitasi non-seragam yang diciptakan oleh massa sumber. Berbeda dengan pendekatan lokal di permukaan bumi ($E_p = mgh$), formulasi gravitasi universal menuntut penetapan titik acuan nol di jarak tak terhingga ($r \to \infty$), yang berkonsekuensi bahwa energi potensial gravitasi suatu benda yang terikat oleh gravitasi planet selalu bernilai negatif ($E_p = -G \frac{Mm}{r}$). Melalui penerapan Hukum Kekekalan Energi Mekanik, kita dapat menurunkan konsep fundamental **Kelajuan Lepas (*Escape Velocity*)**, yakni ambang batas kelajuan kinetik minimum yang wajib dimiliki oleh wahana antariksa atau partikel gas atmosfer agar mampu membebaskan diri seutuhnya dari belenggu tarikan gravitasi suatu benda langit.

---

## 1. Mengapa Rumus $E_p = mgh$ Tak Lagi Berlaku di Antariksa? 🚫📏

Saat belajar di jenjang SMP atau awal SMA, kamu tentu sudah akrab dengan rumus:

$$
E_p = m \cdot g \cdot h
$$

Namun, rumus tersebut menyimpan satu **asumsi tersembunyi**: *percepatan gravitasi $g$ dianggap konstan selama benda bergerak*. Asumsi ini sangat akurat ketika kita hanya melempar bola setinggi $10\text{ meter}$ atau mendaki gedung setinggi $100\text{ meter}$, karena variasi nilai $g$ di rentang ketinggian tersebut sangat kecil dan dapat diabaikan.

Namun, saat kita meninjau roket yang meluncur ratusan kilometer ke atmosfer atas atau satelit yang mengorbit ribuan kilometer dari bumi, nilai percepatan gravitasi meluruh secara drastis mengikuti hukum kuadrat terbalik ($g \propto 1/r^2$). Oleh karena itu, kita memerlukan pendekatan kalkulus integral untuk menghitung usaha dan energi potensial gravitasi universal!

---

## 2. Penurunan Matematis Energi Potensial Gravitasi Universal 📐

Secara definisi mekanika, perubahan energi potensial gravitasi ($\Delta E_p$) sama dengan negatif dari usaha yang dilakukan oleh gaya gravitasi internal ($W_{\text{grav}}$), atau setara dengan usaha yang dilakukan oleh gaya luar ($W_{\text{ext}}$) untuk memindahkan massa $m$ secara perlahan (tanpa percepatan) dari posisi $r_1$ ke $r_2$:

$$
\Delta E_p = E_{p2} - E_{p1} = - \int_{r_1}^{r_2} F(r) \, dr
$$

Karena gaya gravitasi menarik benda ke arah pusat ($F(r) = -G \frac{M m}{r^2}$ ke arah dalam):

$$
\Delta E_p = - \int_{r_1}^{r_2} \left(-G \frac{M m}{r^2}\right) dr = G M m \int_{r_1}^{r_2} r^{-2} \, dr = G M m \left[ -\frac{1}{r} \right]_{r_1}^{r_2}
$$

$$
\Delta E_p = -G M m \left( \frac{1}{r_2} - \frac{1}{r_1} \right)
$$

### Mengapa Energi Potensial Gravitasi Bernilai Negatif? 🕳️
Untuk menentukan nilai mutlak $E_p$ pada suatu posisi $r$, fisikawan menyepakati **titik acuan nol energi potensial berada di jarak tak terhingga ($r \to \infty$)**, di mana gaya gravitasi sudah tidak lagi bekerja sama sekali ($E_p(\infty) = 0$).

Jika benda dipindahkan dari tak terhingga ($r_1 = \infty$) menuju ke titik berjarak $r$ ($r_2 = r$):

$$
E_p(r) - E_p(\infty) = -G M m \left( \frac{1}{r} - \frac{1}{\infty} \right)
$$

Karena $\frac{1}{\infty} = 0$ dan $E_p(\infty) = 0$, maka diperoleh formula baku:

$$
E_p = -G \frac{M m}{r}
$$

> **Keterangan Variabel Formula:**
> - $E_p$ = Energi potensial gravitasi sistem dua massa ($\text{J}$)
> - $G$ = Konstanta gravitasi universal ($6{,}674 \times 10^{-11}\text{ N}\cdot\text{m}^2/\text{kg}^2$)
> - $M$ = Massa benda sumber medan / planet ($\text{kg}$)
> - $m$ = Massa benda uji / satelit ($\text{kg}$)
> - $r$ = Jarak dari pusat massa $M$ ke pusat massa $m$ ($\text{m}$)

> [!important] Makna Fisis Tanda Negatif (Sumur Potensial Gravitasi)
> 1. **Kondisi Terikat (*Bound State*):** Tanda negatif menandakan bahwa massa $m$ terperangkap di dalam "sumur gravitasi" milik massa $M$. Benda tidak dapat kabur dengan sendirinya kecuali ada energi dari luar yang ditambahkan.
> 2. **Nilai Maksimum di Tak Hingga:** Nilai tertinggi dari $E_p$ adalah **$0\text{ Joule}$** (saat $r = \infty$). Di posisi mana pun yang lebih dekat ke planet, nilainya semakin negatif (makin dalam masuk ke sumur potensial).

---

## 3. Potensial Gravitasi ($V$) ⚡

Sama seperti kuat medan gravitasi ($g$) yang merupakan "gaya per satuan massa", **Potensial Gravitasi ($V$)** adalah **"energi potensial gravitasi per satuan massa"**:

$$
V = \frac{E_p}{m} = -G \frac{M}{r}
$$

> **Keterangan Variabel Formula:**
> - $V$ = Potensial gravitasi pada titik berjarak $r$ ($\text{J/kg}$ atau $\text{m}^2/\text{s}^2$)
> - $G$ = Konstanta gravitasi universal ($6{,}674 \times 10^{-11}\text{ N}\cdot\text{m}^2/\text{kg}^2$)
> - $M$ = Massa sumber medan ($\text{kg}$)
> - $r$ = Jarak titik dari pusat massa sumber ($\text{m}$)

### Sifat Skalar Potensial Gravitasi:
Potensial gravitasi adalah **besaran skalar** (tidak memiliki arah vektor). Keuntungannya, jika ada beberapa benda bermassa di sekitar suatu titik, potensial gravitasi total di titik tersebut cukup dijumlahkan secara aljabar aritmatika biasa tanpa perlu repot menghitung sudut vektor:

$$
V_{\text{total}} = \sum_{i=1}^n V_i = -G \left( \frac{M_1}{r_1} + \frac{M_2}{r_2} + \dots + \frac{M_n}{r_n} \right)
$$

Usaha luar ($W$) yang diperlukan untuk memindahkan muatan massa $m$ dari titik $A$ ke titik $B$ dirumuskan:

$$
W_{A \to B} = m \cdot \Delta V = m (V_B - V_A)
$$

---

## 4. Hukum Kekekalan Energi Mekanik Gravitasi 🔄

Jika tidak ada gaya non-konservatif luar (seperti gaya gesek atmosfer), energi mekanik total sistem gravitasi selalu kekal:

$$
E_m = E_k + E_p = \text{konstan}
$$

$$
\frac{1}{2} m v_1^2 - G \frac{M m}{r_1} = \frac{1}{2} m v_2^2 - G \frac{M m}{r_2}
$$

> **Keterangan Variabel Formula:**
> - $v_1, v_2$ = Kelajuan benda pada posisi 1 dan posisi 2 ($\text{m/s}$)
> - $r_1, r_2$ = Jarak pusat massa benda pada posisi 1 dan posisi 2 ($\text{m}$)
> - $M$ = Massa planet ($\text{kg}$)
> - $m$ = Massa benda yang bergerak ($\text{kg}$)

---

## 5. Kelajuan Lepas Planet (*Escape Velocity*) 🚀💨

Pernahkah kamu melempar batu ke atas? Semakin kuat kamu melemparnya, semakin tinggi batu tersebut naik sebelum akhirnya jatuh kembali.
Pertanyaannya: **Berapa kecepatan lemparan minimum agar benda tersebut terus melesat ke angkasa dan TIDAK PERNAH jatuh kembali ke bumi?**

Kecepatan batas kritis ini dinamakan **Kelajuan Lepas (*Escape Velocity*, $v_{\text{esc}}$)**.

### Penurunan Rumus:
Agar benda bermassa $m$ yang ditembakkan dari permukaan bumi ($r_1 = R$) dapat melepaskan diri dari medan gravitasi bumi hingga mencapai jarak tak terhingga ($r_2 \to \infty$) dengan kecepatan sisa tepat nol ($v_2 = 0$):

$$
E_{m1} = E_{m2}
$$

$$
\frac{1}{2} m v_{\text{esc}}^2 - G \frac{M m}{R} = \frac{1}{2} m (0)^2 - G \frac{M m}{\infty}
$$

Karena suku di ruas kanan keduanya bernilai nol ($0 - 0 = 0$):

$$
\frac{1}{2} m v_{\text{esc}}^2 - G \frac{M m}{R} = 0 \implies \frac{1}{2} m v_{\text{esc}}^2 = G \frac{M m}{R}
$$

Coret massa benda $m$ di kedua ruas, lalu selesaikan untuk $v_{\text{esc}}$:

$$
v_{\text{esc}}^2 = \frac{2GM}{R} \implies v_{\text{esc}} = \sqrt{\frac{2GM}{R}}
$$

Karena percepatan gravitasi di permukaan planet adalah $g = \frac{GM}{R^2} \implies GM = g R^2$, kita juga dapat menyatakannya dalam bentuk:

$$
v_{\text{esc}} = \sqrt{2 g R}
$$

> **Keterangan Variabel Formula:**
> - $v_{\text{esc}}$ = Kelajuan lepas dari permukaan planet ($\text{m/s}$)
> - $G$ = Konstanta gravitasi universal ($6{,}674 \times 10^{-11}\text{ N}\cdot\text{m}^2/\text{kg}^2$)
> - $M$ = Massa planet ($\text{kg}$)
> - $R$ = Jari-jari planet ($\text{m}$)
> - $g$ = Percepatan gravitasi di permukaan planet ($\text{m/s}^2$)

### Analisis Kritis Nilai Kelajuan Lepas:
1. **Bebas dari Massa Benda ($m$):** Formula di atas membuktikan bahwa kelajuan lepas sebuah jarum suntik, astronot, maupun roket seberat ribuan ton bernilai **sama persis**! Yang menentukan hanyalah massa dan jari-jari planet peluncur.
2. **Kelajuan Lepas Bumi:**
   Dengan $g = 9{,}8\text{ m/s}^2$ dan $R \approx 6{,}37 \times 10^6\text{ m}$:

$$
v_{\text{esc}} = \sqrt{2 \times 9{,}8 \times 6{,}37 \times 10^6} \approx 11{,}18 \times 10^3\text{ m/s} \approx 11{,}2\text{ km/s}
$$

   Artinya, roket antariksa membutuhkan kelajuan awal minimal **$11{,}2\text{ km/detik}$** (sekitar **$40.320\text{ km/jam}$**) untuk meloloskan diri dari cengkeraman gravitasi bumi tanpa propulsi lanjutan!

---

## 6. Aplikasi Kosmik: Mengapa Bulan Tidak Memiliki Atmosfer? 🌕💨

Pernah bertanya-tanya kenapa Bumi punya atmosfer yang tebal dan kaya oksigen, sementara Bulan hampa udara tanpa atmosfer sama sekali?

Jawabannya adalah pertarungan fisika antara **Kelajuan Termal Gas Molekuler** vs **Kelajuan Lepas Planet**!

1. Menurut teori kinetik gas, molekul-molekul gas atmosfer (seperti $\text{N}_2$, $\text{O}_2$, $\text{H}_2\text{O}$) bergerak acak dengan kelajuan rata-rata termal ($v_{\text{rms}} = \sqrt{\frac{3kT}{m}}$). Pada suhu siang hari ($T \approx 300\text{ K}$), laju molekul udara bumi berkisar $0{,}5\text{ km/s}$.
2. Di Bumi, kelajuan lepasnya sangat tinggi ($v_{\text{esc}} \approx 11{,}2\text{ km/s}$), jauh lebih besar daripada kelajuan molekul gas. Oleh karena itu, molekul gas tidak mampu meloloskan diri ke angkasa luar.
3. Namun di Bulan, massanya yang kecil membuat kelajuan lepasnya hanya sekitar **$2{,}38\text{ km/s}$**. Pada suhu siang hari di Bulan yang mencapai $120^\circ\text{C}$ ($393\text{ K}$), sebagian besar molekul gas bergerak lebih cepat dari $2{,}38\text{ km/s}$ sehingga perlahan-lahan terbang lepas meninggalkannya menuju ruang hampa. Akibatnya, Bulan kehilangan seluruh atmosfernya sejak miliaran tahun silam!

---

## 7. Contoh Soal Terbimbing & Analisis Langkah demi Langkah 📝

### Contoh 1: Usaha Memindahkan Satelit ke Orbit
**Soal:** Sebuah satelit bermassa $m = 500\text{ kg}$ akan dipindahkan dari permukaan bumi ($R = 6.400\text{ km}$) ke orbit lingkaran pada ketinggian $h = R$ dari permukaan bumi. Berapakah usaha luar minimum yang harus dilakukan hanya untuk mengatasi gaya gravitasi bumi? (Massa bumi $M = 6{,}0 \times 10^{24}\text{ kg}$, $G = 6{,}67 \times 10^{-11}\text{ N}\cdot\text{m}^2/\text{kg}^2$).

**Pembahasan:**
Usaha yang dilakukan oleh gaya luar sama dengan perubahan energi potensial gravitasi satelit:

$$
W = \Delta E_p = E_{p2} - E_{p1} = -G \frac{M m}{r_2} - \left(-G \frac{M m}{r_1}\right) = G M m \left(\frac{1}{r_1} - \frac{1}{r_2}\right)
$$

Posisi awal di permukaan: $r_1 = R$.  
Posisi akhir di orbit: $r_2 = R + h = R + R = 2R$.

$$
W = G M m \left(\frac{1}{R} - \frac{1}{2R}\right) = G M m \left(\frac{1}{2R}\right) = \frac{G M m}{2R}
$$

Substitusi nilai angka:

$$
W = \frac{(6{,}67 \times 10^{-11})(6{,}0 \times 10^{24})(500)}{2 \times (6{,}4 \times 10^6)} = \frac{2{,}001 \times 10^{17}}{1{,}28 \times 10^7} \approx 1{,}56 \times 10^{10}\text{ J}
$$

Jadi, usaha yang dibutuhkan adalah sekitar **$15{,}6\text{ GigaJoule}$** ($1{,}56 \times 10^{10}\text{ J}$).

---

### Contoh 2: Kelajuan Lepas Planet Hipotetis
**Soal:** Sebuah eksoplanet baru yang ditemukan memiliki massa $4$ kali massa bumi ($M_p = 4 M_{\oplus}$) dan jari-jari $2$ kali jari-jari bumi ($R_p = 2 R_{\oplus}$). Jika kelajuan lepas dari permukaan bumi adalah $v_0 = 11{,}2\text{ km/s}$, hitunglah kelajuan lepas dari eksoplanet tersebut!

**Pembahasan:**
Rumus kelajuan lepas adalah $v_{\text{esc}} = \sqrt{\frac{2GM}{R}}$.  
Bandingkan kelajuan lepas eksoplanet ($v_p$) terhadap bumi ($v_{\oplus}$):

$$
\frac{v_p}{v_{\oplus}} = \frac{\sqrt{\frac{2GM_p}{R_p}}}{\sqrt{\frac{2GM_{\oplus}}{R_{\oplus}}}} = \sqrt{\frac{M_p}{M_{\oplus}} \times \frac{R_{\oplus}}{R_p}}
$$

Substitusi perbandingan nilai yang diketahui:

$$
\frac{v_p}{v_{\oplus}} = \sqrt{\frac{4 M_{\oplus}}{M_{\oplus}} \times \frac{R_{\oplus}}{2 R_{\oplus}}} = \sqrt{\frac{4}{2}} = \sqrt{2} \approx 1{,}414
$$

Maka kelajuan lepas eksoplanet tersebut:

$$
v_p = \sqrt{2} \times 11{,}2\text{ km/s} \approx 15{,}84\text{ km/s}
$$

---

### Contoh 3: Ketinggian Maksimum Roket Vertikal (HOTS)
**Soal:** Sebuah wahana roket ditembakkan vertikal ke atas dari permukaan bumi dengan kelajuan awal setengah dari kelajuan lepas bumi ($v_0 = \frac{1}{2} v_{\text{esc}}$). Abaikan gesekan udara dan rotasi bumi. Tentukan ketinggian maksimum ($h$) yang dicapai roket tersebut diukur dari permukaan bumi dinyatakan dalam jari-jari bumi $R$!

**Pembahasan:**
Gunakan Hukum Kekekalan Energi Mekanik antara titik peluncuran (titik 1) dan titik tertinggi saat roket berhenti sesaat ($v_2 = 0$ di titik 2):

$$
E_{k1} + E_{p1} = E_{k2} + E_{p2}
$$

$$
\frac{1}{2} m v_0^2 - G \frac{M m}{R} = 0 - G \frac{M m}{r_{\text{maks}}}
$$

Kita tahu bahwa $v_{\text{esc}}^2 = \frac{2GM}{R}$, maka kelajuan awal roket:

$$
v_0^2 = \left(\frac{1}{2} v_{\text{esc}}\right)^2 = \frac{1}{4} v_{\text{esc}}^2 = \frac{1}{4} \left(\frac{2GM}{R}\right) = \frac{GM}{2R}
$$

Substitusi ke persamaan energi kinetik awal:

$$
\frac{1}{2} m \left(\frac{GM}{2R}\right) - G \frac{M m}{R} = - G \frac{M m}{r_{\text{maks}}}
$$

$$
\frac{GMm}{4R} - \frac{GMm}{R} = - \frac{GMm}{r_{\text{maks}}}
$$

Coret faktor bersama $G M m$:

$$
\frac{1}{4R} - \frac{1}{R} = - \frac{1}{r_{\text{maks}}} \implies -\frac{3}{4R} = -\frac{1}{r_{\text{maks}}} \implies r_{\text{maks}} = \frac{4}{3} R
$$

Karena jarak total dari pusat bumi adalah $r_{\text{maks}} = R + h$, maka ketinggian maksimum dari permukaan bumi adalah:

$$
h = r_{\text{maks}} - R = \frac{4}{3} R - R = \frac{1}{3} R
$$

Jadi, roket akan mencapai ketinggian maksimum sebesar **$\frac{1}{3} R$** di atas permukaan bumi!

---

> 📍 **Navigasi Modul:**  
> [[Gravitasi dan Hukum Kepler SMA|🏠 Master Dashboard]] | [[Gaya dan Medan Gravitasi SMA|⏪ Modul 1: Gaya & Medan Gravitasi]] | **[Modul 2: Energi & Kecepatan Lepas]** | [[Hukum Kepler dan Gerak Satelit SMA|Modul 3: Hukum Kepler 🪐 ⏩]]
