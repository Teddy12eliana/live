# SportsSpherePro — All-in-One (Integrity Engine + Intelligence Suite)

**Deploy on Netlify** and get:
- Cinematic homepage (KPIs, sparkline, Top 5 Live, AI narrative, Push Alerts toggle)
- Admin control page `/admin.html`
- Accuracy engine with auto-grader (scheduled), conflicts, manual resolution & exports
- Calibration updates stored in `calibration.json`
- Alerts engine with optional webhook + web push

## Environment Variables (Netlify → Site Settings → Environment)
- `ODDS_API_KEY` (required)
- `THESPORTSDB_KEY` (optional)
- `WEBHOOK_URL` (optional) — Slack/Discord webhook for alerts
- `VAPID_PUBLIC_KEY`, `VAPID_PRIVATE_KEY`, `VAPID_MAILTO` (optional) — for browser push

## Endpoints
- Accuracy: `accuracy-*`, `auto-grade`, `auto-grade-manual`, `calibration-read`
- Live & AI: `live-scores`, `ai-narrative`, `membership-access`
- Push: `push-publickey`, `push-subscribe`, `push-broadcast`
- Alerts: `alerts-engine` (scheduled)

## Deploy
Upload the ZIP to Netlify → set env vars → open `/` and `/admin.html`.
