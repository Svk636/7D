# 90-Day Path — Weekly Training Tracker PWA

Weekly exercise planner for the 90-Day Bruce Lee Protocol, deployable as a Progressive Web App via GitHub Pages.

## Deploy to GitHub Pages

1. Create a new GitHub repository (e.g. `90day-weekly`)
2. Upload all files in this folder to the repo root:
   - `index.html`
   - `manifest.json`
   - `sw.js`
   - `icons/icon-192.png`
   - `icons/icon-512.png`
   - `.nojekyll`
3. Go to **Settings → Pages → Source** → select `main` branch, `/ (root)`
4. Your app will be live at `https://<your-username>.github.io/<repo-name>/`

## PWA Features

- **Offline support** — full cache-first SW caches app shell + CDN fonts + html2pdf
- **Installable** — Add to Home Screen banner on Android/iOS/Desktop
- **This Week button** — auto-detects current week (based on Apr 6 2025 start) and jumps to it; current week highlighted in gold in nav bar
- **Offline badge** — shows when network is unavailable
- **Auto-update** — SW checks for updates every 30 minutes
- **Safe-area aware** — notch/island padding on iOS
- **Scrollable nav bar** — week buttons scroll horizontally on narrow screens
- **PDF export** — download current week or all 12 weeks via html2pdf (cached for offline use)

## File Structure

```
/
├── index.html       ← App shell + all 13 pages (overview + 12 weeks)
├── manifest.json    ← PWA manifest
├── sw.js            ← Service Worker (cache-first, CDN-aware)
├── .nojekyll        ← Prevents Jekyll processing on GitHub Pages
└── icons/
    ├── icon-192.png
    └── icon-512.png
```
