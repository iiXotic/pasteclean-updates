PasteClean
==========

PasteClean removes tracking junk from URLs. It runs as a clean, local‑only desktop app with a clipboard watcher and a simple batch tool.

Features
--------
- Drop tracking parameters: removes `utm_*`, `fbclid`, `gclid`, `msclkid`, etc.
- Drop tracking fragments: clears `#~:text=…`, `#fbclid=…`, and similar.
- Amazon canonicalization: converts product links to `/dp/ASIN` and strips extras.
- Custom rules: add your own parameters to drop.
- Per‑domain rules: drop specific parameters only for chosen domains.
- Ignore lists: domains and parameters that should never be modified.
- Clipboard watcher: automatically cleans copied URLs in the background.
- Tray menu: Show, Clean clipboard now, Pause/Resume, Quit.
- Batch cleaner: paste many links, clean, and copy the result.
- VirusTotal (optional): scan a URL using your API key.
- Import/Export: backup or share your settings as JSON.
- Manual update check: About → “Check for Update”. No auto‑checks, no telemetry.

Download (Users)
----------------
Grab the installer from GitHub Releases.
- NSIS `.exe` and/or MSI are uploaded per version.
- Windows SmartScreen may warn for unsigned builds. Click “More info → Run anyway”.
- Requires the Microsoft WebView2 runtime (the installer bootstraps it automatically on most systems).

Privacy
-------
- No telemetry. PasteClean does not send data anywhere by default.
- VirusTotal requests only occur when you click Scan and require your own API key.
- Manual update checks only happen when you click “Check for Update”.
- Settings are stored locally (browser localStorage inside the app).
