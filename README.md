# HIMATIF Website

Aplikasi web resmi **Himpunan Mahasiswa Teknik Informatika (HIMATIF)**, dibangun dengan framework [Laravel](https://laravel.com). Website ini digunakan untuk menampilkan informasi organisasi serta mengelola berbagai program kerja dan layanan kemahasiswaan secara terpusat, lengkap dengan panel admin untuk pengelolaan data.

## Fitur

- **Profil Organisasi** — anggota, departemen, dan dokumentasi kegiatan
- **Program Kerja (Proker)** — informasi kegiatan dan agenda himpunan
- **Aspirasi & Kritik Saran** — kanal masukan dari mahasiswa
- **Rekrutmen (Open Recruitment)** — pendaftaran anggota baru
- **Donasi** — pengelolaan donasi
- **Buka Bersama (Bukber)** — informasi acara bukber
- **Himatif Muda** — program untuk mahasiswa baru
- **Silaturahmi Mahasiswa** — kegiatan silaturahmi antar mahasiswa
- **Pemesanan PDH** — pemesanan pakaian dinas harian
- **Panel Admin** — dashboard untuk mengelola seluruh data di atas

## Teknologi

- **Backend:** Laravel 10, PHP ^8.1
- **Autentikasi API:** Laravel Sanctum
- **Frontend Build:** Vite, Axios
- **Database:** MySQL

## Instalasi

1. Clone repository
   ```bash
   git clone https://github.com/zah009/himatif11.git
   cd himatif11
   ```

2. Install dependency PHP
   ```bash
   composer install
   ```

3. Install dependency JavaScript
   ```bash
   npm install
   ```

4. Salin file environment dan generate application key
   ```bash
   cp .env.example .env
   php artisan key:generate
   ```

5. Konfigurasi koneksi database pada file `.env`
   ```env
   DB_CONNECTION=mysql
   DB_HOST=127.0.0.1
   DB_PORT=3306
   DB_DATABASE=himatif11
   DB_USERNAME=root
   DB_PASSWORD=
   ```

6. Jalankan migrasi database
   ```bash
   php artisan migrate
   ```

7. Jalankan server pengembangan
   ```bash
   php artisan serve
   npm run dev
   ```

   Aplikasi dapat diakses melalui `http://localhost:8000`.

## Struktur Route Utama

| Route | Deskripsi |
|---|---|
| `/` | Halaman login |
| `/anggota` | Data anggota |
| `/departement` | Data departemen |
| `/proker` | Program kerja |
| `/dokumentasi` | Dokumentasi kegiatan |
| `/aspirasi` | Aspirasi mahasiswa |
| `/recrutment` | Rekrutmen anggota |
| `/donasi` | Donasi |
| `/bukber` | Buka bersama |
| `/himatif_muda` | Himatif Muda |
| `/silaturahmi_mahasiswa` | Silaturahmi mahasiswa |
| `/pemesanan_pdh` | Pemesanan PDH |
| `/kritik_saran` | Kritik dan saran |
| `/pemberdayaan_wanita` | Pemberdayaan wanita |

## Kontribusi

Kontribusi terbuka melalui pull request. Pastikan perubahan sudah diuji secara lokal sebelum diajukan.

## Lisensi

Project ini menggunakan lisensi [MIT](https://opensource.org/licenses/MIT).
