# Setup Amazon Q Developer — AI Gratis dari AWS untuk VSCode

Amazon Q Developer adalah AI assistant dari AWS: chat, code completion, agentic coding, dan security scan langsung di VSCode. Punya **Free tier permanen** (bukan trial):

- Login pakai **AWS Builder ID** — **tidak perlu akun AWS**, tanpa kartu kredit
- Free tier dengan batas pemakaian bulanan: chat, completions, agentic coding, security scan

## Prasyarat

- VSCode terbaru
- Email biasa untuk daftar Builder ID

## Cara Setup di VSCode

1. Buka VSCode → **Extensions** (`Ctrl+Shift+X` / `Cmd+Shift+X`).
2. Cari **"Amazon Q"** (publisher: Amazon Web Services) → **Install**.
3. Klik **ikon Amazon Q** di sidebar VSCode.
4. Ikuti instruksi di browser untuk **authenticate dengan AWS Builder ID** — kalau belum punya akun, langsung daftar di proses sign-in (gratis, cuma email + password).
5. Balik ke VSCode → klik ikon Amazon Q untuk mulai chat, atau pilih **Amazon Q** di navigation bar bawah.

Selesai — tanpa setup API key, tanpa akun AWS.

## Fitur Utama

- **Chat** — tanya kode, file, dan error dengan konteks workspace.
- **Agentic coding** — toggle via ikon `</>` di bawah panel chat; Q bisa edit multi-file & jalankan command dengan persetujuan kamu.
- **Code completion** — suggestions inline saat mengetik.
- **Security scans** — review kerentanan kode.
- **Amazon Q CLI** — versi terminal, juga free tier dengan Builder ID (macOS/Linux).

## Catatan

- Free tier punya **batas bulanan** — detailnya di [halaman pricing Amazon Q Developer](https://aws.amazon.com/q/developer/pricing/).
- Free tier **hanya untuk Builder ID di IDE/CLI**. Login IAM Identity Center/IAM (akun AWS perusahaan) tidak mendapat free tier di IDE.
- Catatan privasi: di free tier, konten bisa dipakai AWS untuk improve service — jangan tempel data sensitif/kredensial.
- Butuh lebih? Upgrade ke **Pro** (~$19/bulan) via subscription.

## Referensi

- [Dokumentasi Amazon Q Developer](https://docs.aws.amazon.com/amazonq/latest/qdeveloper-ug/what-is.html)
- [Setup di IDE](https://docs.aws.amazon.com/amazonq/latest/qdeveloper-ug/q-in-IDE-setup.html)
- [Tiers & Free tier](https://docs.aws.amazon.com/amazonq/latest/qdeveloper-ug/q-tiers.html)
- [Pricing](https://aws.amazon.com/q/developer/pricing/)
