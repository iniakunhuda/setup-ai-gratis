# Setup Trae — AI IDE Gratis dari ByteDance

[Trae](https://www.trae.ai) adalah AI IDE dari ByteDance, berbasis **fork VS Code** (jadi setting/extensions VSCode bisa diimport). Punya plan **Free**:

- **Auto mode** (agent pilih model otomatis) — kuota terbatas
- **5.000 autocomplete/bulan**
- 2 concurrent cloud tasks
- Akses terbatas ke model early-access

> Catatan: docs Trae IDE belum tersedia di context7 — info di bawah dari situs resmi Trae. Detail kuota bisa berubah, cek [trae.ai/pricing](https://www.trae.ai/pricing).

## Prasyarat

- macOS atau Windows (cek halaman download untuk dukungan Linux terbaru)
- Akun Google/GitHub untuk login

## Cara Setup

### 1. Download & Install

1. Buka [trae.ai/download](https://www.trae.ai/download).
2. Download installer sesuai OS → install seperti aplikasi biasa.

### 2. Login

1. Buka Trae.
2. Sign in dengan akun **Google** atau **GitHub** — langsung masuk plan Free.
3. Saat setup awal, pilih **import dari VS Code** kalau ada — extensions, themes, settings, dan keybindings ikut terbawa.

### 3. Mulai Pakai

- **Autocomplete** — inline suggestions saat mengetik (terima dengan `Tab`).
- **Builder / Agent mode** — tulis instruksi bahasa natural, agent generate & edit multi-file sambil jalanin command; kamu review tiap langkah.
- **Chat** — tanya soal kode dengan konteks file/workspace.
- Layout & shortcut familiar karena basisnya VS Code (`Ctrl+L` chat, `Ctrl+I` builder).

## Trae Agent CLI (Opsional, Open Source)

ByteDance juga merilis [Trae Agent](https://github.com/bytedance/trae-agent) — CLI agent open-source yang **BYOK** (bawa API key sendiri). Gratis selama pakai provider free tier (mis. Gemini free tier, OpenRouter `:free`):

```bash
git clone https://github.com/bytedance/trae-agent.git
cd trae-agent
uv sync --all-extras
source .venv/bin/activate

# pakai provider dengan free tier
export GOOGLE_API_KEY="your-google-api-key"
trae-cli run "Fix the bug in main.py" --provider google --model gemini-2.5-flash
```

## Catatan

- Kuota Free terbatas dan tidak reset jadi unlimited — pantau di settings akun.
- Paid plan **Pro** (~$20/bulan) buka semua model + autocomplete unlimited.
- Trae IDE dari ByteDance (perusahaan China) — pertimbangkan kebijakan data kalau kodenya sensitif.

## Referensi

- [Download](https://www.trae.ai/download)
- [Pricing](https://www.trae.ai/pricing)
- [Trae Agent — GitHub](https://github.com/bytedance/trae-agent)
