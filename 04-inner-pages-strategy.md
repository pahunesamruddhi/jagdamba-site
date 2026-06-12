# JAGDAMBA — Full-Site Build: Inner Pages Strategy
### Extends 01-brand-content-strategy.md · Visual language: Heavy Industry Modern (confirmed via landing page)

## 1 · Final Sitemap (7 working pages)

```
index.html        Landing (built) — nav updated to real pages, + Exhibitions teaser strip
products.html     All 11 product lines, incl. full press model-chart tables (4 families)
services.html     5 repair lines + retrofit/conversion + how-we-repair process
about.html        Story · directors · values · clients · certification · timeline
expos.html        NEW — Exhibitions: national & international expo timeline + "invite us" CTA
contact.html      Full contact: form, map, hours, every live channel
calculators.html  Restyled into the Inter/heavy-industry system (logic untouched)
```

Navigation (all pages): Products · Services · About · Exhibitions · Calculators — Contact = persistent orange CTA. Footer identical sitewide: giant wordmark, address, socials, sitemap links.

## 2 · Page Content Architecture

**Products** — one long editorial page, anchor-linked (#presses, #cylinders, #power-packs, #manifolds, #kits, #lifts, #gates, #components). Presses lead with all four model charts as calm data tables (the brochure verbatim — buyers screenshot these). Every line: number · headline · 2–3 sentence promise · spec strip · "Request a quote →". Pneumatic cylinders, gates, accessories, seals, honed tubes, plated rods (from live nav) grouped sensibly so 12 menu items become 8 digestible sections.

**Services** — urgency-first ("Machine down?"), phone CTA above the fold. Five numbered repair disciplines (cylinder, power pack, press, manifold, valve — from live nav) each with what's included; then the 4-step repair process (strip & inspect → hone/replace → reseal with PTFE/bronze → pressure-test & certify); then retrofits & screw-press conversion; ready-machine note.

**About** — positioning narrative (technocrat, import substitute, centre of India), values from live site rewritten in brand voice, the two directors, "valuable clients across OEMs" claim + certification mention (kept general; logos/cert image to be dropped in by team), 2006→today timeline.

**Exhibitions (new)** — Positioning: *"Where the machines meet the industry."* Structure: intro stat strip (national + international presence) → vertical timeline of expo entries (year badge, show name, venue, what was exhibited, photo slot). Seeded with the verified **August 2023** entry from jhydro.in; further entries are template slots marked `[Add show]` for the team — no invented show names presented as fact. Footer CTA: "Exhibiting soon — invite us to your show / book a stand meeting."

**Contact** — everything live from jhydro.in: both phones, all four emails (incl. info_hydropneumatics@yahoo.com), full Butibori address, Google-Maps link, hours (Mon–Sun 9–7, Wed closed), WhatsApp deep link, all four social profiles. Quote form with the live product list as options.

## 3 · UX Patterns (shared)
Sticky light nav with active-page underline · sub-page hero = label + huge sentence-case h1 + one orange accent word + breadcrumb-free (nav suffices) · `.rows` editorial list pattern from landing reused for products/services · data tables: hairline rules, mono numerals, hover row tint · forms identical to landing's charcoal style on contact (light variant elsewhere) · reveal-on-scroll via IntersectionObserver (no GSAP dependency on inner pages — lighter) · same footer wordmark moment everywhere.

## 4 · Mesh Language on Inner Pages
No WebGL off the landing page (performance discipline — veteran restraint). The mesh carries through: the line-drawn SVG icon set (extended to lifts, gates, seals, tubes, rods, expo booth), hairline ground-grid backgrounds on page heroes, and orange-on-ink edge aesthetics in tables and diagrams.
