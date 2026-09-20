# BRIDA Open Journal System

Aplikasi web untuk mengelola alur penerbitan jurnal BRIDA Kota Makassar, mulai dari pengiriman naskah, proses editorial dan *peer review*, revisi, hingga publikasi artikel.

## Stack

- Laravel
- Livewire
- Filament untuk panel administrasi
- Blade dan Tailwind CSS
- SQLite untuk development lokal; MySQL ditargetkan untuk production

## Prasyarat

Pastikan perangkat development memiliki:

- PHP 8.3 atau lebih baru
- Composer
- Node.js dan npm
- Git

## Setup lokal

Clone repository, masuk ke direktori proyek, lalu gunakan branch `develop`:

```bash
git clone git@github.com:anstlichstudent/brida-ojs-09.git
cd rpl-app
git switch develop
```

Siapkan environment dan database SQLite lokal:

```bash
cp .env.example .env
php -r "file_exists('database/database.sqlite') || touch('database/database.sqlite');"
composer run setup
```

Perintah setup memasang dependency PHP dan JavaScript, membuat application key, menjalankan migration, dan membangun aset frontend.

## Menjalankan aplikasi

```bash
composer run dev
```

Buat akun panel administrasi saat pertama kali menjalankan aplikasi:

```bash
php artisan make:filament-user
```

Panel administrasi tersedia pada `/admin`.

## Development workflow

```text
feature/* ─┐
           ├─> develop ─> main ─> deployment
fix/* ─────┘
```

- `main` hanya berisi release yang siap di-deploy.
- `develop` menjadi branch integrasi.
- Setiap fitur atau perbaikan dikerjakan pada branch pendek dari `develop`.
- Perubahan dipromosikan ke `main` hanya setelah seluruh pemeriksaan relevan lulus.
- Setiap release di `main` diberi tag Semantic Versioning, misalnya `v0.2.0`.

Format commit, pemeriksaan wajib, dan aturan release dijelaskan dalam [CONTRIBUTING.md](CONTRIBUTING.md).

## Pemeriksaan lokal

Jalankan test:

```bash
php artisan test --compact
```

Format kode PHP yang berubah:

```bash
vendor/bin/pint --dirty --format agent
```

Verifikasi aset frontend:

```bash
npm run build
```

## Dokumentasi proyek

- [Proposal dan kebutuhan sistem](docs/Proposal_Proyek_RPL.md)
- [Referensi alur OJS](docs/ojs-documentation.md)
- [Aturan kontribusi](CONTRIBUTING.md)
- [Instruksi coding agent](AGENTS.md)

## Keamanan konfigurasi

Gunakan `.env` hanya untuk konfigurasi lokal dan kredensial. File tersebut diabaikan Git; simpan hanya `.env.example` tanpa nilai rahasia sebagai referensi tim.
