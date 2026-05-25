# 🏫 Landing Page Sistem Penerimaan Murid Baru (SPMB) 2026
> **SMK Budi Bakti Ciwidey** — Projek Tugas Kegiatan Kokurikuler Kejuruan (Slicing & Live Deployment)

---

## 📌 Gambaran Umum Projek
Aplikasi berbasis web ini merupakan sebuah halaman *landing page* resmi yang dirancang khusus untuk keperluan **Sistem Penerimaan Peserta Didik Baru (SPMB) SMK Budi Bakti Ciwidey Angkatan 2026/2027**. Projek ini dibangun sebagai implementasi nyata dari kompetensi keahlian Pengembangan Perangkat Lunak dan Gim (PPLG), khususnya dalam pemenuhan standardisasi industri terkait *UI Slicing*, manajemen repositori berbasis Git, serta *automated deployment*.

Website ini dirancang menggunakan pendekatan **Mobile-First Design** untuk memastikan calon siswa baru dapat mengakses informasi pendaftaran dengan sangat nyaman, cepat, dan responsif langsung melalui perangkat ponsel pintar mereka.

---

## 🚀 Tautan Live Project & Akses Dokumentasi
Dokumen dan hasil akhir pengerjaan aplikasi ini dapat diakses secara publik melalui tautan resmi di bawah ini:

* 🌐 **Live Website Preview:** [https://spmb-stellarpath-smkbbc.netlify.app](https://spmb-stellarpath-smkbbc.netlify.app)
* 📋 **Dokumen Kebutuhan Produk:** [Lihat Product Requirement Document (PRD.md)](PRD.md)

---

## ✨ Fitur Utama & Fungsionalitas Sistem

### 1. Desain Responsif Mutakhir (Adaptif Layout)
* **Desktop View:** Menampilkan struktur navigasi atas (*Header Navbar*) yang megah dengan susunan informasi grid multi-kolom yang luas.
* **Mobile View:** Otomatis menyembunyikan navbar atas dan mengaktifkan komponen **Sticky Mobile Bottom Navigation** di bagian bawah layar untuk mengoptimalkan jangkauan ibu jari pengguna.

### 2. Showcase Program Keahlian (Kompetensi Keahlian)
* Menampilkan informasi interaktif untuk 3 program keahlian utama di SMK Budi Bakti Ciwidey:
  * **PPLG** (Pengembangan Perangkat Lunak dan Gim)
  * **DKV** (Desain Komunikasi Visual)
  * **BRP** (Broadcasting dan Perfilman)
* Pada layar HP, komponen ini ditransformasikan menjadi sistem geser yang hemat ruang baca.

### 3. Formulir Registrasi Terintegrasi (WhatsApp CTA Gateway)
* Menyediakan fitur pengisian formulir pendaftaran awal (Nama & Pilihan Jurusan).
* Memanfaatkan pemrosesan logika skrip untuk mengonversi data input secara instan menjadi draf pesan teks formal, yang langsung diarahkan ke nomor WhatsApp Panitia SPMB sekolah via API `https://wa.me/`.

### 4. Mikro Interaksi & Estetika Visual
* Efek transisi halus (*smooth transition*) saat kursor melakukan hover pada tombol-tombol aksi utama.
* Konsistensi penggunaan kode warna identitas instansi sekolah (*Branding Guidelines*).

---

## 🛠️ Spesifikasi Teknologi & Penunjang (Tech Stack)
* **HTML5 (Semantic Elements):** Menjamin struktur dokumen web yang valid, ramah SEO, dan mudah dibaca oleh mesin pembaca layar.
* **Tailwind CSS Framework:** Digunakan untuk pengelolaan tata letak kilat, pewarnaan modern, dan sistem breakpoint responsif tanpa membebani performa pemuatan halaman.
* **Vanilla JavaScript:** Menangani logika pembukaan menu navigasi, interaktivitas halaman, serta penanganan pengiriman data formulir.
* **Google Fonts (Inter):** Sebagai rumpun huruf utama demi menjaga keterbacaan teks teks pada berbagai tingkat resolusi layar.
* **Lucide Icons:** Penyedia aset ikonografi berbasis vektor yang ringan dan tajam.

---

## 📂 Pohon Struktur File Proyek
Struktur manajemen berkas pada repositori ini diatur secara ketat mengikuti standarisasi arsitektur web modern:

```text
spmb-stellarpath-smkbbc/
├── assets/
│   └── img/
│       ├── logo.png
│       ├── model.png
│       ├── lapang.png.jpeg
│       └── mockup-web.png
├── index.html
├── README.md
└── PRD.md

```
## ⚙️ Petunjuk Menjalankan Projek Secara Lokal
Jika Anda ingin menyalin dan menjalankan projek ini di lingkungan komputer lokal Anda, ikuti langkah-langkah berikut:
 1. **Salin Repositori (Clone):**
   ```bash
   git clone [https://github.com/trespage/spmb-stellarpath-smkbbc.git](https://github.com/trespage/spmb-stellarpath-smkbbc.git)
   
   ```
 2. **Masuk ke Folder Projek:**
   ```bash
   cd spmb-stellarpath-smkbbc
   
   ```
 3. **Jalankan Aplikasi:**
   Buka file index.html menggunakan browser kesayangan Anda, atau gunakan ekstensi *Live Server* di VS Code untuk pengalaman pengembangan yang lebih baik.
## 👥 Tim Pengembang (StellarPath — XI PPLG-1)
Projek ini dirancang, dikoding, dan dikelola secara kolaboratif penuh oleh kelompok kami:
 1. 💻 **Anggia Tresa Putri** 
 2. 📝 **Meliza Meilani** 
 3. 🎨 **Nur Aprilia** 
 4. 🔍 **Seina Apriliani**
© 2026 SMK Budi Bakti Ciwidey. Hak Cipta Dilindungi Undang-Undang.
```
