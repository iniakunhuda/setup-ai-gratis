# Setup Qwen Code CLI — AI Coding Agent dari Alibaba

[Qwen Code](https://github.com/QwenLM/qwen-code) adalah agentic CLI open-source dari Alibaba, dioptimalkan untuk model **Qwen3-Coder** (fork dari Gemini CLI).

> ⚠️ **Update penting:** free tier **Qwen OAuth** (yang dulu 2.000 request/hari gratis) **sudah dihentikan 15 April 2026**. Sekarang jalur gratisnya lewat **ModelScope** / free quota baru — lihat di bawah.

## Prasyarat

- [Node.js](https://nodejs.org) 20+

## Install

```bash
npm install -g @qwen-code/qwen-code
```

## Jalur Gratis (Non-BYOK penuh sudah tidak ada, tapi masih ada yang gratis)

### 1. ModelScope — 2.000 calls/hari gratis ✅

[ModelScope](https://modelscope.cn) (milik Alibaba) masih memberi kuota API-Inference gratis harian, termasuk model Qwen:

1. Daftar di [modelscope.cn](https://modelscope.cn) (atau [modelscope.com](https://www.modelscope.com) untuk internasional).
2. Buat API key di halaman token/keys akun kamu.
3. Jalankan `qwen` → `/auth` → **Third-party Providers** → **ModelScope** → tempel API key.

Selesai — pakai model Qwen gratis sampai kuota harian habis, reset besok.

### 2. Model Studio — Free Quota Akun Baru

Alibaba Cloud Model Studio (DashScope) memberi **free quota untuk akun baru** (mis. 1 juta token untuk model tertentu, terbatas waktu):

1. Daftar di [Model Studio intl](https://modelstudio.console.alibabacloud.com).
2. Buat API key → `qwen` → `/auth` → **Alibaba ModelStudio** → **Standard API Key**.

### 3. OpenRouter — Model `:free`

Di `/auth` → pilih **OpenRouter**, pakai API key OpenRouter kamu dan pilih model bertag `:free` (termasuk Qwen coder). ~50 request/hari gratis.

## Integrasi VSCode

- Jalankan `qwen` dari terminal **dalam VSCode** — diff dan konteks workspace tampil di editor.
- Ada **extension JetBrains** resmi; untuk VSCode, CLI di terminal terintegrasi sudah cukup.
- Tersedia juga konfigurasi `modelProviders` di `~/.qwen/settings.json` kalau mau set permanen tanpa menu `/auth`.

## Mulai Pakai

```bash
qwen                    # start TUI di folder project
qwen --model "qwen3-coder-plus"
```

Chat bahasa natural — agent bisa baca codebase, edit multi-file, jalankan command. Model ganti kapan saja via `/auth` atau flag `--model`.

## Catatan

- Qwen OAuth login browser **sudah tidak bisa dipakai untuk request baru** — kalau tutorial lama menyuruh login qwen.ai, itu sudah kadaluarsa.
- Kuota ModelScope bisa berubah — cek halaman API-Inference mereka untuk limit terkini.
- Tertarik plan berbayar? **Coding Plan** Alibaba bulanan quota besar untuk individual developer.

## Referensi

- [GitHub — QwenLM/qwen-code](https://github.com/QwenLM/qwen-code)
- [Dokumentasi Auth](https://github.com/QwenLM/qwen-code/blob/main/docs/users/configuration/auth.md)
- [ModelScope](https://modelscope.cn)
