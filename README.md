# InstinctFi Frontend

This repo contains the static frontend for the InstinctFi DecenTrade demo.

## How it is deployed
- Hosted as a static site (GitHub Pages or any static host).
- Files served directly: `index.html`, `styles.css`, `app.js`.

## How it connects to the backend
- The frontend opens a WebSocket to the Cloudflare Worker proxy defined in the backend repo.
- The URL is configured in `app.js` via `CONFIG.DRIFT_DLOB_WS_URL`.

## Update flow
1. Edit `index.html`, `styles.css`, or `app.js`.
2. Deploy the static files to your host.
3. If you change the worker URL, update `CONFIG.DRIFT_DLOB_WS_URL` and redeploy.
