# Discovery Beauty: Investor Overview

A single-page investor overview for **Discovery Beauty**: a membership-powered beauty commerce platform built off Discovery's affluent base. Static site, no build step, no dependencies.

## Contents

```
.
├── index.html      # The entire site (self-contained: inline CSS, web fonts via Google Fonts)
├── vercel.json     # Vercel static config (clean URLs, security headers)
├── package.json    # Marks the project; no real build step
├── .gitignore
└── README.md
```

## Run locally

No install needed. Either open `index.html` directly in a browser, or serve it:

```bash
npx serve .
```

Then visit the printed local URL.

## Deploy to Vercel

**Option A: Vercel dashboard**
1. Push this folder to a GitHub repo (see below).
2. In Vercel, click **Add New > Project**, import the repo.
3. Framework preset: **Other**. Build command: leave empty. Output directory: `.` (root).
4. Deploy.

**Option B: Vercel CLI**
```bash
npm i -g vercel
vercel        # preview deploy
vercel --prod # production deploy
```

## Push to GitHub

```bash
git init
git add .
git commit -m "Discovery Beauty investor overview"
git branch -M main
git remote add origin https://github.com/<your-username>/<repo-name>.git
git push -u origin main
```

GitHub Pages also works: in repo **Settings > Pages**, set source to the `main` branch root. The site is plain `index.html`, so it serves as-is.

## Fonts

Headers use **Abril Fatface** and body uses **Montserrat**, both loaded from Google Fonts. Montserrat is a rendering stand-in for **Gilroy** (the licensed Prosper & Partners body font). For external distribution, replace the Montserrat `@import` with your licensed Gilroy `@font-face` files and update the `font-family` references.

## Palette (Prosper & Partners)

| Token | Hex |
|---|---|
| Indigo | `#434371` / `#2F2F4F` |
| Teal | `#79AEA3` / `#557A72` / `#A1C6BF` |
| Lime (accent) | `#B6EE4F` / `#CCF384` |
| Brown (footer) | `#352E27` |
| Gray | `#817A73` / `#B0AAA4` / `#E2DFDB` |

---

Prosper & Partners : Strategy & Growth Advisory : Confidential
