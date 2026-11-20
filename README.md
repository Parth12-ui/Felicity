# Felicity

Frontend for **Felicity**, a college-fest event platform with participant, organizer and admin portals: event discovery, registration and QR tickets, team registration, merchandise orders with payment-proof review, real-time discussion forums, and feedback.

Built with React 19, Vite and React Router. The visual design shares its palette with Passing Polygons: GitHub-dark surfaces, a blue accent and football-pitch accents.

- **Live:** https://dass-a1-green.vercel.app
- **Backend:** Express + MongoDB on Render, in [event-management-dashboard](https://github.com/Parth12-ui/event-management-dashboard/tree/main/backend)

## Getting started

```bash
npm install
cp .env.example .env   # point VITE_API_URL at your backend
npm run dev            # http://localhost:5173
```

Without `VITE_API_URL`, requests go to `/api`, which the dev server proxies to `http://localhost:3000`.

## Scripts

| Command | What it does |
| --- | --- |
| `npm run dev` | Start the Vite dev server |
| `npm run build` | Production build to `dist/` |
| `npm run preview` | Serve the production build locally |

## Deployment

Deployed on Vercel from this repository's `main` branch. `vercel.json` rewrites all routes to `index.html` for client-side routing. Set `VITE_API_URL` and `VITE_SOCKET_URL` in the Vercel project's environment variables.
