# Sri Krishna Panchang (శ్రీ కృష్ణ పంచాంగం)

A free, offline-capable Panchang web app in **English and Telugu**: Drik-style monthly calendar, Choghadiya, Hora, Vedic time (ghati/pal/vipal), Kundali, Match Making (Ashta Kuta, doshas, remedies), Rashifal, Muhurta Finder, Shraddha/Tithi finder and a Library of tithis, nakshatras, masams, samvatsaras, poojas and slokas.

Everything runs inside the browser. No account, no server, no data leaves your device. Notes and settings are kept in the browser's local storage.

## Files in this repository

| File | Purpose |
|---|---|
| `index.html` | The app (single file, scrambled/protected build) |
| `manifest.json` | Lets Android Chrome install it as an app |
| `sw.js` | Service worker: offline use on Android and desktop |
| `appcache.manifest` | Offline use on old iPhones and iPads (iOS 10) |
| `icon-180.png`, `icon-192.png`, `icon-512.png` | App icons |
| `.nojekyll` | Tells GitHub Pages to serve the files as they are |
| `LICENSE` | All rights reserved, (c) 2026 V Krishna Vamshi |

## Publish on GitHub Pages (no command line needed)

1. Sign in to GitHub and click **New repository**. Name it, for example, `sri-krishna-panchang`, choose **Public**, and create it.
2. Click **Add file > Upload files**, drag in **all files from this folder** (including `.nojekyll`), and press **Commit changes**.
3. Open **Settings > Pages**. Under **Build and deployment** choose **Deploy from a branch**, pick the `main` branch and the `/ (root)` folder, then **Save**.
4. After a minute your app is live at `https://YOUR-USERNAME.github.io/sri-krishna-panchang/`.

## Use it offline on your phone or iPad

1. Open the address once while online and wait until the green **Offline ready** badge appears at the top.
2. **Android (Chrome):** menu > **Install app**.
3. **iPhone / iPad (including iOS 10.3.3, Safari):** Share > **Add to Home Screen**.
4. After that it opens without internet.

## Updating the app

Replace `index.html` with the new file. Then change the version number in `appcache.manifest` (the line starting with `# version`) and the cache name in `sw.js` (for example `panchang-v4`), so phones download the update. Open the page once online and reopen it.

## Notes

- A free GitHub Pages site needs a **public** repository, so the published `index.html` is visible to everyone. It is a scrambled build; keep your readable source file somewhere private (not in this repository).
- The calculation method can be switched in the app: **Modern Standard** (Drik Ganita with Lahiri ayanamsa, preferred) or **Traditional Panchang** (Moon shifted about 1.55 degrees to match classical printed Telugu panchangs).
- For rituals, always confirm tithi, nakshatra and muhurta with your family priest or temple panchangam. Astrology is traditional guidance for reflection, not a guarantee, and nothing here replaces medical, legal or financial advice.

## License

All rights reserved. (c) 2026 V Krishna Vamshi. See `LICENSE`.
