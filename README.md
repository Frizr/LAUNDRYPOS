# LAUNDRYPOS

Sistem Point-of-Sale (POS) untuk layanan laundry — proyek tugas/mini-app berbasis PHP dan MySQL.

## Deskripsi

Aplikasi ini menyediakan antarmuka untuk membuat dan mengelola pesanan laundry, termasuk halaman admin untuk manajemen layanan, laporan, dan pengguna.

## Fitur utama

- Manajemen pesanan (buat, edit, hapus)
- Halaman admin untuk manajemen layanan dan pengguna
- Ekspor laporan
- Autentikasi dasar untuk admin dan pengguna

## Teknologi

- PHP
- MySQL / MariaDB
- Composer (dependency management)
- JavaScript + HTML/CSS untuk UI
- Library pihak ketiga ada di folder `vendor/` (PHPMailer, PhpSpreadsheet, dll.)

## Persyaratan

- Web server (Apache / Nginx) dengan PHP (7.4+ disarankan)
- MySQL atau MariaDB
- Composer

## Instalasi cepat

1. Salin/clone repo ke folder web server Anda (mis. `htdocs` untuk XAMPP).
2. Jalankan `composer install` di root proyek untuk memasang dependensi:

```bash
composer install
```

3. Konfigurasikan database di `includes/db.php` dengan kredensial MySQL Anda.
4. Buat database kosong dan impor skema jika tersedia. Jika ada skrip pembuatan skema, jalankan atau akses `php/debug_schema.php` melalui browser atau CLI untuk membuat tabel awal.
5. Pastikan folder `vendor/` ada setelah `composer install`.

## Menjalankan aplikasi

1. Jalankan Apache + MySQL (mis. lewat XAMPP atau environment serupa).
2. Akses aplikasi melalui browser di `http://localhost/<folder-proyek>/`.

Halaman admin berada di folder `admin/` (mis. buka `admin/admin.html` atau endpoint yang sesuai).

## Konfigurasi email

Jika fitur email (PHPMailer) digunakan, periksa konfigurasi SMTP di file yang relevan sebelum mengirim email.

## Struktur penting

- `admin/` — UI admin
- `assets/` — CSS dan file statis
- `includes/db.php` — koneksi database (harus dikonfigurasi)
- `js/` — skrip front-end
- `php/` — endpoint back-end dan logika aplikasi
- `vendor/` — dependensi Composer

## Catatan keamanan

- Jangan commit kredensial nyata ke repo (periksa `includes/db.php`).
- Gunakan konfigurasi PHP dan server yang aman untuk produksi.

## Kontribusi

Silakan buat issue atau pull request untuk perbaikan atau fitur baru.

## Kontak

Pemilik proyek / penanggung jawab: lihat header file atau dokumentasi tugas.

---

File ini dibuat otomatis oleh tooling; silakan sesuaikan detail koneksi dan instruksi lokal sesuai kebutuhan.
