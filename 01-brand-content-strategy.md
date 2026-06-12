# JAGDAMBA — Brand, Content & UX Strategy
### Website Redesign for Shree Jagdamba Hydropneumatic · jhydro.in

---

## 1 · Where the Brand Stands Today

The current site is a generic B2B template: stock layouts, keyword-stuffed metadata, lorem-ipsum fragments ("Dramatically disseminate standardized metrics…"), and a navigation with 12+ flat product links. Yet underneath sits a genuinely strong story:

- **20 years** of hydraulic engineering (est. 2006)
- **Import-substitute specialist** — they replace foreign OEM parts with Indian-made equivalents
- **Full-stack fluid power** — they design, build, *and* repair (rare; most firms do one)
- **650-ton press capability**, ultrasonically-tested frames, FEA-designed structures
- Make in India, MIDC Butibori, Nagpur — the literal geographic center of India

The problem is not the company. The problem is that the website says "local vendor" when the work says "national-grade OEM partner."

---

## 2 · Brand Strategy

### Positioning Statement
> **For Indian manufacturers who depend on imported hydraulic equipment, JAGDAMBA is the engineering partner that designs, builds, and services fluid-power systems to OEM spec — from the center of India, at Indian lead times and Indian costs.**

### Positioning Pillars

| Pillar | Proof | Where it shows up |
|---|---|---|
| **Engineered, not assembled** | FEA frame design, ultrasonic-tested steel, PTFE low-friction seals, proximity-sensor controls | Product pages, spec tables, process section |
| **Import substitute** | Replaces foreign OEM manifolds & cylinders 1:1 | Hero subline, About, case mentions |
| **Force at scale** | 25 to 650-ton presses, 13 standard deep-draw models | Interactive model-chart selector |
| **Built + kept running** | Manufacturing AND repair of cylinders, packs, presses, manifolds, valves | Services section |
| **Center of India** | Nagpur/Butibori — equidistant logistics to every industrial belt | About / Contact |

### Brand Idea (the one line everything hangs off)
**"Engineered Force."** — Hydraulics is literally the engineering of force. Jagdamba doesn't sell machines; it sells controlled, reliable tonnage. Every design decision (heavy type, big numerals, pressure-gauge motifs) expresses force under precise control.

### Brand Voice
- **Confident, declarative, specific.** "650 tons. One operator." not "We offer a wide range of solutions."
- **Engineer-to-engineer.** Speak in specs, tolerances, tonnage. The buyer is a plant head or purchase engineer — respect their literacy.
- **Quietly proud, never boastful.** Make in India as fact, not slogan.
- **Verbs of making:** forge, machine, hone, test, commission, retrofit.

Voice samples:
- ❌ "We are pleased to introduce a technocrat company…"
- ✅ "Twenty years of building the machines India's factories run on."
- ❌ "Innovative products for productivity, performance & profitability"
- ✅ "Presses from 25 to 650 tons. Cylinders from sketch to seal. Built in Nagpur, working everywhere."

---

## 3 · Content Strategy

### Audience & Jobs-to-be-Done
1. **Purchase engineer / plant head** — needs spec tables, model charts, fast quote path. → *Model selector, persistent "Request Quote" CTA, WhatsApp deep link.*
2. **OEM design engineer** — needs custom cylinder/manifold capability proof. → *Capabilities section, engineering-process content.*
3. **Maintenance head** — machine is down, needs repair NOW. → *Services with urgency framing, phone-first CTA.*
4. **MSME owner (utensil/FRP/rubber industries)** — buying first deep-draw press. → *Industry/application framing, testimonials, "ready machine" stock.*

### Content Hierarchy Rules
- **Numbers lead.** Tonnage, years, model counts are the headlines; prose supports.
- **Every product gets: 1-line promise → spec data → application list → CTA.**
- **Specs are content, not appendix.** The brochure's model charts become an interactive selector — the single most useful tool a press buyer can have.
- **Repair = a product.** Currently buried in a dropdown; elevated to a primary section.

### Sitemap (target full site)

```
HOME (this build — long-form scrolling flagship)
├── PRODUCTS
│   ├── Hydraulic Presses  ← flagship category
│   │   ├── Deep Draw (SHD model chart, 13 models, 35–650T)
│   │   ├── 4-Column (SHD 25–500T) · C-Type (SHC 5–100T)
│   │   ├── Rubber Compression (SHR 60–250T)
│   │   └── H-Type · Lead Pipe · Workshop · FRP · Stamping · Special Purpose
│   ├── Hydraulic Cylinders (mill/heavy/tie-rod/telescopic/custom) + Cylinder Kits
│   ├── Hydraulic Power Packs
│   ├── Manifold Blocks (Lift · PCM · Regeneration · Sequence · Station)
│   └── Lifts · Gates · Seals · Honed Tubes · Plated Rods · Accessories
├── SERVICES (cylinder / power-pack / press / manifold / valve repair, retrofitting)
├── INDUSTRIES (utensils, auto components, FRP, rubber, steel, cement, power, railways)
├── ABOUT (story, directors, facility, Make in India, certifications)
├── READY MACHINES (in-stock inventory)
└── CONTACT (quote form, WhatsApp, map, hours)
```

The **homepage built here** compresses this into one awwwards-style scroll: Hero → Numbers → Products → Press Configurator → Engineering Process → Services → Industries → Testimonials → Contact.

---

## 4 · Visual Direction

**Lineage:** Swiss-industrial / technical-editorial — the language of engineering drawings and spec plates, modernized. Think Teenage Engineering's spec-sheet rigor × heavy-industry editorial (SSAB, Sandvik) × Indian factory-floor color.

| Token | Choice | Why |
|---|---|---|
| **Base** | Deep graphite `#0D0F12` → carbon `#15181D` | The machine shop at night; lets product imagery & yellow burn |
| **Accent** | Machine yellow `#F5B70A` | Their actual presses are painted this; safety-yellow = industrial truth |
| **Secondary** | Signal orange `#E8622D` | From the brochure's chevrons; used sparingly (hover, tags) |
| **Paper** | Bone `#EDEAE2` | Inverted "spec sheet" sections for contrast rhythm |
| **Type — display** | *Archivo Expanded / Black* | Wide, heavy, machined; reads like stenciled plate lettering |
| **Type — mono** | *JetBrains Mono* | All specs, labels, axis text — engineering-drawing DNA |
| **Motifs** | Hairline rules, crosshair registration marks, dimension arrows, gauge dials, oversized index numerals (01–07) | Drawing-sheet semantics |
| **Motion** | GSAP ScrollTrigger: clipped reveals, counter roll-ups, pinned press configurator; Three.js hero: live wireframe hydraulic cylinder, piston cycling under scroll | Motion = force made visible; every animation communicates pressure/extension |

---

## 5 · UX / Wireframe Logic (see 02-wireframe.html)

1. **HERO** — full-viewport. Three.js cylinder assembly slowly cycling. Headline: "ENGINEERED FORCE." Sub: positioning line. Dual CTA: *Explore machines* / *Request a quote*. Marquee strip of capabilities.
2. **PROOF BAR** — 4 counters: 20 yrs · 650 T max · 30+ press types · 2006.
3. **PRODUCTS** — editorial index list (01–05): Presses, Cylinders, Power Packs, Manifolds, Cylinder Kits. Hover = image swap; mobile = stacked cards.
4. **PRESS CONFIGURATOR** — the centerpiece. Tabs: Deep Draw / 4-Column / C-Type / Rubber. Slider or chips select tonnage → spec readout (table size, stroke, daylight, motor HP) animates. Data = brochure model charts, verbatim.
5. **ENGINEERING** — 4-step process strip (FEA design → ultrasonic-tested fabrication → precision machining → assembly & trials) with the brochure's feature claims.
6. **SERVICES** — "We keep them running" — 5 repair lines, phone-first CTA.
7. **INDUSTRIES** — chip cloud (utensils → railways).
8. **VOICES** — 3 real testimonials, oversized quote treatment.
9. **CONTACT** — split: quote form / address-hours-map links; WhatsApp button.
10. **FOOTER** — full sitemap, Make in India mark, social.

Persistent: slim top bar (logo · nav · yellow "Get Quote" pill). Mobile: hamburger → full-screen overlay menu.

**Accessibility & performance:** WCAG-AA contrast throughout, `prefers-reduced-motion` kills Three.js spin + scroll effects, compositor-only animations, lazy canvas init, 44px touch targets, fluid `clamp()` type, tested at 375 / 768 / 1440.
