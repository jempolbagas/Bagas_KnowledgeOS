---
title: "Hukum Kekekalan Momentum Linear dan Aplikasi Rekayasa"
type: materi
subject: physics
level: sma
target_audience: "SMA Kelas XI"
created: 2026-09-08
sources:
  - "[[Impuls dan Momentum SMA]]"
  - "[[Konsep Impuls dan Momentum SMA]]"
  - "[[Dinamika Gerak SMA]]"
tags:
  - fisika
  - hukum-kekekalan-momentum
  - recoil-senapan
  - roket-propulsi
  - ayunan-balistik
  - tumbukan-2d
  - kelas-11
---

# Hukum Kekekalan Momentum Linear — Dari Tolak Balik Senapan Hingga Menjelajah Antariksa! 🚀🎯

> 📍 **Navigasi Modul:**  
> [[Impuls dan Momentum SMA|🏠 Master Dashboard]] | [[Konsep Impuls dan Momentum SMA|⬅️ 1. Konsep Impuls & Momentum]] | **[2. Kekekalan Momentum & Aplikasi]** | [[Tumbukan dan Koefisien Restitusi SMA|3. Tumbukan & Restitusi ➡️]] | 📝 [[LKPD Impuls dan Momentum SMA|LKPD Inkuiri]]

Pernahkah kamu menonton adegan film di mana seorang astronot tiba-tiba terlepas dari tali pengamannya dan melayang tak berdaya di ruang hampa udara yang hening? Di luar angkasa tidak ada udara untuk berenang, tidak ada lantai untuk berpijak, dan tidak ada dinding untuk didorong. Bagaimana cara astronot itu bisa kembali mendekati stasiun luar angkasa?

Satu-satunya trik penyelamat adalah: astronot tersebut harus melepas tas peralatan atau kunci inggris yang dipegangnya, lalu **melemparnya sekuat tenaga ke arah yang menjauhi stasiun luar angkasa**! Sesaat setelah kunci inggris meluncur ke depan, tubuh sang astronot otomatis akan melayang mundur menuju stasiun!

Fenomena luar biasa ini bukan sihir, melainkan manifestasi dari salah satu hukum paling sakral di alam semesta: **Hukum Kekekalan Momentum Linear**.

---

## 1. Landasan Teoretis: Penurunan dari Hukum III Newton ⚖️

Mengapa momentum total suatu sistem bisa kekal (tidak berubah)? Mari kita tinjau dua benda (benda 1 bermassa $m_1$ dan benda 2 bermassa $m_2$) yang saling bertabrakan atau saling mendorong pada suatu lintasan tanpa dipengaruhi oleh gaya gesek atau gaya luar apa pun (**sistem terisolasi**, di mana $\sum \vec{F}_{\text{luar}} = 0$).

Berdasarkan **Hukum III Newton (Aksi-Reaksi)**, saat kedua benda bersentuhan selama selang waktu $\Delta t$, gaya kontak yang diberikan benda 1 pada benda 2 ($\vec{F}_{12}$) besarnya sama persis tetapi berlawanan arah dengan gaya kontak yang diberikan benda 2 pada benda 1 ($\vec{F}_{21}$):

$$
\vec{F}_{21} = -\vec{F}_{12}
$$

Kalikan kedua ruas dengan durasi kontak interaksi $\Delta t$:

$$
\vec{F}_{21} \Delta t = -\vec{F}_{12} \Delta t
$$

Mengingat bahwa $\vec{F}\Delta t = \vec{I} = \Delta \vec{p}$, maka:

$$
\Delta \vec{p}_1 = -\Delta \vec{p}_2
$$

$$
\Delta \vec{p}_1 + \Delta \vec{p}_2 = 0
$$

Perubahan momentum total sistem adalah nol! Ini berarti jumlah momentum sebelum interaksi sama persis dengan jumlah momentum setelah interaksi:

$$
(m_1\vec{v}_1' - m_1\vec{v}_1) + (m_2\vec{v}_2' - m_2\vec{v}_2) = 0
$$

Pindahkan suku-suku sebelum tumbukan ke ruas kiri dan setelah tumbukan ke ruas kanan:

$$
m_1\vec{v}_1 + m_2\vec{v}_2 = m_1\vec{v}_1' + m_2\vec{v}_2'
$$

$$
\sum \vec{p}_{\text{sebelum}} = \sum \vec{p}_{\text{sesudah}}
$$

**Legenda Variabel:**
- $m_1, m_2$ = Massa benda 1 dan benda 2 ($\text{kg}$)
- $\vec{v}_1, \vec{v}_2$ = Kecepatan awal benda 1 dan 2 sebelum interaksi ($\text{m/s}$)
- $\vec{v}_1', \vec{v}_2'$ = Kecepatan akhir benda 1 dan 2 sesudah interaksi ($\text{m/s}$)

> [!IMPORTANT]
> **Syarat Mutlak Berlakunya Hukum Kekekalan Momentum:**  
> Hukum ini hanya berlaku jika **resultan gaya luar yang bekerja pada sistem bernilai nol** ($\sum \vec{F}_{\text{luar}} = 0$). Gaya-gaya yang terjadi selama tumbukan, ledakan, atau penembakan hanyalah **gaya internal (aksi-reaksi)** yang saling meniadakan di dalam sistem.

---

## 2. Aplikasi 1: Efek Tolak Balik Senapan & Meriam (*Recoil Effect*) 🔫

Ketika sebuah senapan menembakkan peluru, mula-mula senapan dan peluru berada dalam keadaan diam bersama-sama. Artinya, momentum awal total sistem adalah nol ($p_{\text{awal}} = 0$).

Saat pelatuk ditarik, gas hasil ledakan mesiu mendorong peluru ke depan dengan momentum $+m_p v_p'$. Karena tidak ada gaya luar horizontal, momentum total setelah ledakan juga harus tetap nol:

$$
\sum p_{\text{awal}} = \sum p_{\text{akhir}}
$$

$$
0 = m_s v_s' + m_p v_p'
$$

$$
m_s v_s' = -m_p v_p' \implies v_s' = -\frac{m_p}{m_s} v_p'
$$

**Legenda Variabel:**
- $m_s$ = Massa senapan ($\text{kg}$)
- $m_p$ = Massa peluru ($\text{kg}$)
- $v_s'$ = Kecepatan tolak balik senapan (*recoil velocity*) ($\text{m/s}$)
- $v_p'$ = Kecepatan peluru saat melesat keluar moncong ($\text{m/s}$)

### Makna Fisis Tanda Minus & Massa Senapan:
1. **Tanda minus** menunjukkan senapan bergerak ke belakang (menyentak bahu penembak) berlawanan dengan arah melesatnya peluru.
2. Karena massa senapan ($m_s$) jauh lebih besar daripada massa peluru ($m_p$), maka kecepatan sentak senapan ($v_s'$) jauh lebih kecil daripada kecepatan peluru ($v_p'$). Itulah sebabnya meriam kuno sengaja dibuat dari besi cor yang sangat berat agar sentakan mundurnya tidak sampai merusak kapal perang!

---

## 3. Aplikasi 2: Prinsip Propulsi Roket di Luar Angkasa 🌌🔥

Bagaimana sebuah roket luar angkasa bisa mempercepat dirinya di ruang hampa yang tanpa atmosfer? Jawabannya persis sama dengan prinsip senapan: **roket terus-menerus "menembakkan" gas buang ke belakang!**

1. Bahan bakar cair dan oksidator di dalam tangki roket bereaksi di ruang pembakaran menghasilkan gas bersuhu dan bertekanan luar biasa tinggi.
2. Gas panas tersebut disemburkan keluar melalui nosel roket ke arah belakang dengan laju relatif yang sangat tinggi ($v_{\text{gas}}$), membawa momentum ke belakang ($\Delta p_{\text{gas}} < 0$).
3. Agar momentum total sistem (roket + bahan bakar) tetap kekal, badan roket mendapatkan dorongan momentum ke depan ($\Delta p_{\text{roket}} > 0$).
4. Gaya dorong roket (*thrust force*, $F_{\text{dorong}}$) dirumuskan melalui laju massa gas yang disemburkan tiap detik:

$$
F_{\text{dorong}} = v_{\text{rel}} \frac{\Delta m}{\Delta t}
$$

**Legenda Variabel:**
- $F_{\text{dorong}}$ = Gaya dorong ke depan yang dialami roket ($\text{N}$)
- $v_{\text{rel}}$ = Kecepatan semburan gas relatif terhadap badan roket ($\text{m/s}$)
- $\frac{\Delta m}{\Delta t}$ = Laju pembakaran massa bahan bakar per satuan waktu ($\text{kg/s}$)

---

## 4. Sub-Bahasan Pengayaan (Enrichment / Deep Dive) 🔬🚀

### A. Ayunan Balistik (Ballistic Pendulum): Mengukur Kecepatan Peluru Cepat
Sebelum ditemukannya sensor optik berkecepatan tinggi, para insinyur militer menggunakan **Ayunan Balistik** untuk mengukur kecepatan peluru yang melesat ratusan meter per detik. 

Alat ini terdiri dari balok kayu besar bermassa $M$ yang digantung oleh dua utas tali ringan sepanjang $L$. Peluru bermassa $m$ ditembakkan mendatar ke arah balok dengan kelajuan $v$, lalu peluru menancap dan bersarang di dalam balok. Akibat tumbukan tersebut, balok dan peluru bersama-sama berayun naik mencapai ketinggian maksimum $h$.

Analisis fisika ayunan balistik memadukan **dua hukum kekekalan secara berurutan**:

#### Tahap 1: Saat Tumbukan (Hukum Kekekalan Momentum Linear)
Karena proses penetrasi peluru ke dalam balok terjadi sangat cepat, gaya gravitasi luar belum sempat mengubah momentum horizontal sistem:

$$
m v + M(0) = (m + M) v'
$$

$$
v' = \frac{m}{m + M} v
$$

Di mana $v'$ adalah kelajuan balok bersama peluru sesaat setelah tumbukan selesai.

#### Tahap 2: Saat Ayunan Berayun Naik (Hukum Kekekalan Energi Mekanik)
Setelah tumbukan usai, sistem balok+peluru berayun naik melawan gravitasi. Energi kinetik tepat di titik terendah berubah seluruhnya menjadi energi potensial gravitasi di puncak ayunan setinggi $h$:

$$
E_{k} = E_{p}
$$

$$
\frac{1}{2}(m + M)(v')^2 = (m + M)gh
$$

$$
(v')^2 = 2gh \implies v' = \sqrt{2gh}
$$

Substitusikan nilai $v'$ ke persamaan tahap 1:

$$
\sqrt{2gh} = \frac{m}{m + M} v
$$

$$
v = \left(\frac{m + M}{m}\right) \sqrt{2gh}
$$

**Legenda Variabel:**
- $v$ = Kelajuan awal peluru sebelum menumbuk balok ($\text{m/s}$)
- $m$ = Massa peluru ($\text{kg}$)
- $M$ = Massa balok kayu ayunan ($\text{kg}$)
- $g$ = Percepatan gravitasi bumi ($\text{m/s}^2$)
- $h$ = Ketinggian vertikal kenaikan balok dari posisi setimbang ($m$)

---

### B. Tumbukan 2 Dimensi (2D Collision): Analisis Vektor pada Meja Biliar 🎱

Jika dua benda bertumbukan miring (tidak tepat berhadapan segaris), gerak sebelum dan sesudah tumbukan tersebar di dalam bidang $x-y$. Karena momentum adalah besaran vektor, hukum kekekalan momentum **wajib dipenuhi secara terpisah pada masing-masing komponen sumbu**:

#### Kekekalan Momentum Sumbu-$x$:
$$
\sum p_{x,\text{awal}} = \sum p_{x,\text{akhir}}
$$

$$
m_1 v_{1x} + m_2 v_{2x} = m_1 v_{1x}' + m_2 v_{2x}'
$$

#### Kekekalan Momentum Sumbu-$y$:
$$
\sum p_{y,\text{awal}} = \sum p_{y,\text{akhir}}
$$

$$
m_1 v_{1y} + m_2 v_{2y} = m_1 v_{1y}' + m_2 v_{2y}'
$$

Biasanya kita menggunakan dekomposisi trigonometri: $v_x = v \cos\theta$ dan $v_y = v \sin\theta$, di mana $\theta$ adalah sudut arah gerak terhadap sumbu horizontal.

---

## 5. Contoh Soal Terbimbing & Analisis Langkah Demi Langkah 🧠✍️

### Contoh Soal 1: Sentakan Tolak Balik Senapan (Level Fondasi)
Sebuah senapan bermassa $4\text{ kg}$ menembakkan peluru bermassa $20\text{ gram}$ dengan kelajuan mendatar $400\text{ m/s}$. Berapakah kelajuan tolak balik senapan saat menyentak bahu penembak?

**Pembahasan:**
Diketahui:
- Massa senapan $m_s = 4\text{ kg}$
- Massa peluru $m_p = 20\text{ g} = 0{,}02\text{ kg}$
- Kecepatan awal keduanya diam: $v_s = 0$ dan $v_p = 0$
- Kecepatan peluru keluar moncong: $v_p' = +400\text{ m/s}$ (ke kanan)

Gunakan Hukum Kekekalan Momentum:
$$
\sum p_{\text{awal}} = \sum p_{\text{akhir}}
$$

$$
0 = m_s v_s' + m_p v_p'
$$

$$
0 = 4(v_s') + 0{,}02(400)
$$

$$
4v_s' + 8 = 0 \implies 4v_s' = -8 \implies v_s' = -2\text{ m/s}
$$

*Kesimpulan:* Kelajuan sentak tolak balik senapan adalah $2\text{ m/s}$ dengan arah ke belakang (berlawanan dengan arah peluru).

---

### Contoh Soal 2: Orang Melompat dari Perahu Terapung (Level Penerapan)
Sebuah perahu bermassa $150\text{ kg}$ mula-mula diam mengapung di atas danau yang tenang. Seorang pria bermassa $50\text{ kg}$ yang berdiri di buritan perahu tiba-tiba melompat ke arah dermaga (ke kiri) dengan kelajuan horizontal $3\text{ m/s}$. Tentukan kelajuan dan arah gerak perahu sesaat setelah pria tersebut melompat!

**Pembahasan:**
Diketahui:
- Massa perahu $m_p = 150\text{ kg}$
- Massa orang $m_o = 50\text{ kg}$
- Kecepatan awal sistem: $v_p = 0$ dan $v_o = 0$
- Kecepatan pria melompat (ke kiri, kita beri tanda negatif): $v_o' = -3\text{ m/s}$

Gunakan Hukum Kekekalan Momentum:
$$
\sum p_{\text{awal}} = \sum p_{\text{akhir}}
$$

$$
0 = m_o v_o' + m_p v_p'
$$

$$
0 = 50(-3) + 150(v_p')
$$

$$
-150 + 150 v_p' = 0 \implies 150 v_p' = 150 \implies v_p' = +1\text{ m/s}
$$

*Kesimpulan:* Perahu bergerak dengan kelajuan $1\text{ m/s}$ ke arah kanan (menjauhi dermaga).

---

### Contoh Soal 3: Ayunan Balistik (Level Pengayaan & HOTS)
Dalam suatu uji balistik, sebutir peluru bermassa $10\text{ gram}$ ditembakkan secara mendatar ke dalam balok kayu bermassa $1{,}99\text{ kg}$ yang tergantung pada tali panjang. Peluru menancap sempurna di dalam balok kayu dan menyebabkan balok berayun naik hingga mencapai simpangan vertikal setinggi $h = 5\text{ cm}$. Jika percepatan gravitasi bumi $g = 9{,}8\text{ m/s}^2$, hitunglah kelajuan awal peluru sesaat sebelum mengenai balok!

**Pembahasan:**
Diketahui:
- Massa peluru $m = 10\text{ g} = 0{,}01\text{ kg}$
- Massa balok kayu $M = 1{,}99\text{ kg}$
- Massa total gabungan: $m + M = 0{,}01 + 1{,}99 = 2{,}00\text{ kg}$
- Ketinggian vertikal $h = 5\text{ cm} = 0{,}05\text{ m}$
- Gravitasi $g = 9{,}8\text{ m/s}^2$

**Langkah 1: Hitung kelajuan balok + peluru sesaat setelah tumbukan ($v'$)**
$$
v' = \sqrt{2gh} = \sqrt{2 \times 9{,}8 \times 0{,}05} = \sqrt{0{,}98 \times 1} = \sqrt{0{,}98} \approx 0{,}9899\text{ m/s}
$$
*(Atau jika menggunakan $g = 10\text{ m/s}^2$: $v' = \sqrt{2 \times 10 \times 0{,}05} = \sqrt{1} = 1\text{ m/s}$)*. Mari gunakan $g = 9{,}8\text{ m/s}^2$:

$$
v' = \sqrt{0{,}98}\text{ m/s}
$$

**Langkah 2: Hitung kelajuan awal peluru ($v$) via kekekalan momentum**
$$
v = \left(\frac{m + M}{m}\right) v'
$$

$$
v = \left(\frac{2{,}00\text{ kg}}{0{,}01\text{ kg}}\right) \sqrt{0{,}98} = 200 \times 0{,}9899 \approx 197{,}99\text{ m/s}
$$
*(Jika dengan $g = 10\text{ m/s}^2$, diperoleh tepat $v = 200 \times 1 = 200\text{ m/s}$)*.

*Kesimpulan:* Kelajuan peluru yang ditembakkan adalah sekitar $198\text{ m/s}$ (atau $200\text{ m/s}$ jika dibulatkan dengan $g = 10\text{ m/s}^2$).

---

## 6. Rangkuman Intisari Modul 2 📌

1. **Hukum Kekekalan Momentum:** Pada setiap sistem tertutup/terisolasi yang bebas dari gaya luar netto ($\sum \vec{F}_{\text{luar}} = 0$), momentum total sistem sebelum interaksi selalu sama persis dengan momentum total sesudah interaksi.
2. **Asal-Usul Hukum:** Kekekalan momentum merupakan konsekuensi langsung dari Hukum III Newton (gaya aksi-reaksi internal bernilai sama dan berlawanan arah).
3. **Efek Tolak Balik (*Recoil*):** Penembakan peluru, loncatan dari perahu, atau propulsi roket terjadi karena pelepasan massa ke satu arah mewajibkan sisa sistem terdorong ke arah yang berlawanan demi menjaga momentum total tetap kekal.
4. **Ayunan Balistik:** Mengintegrasikan dua konsep: Kekekalan Momentum saat tabrakan/penetrasi dan Kekekalan Energi Mekanik saat ayunan berayun ke atas.

---

> ➡️ **Langkah Selanjutnya:**  
> Kita sudah mempelajari apa yang terjadi pada momentum saat tabrakan. Namun, bagaimana dengan energi kinetik benda saat bertabrakan? Mengapa beberapa tabrakan memantul sempurna, sementara yang lain saling menempel dan mengeluarkan panas?  
> Simak jawabannya di: **[[Tumbukan dan Koefisien Restitusi SMA|Modul 3: Klasifikasi Tumbukan & Koefisien Restitusi ➡️]]**
