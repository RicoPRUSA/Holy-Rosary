# Holy Rosary
A quiet, offline-first companion for praying the Rosary — built as a single self-contained web app with no backend, no account, and no tracking.

---

## What it is

Holy Rosary walks you through a complete, traditional recitation of the Rosary — every prayer, every bead, every mystery — with the day's correct set of mysteries chosen automatically and the whole interface tinted to match the Church's actual liturgical calendar.

**Live app: [ricoprusa.github.io/Holy-Rosary](https://ricoprusa.github.io/Holy-Rosary/)**

Open that link in a browser, or add it to your phone's home screen, and it behaves like a native app — no internet connection required after the first load.

## Features

**Prayer flow**
- Full guided sequence: Preparatory Prayer, Sign of the Cross, Apostles' Creed, all five decades, the Litany of Loreto, Hail Holy Queen, Memorare, and Saint Michael's Prayer
- Correct mystery set surfaced automatically for each day (Joyful, Sorrowful, Glorious, Luminous) per the traditional weekly cycle
- Leader/response text distinguished with bold — the group's response in prayers like the Hail Mary, Our Father, Glory Be, and the Litany is bolded to support group recitation
- Optional personal intention — type what you're praying for, and it's woven into the opening prayer
- Optional dedication for a deceased loved one, which adds the De Profundis and Eternal Rest prayers throughout

**Design**
- Full English and Spanish translation, switchable anytime
- Liturgical-season-aware color theme — the accent color shifts between Advent violet, Christmas gold, Lent violet, the Triduum's deep red, Eastertide gold, Pentecost red, and Ordinary Time green, matching the actual color the Church assigns each season
- Light and dark mode, with a dark-mode-specific palette verified against WCAG AA contrast requirements rather than just inverting colors
- Adjustable text size for the prayer text
- A rosary bead progress tracker, plus a compact circular bead visualizer showing your position in the current decade

**Practical**
- Resumes exactly where you left off if you close the app mid-rosary
- Prayer streak tracker — a 7-day dot row and current streak count on the home screen
- Haptic feedback on taps, with a mute toggle
- Fully offline after first load (service worker caching)
- No accounts, no analytics, no network requests once installed

## Using it

**On a phone (recommended):**
1. Open **[ricoprusa.github.io/Holy-Rosary](https://ricoprusa.github.io/Holy-Rosary/)** in Safari (iOS) or Chrome (Android)
2. Use "Add to Home Screen" (iOS) or "Install app" (Android)
3. It now behaves like a native app — its own icon, no browser bar, works offline

**In a browser:**
Just visit **[ricoprusa.github.io/Holy-Rosary](https://ricoprusa.github.io/Holy-Rosary/)** — no install needed.

## Technical notes

- No build step, no dependencies, no package manager — it's plain HTML/CSS/JS
- The only external resource is the Google Fonts stylesheet (Fraunces + Inter); everything else, including the app icon, is self-contained
- State is kept in `localStorage` only, on-device: active session (for resume), prayer streak history, dark mode preference, haptics preference
- Nothing is ever sent to a server — there is no server

## License / attribution

Prayer texts are traditional Catholic prayers in the public domain. Feel free to adapt the app for personal or parish use.
