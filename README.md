# NTCRS Studio — Official Windows Releases & Installers

**NTCRS Studio** is a zero-install Windows desktop automation suite for creating 9:16 short-form commerce videos with Meta AI, ChatGPT, ElevenLabs / Edge-TTS Thai neural voiceovers, bundled Thai kinetic subtitles, and Shopee Affiliate tooling.

👉 **[Download Latest Release (v1.0.9)](https://github.com/Magntcrs/ntcrs-studio-releases/releases/latest)**

---

## Latest Version: `v1.0.9`

View release page & release notes: **[NTCRS Studio 1.0.9](https://github.com/Magntcrs/ntcrs-studio-releases/releases/tag/v1.0.9)**

| Package | Format | Description |
| --- | --- | --- |
| `NTCRS.Studio-1.0.9.exe` | Windows Setup (`.exe`) | **Recommended** per-user Windows installer with desktop shortcut and full bundled runtime |
| `NTCRS.Studio-1.0.9.msi` | Windows Installer (`.msi`) | Standard Windows MSI installation package with full bundled runtime |
| `NTCRS.Studio.1.0.9.Portable.zip` | Portable ZIP (`.zip`) | No installation required — extract and launch `NTCRS Studio.exe` |
| `checksums-sha256.txt` | Text | SHA-256 checksums for all release artifacts |

---

## What's New (`v1.0.6` – `v1.0.9`)

- **True Zero-Install Out-of-the-Box Packaging (`v1.0.9`)**:
  - **Bundled Node.js & Playwright Core**: Ships standalone `node.exe` and `playwright-core` inside the app so Shopee Affiliate product collection, gallery picking, and shortlink conversion work on clean PCs without installing Node.js.
  - **All 5 Thai Subtitle Font Families Bundled**: Includes `LINE Seed Sans TH`, `Kanit ExtraBold`, `Mali`, `Prompt`, and `Mitr` directly in the app for FFmpeg `libass` subtitle rendering and live preview (no manual Windows font installation).
  - **Bundled BGM, B-Roll & Hardened Paths**: Ships all 6 BGM tracks (`calm`, `chill`, `cinematic`, `happy`, `luxury`, `upbeat`), 3 B-Roll templates, SFX, `ffmpeg`/`ffprobe`, `adb`/`scrcpy`, non-`C:` Edge/Chrome detection, and FFmpeg path escaping for spaces, Thai characters, and apostrophes (`'`).
- **Fresh-PC Startup & KCEF Reliability (`v1.0.8`)**: Fixed ProGuard bytecode `VerifyError` on fresh Windows machines, added automated JVM `-Xverify:all` release checks, and made embedded Chromium (`KCEF`) startup progress-aware during first-launch downloads.
- **Editable AI Input Text & Custom `.md` Skill Files (`v1.0.7`)**: Customize prompt templates with `{product}` / `{skill}` placeholders and attach local `.md` / `.markdown` skill files across Meta AI Studio and Multi-Chat (1–5).
- **Release Integrity & Protection (`v1.0.6`)**: ProGuard bytecode shrinking/obfuscation, build-time JS minification/obfuscation, and encrypted `.enc` skill assets.

---

## System Requirements

- **OS**: Windows 10 or Windows 11 (64-bit)
- **Memory**: 8 GB RAM minimum (**16 GB+ RAM recommended** when running 3–5 Multi-Chat lanes concurrently)
- **Disk Space**: ~2.5 GB free space recommended for the application, KCEF Chromium cache, and video projects
- **Browser**: Built-in **Microsoft Edge** (included with Windows) or **Google Chrome** (used by Playwright Shopee Affiliate helpers)
- **Network**: Internet connection required (first startup automatically downloads the embedded `KCEF` Chromium runtime if not already cached)
- **Zero Manual Runtime Setup**: Includes bundled Java 21 JRE, Visual C++ DLLs, standalone `node.exe` + `playwright-core`, `ffmpeg`/`ffprobe`, 5 Thai subtitle fonts, `adb`/`scrcpy`, SFX/BGM/B-Roll, and native zero-Python Edge-TTS support — no separate Java, Python, Node.js, FFmpeg, VC++, or font installation required.

---

## Quick Start

1. Download **`NTCRS.Studio-1.0.9.exe`** (or extract **`NTCRS.Studio.1.0.9.Portable.zip`**) from the [v1.0.9 release page](https://github.com/Magntcrs/ntcrs-studio-releases/releases/tag/v1.0.9).
2. Run the installer or launch `NTCRS Studio.exe` (first launch will initialize/cache embedded Chromium automatically).
3. Open **Meta AI Studio** and sign in once to ChatGPT / Gemini and Meta AI inside the built-in browser.
4. *(Optional)* Open **Settings** to configure your ElevenLabs API key, preferred Thai voice, and verify runtime status.
5. Select products or enter a topic in **Meta AI Studio** or **Multi-Chat (1-5)** to generate, dub, subtitle, and organize clips in **Video Library**.

---

## Verify File Integrity (SHA-256)

After downloading, you can verify checksums in Windows PowerShell against `checksums-sha256.txt`:

```powershell
Get-FileHash ".\NTCRS.Studio-1.0.9.exe" -Algorithm SHA256
```

---

## Upgrading from Previous Versions

- Installing a newer `.exe` or `.msi` release (or extracting a newer portable archive) upgrades the app while preserving your local settings database (`%LOCALAPPDATA%\NTCRS Studio\ntcrs`) and media library.
- NTCRS Studio checks this repository for new version notifications automatically on startup.

---

## License

© 2026 NTCRS Studio. All rights reserved.
