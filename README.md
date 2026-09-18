# PizzaVala — Redesigned Website

A premium single-page redesign of pizzavala.co.uk, built with React, Vite,
Tailwind CSS and Framer Motion.

## Run locally

```
npm install
npm run dev
```

Then open the printed local URL (usually http://localhost:5173).

## Build for production

```
npm run build
```

Output goes to `dist/`. Deploy that folder to any static host (Netlify,
Vercel, Cloudflare Pages, your own server, etc).

## Content

All real PizzaVala business facts (address, phone, email, stats, category
names, ordering link) live in `src/data/content.js` — sourced from
pizzavala.co.uk and pizzavalaharrow.co.uk. Edit that one file if any detail
changes; no business facts are hard-coded inside components.

## Images

Stock food photography is pulled from Unsplash (free license, no attribution
required) via `images.unsplash.com` URLs. Swap in PizzaVala's own photography
whenever it's available — just replace the URLs in `content.js` and the
`src` attributes in `Hero.jsx`, `BrandStory.jsx`, `FeaturedFood.jsx` and
`Experience.jsx`.

## Structure

```
src/
  components/   Navbar, Hero, BrandStory, Stats, Menu, FeaturedFood,
                WhyPizzaVala, Gallery, Experience, FinalCTA, Contact, Footer
  data/         content.js — single source of truth for business content
  index.css     design tokens (colors, fonts) + base styles
```
