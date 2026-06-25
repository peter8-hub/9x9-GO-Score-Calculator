# 9x9 Go Screenshot Scorer

This is a static, browser-only web app. It does not need a backend.

## Files

- `index.html` — the app
- `manifest.json` — install metadata for phone/home-screen use
- `sw.js` — offline cache when hosted over HTTPS
- `icon-192.png` / `icon-512.png` — app icons

## Best phone setup

Host this folder as a static website, open the URL in Safari on iPhone, then use:

Share → Add to Home Screen → Add

## Recommended static hosts

- GitHub Pages
- Netlify
- Cloudflare Pages
- Vercel

For iPhone install/offline behavior, use an HTTPS URL. Local file previews may block JavaScript.
