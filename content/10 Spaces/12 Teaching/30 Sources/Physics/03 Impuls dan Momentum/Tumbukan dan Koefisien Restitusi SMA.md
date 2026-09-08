---
title: "Klasifikasi Tumbukan dan Koefisien Restitusi"
type: materi
subject: physics
level: sma
target_audience: "SMA Kelas XI"
created: 2026-09-08
sources:
  - "[[Impuls dan Momentum SMA]]"
  - "[[Konsep Impuls dan Momentum SMA]]"
  - "[[Hukum Kekekalan Momentum SMA]]"
tags:
  - fisika
  - tumbukan
  - lenting-sempurna
  - lenting-sebagian
  - tidak-lenting
  - koefisien-restitusi
  - pantulan-bola
  - kelas-11
---

# Klasifikasi Tumbukan dan Koefisien Restitusi — Membedah Nasib Energi Saat Benda Bertabrakan! 🎱💥

> 📍 **Navigasi Modul:**  
> [[Impuls dan Momentum SMA|🏠 Master Dashboard]] | [[Konsep Impuls dan Momentum SMA|1. Konsep Impuls & Momentum]] | [[Hukum Kekekalan Momentum SMA|⬅️ 2. Kekekalan Momentum & Aplikasi]] | **[3. Tumbukan & Restitusi]** | 📝 [[LKPD Impuls dan Momentum SMA|LKPD Inkuiri ➡️]]

Ketika kamu menjatuhkan bola karet (*superball*) ke lantai keramik, bola itu melenting kembali mendekati ketinggian semula. Tetapi, jika kamu menjatuhkan bola tenis, tinggi pantulannya hanya sekitar setengah dari tinggi mula-mula. Dan jika kamu menjatuhkan segumpal tanah liat (*plastisin*), tanah liat itu langsung menempel gepeng di lantai tanpa memantul sama sekali!

Mengapa benda-benda tersebut berperilaku sangat berbeda saat bertabrakan? Padahal, pada semua peristiwa tabrakan tersebut, **Hukum Kekekalan Momentum Linear selalu berlaku**!

Pembeda utama dari ketiga peristiwa di atas terletak pada **nasib energi kinetiknya**: apakah energi kinetik sistem tetap utuh, terdisipasi sebagian, atau hilang secara maksimal menjadi kalor, bunyi, dan perubahan bentuk permanen.

---

## 1. Peta Matriks Tiga Jenis Tumbukan 🔍

Berikut adalah ringkasan visual yang mengklasifikasikan tiga jenis tumbukan dalam mekanika:

![[diagram_physics_jenis_tumbukan_klasifikasi.webp]]

### Tabel Komparasi Karakteristik Fisis Tumbukan:

| Kategori Tumbukan | Nilai Koefisien Restitusi ($e$) | Hukum Kekekalan Momentum | Hukum Kekekalan Energi Kinetik | Kondisi Pasca Tumbukan |
| :--- | :---: | :---: | :---: | :--- |
| **Lenting Sempurna** (*Elastic Collision*) | $e = 1$ | Berlaku ($\sum \vec{p} = \sum \vec{p}'$) | **Berlaku** ($\sum E_k = \sum E_k'$) | Benda memantul sempurna, tidak ada panas atau deformasi. |
| **Lenting Sebagian** (*Partially Inelastic*) | $0 < e < 1$ | Berlaku ($\sum \vec{p} = \sum \vec{p}'$) | **Tidak Berlaku** ($\sum E_k > \sum E_k'$) | Benda memantul dengan tinggi/kelajuan berkurang; timbul bunyi & panas. |
| **Tidak Lenting Sama Sekali** (*Completely Inelastic*) | $e = 0$ | Berlaku ($\sum \vec{p} = \sum \vec{p}'$) | **Tidak Berlaku** (Kehilangan $E_k$ Maksimal) | **Benda menempel dan bergerak bersama** ($v_1' = v_2' = v'$). |

---

## 2. Hakikat Koefisien Restitusi ($e$) 📐

Secara kuantitatif, tingkat elastisitas atau kelentingan suatu tumbukan dinyatakan oleh sebuah bilangan murni tanpa dimensi yang disebut **Koefisien Restitusi ($e$)**.

Koefisien restitusi didefinisikan sebagai **perbandingan negatif antara selisih kecepatan relatif kedua benda sesudah tumbukan dengan selisih kecepatan relatif kedua benda sebelum tumbukan**:

$$
e = -\frac{v_1' - v_2'}{v_1 - v_2} = \frac{v_2' - v_1'}{v_1 - v_2}
$$

**Legenda Variabel:**
- $e$ = Koefisien restitusi elastisitas ($0 \le e \le 1$)
- $v_1, v_2$ = Kecepatan benda 1 dan benda 2 sebelum tumbukan ($\text{m/s}$)
- $v_1', v_2'$ = Kecepatan benda 1 dan benda 2 sesudah tumbukan ($\text{m/s}$)

> [!TIP]
> **Trik Mengingat Rumus Restitusi:**  
> Bentuk paling mudah untuk diingat adalah:
> 
> $$
> v_2' - v_1' = -e(v_2 - v_1)
> $$
> 
> Artinya, kecepatan pisah kedua benda sesudah tumbukan selalu sebanding dengan kecepatan datangnya sebelum tumbukan, namun arah relatifnya terbalik dan tereduksi sebesar faktor $e$!

---

## 3. Kasus Khusus: Bola Memantul Berulang pada Lantai Diam 🎾🏢

Bayangkan sebuah bola bermassa $m$ dijatuhkan bebas tanpa kecepatan awal dari ketinggian $h_0$ di atas lantai keramik horizontal yang sangat masif.

Karena massa lantai bumi dianggap tak berhingga ($M_{\text{lantai}} \to \infty$), lantai tidak bergerak sama sekali sebelum maupun sesudah ditumbuk bola ($v_2 = 0$ dan $v_2' = 0$).

Dari rumus gerak jatuh bebas [[Kinematika Gerak Lurus SMA|Kinematika]]:
1. Kelajuan sesaat sebelum menyentuh lantai (arah ke bawah):  
   $$v_1 = -\sqrt{2gh_0}$$
2. Kelajuan sesaat setelah memantul naik (arah ke atas):  
   $$v_1' = +\sqrt{2gh_1}$$

Masukkan nilai ini ke rumus koefisien restitusi:

$$
e = -\frac{v_1' - v_2'}{v_1 - v_2} = -\frac{\sqrt{2gh_1} - 0}{-\sqrt{2gh_0} - 0}
$$

Tanda minus saling menghilangkan, dan faktor $\sqrt{2g}$ tereliminasi, sehingga menghasilkan rumus emas:

$$
e = \sqrt{\frac{h_1}{h_0}}
$$

Jika bola tersebut terus memantul berulang-ulang pada lantai yang sama, nilai $e$ dari pantulan ke pantulan berikutnya bernilai konstan:

$$
e = \sqrt{\frac{h_1}{h_0}} = \sqrt{\frac{h_2}{h_1}} = \sqrt{\frac{h_3}{h_2}} = \dots = \sqrt{\frac{h_n}{h_{n-1}}}
$$

### Ketinggian Pantulan ke-$n$:
Jika persamaan di atas dikuadratkan berturut-turut, kita peroleh rumus umum ketinggian pantulan ke-$n$:

$$
h_n = h_0 \cdot e^{2n}
$$

**Legenda Variabel:**
- $e$ = Koefisien restitusi antara bola dengan lantai
- $h_0$ = Ketinggian awal bola dijatuhkan ($m$)
- $h_1$ = Ketinggian puncak pantulan pertama ($m$)
- $h_2$ = Ketinggian puncak pantulan kedua ($m$)
- $h_n$ = Ketinggian puncak pantulan ke-$n$ ($m$)

---

## 4. Trik Super Analitis (Pro-Tips) Pengerjaan Soal 💡🚀

### Trik 1: Tumbukan Lenting Sempurna Dua Massa Identik ($m_1 = m_2$)
Jika dua benda memiliki massa yang sama persis ($m_1 = m_2$) dan bertumbukan lenting sempurna ($e = 1$) dalam satu garis lurus:
- **Kecepatan kedua benda saling bertukar posisi!**
- $$v_1' = v_2$$
- $$v_2' = v_1$$
*(Contoh nyata: Ayunan bola Newton's Cradle atau bola biliar nomor 1 menabrak bola biliar nomor 2 yang sedang diam, maka bola 1 langsung berhenti dan bola 2 melesat dengan kecepatan bola 1).*

### Trik 2: Formula Cepat Tumbukan Tidak Lenting Sama Sekali ($e = 0$)
Karena kedua benda menempel setelah tumbukan, mereka memiliki kecepatan akhir gabungan yang sama ($v_1' = v_2' = v'$):

$$
m_1 v_1 + m_2 v_2 = (m_1 + m_2)v'
$$

$$
v' = \frac{m_1 v_1 + m_2 v_2}{m_1 + m_2}
$$

Energi kinetik yang hilang (berubah jadi panas dan deformasi):

$$
\Delta E_k = E_{k,\text{awal}} - E_{k,\text{akhir}} = \left(\frac{1}{2}m_1 v_1^2 + \frac{1}{2}m_2 v_2^2\right) - \frac{1}{2}(m_1 + m_2)(v')^2
$$

---

## 5. Contoh Soal Terbimbing & Analisis Sistematis 🧠✍️

### Contoh Soal 1: Tumbukan Lenting Sempurna Dua Bola (Level Standar)
Bola A bermassa $2\text{ kg}$ bergerak ke kanan dengan kelajuan $6\text{ m/s}$ menumbuk bola B bermassa $1\text{ kg}$ yang sedang bergerak ke kiri dengan kelajuan $3\text{ m/s}$. Jika tumbukan antara kedua bola bersifat lenting sempurna ($e = 1$), tentukan kecepatan masing-masing bola sesaat setelah tumbukan!

**Pembahasan:**
Diketahui:
- $m_A = 2\text{ kg}$, $v_A = +6\text{ m/s}$
- $m_B = 1\text{ kg}$, $v_B = -3\text{ m/s}$ (ke kiri bertanda negatif)
- $e = 1$

**Langkah 1: Terapkan Persamaan Koefisien Restitusi**
$$
e = -\frac{v_A' - v_B'}{v_A - v_B} \implies 1 = -\frac{v_A' - v_B'}{6 - (-3)}
$$

$$
1 = -\frac{v_A' - v_B'}{9} \implies v_B' - v_A' = 9
$$

$$
v_B' = v_A' + 9 \quad \text{...(Persamaan 1)}
$$

**Langkah 2: Terapkan Hukum Kekekalan Momentum**
$$
m_A v_A + m_B v_B = m_A v_A' + m_B v_B'
$$

$$
2(6) + 1(-3) = 2 v_A' + 1 v_B'
$$

$$
12 - 3 = 2 v_A' + v_B' \implies 2 v_A' + v_B' = 9 \quad \text{...(Persamaan 2)}
$$

**Langkah 3: Substitusi Persamaan 1 ke Persamaan 2**
$$
2 v_A' + (v_A' + 9) = 9
$$

$$
3 v_A' + 9 = 9 \implies 3 v_A' = 0 \implies v_A' = 0\text{ m/s}
$$

Substitusi nilai $v_A' = 0$ ke Persamaan 1:
$$
v_B' = 0 + 9 = +9\text{ m/s}
$$

*Kesimpulan:*  
Setelah tumbukan, bola A langsung berhenti ($v_A' = 0$), sedangkan bola B terpental ke arah kanan dengan kelajuan $9\text{ m/s}$.

---

### Contoh Soal 2: Tumbukan Tidak Lenting Sama Sekali & Disipasi Energi (Level Penerapan)
Sebuah gerbong kereta bermassa $10.000\text{ kg}$ melaju dengan kecepatan $4\text{ m/s}$ di rel lurus. Gerbong tersebut menabrak gerbong kedua bermassa $15.000\text{ kg}$ yang sedang diam. Kedua gerbong otomatis terkait dan bergerak bersama-sama.  
a. Tentukan kecepatan kedua gerbong setelah bertabrakan!  
b. Berapakah energi kinetik yang hilang selama proses tumbukan tersebut?

**Pembahasan:**
Diketahui:
- $m_1 = 10.000\text{ kg}$, $v_1 = 4\text{ m/s}$
- $m_2 = 15.000\text{ kg}$, $v_2 = 0\text{ m/s}$
- Tumbukan tidak lenting sama sekali ($e = 0 \implies v_1' = v_2' = v'$)

**a. Menghitung Kecepatan Bersama ($v'$):**
$$
m_1 v_1 + m_2 v_2 = (m_1 + m_2) v'
$$

$$
10.000(4) + 15.000(0) = (10.000 + 15.000) v'
$$

$$
40.000 = 25.000 v' \implies v' = \frac{40.000}{25.000} = 1{,}6\text{ m/s}
$$

**b. Menghitung Energi Kinetik yang Hilang ($\Delta E_k$):**
- Energi Kinetik Awal:
  $$E_{k,\text{awal}} = \frac{1}{2}m_1 v_1^2 + \frac{1}{2}m_2 v_2^2 = \frac{1}{2}(10.000)(4)^2 + 0 = 5.000 \times 16 = 80.000\text{ Joule}$$
- Energi Kinetik Akhir:
  $$E_{k,\text{akhir}} = \frac{1}{2}(m_1 + m_2)(v')^2 = \frac{1}{2}(25.000)(1{,}6)^2 = 12.500 \times 2{,}56 = 32.000\text{ Joule}$$
- Energi Kinetik yang Hilang:
  $$\Delta E_k = E_{k,\text{awal}} - E_{k,\text{akhir}} = 80.000 - 32.000 = 48.000\text{ Joule}$$

*Kesimpulan:* Kecepatan bersama setelah tumbukan adalah $1{,}6\text{ m/s}$ dan energi kinetik sebesar $48.000\text{ Joule}$ ($60\%$ dari energi awal!) hilang berubah menjadi energi panas dan deformasi sambungan gerbong.

---

### Contoh Soal 3: Pantulan Bola Bertingkat pada Lantai (Level HOTS)
Sebuah bola basket dijatuhkan dari ketinggian $4\text{ meter}$ di atas lantai beton. Pada pantulan pertama, bola mencapai ketinggian puncak $2{,}25\text{ meter}$. Tentukan:  
a. Nilai koefisien restitusi ($e$) antara bola dan lantai beton!  
b. Tinggi pantulan kedua ($h_2$) bola tersebut!

**Pembahasan:**
Diketahui:
- Ketinggian awal $h_0 = 4\text{ m}$
- Ketinggian pantulan ke-1: $h_1 = 2{,}25\text{ m}$

**a. Menghitung Koefisien Restitusi ($e$):**
$$
e = \sqrt{\frac{h_1}{h_0}} = \sqrt{\frac{2{,}25}{4}} = \frac{\sqrt{2{,}25}}{\sqrt{4}} = \frac{1{,}5}{2} = 0{,}75
$$

**b. Menghitung Tinggi Pantulan Kedua ($h_2$):**
Gunakan relasi kesebandingan restitusi:
$$
e = \sqrt{\frac{h_2}{h_1}} \implies e^2 = \frac{h_2}{h_1}
$$

$$
h_2 = h_1 \cdot e^2 = 2{,}25 \times (0{,}75)^2 = 2{,}25 \times \frac{9}{16} = \frac{20{,}25}{16} \approx 1{,}2656\text{ meter}
$$

*Kesimpulan:* Nilai koefisien restitusi adalah $0{,}75$ dan tinggi pantulan kedua adalah sekitar $1{,}27\text{ meter}$.

---

## 6. Rangkuman Intisari Modul 3 📌

1. **Tumbukan Lenting Sempurna ($e = 1$):** Kedua hukum kekekalan (Momentum dan Energi Kinetik) berlaku penuh tanpa disipasi energi sedikit pun.
2. **Tumbukan Lenting Sebagian ($0 < e < 1$):** Momentum kekal, tetapi sebagian energi kinetik berkurang berubah menjadi energi termal, akustik, dan deformasi.
3. **Tumbukan Tidak Lenting Sama Sekali ($e = 0$):** Benda menyatu setelah benturan ($v_1' = v_2'$), kehilangan energi kinetik mencapai nilai maksimum.
4. **Pantulan Bola Vertikal:** Mengikuti relasi akar perbandingan ketinggian $e = \sqrt{\frac{h_n}{h_{n-1}}}$, di mana tinggi pantulan ke-$n$ menyusut secara eksponensial $h_n = h_0 \cdot e^{2n}$.

---

> 🎯 **Uji Pemahaman & Praktik Laboratorium:**  
> Teori telah lengkap dikuasai! Sekarang saatnya kamu membuktikannya secara langsung melalui lembar eksperimen inkuiri dan menguji daya nalar fisikamu:  
> - 📝 **[[LKPD Impuls dan Momentum SMA|Lanjut ke Lembar Kerja Peserta Didik (LKPD Inkuiri) ➡️]]**  
> - 🎯 **[[Soal Impuls dan Momentum SMA|Uji Kemampuanmu di Paket Soal Evaluasi HOTS ➡️]]**
