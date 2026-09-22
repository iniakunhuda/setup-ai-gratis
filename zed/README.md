# Setup Zed — Editor Cepat dengan AI Quota Gratis

[Zed](https://zed.dev) adalah editor open-source berperforma tinggi (ditulis in Rust) dengan AI bawaan. Bukan berbasis VS Code, tapi flow-nya mirip dan ada integrasi agent eksternal.

**Plan Personal (gratis selamanya):**

- **Edit predictions** (autocompletion AI) dengan kuota gratis — sekitar **2.000/bulan** menurut perbandingan terbaru
- Chat/agent terbatas di plan gratis
- **Student gratis 1 tahun** (plan Pro) via [GitHub Student Pack](https://education.github.com/pack)

> Angka kuota dari sumber pihak ketiga — verifikasi langsung di [zed.dev/pricing](https://zed.dev/pricing).

## Prasyarat

- **macOS atau Linux** (dukungan Windows masih terbatas — ini pertimbangan utama sebelum pilih Zed)

## Cara Setup

### 1. Install

```bash
# macOS
brew install --cask zed

# Linux
curl -f https://zed.dev/install.sh | sh
```

Atau download dari [zed.dev/download](https://zed.dev/download).

### 2. Sign In

1. Buka Zed → klik ikon profil / **Sign In**.
2. Daftar/login akun Zed (bisa via GitHub/Google).
3. Plan **Personal ($0)** aktif otomatis — edit predictions langsung jalan tanpa setup tambahan.

### 3. Mulai Pakai AI

- **Edit predictions** — inline completion otomatis saat mengetik, terima dengan `Tab`.
- **Agent Panel** (`Ctrl+?` / `Cmd+?`) — chat + agentic editing dengan konteks project.
- Bisa pilih model di settings AI, atau sambungkan provider sendiri (lihat bawah).

## Jalur "Lebih Gratis" via BYOK / ACP

Kalau kuota bawaan habis, Zed punya dua pintu tambahan:

### BYOK (API key sendiri)

Settings → AI → pilih provider: Anthropic, OpenAI, **Gemini** (pakai API key free tier dari [Google AI Studio](https://aistudio.google.com/apikey)), OpenRouter, atau **Ollama** lokal.

### ACP — Agent Eksternal di Dalam Zed

Zed mendukung **Agent Client Protocol (ACP)**: agent CLI eksternal bisa jalan di dalam Zed — misal **Gemini CLI** (free tier Google) tampil sebagai agent di panel Zed, lengkap dengan diff di editor. Pasang dari Agent Panel → **Install Agent** → pilih Gemini.

Ini kombinasi paling hemat: editor gratis + agent pakai kuota gratis dari provider-nya.

## Catatan

- Kuota free terbatas — untuk chat/agent berat, terasa lebih sempit dibanding [Copilot Free](../copilot/README.md) atau [Gemini Code Assist](../gemini/README.md).
- Pro mulai **$10/bln** kalau mau kuota lega.
- Zed bukan VSCode — extensions ecosystem-nya beda (jauh lebih kecil). Kalau workflow kamu bergantung ekstensi VSCode, [Cline](../cline/README.md) atau [OpenCode](../opencode/README.md) lebih pas.

## Referensi

- [zed.dev](https://zed.dev)
- [Download](https://zed.dev/download)
- [Pricing](https://zed.dev/pricing)
- [Dokumentasi AI](https://zed.dev/docs/ai/llm-landscape)
