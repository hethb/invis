# Tulip Trays 🌷

A cute, loving Invisalign companion app — a little gift to help keep that smile glowing 💕

## 🌱 The main idea: your Smiski buddy
Pick a Smiski pet and keep it alive & glowing by caring for your smile. Every day you
hit your wear-time goal and change your bands, its **vitality** grows and it slowly
**grows a tulip** for you. Miss a few days and it gets sleepy — a little tray time
always brings it back (gently, never guilt-trippy). Fill the tulip and it blooms into
your growing garden. 5 Smiskis to choose from; name it whatever you like.

## What's inside
- **Home** — big In/Out toggle, circular wear-time ring (22h goal), last-7-days history
- **Bands** — rubber-band change countdown with a satisfying "Done!" celebration
- **Trays** — current tray tracker, days-left countdown, and a "Switch Tray" bloom celebration
- **Progress** — streak tracker with a growing tulip stem, plus a smile photo timeline
- **Reminders** — on the Home tab, gentle hourly (editable) nudges to keep the trays in

Soft pastels, rounded everything, a tulip motif, and a glow-y Smiski-style mascot that
cheers her on. All data is saved locally in the browser — no accounts, no backend.
Everything starts fresh at zero (Tray 1, no streak, empty week).

## ✏️ Writing your own reminder messages
Open `index.html` and search for **`WRITE YOUR OWN REMINDER MESSAGES`** (near the top of
the `<script>`). Edit the `REMINDER_MESSAGES` list — each item has a `title` (bold line)
and `body` (smaller line). Use `${pet}` anywhere and it becomes her Smiski's name. One is
picked at random each reminder. Commit & push and it goes live in a minute or two.

## Reminders / notifications
Turn them on from the **Reminders** card on Home. They nudge her when the trays are out.
They work while the app is open; for alerts when it's closed, she should **add it to her
home screen** and **allow notifications** when prompted (iOS 16.4+ / Android Chrome).

## Custom Smiski mascot
Want real Smiski photos instead of the drawn one? Drop images into the `images/` folder
(`smiski-idle.png`, `smiski-happy.png`, `smiski-tulip.png`). See `images/README.md`.
Missing files automatically fall back to the built-in SVG.

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
