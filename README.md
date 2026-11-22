# NTCRS Studio — Official Windows Releases & Installers

**NTCRS Studio** is an all-in-one Windows desktop automation suite for creating 9:16 short-form commerce videos with Meta AI, ChatGPT, ElevenLabs / Edge-TTS Thai neural voiceovers, and kinetic subtitles.

👉 **[Download Latest Release (v1.0.5)](https://github.com/Magntcrs/ntcrs-studio-releases/releases/latest)**

---

## Latest Version: `v1.0.5`

View release page & release notes: **[NTCRS Studio 1.0.5](https://github.com/Magntcrs/ntcrs-studio-releases/releases/tag/v1.0.5)**

| Package | Format | Description |
| --- | --- | --- |
| `NTCRS.Studio-1.0.5.exe` | Windows Setup (`.exe`) | **Recommended** per-user Windows installer with desktop shortcut and bundled JRE |
| `NTCRS.Studio-1.0.5.msi` | Windows Installer (`.msi`) | Standard Windows MSI installation package with bundled JRE |
| `NTCRS.Studio.1.0.5.Portable.zip` | Portable ZIP (`.zip`) | No installation required — extract and launch `NTCRS Studio.exe` |
| `checksums-sha256.txt` | Text | SHA-256 checksums for all release artifacts |

---

## What's New in v1.0.5

- **Multi-Chat (1–5 Concurrent Lanes)**: Run 1 to 5 in-app browser chats simultaneously with a shared ChatGPT & Meta AI account, persisted stagger delays, uniform single-line status cards, idle-lane memory cleanup, and collapsible subtitle settings.
- **Video Library Tab**: New `Video Library` workspace tab listing both raw Meta AI clips and finished rendered videos with thumbnails, duration & file-size metadata, category/search filters, Windows Recycle Bin deletion, leftover Temp cleanup (`render-temp`), and 1-click **Send to Studio** editing.
- **Thai TTS & Subtitle Upgrades**: Improved handling for Thai repetition marks (`ๆ`) between speech synthesis and on-screen captions, selectable Thai font styles & font sizes with live preview, collapsible subtitle customization UI, and shared persisted subtitle profiles across Meta AI Studio and Multi-Chat.
- **Cleaner Workspace & Posting Packs**: Removed unused legacy queue/trending tabs, standardized English sidebar navigation tabs, and cleaned up exported affiliate posting pack text.

---

## System Requirements

- **OS**: Windows 10 or Windows 11 (64-bit)
- **Memory**: 8 GB RAM minimum (**16 GB+ RAM recommended** when running 3–5 Multi-Chat lanes concurrently)
- **Disk Space**: ~2 GB free space recommended for the application, browser runtime cache, and video projects
- **Network**: Internet connection required (first startup downloads/initializes the embedded Chromium runtime if not already cached)
- **Zero External Runtime Dependencies**: Includes a bundled Java runtime, built-in Chromium browser (`KCEF`), and native zero-Python Edge-TTS support — no separate Java, Python, or Chrome extension installation is required.

---

## Quick Start

1. Download **`NTCRS.Studio-1.0.5.exe`** (or extract **`NTCRS.Studio.1.0.5.Portable.zip`**) from the [v1.0.5 release page](https://github.com/Magntcrs/ntcrs-studio-releases/releases/tag/v1.0.5).
2. Run the installer or launch `NTCRS Studio.exe`.
3. Open **Meta AI Studio** and sign in once to ChatGPT and Meta AI inside the built-in browser.
4. *(Optional)* Open **Settings** to configure your ElevenLabs API key, preferred Thai voice, and AI provider credentials.
5. Select products or enter a topic in **Meta AI Studio** or **Multi-Chat (1-5)** to generate, dub, subtitle, and organize clips in **Video Library**.

---

## Verify File Integrity (SHA-256)

After downloading, you can verify checksums in Windows PowerShell against `checksums-sha256.txt`:

```powershell
Get-FileHash ".\NTCRS.Studio-1.0.5.exe" -Algorithm SHA256
```

---

## Upgrading from Previous Versions

- Installing a newer `.exe` or `.msi` release (or extracting a newer portable archive) upgrades the app while preserving your local settings database and media library.
- NTCRS Studio also checks this repository for new version notifications automatically on startup.

---

## License

© 2026 NTCRS Studio. All rights reserved.
