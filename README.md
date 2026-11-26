# Mr. Zinger POS — Android PWA / GitHub Pages

This project wraps the supplied `mr_zinger_pos_software (15).html` POS app as an installable Progressive Web App.

## Publish on GitHub Pages

1. Sign in to GitHub and create a **new public repository** (for example `mr-zinger-pos`).
2. Upload **all files and folders** from this project. Keep `index.html`, `manifest.webmanifest`, and `sw.js` in the repository root.
3. Open **Settings → Pages**.
4. Under **Build and deployment**, choose **Deploy from a branch**.
5. Select branch **main** and folder **/(root)**, then Save.
6. Wait for GitHub Pages to publish. Open the generated HTTPS website URL on your Android phone in Chrome.

## Install on Android

1. Open the published website in Chrome while online for the first visit.
2. Tap Chrome's **⋮** menu.
3. Choose **Install app** or **Add to Home screen** (wording varies by Chrome version).
4. Confirm. The Mr. Zinger POS icon will appear on your home screen and open in app-style standalone mode.

## Included POS features from the supplied HTML

- POS menu search/category filtering and cart quantity controls
- Checkout and thermal-style bill printing
- Menu item add/edit/delete and image upload
- Inventory list, stock adjustment and low-stock indicators
- Daily sales / Z-report views and media manager
- Logo/address settings and local browser storage

## Important notes

- PWA installation and service workers require HTTPS; GitHub Pages provides HTTPS.
- The first visit needs internet. The service worker caches the app shell and makes best-effort caches of external assets after they have loaded online.
- The original POS uses browser `localStorage`. Data stays in that browser/device profile; it is **not** automatically synchronized to another phone or computer. Clearing Chrome site data can erase it. Export/backup your records regularly if the app provides that option.
- The original HTML loads Tailwind CSS, Font Awesome, Google Fonts and menu photos from external services. Those assets may not all be available offline unless previously cached.
- GitHub Pages hosts the website; it does not provide a database or secure multi-user backend.
- This package keeps the supplied POS application and adds PWA files; it does not convert the local-only data model into cloud sync.
