# Setup OpenCode — AI Coding Agent Gratis (Open Source)

[OpenCode](https://opencode.ai) adalah AI coding agent **open source & provider-agnostic** — gratis, dan kamu bebas pilih model dari provider mana pun. Cara gratisnya: pakai provider yang sudah punya plan free, misalnya:

- **GitHub Copilot Free** (login akun GitHub, tanpa API key) ✅ paling gampang
- **Gemini API free tier**
- Model gratis di **OpenCode Zen** (`grok-code`, `gpt-5-nano`, dll)

> OpenCode itu aplikasi **TUI (terminal)** + ada **extension VSCode** sebagai penampil/integrasi — jadi tetap nyaman dipakai dengan VSCode sebagai editor utama.

## Prasyarat

- [Node.js](https://nodejs.org) (untuk install via npm)
- Akun GitHub (untuk Copilot Free) atau API key provider lain

## 1. Install OpenCode CLI

```bash
npm install -g opencode-ai
# atau: bun / pnpm / yarn global add opencode-ai
```

## 2. Sambungkan Provider Gratis

Jalankan `opencode` di folder project, lalu di dalam TUI:

1. Jalankan **`/connect`** → cari **GitHub Copilot**.
2. Buka [github.com/login/device](https://github.com/login/device), masukkan kode yang ditampilkan.
3. Jalankan **`/models`** → pilih model dari Copilot (sebagian model butuh Copilot Pro+).

Alternatif tanpa Copilot — pakai API key provider lain:

```bash
opencode auth login
```

Pilih provider (Gemini, OpenRouter, dll) dan tempel API key-nya. Tersimpan di `~/.local/share/opencode/auth.json`.

Lihat semua model yang tersedia:

```bash
opencode models
```

## 3. Extension VSCode

1. Buka VSCode → **Extensions** (`Ctrl+Shift+X` / `Cmd+Shift+X`).
2. Cari **"OpenCode"** → **Install**.
3. Extension butuh CLI yang sudah terinstall (langkah 1) — otomatis konek.

Kalau CLI dijalankan dari terminal **dalam VSCode**, OpenCode juga mendeteksi editor dan menampilkan diff langsung di VSCode.

## 4. Mulai Pakai

Jalankan `opencode` di root project → chat berbahasa natural, agent bisa baca codebase, edit multi-file, dan jalanin perintah. Model ganti-ganti kapan saja via `/models`.

## Catatan

- OpenCode sendiri **selalu gratis** (open source) — yang dibayar hanya pemakaian model, dan itu bisa 0 dengan provider free di atas.
- Kuota mengikuti provider yang dipakai (mis. Copilot Free: 2.000 completions + 50 chat/bulan).
- **OpenCode Zen** opsional — kumpulan model terverifikasi dari tim OpenCode, ada beberapa model gratis.

## Referensi

- [opencode.ai](https://opencode.ai)
- [GitHub — sst/opencode](https://github.com/anomalyco/opencode)
- [Dokumentasi Providers](https://opencode.ai/docs/providers)
