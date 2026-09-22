# Setup Cline — AI Coding Agent Gratis di VSCode

[Cline](https://cline.bot) adalah extension AI coding agent untuk VSCode (juga ada di Cursor, Windsurf, JetBrains, Antigravity) — bisa baca codebase, edit multi-file, dan jalanin terminal command dengan persetujuan kamu.

Cara gratis pakai Cline (pilih salah satu):

1. **Model bertag FREE** di Cline Provider — tanpa kartu kredit ✅ paling gampang
2. **Gemini API free tier** (bring your own key)
3. **Model lokal** di hardware sendiri (Ollama, dll) — 100% gratis selamanya

## Prasyarat

- [VSCode](https://code.visualstudio.com) versi terbaru
- Akun Cline (untuk opsi 1) atau API key provider (opsi 2)

## Cara Setup

### 1. Install Extension

1. Buka VSCode → **Extensions** (`Ctrl+Shift+X` / `Cmd+Shift+X`).
2. Cari **"Cline"** (publisher: Cline Bot Inc.) → **Install**.
3. Klik ikon Cline di activity bar (sidebar).

### 2. Pilih Cara Akses

#### Opsi A: Cline Provider + Model FREE (paling gampang)

1. Saat diminta autorisasi, pilih **Cline Provider**.
2. **Sign in** dengan akun Cline (bisa via Google/GitHub) — tidak perlu API key, extension mengelola auth otomatis.
3. Di model picker, pilih model yang **bertag `FREE`** (mis. `minimax-m2.5`).

Tanpa isi credit, kamu tetap bisa pakai model FREE.

#### Opsi B: Gemini API Free Tier (BYOK)

1. Buat API key gratis di [Google AI Studio](https://aistudio.google.com/apikey).
2. Di settings Cline, **API Provider** pilih **Google Gemini**.
3. Tempel API key → pilih model Gemini (mis. `gemini-2.0-flash`).

Kuota free tier Gemini berlaku sesuai ketentuan Google.

#### Opsi C: Model Lokal (gratis selamanya)

Pilih provider **Ollama** / **LM Studio** di settings, arahkan ke model lokal kamu (mis. Qwen, DeepSeek). Tidak butuh internet/kuota — tapi butuh hardware yang cukup.

### 3. Mulai Pakai

Tulis tugas di panel Cline dengan bahasa natural — Cline mengusulkan edit file & perintah terminal, kamu **review dan approve** setiap langkah (atau set auto-approve untuk file yang aman).

## Tips

- **Konteks**: `@`-mention file/folder atau biarkan Cline baca codebase otomatis.
- **Checkpoints**: setiap perubahan bisa di-snapshot & rollback.
- **Prompts Library**: ada kumpulan rules & workflow komunitas bawaan extension.
- Cline juga punya **CLI** (`cline`) kalau mau agent di terminal.

## Catatan

- Model FREE bisa berubah sewaktu-waktu — cek tag `FREE` di model picker.
- Kalau model berbayar kepakai tanpa sengaja, credit bisa top-up di [app.cline.bot](https://app.cline.bot) (pay-as-you-go, tidak auto-charge).
- Untuk kombinasi provider lain (OpenRouter, Anthropic, Bedrock, dll) semua bisa diatur di settings panel.

## Referensi

- [Dokumentasi Cline](https://docs.cline.bot)
- [Installing Cline](https://docs.cline.bot/getting-started/installing-cline)
- [Free Models](https://docs.cline.bot/getting-started/free-models)
- [Google Gemini Provider](https://docs.cline.bot/provider-config/google-gemini)
