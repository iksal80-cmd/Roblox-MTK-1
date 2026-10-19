# 🗺️ Petualangan Pulau Angka KRN

Game **petualangan 3D** bergaya kotak-kotak untuk **Matematika Kelas 1 · Bab 1: Bilangan sampai 10**
di **Kuttab Raudhah Nabawiyah (KRN)**. Materinya diambil dari Modul Ajar Matematika Kelas 1 (Jam ke-1 s.d. ke-11)
susunan Lala Meirani, S.E., PKBM Raudhah Nabawiyah.

**Kuttab Raudhah Nabawiyah** · PKBM Raudhah Parenting Nabawiyah Bogor
Jl. Bima Raya Ujung No. 31, Cibuluh, Bogor Utara, Kota Bogor, Jawa Barat
Telp +62 812-7272-7938 · www.raudhahnabawiyah.id

## Alur petualangan (11 pos = 11 jam pelajaran)

| Pos | Hewan | Materi | Tantangan |
|---|---|---|---|
| 1 | 🐰 Kelinci | Sama banyak & angka 3 | Hitung kelinci, pilih kelompok yang sama banyak, kumpulkan 3 wortel |
| 2 | 🦩 Flamingo | Angka 1 dan 2 | Hitung flamingo, pilih yang jumlahnya 1, kumpulkan 2 kunci |
| 3 | 🦆 Bebek | Angka 4 dan 5 | Hitung bebek di kolam & burung hantu di dahan, kumpulkan 5 telur |
| 4 | 🐻 Beruang | Balok 1–5 | Susun balok 3D sebanyak apel / angka |
| 5 | 🐳 Paus | Urutan 1–5 | Seberangi sungai lewat **batu angka** 1→2→3→4→5 (batu yang salah tenggelam) |
| 6 | 🐱 Kucing | Angka 6 dan 7 | Hitung melon, bandingkan melon dan orang, kumpulkan 7 jeruk |
| 7 | 🦉 Burung Hantu | Angka 8, 9, 10 | Hitung cangkir teh, kartu titik 9, kumpulkan 10 bintang |
| 8 | 🐦 Burung | Urutan 6–10 | Seberangi sungai kedua lewat batu angka 6→10 |
| 9 | 🦊 Rubah | Angka 0 | Burung terbang semua, kue dimakan habis, lempar gelang, lebih banyak |
| 10 | 🐢 Kura-kura | Lebih besar & urutan | Lewati **gerbang angka yang lebih besar** (10/9, 3/1, 7/5), naiki **Tangga Angka 1–10** |
| 11 | 🐼 Panda | Kartu angka & titik | Cocokkan kartu titik, gabungkan titik, urutkan kartu 1–10 |

- **Suara pemandu** membacakan setiap soal dan menghitung keras-keras ("satu, dua, tiga…") saat santri mengambil benda atau menyusun balok. Cocok untuk santri yang belum lancar membaca.
- Salah tidak dihukum. Santri cukup mencoba lagi. Setiap pos memberi 1–3 ⭐ sesuai banyaknya percobaan.
- Gerbang sekolah, gedung Kuttab, bendera, menu, dan **sertifikat** menampilkan logo dan alamat KRN.
- Progres tersimpan otomatis di perangkat.

## Kontrol

| Aksi | Laptop | HP / Tablet |
|---|---|---|
| Berjalan | W A S D / panah | Geser jempol di sisi kiri layar |
| Kamera | Seret mouse, scroll untuk zoom | Geser di sisi kanan layar |
| Lompat | Spasi | Tombol ⤒ |
| Bicara / serahkan barang | E | Tombol kuning |
| Peta | M | 🗺️ |

Disarankan memegang HP dalam posisi mendatar. Suara pemandu memakai suara bahasa Indonesia bawaan perangkat. Jika tidak terdengar, aktifkan bahasa Indonesia di pengaturan *Text-to-Speech* perangkat.

## Cara upload ke GitHub Pages

1. Buka [github.com](https://github.com) → **New repository** → beri nama, misalnya `pulau-angka` → **Public** → **Create repository**.
2. Klik **uploading an existing file**, seret `index.html` dan `README.md`, lalu **Commit changes**.
3. Buka **Settings → Pages** → *Source*: **Deploy from a branch** → branch **main**, folder **/ (root)** → **Save**.
4. Setelah 1–2 menit, game bisa dibuka di `https://NAMA-AKUN.github.io/pulau-angka/`.

Game membutuhkan internet saat pertama dibuka (untuk mesin 3D three.js). Logo KRN sudah tertanam di dalam file.

## Mengubah soal

Semua materi ada di bagian `const POS=[` di dalam `index.html`. Contoh:

```js
{t:'count', item:'rabbit', n:3, at:[4,-3], q:'Ada berapa kelinci kecil?'},
{t:'pick',  q:'Mana yang jumlahnya SATU?', opts:['🚢','✈️✈️','🚗🚗🚗'], a:0},
{t:'collect', item:'carrot', n:3, q:'Tolong kumpulkan 3 wortel untukku ya!'},
```

Pilihan jawaban bisa berupa emoji, teks, `'num:5'` (angka beserta titiknya), atau `'dots:8'` (kartu titik).

---
Game bergaya kotak-kotak buatan sendiri, tidak berafiliasi dengan Roblox. Mesin 3D: three.js.
