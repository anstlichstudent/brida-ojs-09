# BRIDA Open Journal System

Aplikasi web untuk mengelola alur penerbitan jurnal BRIDA Kota Makassar, mulai dari pengiriman naskah, proses editorial dan *peer review*, revisi, hingga publikasi artikel.

## Stack

- Laravel
- Livewire
- Filament untuk panel administrasi
- Blade dan Tailwind CSS
- SQLite untuk development lokal; MySQL ditargetkan untuk production

## Struktur proyek dan pembagian area

Proyek ini menggunakan Laravel monolith. Frontend, backend, dan database berada dalam satu repository, sehingga pembagian berikut menunjukkan fokus kerja, bukan batas kepemilikan mutlak.

| Area | Folder atau file | Kegunaan |
| --- | --- | --- |
| Frontend | `resources/views/` | Halaman Blade dan view komponen Livewire. |
| Frontend | `resources/css/` | Sumber styling aplikasi dan konfigurasi tema melalui CSS. |
| Frontend | `resources/js/` | JavaScript aplikasi yang diproses oleh Vite. |
| Frontend | `public/` | Entry point web dan aset statis publik. Isi `public/build/` serta aset Filament adalah hasil generate dan tidak diedit manual. |
| Frontend | `vite.config.js`, `package.json` | Konfigurasi build serta dependency frontend. |
| Backend | `app/Http/` | Controller, request, dan middleware HTTP saat ditambahkan. |
| Backend | `app/Models/` | Model Eloquent dan relasi domain. |
| Backend | `app/Providers/` | Registrasi service aplikasi dan panel Filament. |
| Backend | `routes/` | Definisi route web dan perintah console. |
| Backend | `config/` | Konfigurasi Laravel; nilai rahasia tetap berasal dari `.env`. |
| Database | `database/migrations/` | Riwayat perubahan struktur database. Semua perubahan schema dibuat melalui migration. |
| Database | `database/factories/` | Pembuat data uji untuk model. |
| Database | `database/seeders/` | Data awal atau data development yang dapat dibuat ulang. |
| Database | `database/database.sqlite` | Database lokal; file ini diabaikan Git dan bukan sumber data bersama. |
| DevOps | `bootstrap/` | Bootstrap aplikasi dan cache framework. |
| DevOps | `storage/` | Log, cache, session, dan file runtime; data hasil runtime tidak di-commit. |
| DevOps | `tests/`, `phpunit.xml` | Test otomatis dan konfigurasi PHPUnit. |
| DevOps | `.env.example` | Template konfigurasi environment tanpa rahasia. |
| DevOps | `composer.json`, `composer.lock` | Dependency dan script PHP yang harus konsisten antarenvironment. |
| DevOps | `package.json`, `package-lock.json` | Dependency dan script frontend yang harus konsisten antarenvironment. |

Komponen Livewire nantinya ditempatkan di `app/Livewire/` dengan view di `resources/views/livewire/`. Resource, page, dan widget Filament ditempatkan di `app/Filament/` ketika fitur administrasi mulai dibuat.

Perubahan satu fitur boleh menyentuh beberapa area. Contohnya, fitur submission dapat membutuhkan migration, model, komponen Livewire, view, dan test dalam satu branch yang sama.

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
