# Office Services

Convert a whole folder of documents into PDFs — keeping your folder structure
intact — and optionally apply Bates labels. A Windows & macOS desktop app with
**nothing else to install**: the conversion engine (LibreOffice) is bundled inside.

> **Alpha — version 1.0.0.a.** Expect rough edges; please report issues.

## Download

- **Windows:** [`OfficeServices-1.0.0.a-Setup.exe`](https://github.com/donnie108/office-services/releases/latest/download/OfficeServices-1.0.0.a-Setup.exe) (~289 MB)

_(A macOS build is in the works and will be posted here when ready.)_

## Install

### Windows

1. Download and run **`OfficeServices-1.0.0.a-Setup.exe`**.
2. Because this is an unsigned alpha build, Windows SmartScreen may say
   *"Windows protected your PC."* Click **More info → Run anyway**.
3. Approve the **User Account Control** prompt (it installs to Program Files).
4. Launch from **Start Menu → Office Services** (or the desktop shortcut).

## Requirements

- Windows 10 or 11 (64-bit)
- Nothing else — LibreOffice is bundled.

## What it does

- Converts Word, PowerPoint, images, text/HTML, and emails (`.eml` / `.msg`,
  including their attachments) to PDF, mirroring your input folder structure.
- Copies Excel files, existing PDFs, and videos through unchanged.
- **Bates labeling** (optional): sequential page stamps like `SMITH 000001`
  across every file, renaming files and folders to match.

## Quick start

- **Convert** — pick an Input folder and an Output folder (they must differ),
  then click **Convert**.
- **Bates Labels** (runs on the Output folder) — enter a prefix, start number,
  and digits; tick **Dry Run** to preview the plan in the log first; then
  **Apply Bates Labels**.
- **View Log** (either tab) opens the detailed log.

## Settings & logs

Everything writable lives in a per-user folder — `%APPDATA%\DocConverter` on Windows,
`~/Library/Application Support/DocConverter` on macOS — holding `config.json`, the
`logs` folder, and LibreOffice's working profile.

## Reporting problems

Please open an issue with: what you did and what happened, the log (the **View Log**
button, or `…\DocConverter\logs\converter.log` on Windows /
`~/Library/Application Support/DocConverter/logs/converter.log` on macOS), and the
version (**1.0.0.a**).

## Uninstall

- **Windows:** Settings → Apps → **Office Services** → Uninstall.

Your converted PDFs and the per-user data folder are left in place.
