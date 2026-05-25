# Product Requirement Document (PRD)
* **Nama Produk:** Website Informasi & Registrasi SPMB 2026
* **Versi Dokumen:** v1.0 (Final Release)
* **Tim Pengembang:** StellarPath (XI PPLG)
* **Mitra Sekolah:** SMK Budi Bakti Ciwidey

---

## 1. Analisis Kebutuhan & Latar Belakang
Sebagian besar calon siswa baru mencari informasi sekolah pilihan mereka menggunakan perangkat ponsel pintar (smartphone). Landing page ini dirancang untuk menjawab kebutuhan informasi cepat seputar kompetensi keahlian di SMK Budi Bakti Ciwidey (DKV, PPLG, BRP) serta memotong jalur birokrasi pendaftaran konvensional lewat penyediaan formulir digital instan.

## 2. Kriteria Spesifikasi Fungsional
1.  **Sistem Navigasi Adaptif (Responsive Navbar):**
    * Tampilan desktop menggunakan susunen menu horizontal standar di sisi atas.
    * Tampilan mobile otomatis menyembunyikan navbar atas dan mengaktifkan *Sticky Mobile Bottom Navigation* demi kenyamanan navigasi.
2.  **Display Konten Jurusan:**
    * Penayangan 3 program keahlian dikemas menggunakan grid layout (desktop) dan dialihkan menjadi model geser/carousel (mobile) untuk efisiensi ruang baca.
3.  **Integrasi Pesan Instan (WhatsApp CTA):**
    * Tombol pendaftaran utama akan menangkap input pilihan jurusan dan nama user, lalu memformatnya menjadi draf pesan otomatis tertuju ke panitia sekolah.

## 3. Spesifikasi Non-Fungsional
* **Optimasi Kecepatan:** Web dibangun secara ringan dengan minim skrip eksternal pihak ketiga agar kecepatan muat halaman konstan di bawah 3 detik.
* **Panduan Identitas Visual:** Mengikuti standar identitas visual sekolah menggunakan warna Biru Utama (`#1E40AF`) serta aksen Kuning Terang (`#FACC15`) untuk tombol penentu tindakan.
* **Keterbacaan Teks:** Menggunakan tipe huruf sans-serif modern (Inter Fonts) agar dokumen teks nyaman dibaca pada layar dengan densitas piksel rendah.

## 4. Parameter Keberhasilan (Acceptance Criteria)
* [x] Struktur tata letak tidak mengalami kerusakan (*layout overflow*) saat diuji pada mode responsif Google Chrome DevTools.
* [x] Seluruh aset gambar dan berkas kodingan berhasil didorong (*push*) ke repositori publik GitHub tanpa berkas korup.
* [x] Sistem *Continuous Deployment* Netlify berfungsi normal (Setiap ada pembaruan dokumen kodingan di repositori GitHub, pelayan Netlify akan memperbarui tampilan web publik secara otomatis).
*
