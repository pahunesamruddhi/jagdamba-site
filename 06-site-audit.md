# JAGDAMBA — Site Audit & Improvement Plan
### October 2026 · covers index, products, services, about, expos, contact, calculators

---

## 0 · What changed in this pass (images)

19 photos supplied → 16 used, optimised from **~30 MB to 2.2 MB** (WebP, 1600 px + 640 px versions, in `/img`).

| Page | Where | Images |
|---|---|---|
| Home | Product list — desktop hover preview + mobile thumbnails | 450 T deep-draw press, cylinder, power pack, manifold, cylinder cutaway |
| Products | New 8-tile **press gallery** (replaces the empty 16:6 banner) | Deep draw 450 T, 4-column on trial, C-type, 4-pillar, special purpose, notching, deep-drawn parts, servo drive |
| Products | Row thumbnails | Cylinders, power packs, manifolds, kits |
| Products | Lifts / gates / components (no photos yet) | Striped "add photo" placeholders swapped for the line icon, so the page doesn't look unfinished |
| Services | New "On the bench" strip | 3 manifold rebuilds + power pack |
| About | New "The works" strip | 2 shop-floor presses + 2 manifolds |

**Not used, on purpose**
- `Hydraulic-cylinder.jpg` — carries a **HYDRAFLU** watermark (another company's photo). Don't publish it.
- `Deep Draw Press.png` / `450t gem.jpg` — near duplicates of `450t perpx.png`.
- `250lpm-servo-system-1000x1000.jpg` **is** used, but the filename looks like a supplier/marketplace photo. Swap it for your own photo of the servo unit fitted to a Jagdamba press if you can.
- The four `Unconfirmed *.crdownload` files (~200 MB each) in the download folder are **incomplete downloads** (probably videos). Re-download them if they were meant for the site.

## 0b · Content recovered from jhydro.in and the Jhydro YouTube channel

The redesign was missing most of the company's real track record. It is now added:

**Exhibitions (expos.html rebuilt: 8 real shows, each with stand footage and/or photos, plus a 6-video "Watch the presses run" wall)**
| When | Show | Source |
|---|---|---|
| Aug 2026 | HIMTEX 2026, Hyderabad: servo deep-draw press | YouTube Shorts (19–20 Aug 2026) |
| 7–9 Feb 2025 | Advantage Vidarbha (Khasdar Audyogik Mahotsav), Nagpur: Laghu Udyog Bharati pavilion, Hall C | YouTube Short + poster |
| Nov 2024 | IESS XII, Chennai (EEPC India): demo to foreign delegates | YouTube |
| Mar 2024 | IESS, Coimbatore (EEPC India): hosted overseas delegates | YouTube (4,300+ views) |
| 2023 | IMS Bangalore Expo 2023 | YouTube Short |
| 18–21 Aug 2023 | HIMTEX 2023, HITEX Hyderabad: Hall 3, Stall 3A03 | jhydro.in invite poster |
| 2023 | Advantage Maharashtra Expo 2023, Aurangabad: Stall A 52 | jhydro.in gallery (4 photos used) |
| 10–12 Dec 2021 | 11th Steel · Power · Cement · Mining National Expo, Science College Ground, Raipur: Stall D-19, NSIC pavilion | jhydro.in photos (date from EXIF, name from stall banner) |

**Clients** (from jhydro.in, now on Home + About): Larsen & Toubro, BALCO, MAHAGENCO, Western Coalfields Ltd, MOIL Ltd, Sunflag Steel.

**Certification** (About): accredited certificate strip (IAF · EGAC · QRO) and the JAGDAMBA® registered trademark.

**Capabilities missing from the redesign** (now on Products, Home and the About timeline):
- Servo-hydraulic presses up to 425 T ("Central India's biggest"), 200 T servo, ball-crimping servo press
- IoT-enabled remote operation, monitoring and troubleshooting by mobile
- Deep draw press with robotic-arm automation
- 600-ton press for large drawn parts; gib-type guided heavy-duty presses; embossing and notching presses
- Hydropower hydraulic gate (designed, installed, tested); vehicle-levelling jacking systems
- On-site training and testing at customer premises

**Still to do (needs your OK or the source files)**
- ~~Back up the old site~~ **Done:** `../old-site-backup/` holds all 23 pages (HTML + plain text) and 98 assets (117 MB), with `manifest.json`. The failed fetches were links already broken on the live site, e.g. testimonial photos and a "Train Re-railing System" image, so that product may need a photo.
- Client logos (whitespace trimmed), the certificate strip, factory exterior, expo photos, goods lift, gate, seals and telescopic cylinders are now in `/img` and on the pages. The registered logo is saved as `img/logo-jagdamba.webp` but not used yet (see below).
- Several old-site cylinder images are watermarked "favpng" stock. They were not used and should not be reused.
- **Client logos** and the **certificate image**: ask the team for originals in better quality. Confirm the certificate standard (ISO 9001?) and number so the site can state it exactly.
- **Brand mark conflict:** the company has a registered **JAGDAMBA® "H" emblem** (red/blue roundel). The redesign uses an orange square and the concepts in `logos.html`. Decide deliberately: either keep the registered mark, or plan a trademark refresh. A new site shouldn't drop a registered mark by accident.
- Video thumbnails load from YouTube (`i.ytimg.com`) and open YouTube on click. Nothing heavy is embedded.
- Confirm the Advantage Maharashtra month and the IMS Bangalore month so the timeline can show exact dates.

## 0c · Palette + homepage hero (this pass)

**Palette.** Orange/charcoal is replaced site-wide with colours from the company's own machines and logo:
- **Machine yellow `#f5c000`** for highlights, buttons, markers and bars, always with dark text on it.
- **Cobalt `#1c4fa0`** for accent text and links on light backgrounds. It sits between the logo's navy and cyan.
- **Deep navy `#0e1a33`** for the dark bands (configurator, repair process, contact, footer). Accents there switch to yellow automatically via `--org-text`.
- Headline emphasis is now a yellow highlighter band behind dark text, which stays readable at every size.

**Hero 3D (full-height product shot; a soft paper glow behind the copy keeps the headline readable; the readout sits under the buttons), rebuilt as a photoreal model of the SHD 4-column deep-draw press:**
- Off-white crown and base, twin yellow main cylinders with bolted flanges and chrome rams, chrome columns with lock nuts and yellow guide sleeves.
- Yellow slide with a hazard band, perforated yellow base guard, steel T-slot bolster, and a die where a stainless blank deep-draws into a cup.
- HMI pendant with a **live screen** and a stack light (green = running, amber = ready).
- Power unit: white cabinet on a yellow skid with louvres, lamps, motor-pump, accumulator and black hoses.
- PBR materials (clear-coated paint, chrome, stainless), studio reflections and soft contact shadows; three.js r160 module build.
- **The motion is a real cycle** on SHD-75+25 brochure data: fast approach at 150 mm/s → pressing at 9 mm/s up to 100 T → dwell → decompression → fast return at 200 mm/s → cushion eject → load blank. A live readout and the machine's HMI show phase, speed, force, stroke and cycle count. "Run cycle" or clicking the press fires one immediately; drag to orbit.
- **Fixed:**
  - The frame timer bug: animation speed used to depend on refresh rate.
  - The press was cropped top and bottom.
  - The 4-line headline pushed the buttons below the fold.
  - Callout labels overlapped the headline.
  - three.js blocked page load. It now loads after first paint, with the real press photo shown meanwhile and as the no-WebGL fallback.
  - Phones: the machine gets its own stage above the copy, and the header quote button is hidden below 480 px.
- Reduced motion: shows a still frame of a formed cup, and "Run cycle" plays exactly one cycle.

**Suggested next animation improvements**
1. **Model swap with the configurator.** Choosing 4-column, C-type or rubber moulding below morphs the hero machine (C-frame, platen heater plates) and plays that family's real speeds.
2. ~~Parts view in "How we build"~~ **Done:** the flat SVG schematic is replaced by a second 3D view of the same press. Hovering or tapping Frame, Guiding, Hydraulics or Controls keeps that system in full colour, ghosts the rest, moves the camera toward it and labels the components. It tours all four automatically when idle, so phone users see them too. Next step: an exploded view that separates the systems as the visitor scrolls.
3. **Real geometry.** If the team has STEP/SolidWorks files of the SHD frame, export a glTF (Draco-compressed, about 1–2 MB) for exact proportions and bolt detail. The current model is built from primitives to match the photos.
4. **Sound, opt-in:** a muted-by-default toggle with the pump hum and the pressing note. It makes a strong impression at expos on a stand screen.
5. **"Expo mode"** (`?kiosk=1`): full-screen hero, auto-cycling, rotating through product families. Useful on the stand TV that appears in every expo photo.
6. **Performance budget.** Keep the hero under about 60 draw calls on phones by merging static meshes (BufferGeometryUtils.mergeGeometries) and using one baked shadow texture instead of a live shadow map on mobile.

## 0d · Merged with `jagdamba-site-revision-2-yellow` (branch `jagdamba-site-revision-3`)

Built on top of the yellow branch, so its photos, logo files and Pages deploy are kept. Ported into our pages:
- **Capacity 10–1,000 T** (CNC servo deep draw) everywhere it's stated; the configurator, calculators and SEO description updated to match.
- Full press-type list (TLT, notching, hole-punching after bending, universal bending, 2-in-1, bonding).
- **Defence & special purpose:** Products section 09, a homepage row, and a contact-form option that's prefilled from `?product=defence`.
- Flameproof (FLP) power packs, the fail-safe bunker / hydropower gate spec, the hybrid-servo retrofit (up to 70% energy saving), and IS 2062 steel with Class II parallelism.
- **Address** "Plot No. A-11/21, 22", the **registered JAGDAMBA® mark** in the nav, and favicons on every page.
- **Exhibitions: 10 shows**, merging their dates, venues and stalls with our videos and photos. Added Globe-Tech Pune 2023 and Advantage Maharashtra 2026. Raipur stays **D-19** (stall banner photo); HIMTEX 2026 is listed as held; IESS naming kept as ours; IMS 2023 booth photo added.
- **About:** their six facility photos (team, directors, customer visit, frame assembly, servo presses) replace the earlier shop strip. The cylinder-kits 2024 milestone is **kept**.
- **New press-family catalogue** on Products, replacing the photo strip. It has 8 cards (deep draw, CNC servo, 4-column, C-type, rubber moulding, lead pipe, notching & punching, special purpose & bonding), each with a photo, capacity range and typical use; the cards open the matching model chart or the enquiry form.
- Real photos replace renders and stock where available: cylinders, components (manifold with valves).
- Their images were converted to WebP (about 7.6 MB → 3.9 MB). `hydraulic-jacks-range` is **not used** (it looks like a supplier collage and was mislabelled as a gate actuator). The old Fig. 02 source photo was removed, since the 3D parts viewer replaces it.
- The "[BLUE+YELLOW]" title tag is gone.

---

## 1 · Critical — fix before launch

| # | Issue | Where | Fix |
|---|---|---|---|
| C1 | **Every form loses its leads.** Quote, contact and "invite us" forms just `preventDefault()` and change the button text to "✓ Sent". Nothing is sent anywhere, but the visitor is told it was. | index, contact, expos | Wire to a real endpoint: Formspree / Web3Forms / Netlify Forms (no backend needed), or a WhatsApp/email fallback. Add a visible error state if the send fails. |
| C2 | **Internal working files would be public.** Strategy docs, wireframes and the logo-concept page sit in the web root. | `01-…md`, `02-wireframe.html`, `04/05-…md`, `logos.html` | Move to `/docs` (or out of the deploy folder) before publishing. |
| C3 | ~~Public placeholders on Exhibitions~~. **Fixed** (see §0b): the page is now built from real shows and stand videos. | expos.html | Add the Advantage Maharashtra stand photos (see §0b). |
| C4 | **Legal name check.** Footer says "Shree Jagdamba Hydropneumatic **Inc.**", matching the current jhydro.in, but "Inc." is a US company form. | all footers | Use the registered name exactly as on GST/MSME/Udyam (e.g. Pvt. Ltd. / proprietorship). Add the GSTIN to the footer, since Indian B2B buyers look for it. |

## 2 · High impact

**Conversion**
- **Mobile header is crowded.** At 375 px the "Request a quote →" pill wraps to two lines next to the burger. **Fixed:** hidden below 480 px; the hero button, the menu and WhatsApp cover it.
- **Add a click-to-call bar on mobile.** The Services audience ("machine down") is phone-first. Put a sticky `Call · WhatsApp` bar on services.html at least.
- **Homepage hero has no real machine in it.** The 3D wireframe is distinctive, but buyers want proof that you actually build the thing. Add one real press photo near the top: in the intro block, or as a "Fig. 01 → real machine" toggle.
- **Testimonials have no faces or companies** for 2 of 3. Add company name, machine bought (e.g. "SHD-150+50, 2023") and a photo of the machine at their plant if allowed.
- **Client logos / certification.** About says "certified" and "OEM clients", but shows neither. Add an ISO/MSME/Udyam badge and 6–10 client logos (with permission).

**SEO (currently close to zero)**
- No `og:` / Twitter tags anywhere, so WhatsApp and LinkedIn shares show a blank preview. Add `og:title`, `og:description` and `og:image` (use `img/press-deep-draw-450t.webp`, or better a 1200×630 JPG) on every page.
- No favicon on any live page. Export the orange-square mark as `favicon.svg` + 180 px `apple-touch-icon.png`.
- No `canonical`, `robots.txt` or `sitemap.xml`. Add all three, pointing at `https://jhydro.in/`.
- No structured data. Add `LocalBusiness` / `Organization` JSON-LD (name, address, phones, hours, geo, sameAs → socials) on index and contact, and `Product` JSON-LD for each press family.
- Product names live in one long page. For search, give each press family its own URL (`/presses/deep-draw.html` etc.) with its model chart. "Deep draw hydraulic press manufacturer Nagpur" is the query to win.
- Image `alt` text is now set on all content images. Keep doing this for every new photo.

**Accessibility**
- `--ink-40 (#94969b)` on white is about **3:1** contrast, below WCAG AA (4.5:1) for small text. It's used for the mono spec lines, captions, footer and counters. Darken it to about `#6f7177` for text, and keep `#94969b` only for icons and hairlines.
- The hero canvas captures drag/click. Make sure keyboard users can skip it; it's `aria-hidden`, which is good, but the "click to press" hint is mouse-only. That's fine as long as no information is lost.
- The testimonial carousel auto-advances every 8 s and only pauses on pointer hover. Pause it on focus too, and stop it entirely when `prefers-reduced-motion` is set.

## 3 · Medium

**Performance**
- index.html loads three.js r128 (~600 KB) + GSAP + ScrollTrigger on every visit, even on mobile where the scene sits behind the text at 85% opacity. Lazy-load three.js after first paint (or only ≥ 900 px wide), and show a static press image/SVG until then.
- Google Fonts loads 5 Inter weights + 2 mono. Trim to the weights actually used (400/500/600 + mono 500), or self-host.
- About 180 lines of identical CSS are copy-pasted into each of the 7 pages. Extract a shared `site.css` so it's cached once and edits happen in one place.
- Add `width`/`height` to every `<img>` (done for the new galleries) to prevent layout shift.

**Content & trust**
- Footer lists `info_hydropneumatics@yahoo.com` next to the `@jhydro.in` addresses. Drop the Yahoo address; it undercuts the "national-grade OEM" positioning.
- The LinkedIn link points to a **personal profile** (`/in/…`). Create a LinkedIn **company page** and link that.
- Hours read "Mon–Sun 9–7 · Wednesday closed". "Thu–Tue, 9 am–7 pm (Wed closed)" is clearer.
- Proof bar: "100% designed and manufactured in India". If any valves or pumps are imported (the copy mentions Rexroth/Yuken class), reword to "Designed & built in India" to stay defensible.
- The Jhydro YouTube channel (60+ videos, 2.17K subscribers) is now linked from Exhibitions and Products. Next step: a muted autoplay loop of the 425 T servo press on the homepage, self-hosted MP4 of 3 MB or less. The incomplete `.crdownload` files may be the source clips.
- Products → Lifts, Gates, Components still need photos. Shoot them on the shop floor in the same style as the manifold photos (3:4, yellow + black, natural light).

**Photography brief for the next shoot**
1. Each press family in the same angle (¾ front, waist height), clean floor, 3–4 shots.
2. Close-ups that prove the engineering claims: honing, chrome rod, manifold drilling, ultrasonic testing, pressure-test gauge.
3. People: the two directors, fitters at work (builds trust far more than machines alone).
4. Dispatch/installation at customer sites (with permission).
5. Exhibition stands, which fill the empty Exhibitions page.

## 4 · Low / polish
- `index.html` brand link goes to `#top`, while inner pages go to `index.html`. That's fine, but keep it consistent if a shared header is introduced.
- Add `<meta name="theme-color" content="#fdfdfc">`.
- `contact.html` has a Google Maps link but no embedded map. A lazy-loaded map iframe (or static map image) helps visitors planning a factory visit.
- Add a simple 404 page in the same style.
- Calculators page: add a "Need a press for this force? → see matching models" link from the result to the configurator. It's a natural lead path.

---

### Suggested order
1. C1–C4 (one day of work).
2. Favicon, OG tags, JSON-LD, sitemap, contrast fix (half a day).
3. Mobile header + call bar, lazy three.js, shared CSS.
4. Photo/video shoot → lifts, gates, components, expos, testimonials.
5. Split press families into their own SEO pages.
