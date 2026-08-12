# Flourish Commons — Website

The public website for Flourish Commons: a single, static `index.html` page introducing Flourish Commons as a stewarding institution, its initiatives, and its supporting network.

## What this is

A deliberately simple, framework-free static site — plain HTML and CSS, no build step, no JavaScript. See `Flourish_Commons_Website_Specification.md` in the project for the full brief this implements.

## Structure

```
.
├── index.html
├── styles.css
└── assets/
    └── flourish-commons-logo.svg   # the Steward's Mark, vectorised
```

## Running locally

No build step is required. Either:

- Open `index.html` directly in a browser, or
- Serve the folder locally, e.g. `python3 -m http.server`, then visit `http://localhost:8000`

## Deploying

The site is entirely static and can be deployed as-is to GitHub Pages, Cloudflare Pages, Netlify, or any ordinary web server. The production domain is `flourishcommons.africa`.

## Making content changes

- **Copy** (hero statement, About text): edit directly in `index.html`.
- **Initiatives / Network lists**: each is a plain `<li>` inside `.initiative-grid` (`#initiatives`) or `.network-list` (`#network`) in `index.html` — add, remove, or re-link entries there.
- **Colour, type, spacing**: all design tokens are declared as CSS custom properties at the top of `styles.css` (`:root`), drawn from the Steward's Mark's own palette.
- **Logo / mark**: `assets/flourish-commons-logo.svg`, a vectorised version of the Flourish Commons mark.

## Repository

https://github.com/Flourish-Commons
