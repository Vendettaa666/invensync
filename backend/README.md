# Backend — InvenSync (Laravel 11)

**Lokasi**: `./backend`

Backend InvenSync dibangun di atas Laravel 11 dan bertanggung jawab menyediakan RESTful API untuk manajemen inventaris (produk, stok, pengguna, transaksi).

## ✅ Fitur Proyek (Singkat)

- API CRUD untuk entitas inventaris
- Otentikasi & otorisasi menggunakan Laravel Sanctum
- Migrasi & seeder untuk data awal
- Testing via PHPUnit

## 🔧 Prasyarat

- PHP 8.1+
- Composer
- MySQL (atau database lain yang didukung)
- Node.js (jika ingin membangun assets)

## 🚀 Setup Lokal

```bash
cd backend
composer install
cp .env.example .env
# atur DB pada .env
php artisan key:generate
php artisan migrate --seed
php artisan storage:link   # jika perlu
php artisan serve --host=127.0.0.1 --port=8000
```

API default: `http://127.0.0.1:8000`

## 🔐 Autentikasi

Menggunakan **Laravel Sanctum**. Jika frontend berjalan di domain lain, pastikan:

- `SANCTUM_STATEFUL_DOMAINS` berisi domain frontend
- `SESSION_DOMAIN` & konfigurasi CORS cocok

## 🧪 Testing

```bash
php artisan test
```

## 🔁 Commands berguna

- `composer install` — instal dependensi
- `php artisan migrate` — jalankan migrasi
- `php artisan db:seed` — jalankan seeder
- `php artisan tinker` — REPL

## 📋 Env variables penting

- `APP_URL`
- `DB_*` (DB_CONNECTION, DB_HOST, DB_DATABASE...)
- `SANCTUM_STATEFUL_DOMAINS`

## 📦 Deployment singkat

- `composer install --no-dev`
- `php artisan migrate --force`
- `php artisan config:cache` & `php artisan route:cache`

---

## Tentang Laravel

(Informasi Laravel asli: framework expressive dengan dokumentasi lengkap dan banyak resource.)

> Untuk dokumentasi resmi Laravel, lihat https://laravel.com/docs
