---
title: "Impuls dan Momentum Linear — Master Guide & Analisis Tumbukan"
type: master-dashboard
subject: physics
level: sma
target_audience: "SMA Kelas XI"
created: 2026-09-08
sources:
  - "[[Dinamika Gerak SMA]]"
  - "[[Kinematika Gerak Lurus SMA]]"
  - "[[Konsep Impuls dan Momentum SMA]]"
  - "[[Hukum Kekekalan Momentum SMA]]"
  - "[[Tumbukan dan Koefisien Restitusi SMA]]"
tags:
  - fisika
  - impuls
  - momentum
  - tumbukan
  - kelas-11
  - modul-terpadu
  - kurikulum-merdeka
---

# Impuls dan Momentum Linear — Mengapa Tabrakan Bisa Menghancurkan atau Menyelamatkan Nyawa? 💥🚗

> 📍 **Navigasi Modul Terpadu:**  
> **[🏠 Master Dashboard]** | [[Konsep Impuls dan Momentum SMA|1. Konsep Impuls & Momentum]] | [[Hukum Kekekalan Momentum SMA|2. Kekekalan Momentum & Aplikasi]] | [[Tumbukan dan Koefisien Restitusi SMA|3. Tumbukan & Restitusi]] | 📝 [[LKPD Impuls dan Momentum SMA|LKPD Inkuiri]] | 🎯 [[Soal Impuls dan Momentum SMA|Paket Soal HOTS]]

Pernahkah kamu memperhatikan mengapa mobil balap modern yang menabrak pembatas sirkuit sengaja dirancang agar bagian depannya ringsek parah (*crumple zone*), bukannya dibuat dari baja super kaku yang tidak bisa penyok sama sekali? Mengapa pula pemain bisbol harus mengayunkan tongkatnya dan "mengikuti arah bola" (*follow through*), sementara petinju memakai sarung tangan tebal dan meloncat mundur saat menerima pukulan lawan?

Jawabannya berakar pada dua besaran fundamental fisika mekanika: **Momentum ($\vec{p}$)** dan **Impuls ($\vec{I}$)**. 

Jika pada [[Dinamika Gerak SMA|Dinamika Gerak]] kita menganalisis pengaruh gaya luar konstan terhadap percepatan benda melalui Hukum II Newton ($\sum \vec{F} = m\vec{a}$), maka di bab ini kita melangkah lebih jauh: kita membongkar peristiwa tabrakan, ledakan, lentingan, dan dorongan seketika di mana gaya kontak bekerja dalam fraksi waktu yang sangat singkat (**gaya impulsif**).

---

## 1. Peta Konsep Utama & Integrasi Sistem 🌌

Seluruh perjalanan belajar kita di bab ini terangkum dalam alur logika berikut:

![[infographic_physics_impuls_momentum_master.webp]]

### Struktur Tiga Pilar Pembelajaran:

| Modul | Fokus Bahasan | Pertanyaan Pemantik Utama |
| :--- | :--- | :--- |
| **[[Konsep Impuls dan Momentum SMA]]** | Definisi vektor $\vec{p}$, impuls $\vec{I}$, Teorema $\vec{I} = \Delta \vec{p}$, grafik $F-t$, dan rekayasa keselamatan. | *Bagaimana memperpanjang waktu kontak $\Delta t$ mampu menyelamatkan nyawa pengemudi dari gaya tumbukan maut?* |
| **[[Hukum Kekekalan Momentum SMA]]** | Sistem terisolasi, Hukum III Newton, efek tolak balik (*recoil*), propulsi roket, ayunan balistik, dan vektor 2D. | *Mengapa senapan terdorong ke belakang saat peluru melesat ke depan, dan bagaimana astronot bermanuver di ruang hampa?* |
| **[[Tumbukan dan Koefisien Restitusi SMA]]** | Lenting sempurna, lenting sebagian, tidak lenting sama sekali, koefisien restitusi $e$, dan pantulan bertingkat. | *Ke mana hilangnya energi kinetik saat dua mobil bertabrakan dan saling menempel, serta mengapa bola tenis tidak memantul setinggi semula?* |

---

## 2. Tabel Ringkasan Formula Terpadu (Master Cheatsheet) 📐

Di bawah ini adalah kompilasi rumus inti bab Impuls dan Momentum beserta legenda satuan internasional (SI):

| No | Konsep / Hukum Fisis | Persamaan Matematis | Keterangan & Catatan Kunci |
| :---: | :--- | :---: | :--- |
| 1 | **Momentum Linear** | $\vec{p} = m\vec{v}$ | Besaran vektor; arah momentum selalu searah dengan vektor kecepatan. |
| 2 | **Impuls Gaya Konstan** | $\vec{I} = \vec{F} \Delta t$ | Perkalian gaya rata-rata dengan selang waktu kontak sentuh. |
| 3 | **Impuls Gaya Variabel** | $I = \int_{t_1}^{t_2} F(t)\,dt$ | Secara grafis ekuivalen dengan **Luas Area di bawah kurva grafik $F - t$**. |
| 4 | **Teorema Impuls-Momentum** | $\vec{I} = \Delta \vec{p} = m\vec{v}' - m\vec{v}$ | Impuls total yang bekerja pada benda sama dengan perubahan momentum benda. |
| 5 | **Gaya Rata-Rata Impulsif** | $\vec{F}_{\text{rata}} = \frac{\Delta \vec{p}}{\Delta t} = \frac{m(\vec{v}' - \vec{v})}{\Delta t}$ | Semakin singkat $\Delta t$, semakin raksasa gaya benturan $\vec{F}$ yang dirasakan. |
| 6 | **Hukum Kekekalan Momentum** | $m_1\vec{v}_1 + m_2\vec{v}_2 = m_1\vec{v}_1' + m_2\vec{v}_2'$ | Berlaku mutlak pada sistem terisolasi ($\sum \vec{F}_{\text{luar}} = 0$). |
| 7 | **Tolak Balik Senapan / Roket** | $0 = m_s v_s' + m_p v_p' \implies v_s' = -\frac{m_p}{m_s}v_p'$ | Kecepatan tolak balik senapan berlawanan arah dengan gerak peluru. |
| 8 | **Koefisien Restitusi ($e$)** | $e = -\frac{v_1' - v_2'}{v_1 - v_2}$ | Mengukur elastisitas tumbukan: $0 \le e \le 1$. |
| 9 | **Tumbukan Tidak Lenting** | $v' = \frac{m_1 v_1 + m_2 v_2}{m_1 + m_2}$ | Kedua benda menempel dan bergerak bersama ($e = 0$). |
| 10 | **Pantulan Bola pada Lantai** | $e = \sqrt{\frac{h_1}{h_0}} = \sqrt{\frac{h_2}{h_1}} = \sqrt{\frac{h_n}{h_{n-1}}}$ | $h_0$ = tinggi awal, $h_1$ = tinggi pantulan ke-1, $h_2$ = pantulan ke-2. |
| 11 | **Ayunan Balistik (Pengayaan)** | $v_{\text{peluru}} = \left(\frac{m + M}{m}\right) \sqrt{2gh}$ | Integrasi kekekalan momentum saat tumbukan + energi mekanik saat ayunan naik. |

### Legenda Variabel & Satuan Standar:
- $p$ = Momentum linear ($\text{kg}\cdot\text{m/s}$)
- $m$ = Massa partikel/benda ($\text{kg}$)
- $v, \vec{v}$ = Kecepatan awal benda sebelum tumbukan ($\text{m/s}$)
- $v', \vec{v}'$ = Kecepatan akhir benda sesudah tumbukan ($\text{m/s}$)
- $I, \vec{I}$ = Impuls gaya ($\text{N}\cdot\text{s}$ atau $\text{kg}\cdot\text{m/s}$)
- $F, \vec{F}$ = Gaya kontak / gaya impulsif ($\text{N}$)
- $\Delta t$ = Selang waktu kontak durasi benturan ($\text{s}$)
- $e$ = Koefisien elastisitas restitusi (tanpa satuan, $0 \le e \le 1$)
- $h_0, h_1, h_2$ = Tinggi jatuh awal dan tinggi pantulan ($m$)
- $g$ = Percepatan gravitasi bumi ($\approx 9{,}8\text{ m/s}^2$ atau $10\text{ m/s}^2$)

---

## 3. Hubungan Prasyarat & Peta Kesiapan Belajar 🔗

Sebelum mempelajari bab ini secara mendalam, pastikan kamu telah menguasai konsep-konsep berikut:
1. **[[Kinematika Gerak Lurus SMA]]**: Penentuan vektor kecepatan $\vec{v}$, kelajuan, percepatan, serta analisis gerak jatuh bebas ($v = \sqrt{2gh}$).
2. **[[Dinamika Gerak SMA]]**: Konsep Hukum I, II, dan III Newton (gaya aksi-reaksi) serta penguraian gaya vektor pada sumbu kartesius.

---

> 🚀 **Siap mulai belajar?**  
> Langsung buka modul pertama kita: **[[Konsep Impuls dan Momentum SMA|Modul 1: Konsep Impuls, Momentum, & Teorema Impuls-Momentum ➡️]]**
