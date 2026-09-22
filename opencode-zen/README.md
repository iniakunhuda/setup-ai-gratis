# Setup OpenCode Zen — Model AI Terverifikasi untuk OpenCode

**OpenCode Zen** adalah kumpulan model AI yang sudah **di-test & diverifikasi oleh tim OpenCode** (GPT, Claude, Gemini, Grok, Qwen, DeepSeek, GLM, Kimi, dll) di satu endpoint. Pemakaian dibayar **per request (credit)** — jadi gratis selama kamu pakai **model-model gratisnya** atau credit yang tersedia.

> Ini lanjutan dari [OpenCode](../opencode/README.md) — Zen itu provider di dalam OpenCode, bukan aplikasi berdiri sendiri. Pastikan OpenCode CLI sudah terinstall.

## Prasyarat

- OpenCode CLI terinstall (`npm install -g opencode-ai`)
- Akun OpenCode Zen (login di [opencode.ai/zen](https://opencode.ai/zen))

## Cara Setup

### 1. Buat API Key Zen

1. Login ke **OpenCode Zen** console.
2. Klik **Create API Key** → salin key-nya.

> Untuk model berbayar perlu isi billing dulu. Untuk **model gratis** (`grok-code`, `gpt-5-nano`, dll) tidak perlu.

### 2. Sambungkan ke OpenCode

Jalankan `opencode` di folder project, lalu di dalam TUI:

1. Jalankan **`/connect`** → cari **OpenCode Zen**.
2. Tempel API key kamu.
3. Jalankan **`/models`** → pilih model (mis. `grok-code` yang gratis, atau `Qwen 3 Coder 480B`).

### 3. Mulai Pakai

Chat di TUI seperti biasa — Zen bekerja persis seperti provider lain di OpenCode. Model bisa diganti kapan saja via `/models`.

## Integrasi VSCode

Sama seperti OpenCode biasa:

- Install extension **"OpenCode"** di VSCode (butuh CLI terinstall).
- Atau jalankan `opencode` dari terminal **dalam VSCode** — diff tampil langsung di editor.

## Model Gratis yang Bisa Dicoba

| Model | Keterangan |
|-------|------------|
| `grok-code` | Gratis, cocok untuk coding harian |
| `gpt-5-nano` | Gratis, ringan & cepat |
| `big-pickle` | Gratis, placeholder yang merute ke model pilihan tim OpenCode |

Daftar lengkap model berbayar (Claude, GPT, Gemini, Kimi, dll) ada di [dokumentasi Zen](https://opencode.ai/docs/zen).

## Catatan

- Tanpa isi billing, tetap bisa pakai model gratis — cukup buat API key.
- Credit berbayar top-up manual (pay per request), **tidak auto-charge**.
- Kalau mau 100% tanpa Zen, OpenCode tetap bisa pakai provider lain — lihat [README OpenCode](../opencode/README.md).

## Referensi

- [OpenCode Zen](https://opencode.ai/zen)
- [Dokumentasi Zen](https://opencode.ai/docs/zen)
- [Providers](https://opencode.ai/docs/providers)
