# TypeMaster

A modern typing speed tester with multiple time modes, live accuracy, and a clean light/dark theme toggle. Runs entirely in the browser—no build step required.

## Features
- Multiple timed modes (15s, 30s, 60s, 120s) with quick switching
- Live stats: WPM, CPM, errors, accuracy, and remaining time
- Restart via button or keyboard hint (Tab then Enter)
- Theme toggle with preference saved to localStorage
- Randomized practice text pulled from `js/para.js`

## Quick Start
1. Open `index.html` directly in your browser; or
2. Serve the folder locally, e.g.:

```sh
cd TypeMaster
python3 -m http.server 8000
# visit http://localhost:8000
```

## Usage
- Pick a time mode, click anywhere (or start typing) to begin.
- Watch stats update in real time; restart anytime with the button or Tab → Enter.
- Toggle the moon/sun icon to switch themes; preference persists between visits.

## Project Structure
- `index.html` — layout and controls
- `style.css` — themes and UI styling
- `js/para.js` — pool of sample paragraphs
- `js/script.js` — typing logic, timers, stats, and theming

## Customization
- Add or edit practice text by updating the `para` array in `js/para.js`.
- Change default timer options by editing the `.time-btn` values in `index.html`.
- Tweak colors or typography via CSS variables in `style.css` (`:root` and `[data-theme]`).
