# 📦 PalletScan

Mobile warehouse pallet scanner + counter. Scan pallet labels with your phone camera, confirm the transcription, and build a table of counts that exports to CSV.

**Live app:** https://qamotech.github.io/PalletScan/

## What it does

- **SCAN** — Live barcode scanning (html5-qrcode), photo capture with OCR transcription (Tesseract.js) plus a confirmation screen, and manual entry fallback. Duplicate-lot guard, torch toggle, front/back camera flip, rapid-scan auto-add mode.
- **COUNT** — Tap counter (P/R/C) with built-in brand pack specs: Popz (2400/10/24), Waves (2496/8/24), Belle Vie (2400/10/24), Frost & Gridlock (1680/7/12). Shorthand entry (`3p 2r 5c`), pack-aware can math, outlier flags.
- **TABLE** — Full scan/count log: filter, brand filter, sortable columns, edit rows, 6-second undo delete, CSV download matching cycle-count sheet columns, JSON backup/restore.
- **SUMMARY** — Totals by brand, per-location breakdown, live stats.

## Details

- Single-file HTML app — no build step, no server. Open `index.html` and go.
- Dark mobile-first UI, works offline after first load (CDN libraries cache on first visit).
- Data persists in `localStorage`; named sessions keep separate tables.
- Camera requires HTTPS (GitHub Pages URL above) or localhost.

Built for warehouse cycle counts at Arc Beverage.
