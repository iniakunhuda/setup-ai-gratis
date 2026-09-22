# Setup Gemini — AI Gratis untuk VSCode

Gemini dari Google punya **free tier** untuk developer individual. Dengan akun Google biasa (tanpa kartu kredit) kamu dapat:

- **Gemini Code Assist** di VSCode — autocomplete + chat AI langsung di editor
- **Gemini CLI** — agent AI di terminal, gratis **60 request/menit & 1.000 request/hari** dengan model Gemini 3 (context window 1M token)

## Prasyarat

- Akun Google (gratis)
- [VSCode](https://code.visualstudio.com) terinstall
- Node.js 20+ (untuk Gemini CLI)

## 1. Gemini Code Assist di VSCode (Editor Utama)

1. Buka VSCode → **Extensions** (`Ctrl+Shift+X` / `Cmd+Shift+X`).
2. Cari **"Gemini Code Assist"** (publisher: Google).
3. Klik **Install**.
4. Klik ikon Gemini di activity bar → **Sign in with Google**.
5. Login lewat browser dengan akun Google kamu. Kalau belum punya akun Gemini Code Assist, kamu akan diarahkan ke pendaftaran **Gemini Code Assist for individuals** (gratis).

Selesai — autocomplete saat mengetik dan chat AI sudah aktif di VSCode.

## 2. Gemini CLI (Bonus, di Terminal VSCode)

Install global via npm:

```bash
npm install -g @google/gemini-cli
```

Jalankan di folder project:

```bash
gemini
```

Saat ditanya *"How would you like to authenticate?"* pilih **1. Sign in with Google**, lalu login lewat browser. Tidak perlu kelola API key.

## 3. Integrasi Gemini CLI dengan VSCode (Opsional)

Supaya Gemini CLI paham isi workspace dan bisa tampilkan diff langsung di editor:

1. Buka terminal **di dalam VSCode**, jalankan `gemini`.
2. CLI otomatis mendeteksi VSCode dan menawarkan koneksi — jawab **Yes**.
3. Atau manual: jalankan `/ide install` di dalam CLI, lalu `/ide enable`.

Extension-nya juga ada di [VS Code Marketplace](https://marketplace.visualstudio.com/items?itemName=google.gemini-cli-vscode-ide-companion) (nama: *Gemini CLI Companion*).

## Catatan

- Free tier login Google: **60 request/menit, 1.000 request/hari**. Detail kuota: [Gemini quota limits](https://cloud.google.com/gemini/docs/quotas).
- Akun Google milik perusahaan mungkin diblokir admin untuk Gemini Code Assist individuals — pakai akun pribadi.
- Butuh kuota lebih? Upgrade ke [Google AI Pro/Ultra](https://one.google.com/about/google-ai-plans/).

## Referensi

- [Gemini CLI — GitHub](https://github.com/google-gemini/gemini-cli)
- [Dokumentasi Gemini Code Assist](https://developers.google.com/gemini-code-assist)
- [FAQ Gemini Code Assist individuals](https://developers.google.com/gemini-code-assist/resources/faqs)
