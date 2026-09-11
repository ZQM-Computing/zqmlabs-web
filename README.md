# zqmlabs-frontend

React SPA serving [zqmlabs.com](https://zqmlabs.com) — the public portal for ZQM Computing.

## Domain: zqmlabs.com

| Subdomain | Route | Component |
|-----------|-------|-----------|
| zqmlabs.com | `/` | HomePage |
| zqmlabs.com | `/business` | BusinessPage |
| zqmlabs.com | `/data` | DataExplorerPage |
| zqmlabs.com | `/gamification` | GamificationPage |
| zqmlabs.com | `/leaders` | LeadersPage |
| zqmlabs.com | `/maps` | MapsPage |
| zqmlabs.com | `/news` | NewsPage |
| zqmlabs.com | `/residents` | ResidentsPage |
| zqmlabs.com | `/tourists` | TouristsPage |
| zqmlabs.com | `/category/:slug` | CategoryPage |
| zqmlabs.com | `*` | NotFoundPage |
| software.zqmlabs.com | `/business` | BusinessPage |
| leaders.zqmlabs.com | `/leaders` | LeadersPage |

## Domain: volusia.zqmlabs.com

> Serves `volusia.zqmlabs.com` via the `volusia-zqmlabs` backend (separate repo).

## Architecture

This is the **frontend layer** of the ZQM modular architecture. It communicates with:
- **zqmlabs-backend** (FastAPI) — API calls for indicators, data, refresh
- **zqmlabs-gamification** — Gamification missions and leaderboard
- **zqmlabs-shared** — Shared types and utilities

## Development

```bash
npm install
npm run dev
npm run build
```

## Repo Map

```
zqmlabs-frontend ←→ zqmlabs-backend (API)
zqmlabs-frontend ←→ zqmlabs-gamification (gamification API)
zqmlabs-frontend ←→ zqmlabs-shared (shared types/utils)
zqmlabs-frontend → volusia-zqmlabs (volusia.zqmlabs.com backend)
```
