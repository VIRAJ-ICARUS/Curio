# Curio PWA

Curio is a mobile-friendly, installable web app version of the daily brain-game circuit. It uses the supplied Curio palette and the original starter-game list from the shared code.

## Included
- Today, Games, and Settings tabs
- Daily circuit, check-offs, progress bar, streak and week count
- Add/edit/remove games, categories, and circuit inclusion
- Local browser storage (no account or cloud sync)
- JSON export/import backup
- PWA manifest and service worker for installation/offline app shell
- Opens game HTTPS links in a new browser tab; Android may route supported verified app links to installed apps, but app launching cannot be guaranteed for every app

## Publish free with GitHub Pages
1. Create a GitHub account if you do not already have one.
2. Create a new **public** repository named `curio`.
3. Upload the contents of this folder (the files themselves, not the parent folder) to the repository root.
4. In the repository, open **Settings → Pages**. Choose **Deploy from a branch**, select `main` and `/ (root)`, then save.
5. Wait for the Pages deployment and open the published URL on your Android phone in Chrome.
6. In Chrome's menu, choose **Install app** or **Add to Home screen**.

## Important notes
- Test first using the published HTTPS URL; service workers and installation do not work from a `file://` preview.
- The app stores data in the browser's local storage. Clearing browser/site data can erase it, so use Settings → Export my data to back up.
- Data is local to the browser/device and does not sync automatically.
- The current app uses HTTPS links. If Android recognizes a verified app link for an installed app, it may open that app; otherwise the website opens in the browser. Curio cannot universally inspect installed apps from a PWA.
- This is a web app, not an APK and not a native Android app.
