# Befocusy — Design System

> **Befocusy** es una consultora que implanta procesos digitales y sistemas de
> productividad para negocios y pymes. Especialidad: **Notion, IA,
> automatizaciones y productividad digital.** Ayudan a empresas a *enfocarse* en
> lo que importa montando el sistema operativo digital que lo sostiene.

This repository is the brand & product design system for Befocusy. It contains
the brand foundations (logo, color, type), reusable CSS tokens, design-system
preview cards, and a high-fidelity UI kit recreation of the marketing site.

---

## 1. Brand at a glance

| | |
|---|---|
| **Name** | Befocusy |
| **Category** | Digital productivity / operations consultancy |
| **Audience** | SMBs (pymes), founders, ops & team leads who feel buried in manual work |
| **Promise** | "Be focused" — we build the Notion + AI + automation systems so you can focus on the business |
| **Voice** | Spanish-first, warm, expert, calm, practical |
| **Logo idea** | A faceted **teal gem** holding a **white lightning bolt** — value + clarity + energy. Wordmark "be**focus**y" puts FOCUS literally at the center. |

### Sources provided
- `uploads/befocusy.svg` — wordmark only ("focus" in teal-700, "be"/"y" in black)
- `uploads/befocusy-complete.svg` — full lockup: gem isotype above the wordmark
- `uploads/befocusy-isotipo.svg` — the gem + lightning bolt mark alone
- Brief: *"Consultora para implantar procesos digitales y sistemas de
  productividad digital… Especialmente con Notion, IA, automatizaciones."*
- Typography request: **use Inter as the primary text typeface.**

> No codebase, Figma file or live site was supplied — only the logo assets and
> the brief. The marketing-site UI kit in `ui_kits/website/` is therefore a
> **brand-faithful original** built from these foundations, not a recreation of
> an existing screen. Treat it as a proposed system; swap in real copy/screens
> when available.

---

## 1b. Sub-brand — WorkOS (workos.befocusy.com)

This design system houses a **sub-brand: WorkOS**, an all-in-one client work
platform served at `workos.befocusy.com`. It shares Befocusy's DNA and all the
shared foundations (neutrals, spacing, radii, shadows, type) — but runs on a
deeper, bluer **petrol** teal so it reads as a sibling of Befocusy without
competing with it.

| | |
|---|---|
| **Mark** | A geometric **workspace panel** (sidebar + two cards) — the "OS" idea |
| **Primary** | `#1B6C78` petrol teal — `--workos-500` |
| **Deep** | `#0D2E35` deep petrol (wordmark) — `--workos-900` |
| **Asset** | `assets/workos-isotipo.svg` (color, light bg) · `assets/workos-isotipo-white.svg` (white, dark bg) |
| **Wordmark** | "WorkOS" set in `--font-display` (Poppins 700) — "Work" in `--workos-900`, "OS" in `--workos-500` |
| **Tokens** | `--workos-50 … --workos-950` + aliases in `colors_and_type.css` |

**How to design for WorkOS:** use the `--workos-*` color tokens (and the shared
`--font-display` / `--font-sans`) in place of the Befocusy `--teal-*` / `--brand`
tokens. Everything else (slate neutrals, spacing, radii, shadows, type scale,
iconography) is **shared**, so Befocusy and WorkOS feel like one family.

> ⚠️ **Open for WorkOS:** palette, isotipo (color + white) and brand/lockup
> cards are set up. No product screens or voice guidelines yet — tell me which
> surfaces WorkOS needs (dashboard, onboarding, etc.) and I'll build its UI kit.

---

## 2. Products & surfaces

Befocusy is a service business, so the primary surface is its **marketing
website** (lead generation + service explainer + booking). One UI kit is
provided:

- **`ui_kits/website/`** — Marketing site: nav, hero, trust bar, services grid,
  process/method timeline, results/metrics, Notion-template style cards,
  testimonial, pricing/packages, CTA booking band, footer. Interactive
  contact-modal flow included.

Likely future surfaces (not built — flag if needed): a client portal /
dashboard, Notion proposal templates, a slide template for audits & proposals.

---

## 3. CONTENT FUNDAMENTALS

How Befocusy writes. Copy is **Spanish (España), informal-but-professional**.

**Person & address.** Speak to the reader as **"tú"** ("Recupera tu tiempo",
"Tú te enfocas, nosotros automatizamos"). The company is **"nosotros"**. Avoid
the corporate "usted".

**Tone.** Calm, confident, outcome-driven. Sell *time and focus back*, not
software features. Lead with the pain ("demasiadas hojas de cálculo, tareas que
se pierden") and resolve with clarity.

**Casing.** Sentence case everywhere — headlines and buttons. Only the brand
name keeps its all-lowercase styling: **befocusy**. Eyebrows/labels may be
UPPERCASE with wide tracking for structure (e.g. `NUESTRO MÉTODO`).

**Sentence length.** Short. Punchy headlines (3–7 words). One idea per line.
Body in 1–2 sentence chunks.

**Vocabulary.** Plain business Spanish with the tool names as proof:
*Notion, automatización, IA, flujo de trabajo, proceso, sistema, panel,
integración, plantilla*. Anglicisms are okay where natural (*workflow, dashboard,
no-code*) but don't overdo it.

**Numbers as proof.** Use concrete, modest, credible metrics: "−10 h/semana",
"3 semanas de implantación", "+40 % menos tareas manuales". Never inflate.

**Emoji.** **No emoji** in product/marketing copy. Iconography carries that role.
(Exception: a sparing ⚡ may nod to the logo bolt, but prefer the SVG mark.)

**Examples (use as reference voice):**
- Hero: *"Deja de gestionar el caos. Empieza a enfocarte."*
- Sub: *"Implantamos tus procesos en Notion, con IA y automatizaciones, para que
  tu equipo recupere horas cada semana."*
- CTA: *"Reserva tu diagnóstico gratuito"* / *"Habla con nosotros"*
- Eyebrow: *"PRODUCTIVIDAD SIN FRICCIÓN"*
- Service card: *"Centralizamos tu operación en un único Notion a medida."*

---

## 4. VISUAL FOUNDATIONS

The Befocusy look is **calm, clean, teal & airy** — a Notion-adjacent
productivity aesthetic with a gem-sharp brand accent.

**Color.** A single-hue **teal system** drawn straight from the logo
(`#0B3F3A` deep · `#0F766E` brand · `#14B8A6` bright), on generous white and a
faint mint tint (`--teal-50 #F0FDFA`). Neutrals are **cool slate**. Color is
used sparingly — teal for brand moments, CTAs, links and the gem; everything
else is ink-on-white. No second brand hue; status colors (green/amber/red) are
functional only. Avoid purple/blue gradients — off-brand.

**Type.** **Inter** for everything readable (body, UI, most headings). **Poppins**
(geometric, medium-bold) for big display headings only, echoing the rounded
geometric "focus" wordmark. **JetBrains Mono** for automation snippets/data.
Headlines are tight-tracked (`-0.02em`) and balanced; body is `1.55` leading.

**Backgrounds.** Predominantly flat white with alternating `--bg2`
(slate-50) and `--bg-tint` (mint) section bands for rhythm. Occasional **deep
teal section** (`--teal-900`) for high-contrast CTA/closing bands with white
text. No photography-heavy hero by default; if imagery is used, prefer clean
product/Notion screenshots or abstract teal gem facets. **No noisy textures, no
heavy gradients.** A subtle teal radial glow behind the hero gem is allowed.

**Spacing & layout.** Roomy. 4px base scale; generous section padding
(`--space-20`/`--space-24` vertical). Max content width ~1200px, comfortable
gutters. Grid-based service/feature cards. Fixed sticky top nav with blur.

**Corner radii.** Friendly but not bubbly. Cards `--radius-lg` (16px), buttons
`--radius-md`→`pill` for primary CTAs, inputs `--radius-md`, small chips
`--radius-pill`. The gem motif provides the only sharp angles.

**Cards.** White surface, `1px` slate-200 border, `--shadow-sm`, 16px radius,
24–32px padding. On hover they lift to `--shadow-md` and the border warms to
`--border-brand`. Feature cards may use a mint (`--bg-tint`) fill instead of a
border. Avoid the "rounded box with a single colored left border" cliché.

**Shadows / elevation.** Soft, cool, low-opacity (`rgba(12,26,25,…)`). Three
working levels: `sm` (resting cards), `md` (hover / menus), `lg`/`xl`
(modals, popovers). Primary CTAs get a **teal glow** (`--shadow-brand`).

**Borders.** Hairline `1px` slate-200 default; slate-300 for stronger
separation; teal-200 for brand-tinted containers. Dividers are slate-100.

**Buttons & states.**
- *Primary:* solid `--teal-700`, white text, pill or 12px radius, teal glow.
  Hover → `--teal-800` (darker) + slightly stronger glow. Press → scale 0.98.
- *Secondary:* white surface, slate-200 border, ink text. Hover → mint tint
  bg + teal border.
- *Ghost/link:* teal text, underline on hover (offset 3px).
- Focus ring: `2px` teal-500 outer with 2px offset.

**Motion.** Subtle and quick. `150–250ms`, `cubic-bezier(0.4,0,0.2,1)`
(ease-out). Fades + small translateY (8–12px) on scroll-in. Buttons scale on
press. Gem may have a slow, optional float/shine. **No bounce, no parallax
overload.** Respect `prefers-reduced-motion`.

**Transparency & blur.** Sticky nav uses `backdrop-filter: blur(12px)` over a
`rgba(255,255,255,0.8)` fill. Glass is reserved for chrome (nav, sticky CTA),
not decorative.

**Imagery vibe.** When present: bright, cool, clean, real product UI (Notion
boards, automations). Teal-leaning. No stocky business handshakes.

---

## 5. ICONOGRAPHY

- **Icon set:** **Lucide** (https://lucide.dev) — `1.5–2px` stroke, rounded
  caps/joins. Its calm, geometric, rounded-but-precise line style matches the
  logo's geometry and the Notion-adjacent feel. Loaded via CDN in the UI kit
  (`https://unpkg.com/lucide@latest`). **This is a substitution** — no icon set
  was supplied with the brand; flag if Befocusy already uses another.
- **Color:** icons inherit text color; brand moments use `--teal-700`. On deep
  teal surfaces they are white. Default stroke weight `1.75`.
- **Sizing:** 20px inline with text, 24px in nav/cards, 32–40px in feature
  headers. Always on the 4px grid.
- **The brand mark** (`assets/befocusy-isotipo.svg`) — the teal gem + bolt — is
  used as the favicon/app glyph and as an occasional "spark" accent, NOT as a
  generic UI icon.
- **Emoji:** not used as UI.
- **No hand-drawn SVG icons** — use Lucide for consistency.

Available brand assets in `assets/`:
- `befocusy.svg` — wordmark (teal "focus" + black "be/y")
- `befocusy-complete.svg` — full vertical lockup (gem + wordmark)
- `befocusy-isotipo.svg` — gem + lightning bolt mark only

---

## 6. Index / manifest

Root files:
- **`README.md`** — this file (context, content, visual, iconography, index)
- **`colors_and_type.css`** — all design tokens (color, type, spacing, radii,
  shadows) as CSS custom properties + opt-in `.bf-*` semantic classes. Self-hosts
  **Inter** from `fonts/`; loads Poppins + JetBrains Mono from Google Fonts CDN.
- **`SKILL.md`** — Agent Skill entry point for using this system
- **`fonts/`** — Inter brand font files (woff, self-hosted)
- **`assets/`** — logo SVGs (see §5)
- **`preview/`** — Design-System tab cards (color, type, spacing, components, brand)
- **`ui_kits/website/`** — marketing-site UI kit (`README.md`, `index.html`, JSX components)

### Components (`ui_kits/website/`)
App, Nav, Hero, TrustBar, Services, Method, Results, Testimonial, Pricing, CtaBand, Footer, ContactModal, Icon
- **`social/linkedin-motivacion/`** — example deliverable: a brand-styled LinkedIn
  carousel ("Los 3 tipos de motivación", 6 slides, 4:5, print-to-PDF for posting)

---

*Built from the supplied logo assets + brief. The website UI kit is a
brand-faithful proposal, not a copy of an existing site — see §2 caveat.*
