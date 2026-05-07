# SlideForge — HTML Slide Generator

> Buat presentasi HTML profesional langsung di browser — tanpa coding, tanpa instalasi framework.

SlideForge adalah aplikasi web berbasis satu file HTML yang memungkinkan Anda merancang, mengkustomisasi, dan mengekspor presentasi siap pakai dalam format `.html` mandiri. Cukup buka di browser, desain slide Anda, lalu unduh hasilnya.

---

## Daftar Isi

1. [Prasyarat](#1-prasyarat)
2. [Instalasi & Menjalankan Aplikasi](#2-instalasi--menjalankan-aplikasi)
3. [Quick Start: Panduan Penggunaan Dasar](#3-quick-start-panduan-penggunaan-dasar)
4. [Kustomisasi Lanjutan](#4-kustomisasi-lanjutan)
5. [Cara Ekspor Presentasi](#5-cara-ekspor-presentasi)
6. [Referensi Fitur](#6-referensi-fitur)
7. [Troubleshooting](#7-troubleshooting)

---

## 1. Prasyarat

SlideForge dirancang agar **tidak memerlukan instalasi apapun** untuk penggunaan standar. Namun, pastikan kondisi berikut terpenuhi:

| Kebutuhan | Versi Minimum | Keterangan |
|---|---|---|
| Web Browser | Terkini (2022+) | Chrome, Firefox, Edge, atau Safari |
| Koneksi Internet | Opsional | Hanya diperlukan untuk memuat logo dari URL eksternal |
| Node.js | — | **Tidak diperlukan** |
| Server lokal | — | **Tidak diperlukan** |

> **Catatan:** Fitur Google Fonts (font DM Sans) membutuhkan koneksi internet saat pertama kali dibuka. Setelah itu, font akan di-cache oleh browser.

---

## 2. Instalasi & Menjalankan Aplikasi

### Langkah 1: Unduh File Aplikasi

Simpan file `html-slide-generator.html` ke komputer Anda. File ini adalah satu-satunya file yang dibutuhkan.

```
📁 Folder Anda/
└── html-slide-generator.html   ← file tunggal aplikasi
```

### Langkah 2: Buka di Browser

Klik dua kali file tersebut, atau buka browser Anda dan seret file ke jendela browser:

```
# Cara cepat via terminal (opsional):

# macOS
open html-slide-generator.html

# Windows (PowerShell)
start html-slide-generator.html

# Linux
xdg-open html-slide-generator.html
```

### Langkah 3: Verifikasi

Aplikasi berhasil berjalan jika Anda melihat tampilan editor dua panel:
- Panel kiri → Kontrol & konfigurasi slide
- Panel kanan → Live preview slide aktif

> **Tips:** Untuk pengalaman terbaik, gunakan browser dalam mode layar penuh (`F11`).

---

## 3. Quick Start: Panduan Penggunaan Dasar

### 3.1 Membuat dan Mengelola Slide

1. Buka tab **"Slides"** di panel kiri.
2. Klik tombol **"+ Tambah Slide"** untuk menambahkan slide baru.
3. Klik salah satu item di daftar slide untuk memilih dan mengeditnya.
4. Untuk menghapus slide, arahkan kursor ke item slide — tombol **✕** akan muncul di sisi kanan.

> Urutan slide sesuai urutan daftar. Navigasi antar slide menggunakan tombol **‹** dan **›** di atas area preview.

### 3.2 Memasukkan Konten Slide

1. Pilih slide yang ingin diedit dari daftar.
2. Buka tab **"Konten"**.
3. Pilih **tipe slide** yang sesuai dari grid pilihan di bagian atas:

| Tipe Slide | Kegunaan |
|---|---|
| **Cover** | Slide pembuka/judul utama presentasi |
| **Judul** | Pemisah antar bagian (section divider) |
| **Poin** | Daftar bullet points atau teks paragraf |
| **2 Kolom** | Perbandingan atau konten dua sisi |
| **Kutipan** | Menampilkan quote atau testimonial |
| **Penutup** | Slide akhir presentasi |

4. Isi bidang **"Judul"** dan **"Subjudul / Deskripsi"**.

**Format bullet points** pada tipe slide "Poin": awali setiap baris dengan `•` atau `-`:

```
• Poin pertama yang ingin disampaikan
• Poin kedua dengan penjelasan singkat
- Poin ketiga (tanda strip juga berfungsi)
```

5. Isi **"Catatan Speaker"** jika diperlukan — catatan ini tidak tampil di slide, tetapi tersimpan sebagai komentar dalam file HTML hasil ekspor.

### 3.3 Memasang Logo Brand

1. Buka tab **"Desain"**.
2. Pada bidang **"URL Logo"**, masukkan alamat URL gambar logo Anda.

```
Contoh URL logo yang valid:
https://upload.wikimedia.org/wikipedia/commons/thumb/a/a9/Amazon_logo.svg/2560px-Amazon_logo.svg.png
```

3. Logo akan langsung muncul di pojok kiri atas setiap slide pada preview.

> **Jika tidak memiliki URL logo:** Kosongkan bidang URL Logo. Nama brand pada bidang **"Nama Brand"** akan ditampilkan sebagai teks pengganti.

### 3.4 Memilih Warna Brand

1. Pada tab **"Desain"**, temukan bagian **"Warna"**.
2. Klik kotak warna **Primary** (kiri) untuk membuka color picker — pilih warna utama brand Anda.
3. Klik kotak warna **Secondary** (kanan) untuk memilih warna aksen.
4. Gradient strip di atas kotak warna memberikan pratinjau kombinasi kedua warna secara real-time.

> Warna Primary digunakan pada aksen garis, bullet dots, dan elemen dekoratif utama. Warna Secondary digunakan pada gradient dan elemen pendukung.

### 3.5 Memilih Animasi Transisi

1. Buka tab **"Animasi"**.
2. Pilih salah satu dari 6 jenis **Transisi Slide**:

| Efek | Deskripsi |
|---|---|
| **Fade** | Transisi memudar halus (direkomendasikan untuk presentasi formal) |
| **Slide** | Slide bergeser ke samping |
| **Zoom** | Slide muncul dengan efek zoom |
| **Flip** | Rotasi 3D horizontal |
| **Reveal** | Slide terungkap dari kiri ke kanan |
| **None** | Pergantian langsung tanpa animasi |

3. Pilih **Animasi Konten** untuk mengatur cara elemen muncul di dalam slide:

| Efek | Deskripsi |
|---|---|
| **Stagger** | Elemen muncul berurutan dari atas ke bawah |
| **Rise Up** | Elemen naik dari bawah satu per satu |
| **Pop** | Elemen muncul dengan efek bounce |
| **None** | Semua elemen muncul sekaligus |

---

## 4. Kustomisasi Lanjutan

### 4.1 Mengubah CSS Variables untuk Warna Brand

File hasil ekspor menggunakan **CSS Custom Properties** (variabel) sehingga mudah dimodifikasi tanpa mengubah seluruh kode. Buka file `.html` hasil ekspor dengan teks editor, lalu temukan dan ubah nilai berikut:

```css
/* Ubah nilai hex sesuai panduan brand Anda */
--color-primary: #7c6af7;    /* Warna utama brand */
--color-secondary: #06b6d4;  /* Warna aksen/sekunder */
```

**Contoh penerapan warna brand perusahaan:**

```css
/* Contoh: Brand dengan identitas merah-emas */
--color-primary: #c0392b;
--color-secondary: #f39c12;
```

### 4.2 Mengganti Font Keseluruhan

Pada tab **"Desain"** → bagian **"Tipografi"**, tersedia 4 pilihan font:

| Pilihan | Font Stack | Karakter |
|---|---|---|
| **DM Sans** | DM Sans, Segoe UI | Modern, bersih, mudah dibaca |
| **Georgia** | Georgia, Times New Roman | Klasik, formal, elegan |
| **Mono** | Courier New, Courier | Teknikal, kode-estetik |
| **Display** | Impact, Arial Black | Tebal, impactful, dramatis |

Untuk font kustom di luar pilihan yang tersedia, buka file hasil ekspor dan modifikasi bagian `font-family` pada selector `body`:

```css
body {
  font-family: 'Nama Font Kustom', fallback-font, sans-serif;
}
```

Pastikan font telah di-import sebelum selector `body`:

```html
<link rel="preconnect" href="https://fonts.googleapis.com">
<link href="https://fonts.googleapis.com/css2?family=Plus+Jakarta+Sans:wght@400;600&display=swap" rel="stylesheet">
```

### 4.3 Mengubah Ukuran Judul

Gunakan slider **"Ukuran Judul"** pada tab Desain (rentang: 28px — 72px). Nilai ini menjadi acuan dasar ukuran teks; setiap tipe slide akan menyesuaikan secara proporsional.

### 4.4 Mengatur Tema Background

| Tema | Deskripsi | Cocok Untuk |
|---|---|---|
| **Dark** | Background gelap solid | Presentasi teknikal, startup |
| **Light** | Background terang/putih | Presentasi korporat, akademis |
| **Gradient** | Overlay gradient dari warna primary | Pitch deck, kreatif |
| **Glass** | Efek transparan berlapis | Modern, konferensi |

### 4.5 Toggle Elemen Antarmuka

Pada tab Desain, terdapat 4 toggle yang dapat diaktifkan/nonaktifkan:

| Toggle | Fungsi |
|---|---|
| **Nomor Slide** | Menampilkan "1/5" di pojok kanan atas setiap slide |
| **Logo** | Menampilkan logo atau nama brand di pojok kiri atas |
| **Progress Bar** | Bar tipis di bagian bawah yang menunjukkan progres presentasi |
| **Elemen Dekoratif** | Orbs cahaya abstrak sebagai elemen visual latar |

---

## 5. Cara Ekspor Presentasi

### 5.1 Ekspor sebagai File HTML Mandiri

1. Klik tombol **"Export HTML"** di pojok kanan atas aplikasi.
2. File akan otomatis diunduh dengan nama berdasarkan judul slide pertama Anda.
3. Buka file hasil unduhan di browser mana saja — tidak memerlukan server atau koneksi internet.

```
📁 Downloads/
└── judul-presentasi-anda.html   ← file presentasi mandiri
```

### 5.2 Cara Menjalankan Presentasi Hasil Ekspor

Buka file `.html` hasil ekspor di browser, kemudian gunakan kontrol berikut:

| Aksi | Tombol Keyboard | Alternatif |
|---|---|---|
| Slide berikutnya | `→` / `Space` / `Page Down` | Klik tombol **Next →** |
| Slide sebelumnya | `←` / `Page Up` | Klik tombol **← Prev** |
| Mode fullscreen | `F` | — |
| Keluar fullscreen | `Esc` | — |

> Kontrol navigasi (Next/Prev) akan muncul saat kursor diarahkan ke area presentasi. Dalam kondisi normal, tampilan bersih tanpa elemen antarmuka.

### 5.3 Berbagi Presentasi

File HTML hasil ekspor bersifat **sepenuhnya mandiri** (self-contained). Anda dapat:

- Mengirim via email sebagai lampiran
- Mengunggah ke Google Drive / Dropbox untuk dibagikan via link
- Menyimpan ke flashdisk untuk presentasi offline
- Mengunggah ke web hosting sebagai halaman statis

### 5.4 Preview Fullscreen Sebelum Ekspor

Klik tombol **"Preview"** di topbar untuk membuka presentasi dalam tab browser baru tanpa mengunduh file. Fitur ini berguna untuk pengujian tampilan akhir sebelum benar-benar diunduh.

---

## 6. Referensi Fitur

### Shortcut Keyboard (dalam Aplikasi Editor)

| Shortcut | Fungsi |
|---|---|
| `←` `→` (pada kontrol preview) | Navigasi antar slide |

### Struktur Data Slide

Setiap slide menyimpan data berikut secara internal:

```json
{
  "type": "bullets",
  "title": "Judul Slide",
  "subtitle": "• Poin pertama\n• Poin kedua",
  "col2": "",
  "speaker": "Catatan untuk presenter"
}
```

### Konfigurasi Design yang Tersimpan di Ekspor

| Parameter | Nilai Default | Deskripsi |
|---|---|---|
| `colorPrimary` | `#7c6af7` | Warna utama (ungu) |
| `colorSecondary` | `#06b6d4` | Warna aksen (teal) |
| `bgTheme` | `dark` | Tema background |
| `fontFamily` | `modern` | Keluarga font |
| `titleSize` | `48px` | Ukuran judul dasar |
| `transition` | `fade` | Jenis transisi antar slide |
| `duration` | `500ms` | Durasi animasi transisi |
| `autoAdvance` | `0` | Auto-advance (0 = manual) |

---

## 7. Troubleshooting

### Logo tidak muncul

**Gejala:** Bidang URL Logo sudah diisi, tetapi logo tidak tampil di preview.

**Solusi:**
1. Pastikan URL mengarah langsung ke file gambar (berakhiran `.png`, `.jpg`, `.svg`, dll.).
2. Pastikan server sumber gambar mengizinkan akses lintas domain (CORS). Gambar dari Wikipedia, Imgur, atau CDN publik umumnya aman.
3. Gunakan URL HTTPS, bukan HTTP.

### Font tidak terbaca / tampil sebagai font default

**Gejala:** Teks slide tampil dengan font sistem, bukan DM Sans.

**Solusi:** Pastikan ada koneksi internet saat membuka aplikasi. Font DM Sans dimuat dari Google Fonts. Setelah dimuat satu kali, browser akan menyimpannya dalam cache.

### Preview tidak memperbarui perubahan secara real-time

**Gejala:** Perubahan di panel editor tidak langsung tercermin di preview.

**Solusi:**
1. Coba klik area lain di luar bidang input untuk memicu pembaruan.
2. Pastikan JavaScript tidak diblokir oleh ekstensi browser (misalnya, ad blocker agresif).
3. Refresh halaman browser (`F5`) sebagai langkah terakhir (perhatian: data yang belum diekspor akan hilang).

### File hasil ekspor tidak dapat dibuka

**Gejala:** Browser menampilkan halaman kosong atau error saat membuka file `.html` ekspor.

**Solusi:**
1. Pastikan file diunduh secara utuh (periksa ukuran file — seharusnya lebih dari 30KB).
2. Coba buka dengan browser berbeda.
3. Jangan buka file langsung dari aplikasi ZIP/kompresi — ekstrak dulu ke folder.

---

## Lisensi & Kredit

Dibangun dengan teknologi web standar: HTML5, CSS3, dan JavaScript vanilla. Tidak menggunakan library pihak ketiga — semua berjalan murni dari satu file HTML.

Font: [DM Sans](https://fonts.google.com/specimen/DM+Sans) oleh Colophon Foundry, tersedia via Google Fonts (SIL Open Font License).

---

*Dokumentasi ini berlaku untuk SlideForge versi 1.0. Terakhir diperbarui: 2025.*
