# 📦 InvenSync — Inventory Management System

[![Laravel](https://img.shields.io/badge/Backend-Laravel%2011-red?logo=laravel)](https://laravel.com) [![Next.js](https://img.shields.io/badge/Frontend-Next.js%2014-black?logo=next.js)](https://nextjs.org) [![Tailwind CSS](https://img.shields.io/badge/Styling-Tailwind%20CSS-blue?logo=tailwind-css)

**InvenSync** adalah monorepo untuk aplikasi manajemen inventaris berarsitektur *headless*: backend API menggunakan **Laravel 11** dan frontend menggunakan **Next.js 14 (App Router)**.

---

## 🔖 Ringkasan

- Backend: RESTful API, otentikasi dengan Sanctum, migrasi & seeders, testing.
- Frontend: Next.js (App Router), Tailwind CSS, berkomunikasi dengan API backend.

---

## 🚀 Quickstart (Lokal)

Prasyarat: Git, PHP 8.1+, Composer, Node.js 18+, npm/pnpm/yarn, MySQL.

1) Clone repo

```bash
git clone https://github.com/Vendettaa666/invensync.git
cd invensync
```

2) Backend (Laravel)

```bash
cd backend
composer install
cp .env.example .env
# set DB config di .env
php artisan key:generate
php artisan migrate --seed
php artisan serve --host=127.0.0.1 --port=8000
```

API: http://127.0.0.1:8000

3) Frontend (Next.js)

```bash
cd ../frontend
npm install        # atau pnpm install / yarn
cp .env.example .env.local
# set NEXT_PUBLIC_API_URL=http://127.0.0.1:8000
npm run dev
```

Frontend: http://localhost:3000

---

## 🔧 Struktur Proyek

- `backend/` — Laravel API
  - `app/`, `routes/`, `database/migrations`, `database/seeders`
- `frontend/` — Next.js App Router
  - `app/`, `public/`, `next.config.js`

---

## 📋 Dokumentasi Terpisah

- Backend README: `backend/README.md` (setup, env, testing, deployment)
- Frontend README: `frontend/README.md` (setup, env, build, deploy)

---

## 🤝 Kontribusi

1. Fork repo
2. Buat branch fitur: `git checkout -b feat/deskripsi`
3. Commit & push
4. Buka PR dengan deskripsi perubahan

---

## 📬 Kontak

Untuk pertanyaan atau bantuan, buka issue di repo atau hubungi pemilik proyek.

---

Terima kasih! 🙏
