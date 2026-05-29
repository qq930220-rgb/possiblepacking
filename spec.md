# SPEC: Capsule Filling Machine — B2B Industrial Landing Page

## Project Context

**Brand**: ProCaps Pro (fictional professional brand)
**Page Purpose**: B2B lead generation — sell capsule filling machines to pharmaceutical, nutraceutical, and supplement manufacturers
**Target Audience**: 
- Operations managers at supplement companies
- Pharma production directors
- Contract manufacturers (CMOs) looking to upgrade equipment
- Procurement teams for GMP-certified facilities

**Primary Goal**: Get a quote request / contact form submission

---

## Design Direction

**Aesthetic**: Industrial Precision meets Clean Modernism. Think: German engineering × Swiss minimalism × clean SaaS clarity. NOT playful, NOT tech-startup blue. Professional, trustworthy, performance-focused.

**Color Palette** (NO blue/purple):

| Role | Color | Hex |
|------|-------|-----|
| Primary Background | Off-White | `#F8F7F5` |
| Dark Sections | Charcoal | `#1C1C1E` |
| Warm Accent | Copper/Amber | `#C87B3F` |
| Secondary Accent | Sage Green | `#6B7F5C` |
| Body Text | Dark Slate | `#2D2D2D` |
| Muted Text | Warm Gray | `#6B6B6B` |
| Borders | Light Taupe | `#E5E2DD` |

**Typography**:
- Headlines: `DM Serif Display` (Google Fonts) — authoritative, editorial
- Body/UI: `Inter` (Google Fonts) — crisp, technical readability
- Fallback: Georgia, system-ui

---

## Page Structure

```
[HERO] — Dark bg, full-viewport, machine visual + headline + CTA
[TRUST BAR] — logos: GMP / ISO / FDA compliance certifications
[SOCIAL PROOF] — 3 key stats (machines sold, uptime %, countries)
[PRODUCT MODELS] — 3 machine tiers (table/grid format)
[TECH SPECS] — expandable accordion for technical details
[WHY PROCAPS] — 4 differentiators with icons
[TESTIMONIAL] — 1 quote from a real-type customer
[GET A QUOTE] — dark CTA section with form
[FOOTER] — contact info, certifications, links
```

---

## Hero Section

- **Style**: Type-Led + Dark Atmospheric
- Background: Dark charcoal with subtle copper gradient glow (top-right corner)
- Headline: "Precision Capsule Filling. Industrial Scale." (large, serif)
- Subheadline: Short description of the machine line
- Primary CTA: "Request a Quote" (copper button)
- Secondary CTA: "Download Brochure"
- Trust indicators inline: ISO certified • GMP compliant • 24/7 Support

---

## Tech Strategy

- Single-file HTML + inline CSS + minimal vanilla JS
- Google Fonts CDN
- No frameworks, no build step
- CSS gradient simulating industrial atmosphere (no external images required for hero)
- Intersection Observer for scroll animations

---

## Motion Plan

- Hero: Headline fades in on load (no stagger needed for B2B)
- Sections: `reveal` class triggers fade-up on scroll
- Buttons: Subtle scale + shadow lift on hover
- Stats: Number counter effect optional (keep simple for B2B)
- Form: Success state with checkmark feedback

---

## SEO Requirements

- `<title>`: Capsule Filling Machine Manufacturer | ProCaps Pro
- `<meta description>`: High-speed capsule filling machines for pharmaceutical & nutraceutical production. GMP certified, ISO compliant. Request a quote today.
- Open Graph tags for LinkedIn sharing
- Semantic HTML: proper `<header>`, `<main>`, `<section>`, `<footer>`
- H1 exactly once, logical H2/H3 hierarchy
- `alt` attributes on all images
- Schema.org markup for Product + Organization