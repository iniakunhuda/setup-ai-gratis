# Setup Kiro — Agentic IDE Gratis dari AWS

[Kiro](https://kiro.dev) adalah **agentic IDE** dari AWS, dibangun di atas fondasi VS Code. Dikenal dengan pendekatan **spec-driven development**: ide → requirements → design → tasks, lalu agent yang eksekusi.

Plan **Free**:

- **50 credits/bulan** (dipakai fraksional sesuai kompleksitas request)
- Login cukup **Google / GitHub / AWS Builder ID** — tanpa kartu kredit
- Fitur utama (chat agent, specs, steering) tetap bisa dipakai

## Prasyarat

- macOS, Windows, atau Linux
- Akun Google/GitHub (atau email untuk Builder ID)

## Cara Setup

### 1. Download & Install

1. Buka [kiro.dev](https://kiro.dev) → **Download**.
2. Install seperti aplikasi biasa.

### 3. Import Setting VSCode (Opsional)

Karena basisnya VS Code, saat pertama kali dibuka Kiro menawarkan **import profile VSCode** — extensions, themes, keybindings, dan settings langsung terbawa.

### 2. Login

1. Buka Kiro.
2. Sign in dengan **Google**, **GitHub**, atau **AWS Builder ID**.
3. Otomatis masuk plan **Free** (50 credits).

### 3. Mulai Pakai

- **Chat agent** — tulis instruksi bahasa natural, agent edit multi-file & jalankan command (kamu review tiap langkah).
- **Specs** — klik `+` di spec pane atau buka spec session di chat: Kiro generate `requirements.md`, `design.md`, `tasks.md` di `.kiro/specs/<fitur>/` lalu eksekusi task satu per satu.
- **Steering** — file panduan proyek di `.kiro/steering/` supaya agent konsisten dengan konvensi codebase.

## Kiro CLI (Opsional)

Versi terminal, sama-sama pakai free tier:

```bash
curl -fsSL https://cli.kiro.dev/install | bash
kiro-cli login --social github    # atau google, atau Builder ID (free)
```

## Tips Hemat Credit

- Free tier **tidak support add-on credits** — habis 50 credits harus tunggu reset bulanan.
- Buat request yang kompleks jadi **spec** (planning lebih murah daripada trial-error dengan agent).
- Model besar/pro thinking makan credit lebih cepat — pilih model sesuai kebutuhan.

## Catatan

- Seperti Amazon Q free tier, konten individual/free tier bisa dipakai untuk service improvement (bisa **opt-out** di settings).
- Paid: Pro mulai ~$19-20/bulan (1.000+ credits, bisa beli add-on $0.04/credit).

## Referensi

- [Kiro](https://kiro.dev)
- [Dokumentasi](https://kiro.dev/docs)
- [Migrasi dari VS Code](https://kiro.dev/docs/migrating-from-q-developer)
- [Billing & Tiers](https://kiro.dev/docs/cli/billing)
