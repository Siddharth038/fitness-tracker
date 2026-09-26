# Personal Fitness Dashboard — iPhone/PWA version

## Important
A local `file://` HTML page is not the reliable way to run a full PWA on iPhone.
This version is designed to be opened from a normal **HTTPS web address** in Safari.
It needs **no backend, database, login, or server-side code**. It is just static files.

## iPhone
1. Put this folder on a static host (GitHub Pages, Netlify Drop, Cloudflare Pages, etc.).
2. Open the resulting HTTPS URL in Safari.
3. Tap **Share → Add to Home Screen**.
4. Open it from the new home-screen icon.

## Tracking data
The app uses `localStorage`.
- Same website/origin + future app version that keeps the same storage key = old tracking data remains.
- A different domain, different origin, or unrelated local `file://` location = it may have separate storage.
- The app includes Backup/Restore and creates an automatic local snapshot before writes, so data recovery is easier.
- Export a JSON backup before replacing or moving the website.

## Versioning policy
Future versions should keep:
`const KEY = "sid_fitness_dashboard_v1";`
If the data schema changes, migrate/merge fields instead of replacing the stored object.

## Files
- `index.html` — app
- `manifest.webmanifest` — iPhone install metadata
- `sw.js` — offline cache
- `icon-192.svg`, `icon-512.svg` — home-screen icons
