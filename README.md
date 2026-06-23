# Prodocere

Convert a whole folder of documents into PDFs — keeping your folder structure
intact — and optionally apply Bates labels. A Windows & macOS desktop app with
**nothing else to install**: the conversion engine (LibreOffice) is bundled inside.

## Download

**[⬇ Get the latest release](https://github.com/donnie108/prodocere/releases/latest)**

The releases page always lists the current version and its installers:

- **Windows** — `Prodocere-<version>-Setup.exe` (~290 MB)
- **macOS** — `Prodocere-<version>.dmg` (Apple Silicon)

## Install

### Windows

1. Download and run the **`Prodocere-…-Setup.exe`** from the release above.
2. Because this is an unsigned build, Windows SmartScreen may say
   *"Windows protected your PC."* Click **More info → Run anyway**.
3. Approve the **User Account Control** prompt (it installs to Program Files).
4. Launch from **Start Menu → Prodocere** (or the desktop shortcut).

### macOS

1. Download and open the **`Prodocere-….dmg`**, then drag **Prodocere** to Applications.
2. Because this is an unsigned build, Gatekeeper blocks a normal double-click the
   first time. **Right-click the app → Open**, then confirm — macOS remembers the
   choice for future launches.

## Requirements

- Windows 10 or 11 (64-bit), or macOS on Apple Silicon.
- Nothing else — LibreOffice is bundled.

## What it does

- Converts Word, PowerPoint, images, text/HTML, and emails (`.eml` / `.msg`,
  including their attachments) to PDF, mirroring your input folder structure.
- Copies Excel files, existing PDFs, and videos through unchanged.
- **Bates labeling** (optional): sequential page stamps like `SMITH 000001`
  across every file, renaming files and folders to match.

## Quick start

- **Convert** — pick an Input folder; Prodocere writes the PDFs to a new folder
  named for it, right next to the original.
- **Bates Labels** — choose a folder, enter a prefix, start number, and digits;
  tick **Dry Run** to preview the plan in the log first; then **Apply Bates Labels**.
- **View Log** (either tab) opens the detailed log.

## Settings & logs

Everything writable lives in a per-user folder — `%APPDATA%\DocConverter` on Windows,
`~/Library/Application Support/DocConverter` on macOS — holding `config.json`, the
`logs` folder, and LibreOffice's working profile.

## Reporting problems

Please open an issue with: what you did and what happened, the log (the **View Log**
button, or `…\DocConverter\logs\converter.log` on Windows /
`~/Library/Application Support/DocConverter/logs/converter.log` on macOS), and the
version you installed (shown in **Help → About**).

## Uninstall

- **Windows:** Settings → Apps → **Prodocere** → Uninstall.
- **macOS:** drag **Prodocere** from Applications to the Trash.

Your converted PDFs and the per-user data folder are left in place.
