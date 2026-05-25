# 📋 Product Requirement Document (PRD)
* **Nama Produk:** Website Informasi & Registrasi Mandiri SPMB 2026
* **Versi Dokumen:** v1.0 (Final Production Spec)
* **Status Produk:** Siap Rilis (Deployment Ready)
* **Tim Pengembang:** StellarPath (XI PPLG-1)
* **Instansi Mitra:** SMK Budi Bakti Ciwidey

---

## 1. Analisis Kebutuhan & Latar Belakang
Sebagian besar calon peserta didik baru yang merupakan generasi Z mengakses informasi sekolah pilihan mereka menggunakan perangkat ponsel pintar (*smartphone*). Sistem konvensional yang mengharuskan calon siswa datang langsung atau mengisi formulir yang rumit sering kali menurunkan minat daftar. 

Landing page SPMB 2026 ini dirancang untuk menjawab kebutuhan informasi cepat seputar kompetensi keahlian di SMK Budi Bakti Ciwidey (DKV, PPLG, BRP) serta memotong jalur birokrasi pendaftaran konvensional lewat penyediaan formulir digital instan yang terintegrasi langsung ke WhatsApp panitia.

---

## 2. Tujuan Produk (Product Objectives)
* **Aksesibilitas Tinggi:** Menyediakan platform informasi promosi sekolah yang sangat ringan dan mudah diakses dari jaringan internet seluler yang lambat sekalipun.
* **Meningkatkan Konversi Pendaftar:** Mempermudah alur penyerahan data awal calon siswa dari yang tadinya manual menjadi otomatis digital dalam hitungan detik.
* **Standardisasi Industri:** Menghasilkan produk perangkat lunak berbasis web yang patuh terhadap kaidah kode semantik, tata letak adaptif (*responsive layout*), dan arsitektur repositori yang bersih.

---

## 3. Spesifikasi Fungsional & Alur Pengguna (User Flow)

### 3.1 Sistem Navigasi Komponen Adaptif
* **Skenario Layar Desktop (Lebar ≥ 1024px):**
  * Navbar atas bersifat *sticky* atau menetap di atas halaman saat di-scroll.
  * Menampilkan menu horizontal penuh: *Home, Jurusan, Fasilitas, Alur Pendaftaran, Kontak*.
* **Skenario Layar Mobile (Lebar < 768px):**
  * Navbar atas otomatis disembunyikan untuk menghemat ruang vertikal layar.
  * Mengaktifkan *Sticky Mobile Bottom Navigation* dengan ikon interaktif (Beranda, Jurusan, Daftar, Kontak) yang diposisikan di area bawah demi kenyamanan jangkauan jempol user.

### 3.2 Ruang Informasi Kompetensi Keahlian (Program Studi)
* Sistem menampilkan 3 kartu informasi utama untuk jurusan DKV, PPLG, dan BRP.
* Setiap kartu wajib memuat: Ikon jurusan, nama kompetensi keahlian, deskripsi singkat keunggulan, serta prospek kerja lulusan.
* Transformasi tata letak: Otomatis berubah dari susunan Grid 3 Kolom (Desktop) menjadi susunan baris vertikal atau komponen geser horizontal/carousel (Mobile).

### 3.3 Integrasi Formulir Pendaftaran Awal (WhatsApp CTA Gateway)
* **Komponen Input:** Teks boks untuk "Nama Lengkap" dan pilihan Dropdown/Radio Button untuk "Pilihan Jurusan".
* **Logika Pemrosesan (JavaScript):** Ketika tombol "Kirim Data" diklik, sistem menjalankan fungsi enkripsi string URL (`encodeURIComponent`) untuk menyusun pesan teks otomatis.
* **Format Pesan:** ```text
  Halo Panitia SPMB SMK Budi Bakti Ciwidey! Saya ingin mendaftar awal. 
  Nama: [Nama Pendaftar] 
  Pilihan Jurusan: [Jurusan yang Dipilih]
  Mohon informasi langkah selanjutnya, terima kasih.

```
 * **Aksi Akhir:** Sistem membuka tab baru dan mengarahkan pengguna langsung ke aplikasi WhatsApp tujuan melalui API https://wa.me/628123456789?text=....
## 4. Spesifikasi Non-Fungsional (Kualitas Teknis)
### 4.1 Performa & Kecepatan Muat (Performance)
 * Kode CSS dan komponen tata letak wajib memanfaatkan *utility classes* dari Tailwind CSS guna menekan ukuran file stylesheet di bawah 50 KB.
 * Optimalisasi gambar: Seluruh aset visual promosi (seperti gambar lapangan dan model) wajib dikompresi agar tidak melebihi 300 KB per file untuk menjamin kecepatan *First Contentful Paint (FCP)* di bawah 2.5 detik pada koneksi 4G.
### 4.2 Identitas Visual & Aksesibilitas (Design System)
 * **Palet Warna Utama:** Mengikuti panduan warna instansi, menggunakan warna Biru Safir (#1E40AF) untuk kesan formal-profesional, dan Kuning Emas (#FACC15) untuk tombol penentu tindakan (Call to Action).
 * **Tipografi:** Rumpun font sans-serif *Inter* dari Google Fonts dengan variasi ketebalan (Regular 400, Medium 500, Bold 700) untuk menjaga hierarki baca teks.
 * **Kontras Rasio:** Kontras warna antara teks dan latar belakang wajib memenuhi standar WCAG 2.1 AA agar teks tetap nyaman dibaca oleh pengguna yang memiliki gangguan penglihatan ringan.
## 5. Matriks Pengujian Kelayakan (Acceptance Criteria)
### 5.1 Pengujian Antarmuka (UI Testing)
 * [x] Elemen halaman tidak mengalami kerusakan (*layout overflow*) atau teks keluar dari batas kotak saat diuji pada mode responsif Google Chrome Developer Tools (iPhone SE, iPhone 12 Pro, dan Samsung Galaxy S20 Ultra).
 * [x] Jarak margin dan padding antar seksian konsisten (minimal memiliki ruang pemisah yang proporsional).
### 5.2 Pengujian Git & Integrasi Platform (Deployment Testing)
 * [x] Seluruh aset gambar dan file kodingan (index.html, README.md, PRD.md) berhasil didorong (*push*) ke repositori GitHub tanpa file korup atau salah penempatan direktori.
 * [x] Sistem *Continuous Deployment* Netlify berfungsi normal (Setiap ada pembaruan dokumen kodingan di repositori GitHub, pelayan Netlify akan mendeteksi perubahan dan memperbarui tampilan web publik secara otomatis dalam waktu kurang dari 1 menit).
*Dokumen ini sah dan menjadi acuan utama pengembangan akhir tim StellarPath XI PPLG-1.*
```

---
