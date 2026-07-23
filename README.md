# Timestamp Log

Minimal offline-first PWA for a continuously growing timestamped log.

Live app: https://jukkah.github.io/timestamp-log-pwa/

## Features

- One fullscreen textarea — speed of capture over appearance
- Automatic `YYYY-MM-DD HH:mm` timestamp when you type on an empty line
- Floating **+** button to insert a timestamp
- Autosave to `localStorage` (text, cursor, scroll)
- Installable, works offline
- Follows system light/dark theme
- No accounts, sync, backend, or external dependencies

## Usage

1. Open or install the app
2. Type on a new line — a timestamp is prepended automatically
3. Press Enter for a blank line
4. Use **+** to insert a timestamp without typing first

Data stays on the device only.

## Files

- `index.html` — UI and app logic
- `manifest.json` — PWA manifest
- `sw.js` — cache-first service worker
- `icon.svg` — app icon

## Local development

Serve the folder over HTTP (required for the service worker):

```bash
python3 -m http.server 8765
```

Then open http://127.0.0.1:8765/

## License

[MIT](LICENSE)
