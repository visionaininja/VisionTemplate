# App Template

A clean, ready-to-demo starting point built with **React Router 8**, **Tailwind v4**,
and the "Signal" design system — cool indigo brand, Geist type, dark mode by default.

Use it as a **GitHub template**: create a new repo from it for each demo, rename in
`app/config.ts`, and start building.

## Quick start

```bash
npm install
npm run dev
```

The app runs at `http://localhost:5173`.

## Make it yours

- **Name & description** — edit `SITE` in `app/config.ts` (drives the navbar, footer, and `<title>`).
- **Nav links** — add routes in `app/routes.ts`, then list them in `NAV_LINKS` in `app/config.ts`.
- **Brand mark** — swap the SVG in `app/components/Logo.tsx`.
- **Theme** — all colors live as semantic tokens in `app/app.css` (`:root` for light, `.dark` for dark).

## What's included

| Path | What it is |
| --- | --- |
| `app/app.css` | Design system: theme tokens, fonts, and utilities (`aurora`, `grain`, `gradient-text-brand`, `card-lift`, `text-display`). |
| `app/config.ts` | Site name, description, and nav links. |
| `app/root.tsx` | Document shell, dark-by-default boot script, app frame (Navbar + Footer). |
| `app/components/` | `Button` / `LinkButton`, `Navbar`, `Footer`, `Logo`, `ThemeToggle`. |
| `app/routes/home.tsx` | Example landing page showing the style in use. |

Style with the **semantic tokens** (`bg-background`, `text-muted-foreground`,
`border-border`, `bg-primary`, …) rather than raw Tailwind colors so light/dark
stay consistent.

## Build & deploy

```bash
npm run build   # output in build/
npm run start   # serve the production build
```

A `Dockerfile` is included for container deploys (Railway, Fly.io, Cloud Run, etc.).
