# GN Purchasing System – ការដំឡើង / Installation Guide

## 1. Host it once (HTTPS required / ត្រូវការ HTTPS)
A PWA installs only from an HTTPS link (not by double-clicking the file).
Upload this whole folder to any static host, e.g.:
- **Netlify Drop**: go to app.netlify.com/drop, drag the folder in → you get an https link.
- **GitHub Pages** or **Cloudflare Pages**: upload the folder, enable Pages.
Share the link with staff. Keep all files together (index.html, sw.js, manifest.webmanifest, icons/).

## 2. Android (Chrome) / ទូរស័ព្ទ Android
1. Open the link in Chrome.
2. Tap ⋮ menu → **Install app** (or *Add to Home screen*).
3. Open "GN Purchasing" from the home screen.

## 3. iPhone / iPad (Safari only) / iPhone
1. Open the link in **Safari**.
2. Tap Share ⬆ → **Add to Home Screen** → Add.

## 4. Computer (Chrome / Edge) / កុំព្យូទ័រ
1. Open the link.
2. Click the install icon ⊕ at the right of the address bar → **Install**.
   (Edge: ⋯ → Apps → Install this site as an app.)

## Notes
- Data and login still use Supabase online; the app shell opens offline, but saving/syncing needs internet.
- To release an update: replace index.html and change `CACHE = 'gn-purchasing-v1'` in sw.js to `v2`.
- If you can't host: send GN_Purchasing_System_LIVE.html directly; it works in a browser but can't be installed.
