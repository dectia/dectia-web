# Dectia — Marketing Website

Landing page for [Dectia](https://app.dectia-ai.com), an AI-assisted physical security risk analysis platform. Built as a static single-page site with CDN-loaded React, Tailwind CSS, and GSAP animations.

## About

Dectia helps security consultants and teams turn weeks-long site surveys and audits into same-day reports. The platform targets compliance frameworks such as ISO 27001, ASIS, NFPA 730, and ISO 31000.

This repo contains only the **marketing landing page** — no backend or application logic.

## Tech Stack

| Layer | Technology |
|-------|------------|
| Markup | Single `index.html` |
| UI | React 18 (UMD via unpkg) + Babel Standalone (in-browser JSX) |
| Styling | Tailwind CSS 3 (CDN) + custom CSS |
| Animation | GSAP 3.12.5 + ScrollTrigger |
| Fonts | Google Fonts — Sora, Outfit, Cormorant Garamond, JetBrains Mono |
| Booking | Calendly embed |

## Project Structure

```
sentria-web/
├── index.html     # Entire site — HTML shell + inline React components
├── hero-bg.jpg    # Hero section background image
└── README.md
```

## Running Locally

No build step or `npm install` required. Serve the folder with any static HTTP server:

```bash
# Python (built-in)
python3 -m http.server 8080

# Node
npx serve .
```

Then open [http://localhost:8080](http://localhost:8080).

> Opening `index.html` directly via `file://` may cause issues with CDN scripts in some browsers.

## Deployment

Upload `index.html` and `hero-bg.jpg` to any static host — GitHub Pages, Netlify, S3, Cloudflare Pages, etc. No build step needed.

## Page Sections

| Section | Description |
|---------|-------------|
| **Navbar** | Logo, internal anchors, "Agendar Demo", and "Acceder" link to the live app |
| **Hero** | Main headline with primary CTAs |
| **Plataforma** | Animated feature cards (risk dashboard, compliance standards, AI telemetry, document upload, team capacity) |
| **Metodología** | 4-step workflow from evaluation design to executive report |
| **Casos de Uso** | Sticky stacked cards for facility types with compliance tags |
| **Footer / Demo** | Expandable Calendly booking widget |

## External Links

- Live app: [app.dectia-ai.com](https://app.dectia-ai.com)
- Demo booking: Calendly (`montillajafet/reunion-valorant`)
