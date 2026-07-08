# Marvin — Sugar-free Confectionery Brand Website

Static marketing site for a sugar-free confectionery manufacturer, covering six
in-house brands plus private-label production.

## Pages
- `Home.dc.html` — homepage / entry point
- `BioGum.dc.html` — plant-based gum with vitamins
- `Marvins.dc.html` — Marvin's Gum
- `Xylitol.dc.html` — 100% xylitol-sweetened gum
- `Drops.dc.html` — sugar-free drops
- `Mints.dc.html` — sugar-free mints
- `PrivateLabel.dc.html` — B2B private-label offer
- `Company.dc.html` — about the company
- `SiteHeader.dc.html` / `SiteFooter.dc.html` — shared components
- `support.js` — design-tool client runtime (renders the `<x-dc>` markup)
- `photos/` — product photography

## Notes
The pages are a client-rendered export: `support.js` parses the `<x-dc>` /
`<dc-import>` markup and renders it with React (loaded from a CDN at runtime),
so the site only needs static hosting. The root path `/` redirects to
`Home.dc.html` (see `vercel.json`).
