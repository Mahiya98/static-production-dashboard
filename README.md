# Production Dashboard — Static Demo

A standalone, fully static copy of the production dashboard. All figures are
generated in the browser; there are **no external data sources or third-party
network connections**.

## Live app (GitHub Pages)

https://mahiya98.github.io/static-production-dashboard/

Open the link on a phone and tap **Download app** (Android Chrome) or use
**Share → Add to Home Screen** (iPhone) to install it.

## Run locally

```bash
npm start
```

Then open http://localhost:5600

You can also open `public/index.html` directly, though the local server is
recommended so the PWA/service worker works.

## Notes

- Data is deterministic per refresh seed; **Refresh** generates a new simulated dataset.
- Date range covers the last 120 days.
- `server.js` only serves files from `public/` — it makes no outbound requests.
- Pushes to `main` auto-deploy via GitHub Actions to GitHub Pages.
