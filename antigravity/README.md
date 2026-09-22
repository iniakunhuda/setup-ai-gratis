# Setup Google Antigravity — AI Gratis dari Google

[Google Antigravity](https://antigravity.google) adalah agentic development environment (IDE + CLI) dari Google. Dengan **akun Google biasa (gratis)** kamu langsung dapat kuota pemakaian model AI (free tier) — termasuk model Gemini, Claude, dan lainnya — tanpa kartu kredit.

## Prasyarat

- Akun Google (gratis, tinggal daftar biasa)
- macOS, Windows, atau Linux

## Cara Setup

### 1. Download & Install

Kunjungi [antigravity.google/download](https://antigravity.google/download) dan unduh installer sesuai OS kamu, lalu install seperti aplikasi biasa.

### 2. Login dengan Akun Google

1. Buka aplikasi Antigravity.
2. Klik **Sign In**.
3. Autentikasi lewat browser default kamu dengan akun Google.
4. Selesai — sesi otomatis tersambung ke plan kamu (termasuk **free tier**).

### 3. Mulai Pakai

Buat/buka project, lalu ajak agent-nya ngoding. Model AI bisa dipilih langsung di interface.

## Alternatif: Antigravity CLI (Terminal)

Kalau lebih suka kerja dari terminal:

```bash
# macOS / Linux
curl -fsSL https://antigravity.google/cli/install.sh | bash

# Windows PowerShell
irm https://antigravity.google/cli/install.ps1 | iex
```

Lalu jalankan:

```bash
mkdir my-project && cd my-project
agy
```

Saat pertama kali jalan, ikuti instruksi di terminal untuk login akun Google.

Lihat model yang tersedia:

```bash
agy models
```

## Alternatif: Extension di Editor Lain

Antigravity juga tersedia sebagai extension:

- **Zed** (v0.140.0+, macOS/Linux) — set auth `type: "oauth-personal"` di config
- **JetBrains IDE** (2026.2.1+, semua OS) — klik ikon Antigravity di activity bar → **Sign In**

## Catatan

- Free tier punya **rate limit / kuota harian**. Kalau butuh lebih, upgrade ke plan Google AI (Pro/Ultra).
- Model yang tersedia bisa berubah — cek [antigravity.google/docs/models](https://antigravity.google/docs/models) dan [pricing](https://antigravity.google/pricing).

## Referensi

- [Download](https://antigravity.google/download)
- [Dokumentasi](https://antigravity.google/docs)
- [Plans & Pricing](https://antigravity.google/pricing)
