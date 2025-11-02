# Typing Speed Test

 A lightweight, browser-based typing speed and accuracy tester with levels and a simple dashboard.

## What it is

This project is a small web app that lets users practice typing against sample sentences and track performance (WPM, accuracy, levels, achievements). It's built with plain HTML, CSS and JavaScript — no build step required.

## Files

- `index.html` — Main typing test UI (start screen + test area).
- `dashboard.html` — Simple dashboard/achievements view.
- `css/style.css` — Styles for the app; updated to a modern, responsive look.
- `js/main.js` — Typing test logic (not modified by this change).
- `js/dashboard.js` — Dashboard logic.
- `data/sentences.json` — Sentences used in the typing tests.
- `app.js` — (If present) extra app code.

## Run locally

1. Open the project folder.
2. Double-click `index.html` (or `dashboard.html`) to open in your browser.

Alternatively, to serve with a simple local HTTP server (recommended for some browsers):

On Windows PowerShell:

```powershell
# From project root
py -m http.server 8000; Start-Process "http://localhost:8000/index.html"
```

Or with Node (if installed):

```powershell
npx http-server -c-1 -p 8000
```

## Notes for developers

- Styles were modernized to use card layout, subtle glassmorphism, and responsive grid.
- No changes were made to JS functionality in this update. If you want the UI to show character-level highlights or animated stats, update `js/main.js` and `js/dashboard.js` accordingly.
- Accessibility: inputs and buttons use clearer focus states; further ARIA improvements are recommended.

## Next steps / Suggestions

- Add persistent storage (localStorage) to save best scores and achievements.
- Add selectable themes (dark/light) and adjustable test durations.
- Add unit tests for the scoring logic.

---

Made UI improvements to `index.html`, `dashboard.html`, and `css/style.css` to give the app a modern, responsive look.