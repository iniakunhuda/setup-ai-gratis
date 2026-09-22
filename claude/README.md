# Setup Claude — AI untuk VSCode

> ⚠️ **Penting:** Berbeda dengan Gemini dan Antigravity, Claude Code **tidak punya free tier**. Plan gratis claude.ai tidak termasuk akses Claude Code. Pilihan gratis/termurah ada di bagian [Catatan](#catatan).

Claude Code dari Anthropic adalah agentic coding tool yang tersedia sebagai **extension VSCode** dan **CLI**. Login cukup pakai akun Claude — tanpa kelola API key.

## Prasyarat

- Akun Anthropic: langganan berbayar (Pro, Max, Team, Enterprise) **atau** akun [Claude Console](https://console.anthropic.com) (bayar per pakai)
- VSCode versi **1.94.0** atau lebih baru

## 1. Install Extension Claude Code di VSCode

1. Buka VSCode → **Extensions** (`Ctrl+Shift+X` / `Cmd+Shift+X`).
2. Cari **"Claude Code"** (publisher: Anthropic).
3. Klik **Install**. Atau langsung dari [VS Code Marketplace](https://marketplace.visualstudio.com/items?itemName=anthropic.claude-code).
4. Buka panel Claude Code → login lewat browser dengan akun Claude kamu. Tidak perlu API key.

Kalau extension tidak muncul, reload VSCode (`Developer: Reload Window`).

Fitur extension: review plan sebelum dieksekusi, auto-accept edit, `@`-mention file dengan range baris, riwayat percakapan, multi-tab chat.

## 2. Claude Code CLI (Opsional)

Extension sudah membundel CLI-nya sendiri untuk chat panel. Tapi kalau mau jalanin `claude` di terminal:

```bash
# macOS / Linux
curl -fsSL https://claude.ai/install.sh | bash

# Windows CMD
curl -fsSL https://claude.ai/install.cmd -o install.cmd && install.cmd && del install.cmd

# Atau via npm (butuh Node.js 22+)
npm install -g @anthropic-ai/claude-code
```

Jalankan `claude` di terminal **dalam VSCode** — otomatis terintegrasi (diff di editor, share diagnostic). Dari terminal eksternal, jalankan `/ide` di dalam Claude Code untuk konek ke VSCode.

## Catatan: Pilihan Gratis / Termurah

| Opsi | Biaya | Keterangan |
|------|-------|------------|
| claude.ai plan gratis | Rp 0 | Chat Claude di web saja, **tanpa** Claude Code |
| Claude Console | Bayar per pakai (API) | Akun baru biasanya dapat **free credit** terbatas — cek [console.anthropic.com](https://console.anthropic.com) |
| Claude Pro | ~$20/bulan | Termasuk Claude Code di VSCode + web + desktop |

Kalau targetnya **AI coding gratis di VSCode**, lebih realistis pakai [Gemini](../gemini/README.md) atau [Antigravity](../antigravity/README.md) yang memang punya free tier resmi.

## Referensi

- [Dokumentasi Claude Code](https://code.claude.com/docs)
- [Setup VSCode](https://code.claude.com/docs/en/vs-code)
- [Autentikasi](https://code.claude.com/docs/en/authentication)
