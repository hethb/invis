# Tulip Trays 🌷

A cute, loving Invisalign companion app — a little gift to help keep that smile glowing 💕

## What's inside
- **Home** — big In/Out toggle, circular wear-time ring (22h goal), last-7-days history
- **Bands** — rubber-band change countdown with a satisfying "Done!" celebration
- **Trays** — current tray tracker, days-left countdown, and a "Switch Tray" bloom celebration
- **Progress** — streak tracker with a growing tulip stem, plus a smile photo timeline

Soft pastels, rounded everything, a tulip motif, and a glow-y Smiski-style mascot that
cheers her on. All data is saved locally in the browser — no accounts, no backend.

## How to open it
Just open `index.html` in any modern browser (double-click works). It's fully self-contained.

### To use it as a phone app (installable PWA)
It needs to be served over http(s) for install + offline to work. Easiest way:

```bash
cd tulip-trays
python3 -m http.server 8000
```

Then on the phone (same Wi-Fi), visit `http://<your-computer-ip>:8000/` and use
**Share → Add to Home Screen** (iOS) or the **Install** prompt (Android/Chrome).

Or drop the folder on any static host (GitHub Pages, Netlify, Vercel) and open the link.

## Files
| file | purpose |
|------|---------|
| `index.html` | the entire app (HTML + CSS + JS, self-contained) |
| `manifest.webmanifest` | PWA metadata |
| `sw.js` | service worker for offline use |
| `icon.svg`, `icon-*.png`, `apple-touch-icon.png` | app icons (tulip + Smiski) |

Made with love. 🌷💙
