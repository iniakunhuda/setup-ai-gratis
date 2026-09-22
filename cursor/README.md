# Setup Cursor — AI Editor dengan Plan Gratis

Cursor adalah AI code editor berbasis VS Code (fork). Punya plan **Hobby gratis** tanpa kartu kredit:

- Tab completions terbatas
- Kuota terbatas untuk Agent/Chat dengan model andalan (Composer, dll)
- **Trial Pro 14 hari** untuk merasakan unlimited completions & akses penuh model

> Catatan: karena Cursor adalah **editor sendiri** (bukan extension), setup-nya agak beda dari Gemini/Copilot — kamu migrasi dari VSCode ke Cursor, bukan pasang di VSCode.

## Prasyarat

- Akun [Cursor](https://cursor.com) — bisa daftar pakai Google/GitHub
- macOS, Windows, atau Linux

## Cara Setup

### 1. Download & Install

- Download dari [cursor.com/download](https://cursor.com/download) sesuai OS kamu.
- Install seperti aplikasi biasa.

### 2. Import Setting VSCode (Opsional, disarankan)

Kalau sudah pakai VSCode, semua setup bisa dipindah sekali klik:

1. Buka **Cursor Settings** (`Ctrl+Shift+J` / `Cmd+Shift+J`).
2. **General > Account > VS Code Import** → klik **Import**.

Extensions, themes, settings, dan keybindings VSCode kamu langsung terbawa.

### 3. Login

Buka Cursor → sign in dengan akun Google/GitHub kamu → otomatis masuk plan **Hobby (gratis)** dengan trial Pro 14 hari.

### 4. Mulai Pakai

- **Tab** — autocomplete AI (terima dengan `Tab`)
- **Ctrl+L / Cmd+L** — chat dengan konteks kode kamu
- **Ctrl+I / Cmd+I** — Agent mode: tulis instruksi, agent eksekusi multi-file

## Cursor CLI (Opsional)

Agent AI di terminal:

```bash
curl https://cursor.com/install -fsS | bash
```

## Catatan

- Kuota Hobby terbatas dan **tidak reset jadi unlimited** — kalau sering pakai agent, kuota cepat habis. Pantau di [usage dashboard](https://cursor.com/dashboard/usage).
- Setelah trial Pro 14 hari selesai, otomatis turun ke Hobby (tidak auto-charge kalau tidak isi kartu).
- Kalau target utama AI **gratis jangka panjang** di VSCode, [Copilot Free](../copilot/README.md) atau [Gemini](../gemini/README.md) lebih lega; Cursor unggul di kualitas agent-nya.

## Referensi

- [Download Cursor](https://cursor.com/download)
- [Quickstart](https://cursor.com/docs/get-started/quickstart)
- [Models & Pricing](https://cursor.com/docs/models-and-pricing)
- [Migrasi dari VS Code](https://cursor.com/docs/configuration/migrations/vscode)
