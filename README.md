PasteClean — Paste clean links. One hotkey.

What it does
- Removes tracking junk from URLs automatically when you copy or paste.
- Works system‑wide from the tray. Fast, lightweight, and local‑only.
- WPF on .NET 8. Portable single‑file build supported.

Hotkeys (defaults)
- Clean & Paste: Ctrl+Shift+V
- Undo last paste: Ctrl+Alt+V
- Open Settings: Ctrl+Shift+,
- Hold Shift while pressing Clean & Paste to bypass cleaning

Lite vs Pro
- Lite (free):
  - Auto‑clean on copy/paste (Conservative/Balanced/Aggressive)
  - Clean & Paste hotkey; Shift to bypass; Undo; Pause
  - History (keeps last 100 items)
- Pro (license):
  - External Link Clean (open cleaned URLs from apps like Slack)
  - Batch Cleaner (extract + clean URLs from text; copy/export TXT/CSV)
  - Filter lists import (AdGuard/uBO $removeparam/$queryprune, wildcards, regex)
  - Smart Packs (curated lists), unlimited history + export
  - More tools coming: per‑app profiles, HTML copy, diff, local stats

Install
- Download the latest EXE from Releases and run it.
- First run opens Settings; Save/Close to hide to the tray.
- Next runs start in the tray (toggle in Settings).

Updates
- Built‑in update feed is preconfigured; use About → Check for updates.
- Updates are downloaded and staged only when you choose; no auto‑install on launch.

Licensing
- One EXE. Lite by default; unlock Pro with a Gumroad license key.
- Settings → License: paste product_id and key → Activate.
- Verification occurs once (increment_uses_count=false). We cache a DPAPI‑protected token with a 7‑day offline grace. Keys are never logged.
- Optional 3‑day trial (opt‑in).

Privacy
- 100% local. No telemetry. Logs never include clipboard contents or license keys.

Build (developer)
- Requires .NET 8 SDK.
- Publish self‑contained single file:
  dotnet publish .\App\App.csproj -c Release -r win-x64 -p:SelfContained=true -p:PublishSingleFile=true -p:IncludeNativeLibrariesForSelfExtract=true -p:PublishTrimmed=false

Diagnostics
- Logs are stored under %AppData%\PasteClean\Logs.

Changelog
- See docs/patch-notes.txt

Support
- Open an issue
