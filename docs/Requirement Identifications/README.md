# Dokumen Teknis Kebutuhan Aplikasi Backend: Sosial Media Mirip Instagram

## 1. Pendahuluan

### 1.1 Tujuan Dokumen

Dokumen ini bertujuan untuk merinci kebutuhan fungsional dan non-fungsional untuk pengembangan aplikasi backend sosial media yang mirip dengan Instagram.

### 1.2 Ruang Lingkup Proyek

Proyek ini bertujuan untuk mengembangkan platform sosial media yang memungkinkan pengguna berbagi foto dan video, berinteraksi dengan konten pengguna lainnya, serta memperluas jaringan sosial mereka.

## 2. Kebutuhan Fungsional

### 2.1 Deskripsi Kasus Pengguna

- Pengguna dapat mendaftar dan membuat profil pengguna.
- Pengguna dapat mengunggah foto dan video.
- Pengguna dapat menambahkan deskripsi, tag, dan lokasi ke unggahan mereka.
- Pengguna dapat menelusuri konten berdasarkan tag atau lokasi.
- Pengguna dapat mengikuti pengguna lain dan melihat unggahan mereka di feed.
- Pengguna dapat memberikan like, komentar, dan berbagi unggahan pengguna lain.

### 2.2 Daftar Fitur

- Autentikasi Pengguna
- Manajemen Profil Pengguna
- Unggah dan Manajemen Konten
- Pencarian dan Penelusuran Konten
- Interaksi dengan Konten
- Manajemen Hubungan Pengguna

### 2.3 Prioritas Fitur

- Autentikasi Pengguna
- Manajemen Profil Pengguna
- Unggah dan Manajemen Konten
- Interaksi dengan Konten
- Pencarian dan Penelusuran Konten
- Manajemen Hubungan Pengguna

### 2.4 Diagram Use Case

## 3. Kebutuhan Non-Fungsional

### 3.1 Kinerja

- Waktu tanggapan aplikasi harus kurang dari 500ms.
- Kemampuan untuk menangani setidaknya 10.000 pengguna aktif secara bersamaan.

### 3.2 Skalabilitas

- Kemampuan untuk menangani peningkatan pesat dalam jumlah pengguna dan unggahan konten.

### 3.3 Keamanan

- Implementasi mekanisme otentikasi yang kuat dan enkripsi data sensitif.
- Perlindungan terhadap serangan seperti SQL injection dan Cross-Site Scripting (XSS).

### 3.4 Ketersediaan

- Persentase waktu operasi (uptime) harus minimal 99% setiap bulannya.
- Pemulihan bencana yang cepat dan efisien untuk memastikan ketersediaan layanan yang berkelanjutan.

### 3.5 Kualitas Kode

- Mengikuti standar kode yang ditetapkan oleh komunitas dan menggunakan praktik pengkodean terbaik untuk memastikan kode yang mudah dipahami, dikelola, dan diperbarui.

## 4. Lingkungan Pengembangan

### 4.1 Teknologi dan Platform

- Bahasa Pemrograman: Python
- Framework: Django
- Database: PostgreSQL
- Layanan Cloud: AWS (Amazon Web Services)

### 4.2 Alat dan Framework

- Django REST Framework untuk pengembangan API
- Amazon S3 untuk penyimpanan dan pengelolaan file multimedia
- Celery untuk manajemen antrian tugas asinkron
- Redis untuk caching dan manajemen sesi

### 4.3 Konfigurasi Lingkungan

- Konfigurasi server EC2 di AWS dengan skalabilitas otomatis
- Penyediaan instance PostgreSQL dengan skema basis data yang didefinisikan dengan baik
- Penggunaan layanan Amazon S3 untuk menyimpan foto dan video

## 5. Referensi

### 5.1 Dokumentasi Tambahan

- Dokumentasi Django: https://docs.djangoproject.com/
- Dokumentasi Django REST Framework: https://www.django-rest-framework.org/

## 6. Lampiran

### 6.1 Istilah dan Definisi

- Feed: Halaman beranda yang menampilkan unggahan terbaru dari pengguna yang diikuti.
- Tag: Label yang ditambahkan ke unggahan untuk memudahkan pencarian dan klasifikasi.
- Lokasi: Informasi tentang lokasi fisik tempat unggahan diambil.
