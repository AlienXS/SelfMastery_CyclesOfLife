# Cycles of Life — PWA
### Based on *Self Mastery and Fate with the Cycles of Life* by H. Spencer Lewis (AMORC, 1929)

---

## Files in this package

```
index.html      ← The complete app (all logic is inside this one file)
manifest.json   ← PWA metadata for installation
sw.js           ← Service worker (enables offline use)
icons/
  icon-192.png  ← App icon (Android / PWA)
  icon-512.png  ← App icon (splash screen / high-res)
```

---

## How to install as a standalone app

The app is a **Progressive Web App (PWA)**. No app store needed.
You just need to host the files anywhere — including your own PC — and open them in a browser.

---

### Option A — Host for free on GitHub Pages (recommended)

1. Create a free account at [github.com](https://github.com)
2. Create a new repository (e.g. `cycles-of-life`)
3. Upload all four files + the `icons/` folder
4. Go to **Settings → Pages → Source → main branch / root**
5. Your app will be live at `https://yourusername.github.io/cycles-of-life/`

**Android:** Open that URL in Chrome → tap the **⋮ menu → "Add to Home screen"** → the app installs as a full-screen icon, no browser bar, works offline.

**iPhone/iPad:** Open in Safari → tap **Share → "Add to Home Screen"**.

---

### Option B — Run locally from your computer

If you have Python installed:

```bash
cd /path/to/cycles-of-life-pwa
python3 -m http.server 8080
```

Then open `http://localhost:8080` in your browser.

> ⚠️ You must use a local server (not just open the HTML file directly) for the service worker and PWA features to work.

---

### Option C — Use any web host

Upload the four files + `icons/` folder to any web server, shared hosting, Netlify, Vercel, etc. The app works on any HTTPS host.

---

## Features

- **Daily Hour Cycle** — all 7 time periods for the day, based on your timezone
- **Practical Guidance** — Lewis's specific Favour / Avoid advice for each period
- **Year Periods** — your 7 × 52-day year cycle from birthday to birthday
- **My Cycles** — Life Cycle, Soul Cycle, and Birth Hour interpretation
- **Timezone support** — standard time offset selector with auto-detect
- **24-hour clock** throughout
- **Offline support** — works without internet once installed
- **Remembers your birth data** — saved in browser storage between sessions

---

## Lewis's instruction on time

> *"Standard time as measured from Greenwich must be used. If daylight saving time is used in any locality, these variations must be ignored."*

The app follows this exactly — always use standard (winter) time for your location.

---

*Based faithfully upon Self Mastery and Fate with the Cycles of Life by H. Spencer Lewis, published by the Rosicrucian Order AMORC, 1929.*
