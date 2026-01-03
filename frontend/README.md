# Frontend — InvenSync (Next.js 14)

**Lokasi**: `./frontend`

UI dibangun dengan Next.js 14 (App Router) dan Tailwind CSS.

## Prasyarat

- Node.js 18+
- npm / pnpm / yarn

## Setup Lokal

```bash
cd frontend
npm install   # atau pnpm install / yarn
cp .env.example .env.local
# atur NEXT_PUBLIC_API_URL=http://127.0.0.1:8000
npm run dev
```

- Buka `http://localhost:3000`
- File entry utama: `app/page.tsx`

## Build & Production

```bash
npm run build
npm run start
```

## Testing & Linting

- `npm run lint`
- `npm run typecheck` (jika di-setup)

## Env variables penting

- `NEXT_PUBLIC_API_URL` — URL backend API
- `NEXT_PUBLIC_ENV` — environment label

## Deploy

Disarankan deploy ke Vercel atau platform yang mendukung Next.js App Router. Pastikan env var `NEXT_PUBLIC_API_URL` diset di environment produksi.

---

Untuk informasi umum Next.js lihat: https://nextjs.org/docs
