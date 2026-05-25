# 📋 Product Requirement Document (PRD)
* **Nama Produk:** Website Informasi & Slicing Landing Page SPMB 2026
* **Versi Dokumen:** v1.0 (Slicing Release)
* **Status Produk:** Tahap Antarmuka Selesai (Frontend Slicing Ready)
* **Tim Pengembang:** StellarPath (XI PPLG-1)
* **Instansi Mitra:** SMK Budi Bakti Ciwidey

---

## 1. Analisis Kebutuhan & Latar Belakang
Sebagian besar calon peserta didik baru mencari informasi sekolah pilihan mereka menggunakan perangkat ponsel pintar (*smartphone*). Landing page ini dirancang khusus untuk memenuhi kebutuhan informasi visual yang cepat dan interaktif seputar kompetensi keahlian di SMK Budi Bakti Ciwidey (DKV, PPLG, BRP) melalui tampilan antarmuka yang modern dan responsif.

Fokus utama dari pengembangan tahap ini adalah melakukan *slicing* desain menjadi kode komponen HTML & Tailwind CSS yang presisi, ringan, dan ramah pengguna di layar HP.

---

## 2. Tujuan Produk (Product Objectives)
* **Aksesibilitas Tinggi:** Menyediakan platform informasi promosi sekolah yang sangat ringan saat diakses dari jaringan internet seluler.
* **Standardisasi Kode Frontend:** Menghasilkan produk perangkat lunak berbasis web yang patuh terhadap kaidah kode semantik dan sistem breakpoint responsif.
* **Presentasi Interaktif:** Menampilkan informasi profil jurusan dengan tata letak yang menarik dan nyaman dibaca oleh calon siswa baru.

---

## 3. Kriteria Spesifikasi Fungsional (Fitur Antarmuka)

### 3.1 Sistem Navigasi Komponen Adaptif (Responsive Navbar)
* **Skenario Layar Desktop:**
  * Navbar atas bersifat *sticky* atau menetap di atas halaman saat di-scroll.
  * Menampilkan menu horizontal penuh untuk mempermudah perpindahan pandangan halaman.
* **Skenario Layar Mobile:**
  * Navbar atas otomatis disembunyikan untuk menghemat ruang vertikal layar HP.
  * Mengaktifkan komponen *Sticky Mobile Bottom Navigation* di bagian bawah layar untuk kenyamanan jangkauan jempol pengguna saat menggenggam HP.

### 3.2 Ruang Informasi Kompetensi Keahlian (Showcase Cards)
* Tampilan antarmuka menampilkan kartu informasi visual untuk 3 jurusan utama: PPLG, DKV, dan BRP.
* Setiap kartu memuat judul kompetensi keahlian, ikon penanda, serta deskripsi singkat keunggulan jurusan.
* Transformasi tata letak: Otomatis berubah dari susunan Grid 3 Kolom pada layar komputer menjadi susunan baris vertikal atau sistem geser yang rapi pada layar HP.

### 3.3 Tautan Informasi & Aksi Sosial Media (Call to Action Buttons)
* Menyediakan tombol aksi statis (CTA) yang mencolok untuk mengarahkan calon siswa ke saluran informasi eksternal sekolah.
* Integrasi tautan luar menuju akun media sosial resmi atau kontak sekolah menggunakan tag jangkar (`<a href="...">`) standar tanpa pemrosesan skrip pengiriman data.

---

## 4. Spesifikasi Non-Fungsional (Kualitas Teknis)

### 4.1 Performa Antarmuka (Performance)
* Kode tata letak wajib memanfaatkan *utility classes* dari Tailwind CSS guna menekan ukuran file dan menghindari penulisan kode CSS manual yang berulang.
* Optimalisasi Gambar: Seluruh aset visual promosi (seperti gambar logo, model, dan lapangan) dikompresi agar berukuran ringan untuk menjamin kecepatan muat halaman yang instan.

### 4.2 Identitas Visual & Aksesibilitas (Design System)
* **Palet Warna:** Mengikuti panduan identitas sekolah, dominan menggunakan warna Biru Utama (`#1E40AF`) untuk kesan formal-pendidikan, dan aksen Kuning Terang (`#FACC15`) untuk tombol-tombol penentu tindakan.
* **Tipografi:** Menggunakan rumpun font sans-serif *Inter* dari Google Fonts untuk memastikan teks tetap tajam dan mudah dibaca pada berbagai tingkat kerapatan piksel layar HP.

---

## 5. Matriks Pengujian Kelayakan (Acceptance Criteria)

### 5.1 Pengujian Tata Letak (UI Layout Testing)
* [x] Struktur elemen halaman tidak mengalami kerusakan (*layout overflow*) atau teks terpotong saat diuji pada berbagai mode responsif di Google Chrome Developer Tools.
* [x] Seluruh tombol navigasi bawah pada mode mobile tampil presisi di posisi bawah layar tanpa menutupi konten utama.

### 5.2 Pengujian Integrasi Platform (Deployment Testing)
* [x] Seluruh berkas kodingan (`index.html`, `README.md`, `PRD.md`) beserta folder `assets` berhasil didorong ke repositori GitHub tanpa salah penempatan direktori.
* [x] Sistem *Continuous Deployment* Netlify berfungsi normal dan berhasil menampilkan visual landing page secara *live* dari data repositori GitHub.

---
*Dokumen spesifikasi ini dibuat sesuai dengan hasil akhir pengembangan antarmuka oleh tim StellarPath XI PPLG-1.*
