---
title: "Hubungan Roda Roda dan Transmisi Gerak SMA"
type: materi
subject: Physics
level: sma
target_audience: "SMA Kelas XI"
created: 2026-09-09
sources:
  - "[[Gerak Melingkar Beraturan SMA]]"
  - "[[Besaran Sudut dan Karakteristik GMB SMA]]"
  - "[[Percepatan Sentripetal dan Dinamika Melingkar SMA]]"
tags:
  - fisika
  - sma_kelas_11
  - kurikulum_merdeka
  - materi_ajar
  - hubungan_roda_roda
  - transmisi_gerak
  - gear_ratio
  - puli_mesin
  - gir_sepeda
---

> [!info] Navigasi Pembelajaran Terpadu
> [[Gerak Melingkar Beraturan SMA|🏠 Master Dashboard]] | [[Besaran Sudut dan Karakteristik GMB SMA|⏱️ Modul 1: Besaran Sudut & GMB]] | [[Percepatan Sentripetal dan Dinamika Melingkar SMA|🎯 Modul 2: Percepatan Sentripetal]] | **⚙️ Modul 3: Hubungan Roda-Roda** | [[LKPD Gerak Melingkar Beraturan SMA|📝 LKPD Inkuiri]] | [[Soal Gerak Melingkar Beraturan SMA|🎯 Soal Evaluasi]]

---

# Hubungan Roda-Roda dan Transmisi Gerak — Rekayasa Aliran Putaran & Rasio Gir ⚙️🚴

Hubungan roda-roda adalah aplikasi kinematika gerak melingkar yang mempelajari transmisi daya, kecepatan sudut, dan torsi antar dua atau lebih piringan berputar yang saling terhubung secara mekanis. Dalam rekayasa permesinan dan kehidupan sehari-hari—mulai dari transmisi rantai sepeda kayuh, mekanisme roda gigi jam tangan mekanik, hingga sabuk konveyor industri dan transmisi otomatis *Continuously Variable Transmission* (CVT)—tenaga rotasi dari satu sumber penggerak harus disalurkan ke komponen lain dengan mengubah laju putaran atau arah rotasinya. Terdapat tiga konfigurasi fundamental hubungan roda-roda dalam fisika: sistem seporos (*coaxial*), sistem bersinggungan langsung (*directly meshed*), dan sistem yang dihubungkan melalui perantara sabuk atau rantai (*belt/chain driven*). Modul ini mengupas tuntas formulasi matematis ketiga hubungan tersebut, menyusun matriks komparasinya, serta menganalisis secara mendalam rasio transmisi roda gigi pada sepeda multi-kecepatan.

---

## 1. Tiga Model Konfigurasi Transmisi Roda-Roda

Dalam menganalisis hubungan roda-roda, kunci utamanya adalah mengidentifikasi **besaran fisis apa yang bernilai sama** di antara kedua roda yang saling berinteraksi: apakah kecepatan sudutnya ($\omega$) ataukah kelajuan linier tepinya ($v$).

![[diagram_physics_gmb_hubungan_roda_roda.webp]]

---

## 2. Model 1: Roda-Roda Seporos / Sesumbu (*Coaxial*)

Dua atau lebih roda dikatakan seporos apabila roda-roda tersebut terpasang mati pada satu batang poros as yang sama dan berputar bersama-sama sebagai satu kesatuan benda tegar.

### Karakteristik Fisis:
1. **Kecepatan Sudut Identik:** Karena terikat pada poros yang sama, setiap kali poros berputar satu putaran penuh ($2\pi\text{ rad}$), seluruh roda yang melekat padanya juga menempuh satu putaran penuh dalam waktu yang sama.
2. **Arah Putaran Identik:** Seluruh roda berputar searah jarum jam atau seluruhnya berlawanan arah jarum jam.
3. **Kelajuan Linier Tepi Berbanding Lurus dengan Jari-Jari:** Karena $v = \omega r$ dan $\omega$ sama, roda dengan jari-jari lebih besar akan memiliki kelajuan linier tepi yang lebih kencang.

### Formulasi Matematis:
$$
\omega_A = \omega_B \quad \Longleftrightarrow \quad f_A = f_B \quad \Longleftrightarrow \quad T_A = T_B
$$

Dengan menyubstitusikan $\omega = \frac{v}{r}$:

$$
\frac{v_A}{r_A} = \frac{v_B}{r_B} \quad \Longleftrightarrow \quad v_B = v_A \left(\frac{r_B}{r_A}\right)
$$

**Legenda Variabel:**
- $\omega_A, \omega_B$ = Kecepatan sudut roda $A$ dan roda $B$ ($\text{rad/s}$)
- $v_A, v_B$ = Kelajuan linier tepi roda $A$ dan roda $B$ ($\text{m/s}$)
- $r_A, r_B$ = Jari-jari roda $A$ dan roda $B$ ($\text{m}$)

> [!TIP]
> **Contoh Aplikasi Nyata:**  
> Roda belakang sepeda dengan piringan gir kecil (*sprocket*) yang menempel di pusat roda. Ketika sprocket belakang berputar 1 putaran, ban sepeda berdiameter besar juga berputar tepat 1 putaran ($\omega_{\text{gir}} = \omega_{\text{ban}}$).

---

## 3. Model 2: Roda-Roda Bersinggungan Langsung (*Meshed Gears*)

Dua roda atau roda gigi (gir) yang tepinya saling bersentuhan atau saling mengunci geriginya tanpa mengalami selip.

### Karakteristik Fisis:
1. **Kelajuan Linier Tepi Identik:** Setiap sentimeter tepi roda pertama yang melewati titik singgung harus menggerakkan tepat satu sentimeter tepi roda kedua agar tidak terjadi benturan atau selip ($v_A = v_B$).
2. **Arah Putaran Berlawanan:** Jika roda $A$ berputar searah jarum jam (*clockwise*), roda $B$ akan dipaksa berputar berlawanan arah jarum jam (*counter-clockwise*).
3. **Kecepatan Sudut Berbanding Terbalik dengan Jari-Jari:** Roda yang berukuran lebih kecil harus berputar lebih sering (lebih banyak putaran per detik) agar dapat mengimbangi kelajuan linier roda yang lebih besar.

### Formulasi Matematis:
$$
v_A = v_B
$$

Substitusikan $v = \omega r$:

$$
\omega_A \cdot r_A = \omega_B \cdot r_B \quad \Longleftrightarrow \quad \frac{\omega_A}{\omega_B} = \frac{r_B}{r_A}
$$

### Relasi dengan Jumlah Gigi ($N$):
Untuk roda gigi bergigi (*toothed gears*), ukuran jarak antar gigi harus seragam agar dapat mengunci dengan sempurna. Oleh karena itu, keliling roda (dan jari-jarinya) sebanding langsung dengan jumlah gigi ($r \propto N$):

$$
N_A \cdot \omega_A = N_B \cdot \omega_B \quad \Longleftrightarrow \quad N_A \cdot f_A = N_B \cdot f_B
$$

**Legenda Variabel:**
- $v_A, v_B$ = Kelajuan linier pada titik singgung ($\text{m/s}$)
- $\omega_A, \omega_B$ = Kecepatan sudut roda $A$ dan roda $B$ ($\text{rad/s}$)
- $r_A, r_B$ = Jari-jari efektif roda $A$ dan $B$ ($\text{m}$)
- $N_A, N_B$ = Jumlah gigi roda $A$ dan $B$ ($\text{buah}$)

---

## 4. Model 3: Roda-Roda Dihubungkan Sabuk atau Rantai (*Belt / Chain*)

Dua roda terpisah yang dihubungkan melalui sebuah rantai logam atau sabuk karet (*belt*) yang melingkari kedua tepinya tanpa selip.

### Karakteristik Fisis:
1. **Kelajuan Linier Tepi Identik:** Karena seluruh elemen rantai bergerak dengan kelajuan yang sama di sepanjang lintasan penghubung, kelajuan linier tepi roda $A$ sama dengan kelajuan rantai, dan sama pula dengan kelajuan linier tepi roda $B$ ($v_A = v_{\text{rantai}} = v_B$).
2. **Arah Putaran Searah (Sabuk Terbuka):** Jika sabuk dipasang lurus/terbuka (seperti rantai sepeda), kedua roda berputar dalam arah yang sama.  
   *(Catatan Khusus: Jika sabuk dipasang menyilang seperti angka 8, arah putaran kedua roda akan menjadi berlawanan).*
3. **Kecepatan Sudut Berbanding Terbalik dengan Jari-Jari:** Sama seperti sistem bersinggungan, roda berdiameter kecil akan berputar dengan kecepatan sudut lebih tinggi.

### Formulasi Matematis:
$$
v_A = v_B
$$

$$
\omega_A \cdot r_A = \omega_B \cdot r_B \quad \Longleftrightarrow \quad 2\pi f_A r_A = 2\pi f_B r_B
$$

$$
N_A \cdot \omega_A = N_B \cdot \omega_B \quad \Longleftrightarrow \quad \frac{\omega_A}{\omega_B} = \frac{N_B}{N_A}
$$

**Legenda Variabel:**
- $v_A, v_B$ = Kelajuan linier tepi roda / kelajuan sabuk rantai ($\text{m/s}$)
- $\omega_A, \omega_B$ = Kecepatan sudut roda $A$ dan roda $B$ ($\text{rad/s}$)
- $r_A, r_B$ = Jari-jari roda $A$ dan roda $B$ ($\text{m}$)
- $N_A, N_B$ = Jumlah gigi sproket roda $A$ dan $B$

---

## ⚖️ Matriks Komparasi Sintesis Hubungan Roda-Roda

| Parameter Fisis | Seporos (Sesumbu) | Bersinggungan Langsung | Dihubungkan Sabuk / Rantai |
| :--- | :--- | :--- | :--- |
| **Besaran yang Sama** | Kecepatan sudut ($\omega_A = \omega_B$) | Kelajuan linier tepi ($v_A = v_B$) | Kelajuan linier tepi ($v_A = v_B$) |
| **Relasi Jari-Jari** | $$\frac{v_A}{r_A} = \frac{v_B}{r_B}$$ | $$\omega_A r_A = \omega_B r_B$$ | $$\omega_A r_A = \omega_B r_B$$ |
| **Relasi Jumlah Gigi** | Tidak relevan (poros kaku) | $$N_A \omega_A = N_B \omega_B$$ | $$N_A \omega_A = N_B \omega_B$$ |
| **Arah Putaran** | Searah | Berlawanan arah | Searah (sabuk terbuka) |
| **Contoh Sistem Nyata** | Poros roda mobil, gir belakang ke ban | Gearbox jam, transmisi roda gigi lurus | Rantai sepeda, sabuk CVT motor matic |

---

## 🚴 Studi Kasus Rekayasa: Dekonstruksi Transmisi Gir Sepeda Balap

Sistem transmisi sepeda adalah contoh luar biasa dari kombinasi dua model hubungan roda-roda:

```
[Pedal & Gir Depan A (Chainring)] 
             │
             │ (Dihubungkan Rantai: v_A = v_B)
             ▼
[Gir Belakang B (Sprocket)] 
             │
             │ (Seporos / Sesumbu: ω_B = ω_C)
             ▼
[Roda Belakang C (Ban Sepeda)]
```

### 1. Analisis Aliran Kinematika:
1. Peserta mengayuh pedal dengan kecepatan sudut $\omega_A$ (frekuensi kayuhan disebut *cadence*).
2. Gir depan $A$ memutar gir belakang $B$ melalui rantai:
   $$
   v_A = v_B \quad \Longrightarrow \quad \omega_B = \omega_A \left(\frac{N_A}{N_B}\right)
   $$
   Di mana rasio $\frac{N_A}{N_B}$ disebut **Rasio Gir (*Gear Ratio*)**.
3. Gir belakang $B$ dan roda belakang $C$ berada pada satu poros gandar:
   $$
   \omega_C = \omega_B = \omega_A \left(\frac{N_A}{N_B}\right)
   $$
4. Kelajuan laju sepeda di jalan aspal ($v_{\text{sepeda}}$) ditentukan oleh kelajuan linier tepi luar ban sepeda $C$ berjejari $r_C$:
   $$
   v_{\text{sepeda}} = v_C = \omega_C \cdot r_C = \omega_A \left(\frac{N_A}{N_B}\right) r_C
   $$

### 2. Mengapa Ada Pilihan Gir Tanjakan vs Gir Datar?
- **Medan Menanjak (Mengejar Torsi / Ringan Dikuasai):** Kita memilih gir depan kecil ($N_A$ kecil) dan gir belakang besar ($N_B$ besar). Rasio $\frac{N_A}{N_B}$ bernilai kecil (misal $34/32 \approx 1{,}06$). Setiap satu putaran kayuhan kaki hanya memutar roda belakang sekitar 1 kali putaran, sehingga kayuhan terasa sangat enteng meskipun laju sepeda lambat.
- **Medan Datar / Balapan Sprint (Mengejar Laju Kencang):** Kita memilih gir depan besar ($N_A$ besar) dan gir belakang kecil ($N_B$ kecil). Rasio $\frac{N_A}{N_B}$ bernilai besar (misal $53/11 \approx 4{,}82$). Setiap satu putaran kayuhan kaki akan memutar roda belakang hampir 5 kali putaran! Sepeda melaju sangat cepat, meskipun torsi kayuhan terasa berat.

---

## ✍️ Worked Examples: Contoh Soal & Analisis Terpandu

### Contoh Soal 1: Sistem Transmisi Tiga Roda Terpadu
Tiga buah roda $A$, $B$, dan $C$ dirangkai sedemikian rupa:
- Jari-jari roda $A$ adalah $r_A = 20\text{ cm}$.
- Jari-jari roda $B$ adalah $r_B = 10\text{ cm}$.
- Jari-jari roda $C$ adalah $r_C = 30\text{ cm}$.

Roda $A$ dihubungkan dengan roda $B$ menggunakan seutas sabuk tanpa selip. Roda $B$ dan roda $C$ dipasang seporos pada satu sumbu putar. Jika roda $A$ diputar dengan kecepatan sudut konstan $\omega_A = 6\text{ rad/s}$, tentukan:
a) Kecepatan sudut roda $B$ ($\omega_B$).  
b) Kecepatan sudut roda $C$ ($\omega_C$).  
c) Kelajuan linier tepi roda $C$ ($v_C$).

#### Pembahasan:
**Identifikasi Data:**
- $r_A = 0{,}2\text{ m}$, $r_B = 0{,}1\text{ m}$, $r_C = 0{,}3\text{ m}$.
- $\omega_A = 6\text{ rad/s}$.
- Hubungan $A$ dan $B$: Dihubungkan sabuk ($v_A = v_B$).
- Hubungan $B$ dan $C$: Seporos ($\omega_B = \omega_C$).

**Penyelesaian Bagian (a):**  
Karena roda $A$ dan $B$ dihubungkan sabuk:
$$
v_A = v_B \quad \Longrightarrow \quad \omega_A \cdot r_A = \omega_B \cdot r_B
$$
$$
6 \times 0{,}2 = \omega_B \times 0{,}1 \quad \Longrightarrow \quad \omega_B = \frac{1{,}2}{0{,}1} = 12 \text{ rad/s}
$$

**Penyelesaian Bagian (b):**  
Karena roda $B$ dan $C$ seporos:
$$
\omega_C = \omega_B = 12 \text{ rad/s}
$$

**Penyelesaian Bagian (c):**  
Kelajuan linier tepi roda $C$:
$$
v_C = \omega_C \cdot r_C = 12 \times 0{,}3 = 3{,}6 \text{ m/s}
$$
*Kesimpulan Fisis:* Dengan menyalurkan putaran dari roda besar $A$ ke roda kecil $B$, kecepatan sudut berlipat ganda dari $6\text{ rad/s}$ menjadi $12\text{ rad/s}$, dan ketika digandengkan seporos dengan roda besar $C$, kelajuan linier tepi yang dihasilkan melonjak tinggi mencapai $3{,}6\text{ m/s}$.

---

### Contoh Soal 2: Analisis Kecepatan Laju Sepeda Berdasarkan Rasio Gir
Seorang pesepeda mengayuh pedal sepedanya dengan irama kayuhan (*cadence*) tetap sebesar $60\text{ rpm}$. Sepeda tersebut memiliki gir depan (chainring) dengan $48$ gigi dan gir belakang (sprocket) dengan $16$ gigi. Diameter luar ban belakang sepeda adalah $70\text{ cm}$. Dengan menggunakan pendekatan $\pi \approx \frac{22}{7}$, hitunglah kelajuan laju sepeda tersebut di jalan raya dalam satuan $\text{km/jam}$!

#### Pembahasan:
**Identifikasi Data:**
- Irama kayuhan pedal: $n_{\text{pedal}} = 60\text{ rpm} \rightarrow f_A = \frac{60}{60} = 1\text{ Hz}$.
- Kecepatan sudut gir depan $A$: $\omega_A = 2\pi f_A = 2\pi(1) = 2\pi\text{ rad/s}$.
- Jumlah gigi: $N_A = 48$, $N_B = 16$.
- Diameter ban roda $C$: $D_C = 70\text{ cm} \rightarrow r_C = 35\text{ cm} = 0{,}35\text{ m} = \frac{7}{20}\text{ m}$.

**Langkah 1: Hitung Kecepatan Sudut Gir Belakang ($\omega_B$):**
Karena gir depan dan gir belakang dihubungkan rantai:
$$
N_A \cdot \omega_A = N_B \cdot \omega_B \quad \Longrightarrow \quad \omega_B = \omega_A \left(\frac{N_A}{N_B}\right)
$$
$$
\omega_B = 2\pi \times \left(\frac{48}{16}\right) = 2\pi \times 3 = 6\pi \text{ rad/s}
$$

**Langkah 2: Tentukan Kecepatan Sudut Roda Belakang ($\omega_C$):**
Karena gir belakang dan ban belakang seporos:
$$
\omega_C = \omega_B = 6\pi \text{ rad/s}
$$

**Langkah 3: Hitung Kelajuan Linier Sepeda ($v_C$):**
$$
v_C = \omega_C \cdot r_C = 6\pi \times 0{,}35 \text{ m/s}
$$
Substitusikan $\pi \approx \frac{22}{7}$:
$$
v_C = 6 \times \frac{22}{7} \times \frac{7}{20} = \frac{6 \times 22}{20} = \frac{132}{20} = 6{,}6 \text{ m/s}
$$

**Langkah 4: Konversi ke $\text{km/jam}$:**
$$
v_{\text{sepeda}} = 6{,}6 \times 3{,}6 = 23{,}76 \text{ km/jam}
$$
*Kesimpulan Fisis:* Dengan mengayuh santai 1 putaran per detik pada rasio gir $3:1$, pesepeda tersebut mampu melaju stabil di aspal dengan kecepatan $23{,}76\text{ km/jam}$.

---

> [!info] Navigasi Pembelajaran Terpadu
> [[Gerak Melingkar Beraturan SMA|🏠 Master Dashboard]] | [[Besaran Sudut dan Karakteristik GMB SMA|⏱️ Modul 1: Besaran Sudut & GMB]] | [[Percepatan Sentripetal dan Dinamika Melingkar SMA|🎯 Modul 2: Percepatan Sentripetal]] | **⚙️ Modul 3: Hubungan Roda-Roda** | [[LKPD Gerak Melingkar Beraturan SMA|📝 LKPD Inkuiri]] | [[Soal Gerak Melingkar Beraturan SMA|🎯 Soal Evaluasi]]
