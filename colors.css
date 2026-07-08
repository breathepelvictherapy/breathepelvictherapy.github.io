# BREATHE Pelvic Health Center — Design System

> **Aesthetic in one line:** Elegant and clinical — the polished, trustworthy warmth of a premium integrative-health practice, grounded in nature and breath.

A design system for the BREATHE Pelvic Health Center brand. Use it to generate well-branded, on-tone interfaces, marketing pages, and assets.

---

## Brand context

**Brand:** BREATHE Pelvic Health Center
**Category:** Pelvic floor physical therapy and fitness
**Personality:** Elegant · Clinical · Calming · Trustworthy · Human · Grounded in nature

**North stars**
- **Credible, not cold.** Medical authority delivered with warmth — never sterile, never clinical-blue-hospital.
- **Calm and spacious.** Generous whitespace lets a sensitive, intimate topic feel safe and unhurried.
- **Quietly elegant.** Serif headlines, a refined gold accent, and restraint signal premium care.
- **Rooted in nature.** The two-leaf logo (growth, breath, balance) carries through in green-forward color and organic touches.

**Inspiration reference:** [wellesthealth.com](https://www.wellesthealth.com/) — airy whitespace, gentle rounded corners, warm lifestyle photography, card-based service tiles, "symptoms are a story" patient-empowerment tone. Where Wellest is sans-serif throughout, BREATHE elevates it with **elegant serif headlines** (Fraunces).

### Sources provided
- A written brand/design-system specification (pasted brief) and the **official logo** (`BREATHE Pelvic Health Center` PNG, provided by the user — processed into transparent `assets/logo-full.png` / `logo-full-light.png` / `leaf-mark.png`). **No codebase or Figma file was provided.** All brand copy now uses the official **"Pelvic Health Center"** wording.

---

## CONTENT FUNDAMENTALS

**Voice:** Warm, calm, empowering, knowledgeable. The throughline is *"symptoms are a story"* — patient empowerment over clinical detachment.

- **Person:** Speak to the reader as **"you"**; refer to the practice as **"we."** Inclusive and destigmatizing about a sensitive, intimate topic.
- **Tone:** Plain-language, reassuring, expert-without-jargon. Never alarmist, never coy. Dignity over clinical literalism.
- **Headlines:** Short, human, benefit-led. Examples: *"Heal at your own pace," "Strength starts with your breath," "Your body is telling a story."* Sentence-style phrasing set in serif.
- **Eyebrows:** Uppercase, letter-spaced labels above headings (e.g. `PELVIC HEALTH`, `OUR APPROACH`, `POSTPARTUM CARE`).
- **CTAs:** Make the next step easy and pressure-free. Prefer *"Book a free discovery call," "Book a consult," "Start your assessment."* Avoid hard-sell verbs.
- **Casing:** Sentence case for body and most headings; UPPERCASE only for eyebrows, nav, and button labels (with letter-spacing).
- **Emoji:** **Not used.** Brand warmth comes from photography, serif type, and botanical motifs — not emoji.
- **Numerals/stats:** Display stats in serif for an editorial feel (e.g. a large serif `92%` with a small sans label).

---

## VISUAL FOUNDATIONS

**Color** — Green-forward palette drawn from the logo's forest-green leaf, supported by slate blue, warm sand/cream neutrals, sage/olive botanicals, and a single warm-gold accent reserved for CTAs. Target ratio **~70 / 20 / 10**: ~70% neutral earth tones, ~20% brand greens/blues, ~10% gold + sage. **Gold is a rare jewel** — primary CTAs and tiny elegant details only. Never put gold text on cream (fails contrast); gold is for fills, lines, and large display.

**Backgrounds** — Default to `--color-cream` (warm off-white, never stark). Alternate sections with `--color-sand` or `--color-sage-mist` for rhythm. Occasional full-bleed `--color-forest-green-deep` "anchor" sections (footer, CTA bands) with white text. No gradients as a default; warm flat fills and photography lead.

**Type** — Elegant serif headlines (**Fraunces**) + clean sans body (**Mulish**). Tight line-height on headings for impact; body line-height 1.7 at ~65–72ch max measure. Emphasis via weight/size, not color (use `--color-forest-green` when color emphasis is truly needed).

**Spacing** — Airy and spacious. Section vertical padding 96–128px desktop / 56–72px mobile. Card padding 32–40px. This generous rhythm is what makes it feel calm and premium.

**Corners** — Subtly rounded: 6px inputs, 10px buttons/cards, 16px large cards, 24px feature panels, pill for chips. Avoid sharp 0px (too cold) and heavy 30px+ (too playful).

**Borders & shadows** — Prefer **thin warm borders** (`1px solid --color-sand-deep`) over shadows for many cards — flatter and more elegant. When shadows are used they are soft, low, and warm-tinted (`rgba(28,38,32,...)`), never harsh gray drop shadows.

**Cards** — White on cream (or sand on white), `--radius-lg`, 32px padding, thin warm border or `--shadow-md`. Structure: small line icon/image → serif H3 → sans body → ghost "Learn more →" link.

**Imagery** — Warm lifestyle photography: real, diverse people in calm, candid wellness/recovery moments. Soft natural light, warm color grade that sits harmoniously on cream/sand. Rounded corners (`--radius-lg`/`xl`); occasional organic "leaf"/arch-topped image masks as a brand nod. Avoid clinical stock and stereotypes.

**Motion** — Calm and unobtrusive, "like a slow exhale." Transitions 0.2–0.3s ease/ease-out. Gentle fade-and-rise on scroll-in (`opacity` + `translateY(16px)`), staggered for card grids. Hover = subtle lift + color shift + soft shadow growth; never bouncy. Respect `prefers-reduced-motion`.

**Hover/press** — Hover: gentle `translateY(-4px)` lift on cards, darker color shift on buttons (gold→gold-deep, green→green-deep), soft shadow growth. Press: settle back, slightly darker. Outline buttons fill with `--color-sage-mist` on hover.

**Transparency/blur** — Sparingly. Sticky nav may be translucent cream with a subtle bottom border on scroll. Optional very subtle forest-green or sand overlay on hero photos for text legibility.

---

## ICONOGRAPHY

- **Style:** Thin line icons, **1.5px stroke**, rounded caps and joins. Calm, simple, consistent stroke weight.
- **Color:** `--color-forest-green` or `--color-ink-soft`. Optionally seated in a `--color-sage-mist` rounded square (`--radius-md`).
- **Source:** No proprietary icon set was provided. This system uses **[Lucide](https://lucide.dev)** (1.5–2px stroke, rounded — the closest match to the brief) loaded from CDN. *Substitution flagged — swap for an official set if one exists.*
- **Emoji:** Never used as icons. **Unicode** decorative characters are avoided too, except a plain right-arrow `→` in "Learn more →" ghost links.
- **Logo/botanical:** The two-leaf mark (slate-blue left, forest-green right) and sparse leaf accents live in `assets/`. Use leaves as quiet accents, never busy patterns.

---

## Index / manifest

**Root**
- `styles.css` — global entry point (import this); `@import`s all tokens.
- `tokens/` — `colors.css`, `typography.css`, `spacing.css`.
- `assets/` — `logo-full.png` (official two-leaf mark + wordmark), `logo-full-light.png` (for dark surfaces), `leaf-mark.png`.
- `readme.md` — this file. `SKILL.md` — portable skill wrapper.

**Components** (`components/`) — namespace exposed on `window` (run `check_design_system` for exact name)
- `core/Button`, `core/Badge`, `core/Tag`, `core/Card`
- `forms/Input`, `forms/Textarea`
- `layout/EyebrowHeading`, `feedback/Stat`

**UI kits** (`ui_kits/`)
- `website/` — BREATHE marketing site: Nav, Hero, Services, Testimonial, CTA band, Footer.

**Design System tab** — foundation + component specimen cards live as `@dsCard`-tagged HTML throughout (`guidelines/`, component dirs, kit dirs).
