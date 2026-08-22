# Landscaping Landing Page — Demo

**Live demo: https://davidfigueroacisneros-byte.github.io/landscaping-landing-demo/**

A high-conversion landing page for a **fictional** hardscape company ("Copperstone Pavers"), built as a portfolio demonstration. Single self-contained `index.html` — no build step, no dependencies.

## What it demonstrates

- **Animated SVG installation diagrams** — three hand-drawn cross-section animations (base compaction, drainage slope, joint lock) built with inline SVG + CSS keyframes. No video files, no libraries, ~0 KB of media weight, and full `prefers-reduced-motion` support.
- **Conversion-focused structure** — problem → system → process → post-install care → lead form, with scroll-in animations via `IntersectionObserver`.
- **Webhook-ready lead form** — posts JSON to any endpoint (n8n, Make, Zapier, or a custom API). Ships in demo mode; going live is a one-line change (`WEBHOOK_URL`).
- **Accessible by default** — semantic sections, ARIA labels on every diagram, focus states, keyboard-friendly form, reduced-motion fallbacks.

## Why a fictional company?

My production landing pages (with real tracking IDs, live webhook endpoints, and client branding) are private — this demo shows the same techniques with original content, so nothing confidential is exposed.

## Run it

Open `index.html` in a browser. That's it.

To wire the form to a real endpoint, set `WEBHOOK_URL` at the bottom of the file:

```js
const WEBHOOK_URL = 'https://your-n8n-host.example.com/webhook/lead';
```

## License

MIT — see [LICENSE](LICENSE).
