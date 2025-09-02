PasteClean â€” Paste clean links. One hotkey.

What it does
- Removes tracking junk from URLs automatically when you copy or paste.
- Works system wide from the tray. Fast, lightweight, and local only.
- WPF on .NET 8. Portable single file build supported.

Hotkeys (defaults)
- Clean & Paste: Ctrl+Shift+V
- Undo last paste: Ctrl+Alt+V
- Open Settings: Ctrl+Shift+,
- Hold Shift while pressing Clean & Paste to bypass cleaning

Lite vs Pro
- Lite (free):
  - Autoclean on copy/paste (Conservative/Balanced/Aggressive)
  - Clean & Paste hotkey; Shift to bypass; Undo; Pause
  - History (keeps last 100 items)
- Pro (license):
  - External Link Clean (open cleaned URLs from apps like Slack)
  - Batch Cleaner (extract + clean URLs from text; copy/export TXT/CSV)
  - Filter lists import (AdGuard/uBO $removeparam/$queryprune, wildcards, regex)
  - Smart Packs (curated lists), unlimited history + export
  - More tools coming: perâ€‘app profiles, HTML copy, diff, local stats

Install
- Download the latest EXE from Releases and run it.
- First run opens Settings; Save/Close to hide to the tray.
- Next runs start in the tray (toggle in Settings).

Updates
- Builtâ€‘in update feed is preconfigured; use About â†’ Check for updates.
- Updates are downloaded and staged only when you choose; no autoâ€‘install on launch.

Licensing
- One EXE. Lite by default; unlock Pro with a Gumroad license key.
- Settings at’ License: paste product_id and key at Activate.
- Verification occurs once (counts device uses if you set a limit). Pro is perpetual on this device. Keys are never logged.
- Optional 3â€‘day trial (optâ€‘in).

Privacy
- 100% local. No telemetry. Logs never include clipboard contents or license keys.

Build (developer)
- Requires .NET 8 SDK.
- Publish selfâ€‘contained single file:
  dotnet publish .\ App \ App.csproj -c Release -r win-x64 -p:SelfContained=true -p:PublishSingleFile=true -p:IncludeNativeLibrariesForSelfExtract=true -p:PublishTrimmed=false

Diagnostics
- Logs are stored under %AppData%\PasteClean\Logs.

Changelog
- See docs/patch-notes.txt

Support`n- Open an issue or email (see your store receipt) if you hit problems.`  Buy Pro on Gumroad: https://iamxotic.gumroad.com/l/pasteclean
