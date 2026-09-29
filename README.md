# Urban Concrete and Construction LLC — Homepage

A premium, redesigned homepage for **Urban Concrete and Construction LLC**, a VA Class A
concrete contractor with 20 years of experience serving Northern Virginia and Montgomery
County, MD. Rebuilt from the existing site at
[northernvirginiaconcrete.com](https://northernvirginiaconcrete.com/).

Built as a fast, dependency-free static site — designed to look like an established
professional construction brand and structured so real content drops straight in.

**Live site:** _(GitHub Pages — see repo Settings → Pages)_

---

## Business details
- **Company:** Urban Concrete and Construction LLC
- **Contact:** Alex Flores, Master Craftsman
- **Phone:** +1 703-626-1684
- **Email:** northernvirginiaconcrete@gmail.com
- **Address:** 6912 Rolling Road, Springfield, VA 22152
- **Credentials:** VA Class A Contractor · Licensed & Insured · 20 years of experience
- **Hours:** Leave a message 24/7 · Free estimates
- **Market:** Northern Virginia & Montgomery County, MD
- **Service areas:** Alexandria · Annandale · Arlington · Ashburn · Bethesda MD · Bristow ·
  Burke · Centreville · Chantilly · Falls Church · Fairfax · Gainesville · Great Falls ·
  Herndon · Leesburg · Lorton · Manassas · McLean · Mount Vernon · Oakton · Potomac MD ·
  Reston · Springfield · Tysons Corner · Vienna

## Services
Driveways & flatwork · Patios & porches · Sidewalks & walkways · Slabs & foundations ·
Retaining walls · Stamped & stained concrete · Decorative overlays & scoring · Stucco &
block · Concrete repair & restoration (crack repair, sinking steps/porch) · Hardscape
pavers & stone (flagstone) · French drains · Material delivery (gravel, topsoil, sand,
mulch, compost).

## Tech
- Static **HTML + CSS + vanilla JS** — no build step, no framework, no dependencies.
- Google Fonts (Archivo + Inter). Everything else is local.
- Accessible: semantic landmarks, single `<h1>`, keyboard nav, visible focus,
  `prefers-reduced-motion`, descriptive alt text.
- SEO: descriptive title/meta, Open Graph, and `GeneralContractor` JSON-LD structured data
  with full NAP and service areas.
- **Analytics:** Vercel Web Analytics — enable *Analytics* on the Vercel project and Vercel
  serves the script automatically (no key to paste). A custom `estimate_request` event fires
  on form submit so you can track lead conversions.

## Structure
```
index.html            # full homepage
css/styles.css        # design system + all sections + responsive
js/main.js            # sticky header, mobile menu, scroll reveals, before/after slider, form shell
assets/img/           # photography + logo/favicon
```

## Design
**Graphite & construction-amber** palette — deep charcoal dark sections, cool off-white,
and one confident amber accent. Editorial typography with strong scale. Typographic "UC"
monogram logo. No stock-template feel.

---

## ⚠️ Placeholders & notes for the client
- **Logo** — the header/footer use a clean SVG "UC" monogram wordmark. If you have a vector
  (SVG/PDF) of an official logo, drop it in `assets/img/` and swap the inline SVG for an
  `<img>`.
- **Hero video** — the hero uses a lightly-frosted looping background video
  (`assets/video/hero-720.mp4`, muted/autoplay/loop, ~2 MB, 720p) from Pexels
  (free license), with `hero-poster.jpg` as the poster/fallback and reduced-motion
  users getting the still frame. Swap the files to change it.
- **Photography** — all project photos are high-quality **placeholder** construction images.
  Replace the files in `assets/img/` with real Urban Concrete photos, keeping the same
  filenames, and the site updates automatically. The before/after slider and gallery are
  ready for real project pairs.
- **Estimate form** — front-end only; it does not submit anywhere yet. Wire it to email or a
  CRM (e.g. Formspree, Netlify Forms, or GHL) to start capturing leads.

### Verified facts used on the page
All business claims come from the client's own site: 20 years of experience, VA Class A
contractor, insured, free estimates, master craftsman Alex Flores, and the address, phone,
email, and service areas above. Nothing beyond that is fabricated — no invented review
counts, project totals, awards, or guarantees.

## Deploy
**Vercel (recommended — for Web Analytics):** import the GitHub repo into Vercel, deploy as a
static site (no build command, output = repo root), then turn on **Analytics** in the project.
Update the `<link rel="canonical">` and `og:url` to the final domain once assigned.

**GitHub Pages (alternative):** Settings → Pages → Source: `main` / root. Note that Vercel
Web Analytics only reports when served from Vercel.

Local preview: open `index.html`, or run `python3 -m http.server` in the repo root.
