# Setup v0 by Vercel — AI Gratis untuk Generate UI & Full-stack App

[v0](https://v0.app) adalah platform AI dari Vercel yang mengubah deskripsi bahasa natural jadi aplikasi web full-stack (React/Next.js) siap produksi. Plan **Free** tanpa kartu kredit:

- **$5 credit tiap bulan**
- Sampai **200 projects**
- Generate UI dari prompt/wireframe/screenshot, fix error otomatis, deploy 1-klik ke Vercel
- Editor **VS Code-style** di dalam v0 + **integrasi Git** dua arah

> Catatan: v0 itu **web-based**, bukan extension VSCode. Alur kerjanya: generate di v0 → sinkron ke repo → lanjut coding di VSCode kamu.

## Prasyarat

- Akun [Vercel](https://vercel.com) atau GitHub (tinggal login)

## Cara Setup

### 1. Login

1. Buka [v0.app](https://v0.app).
2. Klik **Sign Up / Log in** → pilih login pakai akun GitHub atau Vercel.
3. Langsung masuk plan **Free** — tanpa setup tambahan.

### 2. Generate Aplikasi Pertama

1. Tulis deskripsi app yang mau dibuat di prompt box (bahasa apa saja, termasuk Indonesia).
2. v0 membuat UI + kode lengkap dengan preview live.
3. Iterasi: minta perubahan via chat, atau edit langsung di editor bawaan v0 (syntax highlighting, diff view, split editing).

### 3. Sinkron ke VSCode (Integrasi Git)

Supaya hasil v0 bisa dilanjutkan di VSCode:

1. Di project v0, hubungkan ke **repo GitHub** kamu (integrasi Git bawaan).
2. v0 otomatis bikin branch & pull request dari setiap perubahan.
3. Di VSCode: `git clone` / `git pull` repo tersebut, lanjut edit lokal seperti biasa.

Alurnya dua arah — commit lokal kamu juga bisa disinkronkan balik ke v0.

## v0 API (Opsional, untuk Developer)

Kalau mau panggil v0 secara programatik (misal dari script/agent kamu sendiri), pakai SDK:

```bash
npm install v0-sdk
```

Butuh API key dari dashboard v0 — pemakaian mengonsumsi credit yang sama.

## Tips Hemat Credit

- Satu prompt deskriptif lebih hemat daripada banyak prompt kecil (tiap generasi ngambil credit).
- Generate UI/draft di v0 (yang jago), lalu refactor & detail kecil di VSCode (gratis, pakai AI lokal/Gemini).

## Catatan

- Credit habis = tunggu reset bulan depan, tidak auto-charge di plan Free.
- Untuk AI coding **di dalam** VSCode, kombinasi v0 + [Gemini](../gemini/README.md) atau [Copilot Free](../copilot/README.md) cocok: v0 untuk scaffold UI, yang lain untuk coding harian.

## Referensi

- [v0](https://v0.app)
- [Dokumentasi](https://v0.app/docs)
- [Pricing & Plans](https://v0.app/docs/pricing)
- [v0 SDK](https://v0.app/docs/api/platform/overview)
