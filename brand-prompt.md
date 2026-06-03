# Heritage Strategies LLC brand prompt

Standalone brand brief for an AI tool building a Heritage Strategies LLC surface, the Heritage marketing site, a stewardship dashboard, a family-office partner portal, a private client report (quarterly statement, generational asset summary, fiduciary memo), an investor or partner deck, an email template, or any artifact representing Heritage externally. Apply these values directly, no token system or design-system install required.

---

## Brand foundation, read this before touching a color or a font

Heritage Strategies is a multi-generational wealth and family-office firm. The brand is **not** about wealth as a lifestyle; it is about the quiet, patient work of stewarding a family's assets across generations after the principal is gone. Every design decision answers to that promise.

- **Archetype:** Custodian / Trustee. Calm, fiduciary, multi-generational, archival. Never Hero, never Disruptor, never Lifestyle, never Tech-Bro.
- **Enemy:** the warning-orange-and-cobalt fintech aesthetic that has crept into wealth marketing, stock photography of suited men shaking hands in glass lobbies, sunset boardrooms, champagne flutes, "luxury" used as an adjective on every page, and the dark-only "cigar club" treatment that reads as men's-club rather than fiduciary. Heritage positions against all of that posture. Restraint is the differentiator.
- **Posture:** prestige and quiet. Closer to a private bank's letterhead, an estate library, or the title page of a trust instrument than a fintech landing page. Confidence reads as understatement, the brand is the **stewardship**, not the assets.
- **The unifying brief:** be the most credible voice in multi-generational stewardship by behaving like a trustee, not a salesperson.

If a design decision makes the brand louder, faster, glossier, or more obviously "luxury," it is wrong, regardless of how well-executed it is in isolation. Old prestige, not new prestige. Old money, not new money.

---

## Output context, classify before you apply anything

Read the user's request and decide which output you are building:

- **Marketing surface,** public-facing pages for heritagestrategiesllc.com, partner or investor decks, one-page tear sheets, client-facing PDFs (quarterly statements, generational asset summaries, stewardship reports, fiduciary memos), email templates. **Editorial mode applies in full.** Skip status colors and form/input chrome unless the page actually contains a form.
- **App or prototype** (the family-office portal, the stewardship dashboard, the partner CMS), the working software used internally by partners, fiduciary officers, and accounts, or by named principals checking their position. **All sections apply, including status colors and tabular-figure rules.**
- **Internal document,** Notion-style notes, decision memos, ops docs, fiduciary post-mortems. Apply only typography, page surfaces, and surface neutrals. No buttons, no status badges, no charts unless the content needs them.

If unsure, ask before applying status colors or form/input guidance. **Never invent UI controls** (buttons, badges, alerts, status indicators, forms) **just to apply the colors below.** Use only what the content actually requires.

---

## Aesthetic

Editorial and archival. Screens should read like the cover of a fiduciary instrument, the inside of an estate library binder, or the title page of a private-client trust dossier. Restraint as the organizing principle, one warm ivory ground, one deep navy reserved for nav and filled CTA, one mid-page navy band, one aged-bronze hairline metallic accent. The wax-seal red lives only inside the supplied logo file, never in the surrounding UI. Generous negative space on the ivory ground. Hierarchy comes from scale, spacing, and 1px bronze hairlines, not from heavy color contrast or busy chrome.

Asymmetric balance over centered stacks. Type does the heavy lifting, the luminous arc is the only piece of motion ornament, and even it sits quietly behind the hero copy at low opacity until it has earned the foreground.

The site of a firm at this tier should age slowly on purpose. Avoid every signal that will look dated in five years, animated counter widgets for AUM, chrome gradients, autoplay aerial b-roll, "Start investing in 60 seconds" urgency banners, glassmorphism, mascot illustrations, oversaturated marketing-orange CTAs.

**The ground is light.** This is the single most important rule. Wealth-brand peers (Bessemer, Pictet, Brown Brothers Harriman, Lombard Odier, Northern Trust, Rothschild & Co, JPMorgan Private Bank, Roemer Capital, Creative Planning, Edelman Financial Engines, Hightower) all run a white or warm-off-white page background. Dark surfaces appear **only** as contrast panels, not as the default ground. A fiduciary brand on a black page reads as a casino or a hedge-fund poster, never as stewardship. Default to warm ivory, navy is a contrast inset.

---

## The mark

Heritage Strategies' identity mark is the **wax-seal HS monogram** paired with the **Heritage Strategies LLC** serif wordmark. Treat it as an insignia, not a tech logo. The real logo file is shipped with this brand system as `heritage-logo.webp`.

- **Use the real file.** Never redraw the seal as inline SVG, never reconstruct the wordmark from CSS, never reletter "Heritage Strategies" in a different family. The actual file is the source of truth. Render at `height: 40px; width: auto;` in nav contexts. Render at `height: 64–96px` in hero/footer detail contexts.
- **The seal is a detail element, not a hero element.** The wax seal monogram appears at 24–48px in section terminators, footer, and as the favicon. It does not appear at hero scale, it does not appear behind type, it does not appear as a watermark inside cards. Demote it on purpose. The seal is the family crest, not the family.
- **Two surfaces.** Place the lockup on warm ivory (the default page surface) as the canonical treatment. Place it on the navy contrast panel only when a hero or quote inset calls for it, render it on a warm-white pill if contrast falls below WCAG AA, otherwise use the file directly.
- **Clear space.** Reserve at least the cap-height of the "H" in "Heritage" around the entire lockup. Nothing crosses that boundary, not a bronze hairline, not the luminous arc, not adjacent type.
- **Never alter.** The logo is never stretched, rotated, recolored, outlined, embossed, drop-shadowed, or set inside a containing shape. No "logo in a circle," no "logo in a square card."

---

## Typography

Two families only, plus a mono for fiduciary detail. Never more than two display + body fonts in a single design. Display serif for headings and the wordmark, clean sans for body, navigation, and all dense data, JetBrains Mono for account numbers, document IDs, ticker symbols, and code.

| Role | Family | Weights | Used for |
|------|--------|---------|----------|
| Display serif | **Source Serif 4** (Google Fonts, variable, opsz 8..60) | 400, 500, 600 | h1, h2, section headings, page titles, the Heritage wordmark in long-form, hero copy, pull quotes |
| Sans (UI + body) | **Inter** (Google Fonts, variable) | 300, 400, 500, 600, 700 | h3–h6, body, navigation, captions, tables, all dense data |
| Mono | **JetBrains Mono** | 400 | account numbers, statement IDs, CUSIPs, document references, code |

Three families, no exceptions. Source Serif 4 was selected over Source Serif 4 and Cormorant Garamond after explicit feedback: Source Serif 4 reads "fashion / wedding stationery" and is wrong for a fiduciary brand; Cormorant is too thin to register as authoritative; Source Serif 4 is a contemporary editorial serif designed by Frank Grießhammer at Adobe for professional and editorial use, and it carries the institutional gravity a US family office requires. The `opsz` axis lets the same font breathe at 56px display and tighten at 14px body, so a single typeface covers the full hierarchy without an additional family.

Load via Google Fonts. Set `font-display: swap`. Apply `font-variation-settings: "opsz" 60` on display sizes and `"opsz" 14` on serif body.

```css
@import url('https://fonts.googleapis.com/css2?family=Source+Serif+4:ital,opsz,wght@0,8..60,300..700;1,8..60,400..600&family=Inter:wght@300;400;500;600;700&family=JetBrains+Mono:wght@400&display=swap');

:root {
  --font-serif: 'Source Serif 4', 'Source Serif Pro', Georgia, 'Times New Roman', serif;
  --font-sans:  'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', system-ui, sans-serif;
  --font-mono:  'JetBrains Mono', 'SF Mono', ui-monospace, monospace;
}

/* Display sizes pick up a larger opsz */
.display { font-variation-settings: "opsz" 60; }
/* Body in serif uses a smaller opsz */
.serif-body { font-variation-settings: "opsz" 14; }
```

### Type scale

| Element | Size | Line height | Weight | Family | Notes |
|---------|------|-------------|--------|--------|-------|
| Display title (hero) | 64–88px | 1.05 | 400 | Display serif | Use `opsz` 144 for proper display optical size. Color: navy on ivory, warm cream on dark contrast panel |
| h1 (marketing) | 44px | 1.15 | 400 | Display serif | Letter-spacing default, never bold |
| h2 (marketing) | 32px | 1.2 | 400 | Display serif | |
| Section eyebrow (small-caps bronze) | 12–13px | 1.3 | 500 | Sans, **all-caps**, letter-spacing 0.18em | Bronze on ivory, cream on navy. Replaces JetHQ's serif gold label |
| Subheading | 20–22px | 1.3 | 500 | Sans | Used directly beneath a serif heading, see "Heading + Subheading pattern" |
| h1 (app) | 28px | 1.25 | 500 | Sans Medium | |
| h2 (app) | 22px | 1.3 | 500 | Sans Medium | |
| h3 | 18–20px | 1.35 | 500 | Sans Medium | |
| h4 | 16px | 1.4 | 500 | Sans Medium | |
| Body | 15–16px | 1.6 | 400 | Sans | Inter 400 is the default body weight. Larger than JetHQ because the ground is light and AA reads at 16px more reliably |
| Small / metadata / nav labels | 12–13px | 1.4 | 500 | Sans Medium | Used for nav items and trust-bar credentials |
| Mono / account / CUSIP | 13–14px | 1.4 | 400 | Mono | Always uppercase for CUSIPs and document IDs |

### Heading + Subheading pattern (signature device)

Heritage's signature type lockup is a **serif HEADING in navy** stacked directly above a **sans SUBHEADING in muted ink**, the prestige inverse of JetHQ's gold-on-dark. Reproduce it exactly where a section needs emphasis:

```html
<header class="section-title">
  <p class="section-eyebrow">SECTION EYEBROW</p>
  <h2 class="section-heading">Heading</h2>
  <p class="section-subheading">Subheading</p>
</header>
```

```css
.section-eyebrow {
  font-family: var(--font-sans);
  font-size: 12px;
  font-weight: 500;
  letter-spacing: 0.22em;
  color: var(--bronze);
  text-transform: uppercase;
  margin: 0 0 24px 0;
}
.section-heading {
  font-family: var(--font-display);
  font-variation-settings: "opsz" 144;
  font-size: clamp(36px, 5vw, 56px);
  font-weight: 400;
  line-height: 1.05;
  color: var(--navy);
  margin: 0 0 12px 0;
}
.section-subheading {
  font-family: var(--font-sans);
  font-weight: 400;
  font-size: clamp(18px, 1.8vw, 22px);
  color: var(--text-muted);
  margin: 0;
}
```

### Section eyebrow (bronze small-caps)

Anywhere a section opens, a card, a panel, a deck slide, a PDF section break, use the **bronze small-caps eyebrow**. It is the spine of the Heritage hierarchy. Never use serif for this label, the eyebrow is sans on purpose to keep the serif heading singular.

```css
.eyebrow-bronze {
  font-family: var(--font-sans);
  font-size: 12px;
  font-weight: 500;
  letter-spacing: 0.22em;
  color: var(--bronze);
  text-transform: uppercase;
}
```

### Letter-spacing

- Display serif headings, default tracking, never tighten below `-0.01em`. Source Serif 4 and Source Serif 4 want room.
- Small-caps bronze eyebrows, `letter-spacing: 0.22em`. Wider than JetHQ on purpose, this is the archival voice.
- Body and UI, default tracking.
- Mono (account, CUSIP), default tracking, uppercase.

### Numerals, tabular figures in any dense data

Anywhere numbers stack, a quarterly statement, a generational asset summary, a stewardship table, an AUM line, use tabular figures so columns align:

```css
font-variant-numeric: tabular-nums;
font-feature-settings: "tnum" 1;
```

Apply on `table`, `.statement`, `.position`, `.aum`, `.amount`, `pre`, `code`, and any data-bearing component. **Reject counter animations** on AUM, family count, or founding year, set them in static Source Serif 4. The reason a private bank does not animate its AUM ticker is because the number is supposed to feel old, not new.

### Type rules

- **Maintain a clean and professional hierarchy in text sizes.**
- **Avoid using more than two display + body fonts per design.** Display serif + sans + mono is the entire system.
- **Keep text contrast high for readability.** WCAG AA minimum, AAA preferred. Body text is `#1B2230` on the ivory ground at 16px, `#E8E2D2` on navy at 16px. Never use muted-text colors for body copy, only for metadata.
- **Tabular figures are mandatory** in any artifact that shows a dollar amount, a percentage, or a date column.

---

## Colors

All values are HSL components, paste inside `hsl()` to use as a CSS color. HEX values follow the calibrated palette exactly.

### The ten-swatch system

| # | Role | HEX | HSL | Where |
|---|------|-----|-----|-------|
| 1 | **Page Ivory** (default page) | `#FAF7F2` | `hsl(36 40% 97%)` | The default page background on every Heritage marketing surface, statement, and deck. Warm, never pure white. |
| 2 | **Surface White** (cards, tables) | `#FFFFFF` | `hsl(0 0% 100%)` | Cards, tables, and the inside of statement tear-sheets. Pure white sits on the ivory ground with a quiet hue gap. |
| 3 | **Ink Navy** (primary text) | `#1B2230` | `hsl(218 27% 14%)` | Body text and headings on ivory, never pure black. Inherits the warmth of the page. |
| 4 | **Text Muted** (secondary) | `#6B7280` | `hsl(220 9% 47%)` | Secondary text, metadata, captions, dot-separators on the trust bar. Never for body copy. |
| 5 | **Heritage Navy** (nav, contrast) | `#1E2A44` | `hsl(220 38% 19%)` | The nav background, the hero contrast panel, principle-quote insets, deck cover backgrounds. The signature dark color. |
| 6 | **Contrast Dark** (hero panel) | `#0F1626` | `hsl(220 44% 11%)` | The deeper of the two dark surfaces. Used for the hero panel and the single mid-page principle-quote inset. Sits one step deeper than Heritage Navy. |
| 7 | **Aged Bronze** (hairlines, detail) | `#8C7351` | `hsl(35 26% 43%)` | 1px structural hairlines (top of page, bottom of page, beneath nav). **Never a button fill, never a text color, never a chart series.** Bronze is the picture frame, not the picture. |
| 8 | **Reserved Blue** (state only) | `#2C5282` | `hsl(214 50% 34%)` | **State only**, active, selected, focus, info. Never decorative, never a hero color, never a chart series. A reserved-blue focus ring or active tab indicator. |
| 9 | **Cream on Dark** (text on navy) | `#F4F0E6` | `hsl(44 36% 93%)` | Body copy on the navy / contrast-dark panels. Warm cream, never pure white. |

> **The system carries no red.** The wax seal in the supplied logo file `heritage-logo.webp` is the only red the brand uses, and it stays inside the logo. Do not introduce a burgundy CTA, link, badge, accent, divider, chart series, or rule color. If a designer reaches for red because "the seal is red," they have misunderstood the system. The seal lives in the lockup. The rest of the surface is ivory, navy, and ink.

### Usage ratio (the most important rule)

The brand is **80 / 14 / 5 / 1**:

- **80%** Page Ivory (`#FAF7F2`) and Surface White (`#FFFFFF`).
- **14%** Heritage Navy (`#0F1E36`), the nav text, headlines, filled CTA, and the one mid-page principle-quote inset.
- **5%** Contrast Dark (`#0A1628`), the deepest panel, used inside the inset band and the splash mode.
- **1%** Aged Bronze (`#8C7351`), the 1px hairline top + bottom + beneath nav, section eyebrows.

Reserved Blue and the viz palette are below 1% combined, they appear only inside the family-office portal app.

### The strict color partitioning

Heritage has three colors that signal interaction or state. They are strictly partitioned:

1. **Heritage Navy (`#0F1E36`)** is the system's only chromatic identity. Use for nav text, headlines, filled CTA, the principle-quote inset, and the splash-mode background. It is the one deep color, doing the heavy lifting.
2. **Aged Bronze (`#8C7351`)**, **structural metallic**, used for 1px hairlines and detail rules. **Never a button fill, never a chart series, never a paragraph color.** Bronze is the picture frame, not the picture.
3. **Reserved Blue (`#2C5282`)**, **state only**, active, selected, focus, informational status. A reserved-blue focus ring. A reserved-blue "active tab" underline. **Never a decorative accent. Never a hero color. Never a chart series default.** Once reserved blue appears on a decorative element, its meaning as a state indicator is broken everywhere else.
4. **Ink (`#1B2230`)** for body type on light, **Cream (`#F4F0E6`)** for body type on dark. These two text colors are not interchangeable, ink on dark or cream on light are both wrong.

### Page surfaces

The default Heritage surface is **light**. Warm ivory (`#FAF7F2`) is the page, never pure white. Cards and tables sit on **pure white (`#FFFFFF`)** with a quiet hue gap that gives the page a paper feel. Dark surfaces (Heritage Navy, Contrast Dark) appear only as contrast panels, not as the default ground.

| Role | Value | Where |
|------|-------|-------|
| Page Ivory (default page background) | `hsl(36 40% 97%)`, `#FAF7F2` | Default for every Heritage marketing surface, deck, and PDF body |
| Surface White (cards, tables) | `hsl(0 0% 100%)`, `#FFFFFF` | Cards, statement tables, partner-bio modules |
| Heritage Navy (nav, contrast panel) | `hsl(220 38% 19%)`, `#1E2A44` | Sticky nav, principle-quote inset, deck cover backgrounds |
| Contrast Dark (hero panel) | `hsl(220 44% 11%)`, `#0F1626` | The hero ground beneath the luminous arc. Deepest panel in the system |
| Card on dark (rare) | `hsl(220 35% 22%)` | Used inside the navy hero panel only, when a CTA card needs to lift slightly from the ground |

The page is ivory, cards on ivory go **whiter, not darker**. This is the opposite of JetHQ and the opposite of most "modern" wealth-fintech surfaces, and is core to the Heritage feel. The layout reads like ink-on-paper, not pixels-on-screen.

### Action color, interactive elements

Heritage's primary button is **filled Heritage Navy with ivory text on a light ground**. Secondary is **navy-outlined with navy text**. Ghost is a quiet rule-bordered tertiary. **There is no burgundy or red button. There is no burgundy or red link.** The wax seal in the logo file is the only red the brand ever shows.

| Role | Value |
|------|-------|
| Primary button bg (filled navy, one per page) | `hsl(218 57% 14%)`, `#0F1E36` |
| Primary button text on filled navy | `hsl(36 40% 97%)`, `#FAF7F2` (ivory) |
| Primary button hover (filled) | `hsl(220 44% 11%)`, `#0A1628` (one step deeper) |
| Secondary button bg on ivory (outline) | transparent |
| Secondary button border on ivory | `hsl(218 57% 14%)`, navy |
| Secondary button text on ivory | `hsl(218 57% 14%)`, navy |
| Secondary button hover on ivory | navy fill, ivory text (full inversion on hover) |
| Ghost button | transparent, `hsl(38 22% 88%)` border, navy text |
| Ghost hover | `hsl(38 22% 92%)` background (light surface-2 tint) |
| Focus ring (everywhere) | `hsl(214 50% 34%)`, reserved blue, 2px, 2px offset |
| Inline link (on ivory) | `hsl(218 57% 14%)` (navy) with `border-bottom: 1px solid hsl(38 22% 85%)` |
| Inline link hover (on ivory) | navy text, border-bottom color navy |
| Inline link (on dark) | `hsl(44 36% 93%)` (cream) with bronze underline |

**Buttons are rectangles with a 4px radius, not pills.** Pills read as consumer-app casual and break the fiduciary posture. The only pill-radius elements are status indicators and avatars (`9999px`).

### Surface neutrals

Borders on the ivory ground are warm hairlines, on navy they are mist at low alpha. Use the listed values directly, do not substitute a solid gray.

| Role | Value |
|------|-------|
| Foreground (body text on ivory) | `hsl(218 27% 14%)`, `#1B2230` |
| Foreground (body text on dark) | `hsl(44 36% 86%)`, `#E8E2D2` |
| Muted foreground (secondary text, ivory) | `hsl(220 9% 47%)`, `#6B7280` |
| Muted foreground (secondary text, dark) | `hsl(220 9% 67%)` |
| Placeholder text | `hsl(220 9% 60%)` |
| Border (default, ivory) | `hsl(38 22% 88%)`, `#E7E2D9` (warm hairline) |
| Border (input / field, ivory) | `hsl(220 9% 75%)` |
| Border (strong / hover, ivory) | `hsl(218 27% 14% / 0.2)` |
| Border (default, dark) | `hsl(218 27% 28%)` |
| Hairline structural (top + bottom of page, beneath nav) | `hsl(35 26% 43%)`, solid bronze, **1px only** (no thick bar) |

### Status colors (app / prototype mode only)

**Skip this section entirely if you are building a marketing surface, deck, or PDF.** Status colors exist for success / warning / error / info feedback inside the family-office portal. **They are semantic-only, never use a status color as a decorative or brand accent.**

Heritage status colors are calibrated to sit on the ivory ground without competing with the navy identity. Backgrounds are pale tints, not saturated fills. **No red destructive state**, destructive actions use a typed confirmation modal instead of a color.

| Status | Background (on ivory) | Text / Icon | Border |
|--------|----------------------|-------------|--------|
| Success | `hsl(150 30% 94%)` | `hsl(150 50% 22%)` | `hsl(150 30% 70%)` |
| Warning | `hsl(46 50% 92%)` | `hsl(46 60% 24%)` | `hsl(46 50% 70%)` |
| Error   | `hsl(0 40% 94%)`  | `hsl(0 60% 28%)`  | `hsl(0 40% 70%)` |
| Info (uses Reserved Blue) | `hsl(214 50% 94%)` | `hsl(214 50% 28%)` | `hsl(214 50% 70%)` |

Note the warning hue is at 46°, **above the warning band threshold** (45°) and **outside the navy identity's hue family** (218°). Warning is for app state only, it never appears on a marketing surface.

Info status and Reserved Blue are the same hue family, this is intentional. Reserved Blue means "currently active / informational" everywhere it appears.

### Visualization palette

Eight calibrated identity colors for charts inside the family-office portal, position-vs-benchmark grids, sector allocation rings, and entity markers on map views. Three permitted uses, (1) data visualization, (2) categorical markers, (3) brand-decorative accents on long-form surfaces. **No red or burgundy in the viz palette** — the seal red stays inside the logo file.

Never use viz colors on UI controls (buttons, alerts, status indicators, badges). Never use **Reserved Blue** as a chart series, it has another job (state). Never use **Aged Bronze** as a chart series, it has only one job (hairlines).

**Chart series assignment.** Single-series charts use index 0 (Slate Navy). Multi-series charts cycle 0 → 7 before any reuse.

| Index | Name | Base | Background tint (on ivory) | Foreground on base |
|-------|------|------|----------------------------|--------------------|
| 0 | Slate Navy   | `hsl(220 38% 35%)` | `hsl(220 38% 94%)` | light, `hsl(44 36% 96%)` |
| 1 | Bronze Tan   | `hsl(35 26% 55%)`  | `hsl(35 26% 94%)`  | dark, `hsl(218 27% 14%)`  |
| 2 | Moss         | `hsl(140 18% 38%)` | `hsl(140 18% 94%)` | light, `hsl(44 36% 96%)` |
| 3 | Aubergine    | `hsl(295 16% 38%)` | `hsl(295 16% 94%)` | light, `hsl(44 36% 96%)` |
| 4 | Sand         | `hsl(50 28% 64%)`  | `hsl(50 28% 95%)`  | dark, `hsl(218 27% 14%)`  |
| 5 | Sky          | `hsl(210 32% 50%)` | `hsl(210 32% 94%)` | light, `hsl(44 36% 96%)` |
| 6 | Plum         | `hsl(340 18% 38%)` | `hsl(340 18% 94%)` | light, `hsl(44 36% 96%)` |
| 7 | Fog          | `hsl(220 6% 55%)`  | `hsl(220 6% 95%)`  | dark, `hsl(218 27% 14%)`  |

Index 7 (Fog) is the low-chroma "uncategorized / unknown" slot. Assign chart colors by stable position in the list (`index = position % 8`), never by hashing the name.

For more than 8 categories, cycle back with darkened, desaturated versions:

```css
color-mix(in srgb, hsl(var(--color-viz-N)) 70%, black)
```

---

## Decorative motifs

Heritage has exactly **three** sanctioned decorative devices. The first is the only piece of motion in the entire system. The second is the family crest. The third is a structural frame.

### 1. The luminous arc (the signature motif, animated)

A single luminous arc, drawn slowly across the navy hero panel from lower-left to upper-right. It is the only piece of motion ornament in the brand. It evokes a generational horizon, a meridian, a long arc of stewardship across decades, the bend of time over multiple lifetimes. Use it once per page, inside the hero panel only.

**When to use:**
- **Inside the hero panel,** behind the wordmark and hero copy. Always on the contrast-dark background. Always at low opacity once drawn (≤ 0.9).
- **Nowhere else.** Not inside cards, not in the body, not as a footer ornament, not as a section divider. One arc per page.

**When NOT to use:**
- Never on the ivory ground.
- Never with a gradient tint outside the warm-ivory to soft-bronze spectrum.
- Never animated faster than the spec (6s draw, 9s breathe).
- Never with `prefers-reduced-motion: reduce` overridden.

```html
<div class="hero-arc" aria-hidden="true">
  <svg viewBox="0 0 1440 600" preserveAspectRatio="xMidYMid slice" role="presentation">
    <defs>
      <linearGradient id="arcGrad" x1="0" y1="0" x2="1" y2="0">
        <stop offset="0%"   stop-color="#F5EFE2" stop-opacity="0"/>
        <stop offset="50%"  stop-color="#F5EFE2" stop-opacity="1"/>
        <stop offset="100%" stop-color="#C9B98A" stop-opacity="0"/>
      </linearGradient>
      <filter id="arcGlow" x="-20%" y="-20%" width="140%" height="140%">
        <feGaussianBlur stdDeviation="4" result="blur"/>
        <feMerge>
          <feMergeNode in="blur"/>
          <feMergeNode in="SourceGraphic"/>
        </feMerge>
      </filter>
    </defs>
    <path
      class="arc"
      d="M -80 460 Q 360 120 720 240 T 1520 180"
      fill="none"
      stroke="url(#arcGrad)"
      stroke-width="1.25"
      stroke-linecap="round"
      filter="url(#arcGlow)"
      pathLength="1"
    />
  </svg>
</div>

<style>
  .hero-arc { position: absolute; inset: 0; pointer-events: none; overflow: hidden; }
  .hero-arc svg { width: 100%; height: 100%; display: block; }
  .arc {
    stroke-dasharray: 1;
    stroke-dashoffset: 1;
    opacity: 0;
    animation:
      arc-draw    6s cubic-bezier(.22, .61, .36, 1) .4s forwards,
      arc-breathe 9s ease-in-out 6.4s infinite;
  }
  @keyframes arc-draw {
    0%   { stroke-dashoffset: 1; opacity: 0; }
    15%  { opacity: .9; }
    100% { stroke-dashoffset: 0; opacity: .9; }
  }
  @keyframes arc-breathe {
    0%, 100% { opacity: .55; }
    50%      { opacity: .95; }
  }
  @media (prefers-reduced-motion: reduce) {
    .arc { animation: none; stroke-dashoffset: 0; opacity: .8; }
  }
</style>
```

The arc is the only piece of motion in the brand. No counter animations, no scroll-jacking, no parallax. The arc breathes, that is all.

### 2. The wax-seal HS monogram (demoted to detail)

The actual `heritage-logo.webp` file is the canonical seal. The wax-seal red and the bronze interior typography are properties of that file. They are not extracted as system colors. The seal is a **detail element**, not a hero element.

**When to use:**
- **Section terminator,** a 24–32px seal at the bottom-right of a section as a quiet closing punctuation mark.
- **Footer,** a 32–48px seal in the footer, beside the colophon line.
- **Favicon,** a 32px export of the seal.
- **Statement tear-sheet header,** a 32px seal in the top-right corner of a quarterly statement PDF.

**When NOT to use:**
- Never at hero scale. Never larger than 64px outside the lockup contexts above.
- Never as a watermark behind body type.
- Never recolored. Never gradient-tinted. The seal ships with the colors it has, those are the brand colors.
- Never animated.

```html
<!-- Section terminator -->
<div class="section-seal" aria-hidden="true">
  <img src="./heritage-logo.webp" alt="" width="32" height="32" style="opacity: 0.9;">
</div>
```

```css
.section-seal {
  display: flex;
  justify-content: flex-end;
  padding-top: 32px;
  border-top: 1px solid var(--rule);
}
```

### 3. The bronze hairlines (top + bottom of page, beneath nav)

Three non-negotiable structural elements on every full-page surface:

- **Top of viewport,** a 1px bronze hairline directly beneath the sticky nav.
- **Bottom of page,** a 1px bronze hairline above the footer, the final stroke of the page.
- **Section dividers,** a 1px warm-rule (`hsl(38 22% 88%)`) between major sections. The bronze is reserved for the structural top and bottom, the warm-rule does the internal work.

These three rules frame every Heritage surface like the hairlines on a fiduciary instrument. They are 1px only, the thick 12px bottom bar of JetHQ is wrong for Heritage. Heritage is quieter, hairlines only.

```css
.hairline-bronze { height: 1px; background: var(--bronze); width: 100%; }
```

**Do not** invent new decorative shapes (triangles, dots, ornaments, dividers, brackets, mascots). The arc + seal + bronze hairlines are the three motifs. A fourth is a redesign.

---

## Layout

### Grid

12-column grid, 24px gutter at desktop, 16px at tablet, 8px at mobile. Container max-widths:

- Editorial marketing, 1200px outer, 680px text measure for long-form prose.
- App (family-office portal), 1440px outer, full-bleed tables and sheets inside.
- PDF / deck slide, 1140px (matches a standard 16:9 deck export at 1920×1080 with margins).

### Page shell

Every full-page surface follows the same shell:

```
┌──────────────────────────────────────────────────────────┐
│  [Heritage logo]      Logo · Type · Color · Components   │  ← nav, 72px tall, warm ivory bg
├──────────────────────────────────────────────────────────┤  ← 1px bronze hairline
│  ╔══════════════════════════════════════════════════════╗ │
│  ║  HERO, navy/contrast-dark, full-bleed               ║ │  ← the only dark band above the fold
│  ║  [animated luminous arc behind copy]                ║ │
│  ╚══════════════════════════════════════════════════════╝ │
│                                                          │
│           [page content on warm ivory]                   │
│                                                          │
│  ╔══════════════════════════════════════════════════════╗ │
│  ║ PRINCIPLE QUOTE, navy contrast inset (one only)     ║ │
│  ╚══════════════════════════════════════════════════════╝ │
│                                                          │
│           [more page content on warm ivory]              │
│                                                          │
├──────────────────────────────────────────────────────────┤  ← 1px bronze hairline
│  [footer, ivory, muted ink, view-source link]            │
└──────────────────────────────────────────────────────────┘
```

The nav, the top bronze hairline, the hero contrast panel, the single mid-page principle inset, and the bottom bronze hairline are present on **every** marketing surface and PDF cover. Internal app pages may drop the principle inset and may simplify the hero to a single ivory band with a navy heading, but never drop the hairlines.

### Spacing

Base unit: **8px**. Spacing tokens: 4, 8, 12, 16, 24, 32, 48, 64, 96, 128. Marketing layouts bias toward 64–128. App layouts use 8–24 most often.

### Border-radius

Disciplined small set: `0` (table cells, hairline dividers), `4px` (cards, inputs, buttons), `8px` (modals, large panels, the principle-quote inset), `9999px` (status pills, avatars only, never primary buttons).

### Elevation

Almost flat. Default surfaces use a 1px border, no shadow. Cards on ivory sit on pure white with a 1px warm-rule border. Modals and dropdowns get a single soft elevation:

```css
box-shadow: 0 8px 24px -8px rgba(27, 34, 48, 0.18);
```

Never use heavy drop shadows, they read as dated and salesy.

### Motion

The luminous arc is the only piece of motion ornament in the brand.

- **Arc draw,** 6s, ease-out, runs once on page load with a 400ms delay.
- **Arc breathe,** 9s, ease-in-out, runs after the draw completes (6.4s start), loops infinitely.
- **Reveal-on-scroll,** section headers fade and translate-y(8px) to 0 over 400ms, ease-out, triggered by IntersectionObserver at 20% threshold. **Subtle, single transition per element, no stagger choreography.**
- **No counter animations.** AUM, family count, founding year, all set in static Source Serif 4. The reason a private bank does not animate its AUM ticker is because the number is supposed to feel old.
- **No scroll-jacking, no parallax, no spring physics, no decorative motion.**

Fast 150ms, base 250ms, slow 400ms; ease-out for fades, ease-in-out for transforms. Honor `prefers-reduced-motion: reduce` with a zero-duration variant on every animation in the system. The arc snippet above already does this, every other transition must too.

---

## Imagery

The biggest mistake firms in this category make is generic wealth stock, tarmac handshakes, sunset boardrooms, leather-cabin close-ups with a champagne flute, hands signing documents in soft focus. Heritage does not use them. Imagery is either:

1. **Commissioned portraiture,** real partners, real principals, real fiduciary officers, shot in available light, never the glossy-headshot cliché. 1:1 portrait crops. Mid-tone backgrounds. No vignettes, no chrome. The face does the work.
2. **Architectural photography of estate libraries, vault interiors, oil-on-canvas surfaces, the spine of a leather-bound book, the corner of a deed,** restrained, editorial, never lifestyle. The artifact does the work, not the lifestyle around the artifact.
3. **Document specimens,** a redacted excerpt of a quarterly statement, a stylized fragment of a generational asset summary, a fiduciary memo letterhead. Heritage's own artifacts, treated as portraits.

**The test:** could a generic wealth-management competitor lift this image onto their own site? If yes, it is working against you. Replace it.

Stock wealth imagery is forbidden. If a photograph is required and no commissioned shot exists, default to an architectural photograph of an estate library interior or a vault corner, monochromatic, ivory + navy + brown only.

---

## Voice and page patterns

Marketing surfaces sell calm stewardship, not "premium investment experiences." Concretely:

- **Hero copy must speak like a trustee, not a marketer.** "We steward what your family has built" lands harder than "Premium private wealth, reimagined." Speak to the specific situation, multi-generational transition, a family business sale, a private foundation, a complex trust structure, a charitable remainder. The visitor knows what a wealth manager is, what they want to know is whether you are competent, discreet, and patient.
- **Proof goes high on the page, as numbers.** Founding year, AUM, named family count, regulatory affiliations (state trust company charter, federal RIA registration) shown as a quiet trust bar, never as logos-soup. **Numbers beat adjectives.** No "premier," no "trusted," no "world-class," no "boutique," no "white-glove." Show $X under stewardship, Y generations, Z years.
- **One low-pressure call to action per page.** "Request a Stewardship Conversation" or "Speak with a Partner." Framed as a conversation, not a transaction. A single field, name, email, a short message. Never a ten-field RFP form on the marketing site, never urgency banners, never countdown timers, never chatbots.
- **No marketing motion.** No autoplay aerial b-roll. No animated counters ("$2.4B in stewardship"). No carousels. No exit-intent overlays. Each reads as salesy and erodes the fiduciary posture.
- **Body voice, direct, declarative, owner / date / next-step framed.** No em dashes. No hedging. No "we believe." No "we are passionate about." Short sentences sit comfortably next to long ones. Show, never claim. Account numbers, CUSIPs, and document IDs appear in mono and uppercase.
- **The AI Employee is named Foreman.** Not Elliot. Reference Foreman by name in any artifact that mentions the firm's AI tooling.

App surfaces (the family-office portal) sell competence and care. Keep the same restraint, but allow density:

- Statement breakdowns, position tables, and generational asset summaries are dense by necessity. Respect the density, do not pad data screens with marketing whitespace, and do not import editorial display type into app chrome.
- Surface only one primary action per screen. Secondary actions ghost. Destructive actions (close an account, transfer custody) require a typed confirmation, never just a "Cancel" button at hover-distance.
- Audit trail and provenance are part of the brand. Show "stewarded by [partner] since [year]" on every position artifact. This is how the product earns trust the way the firm does.

---

## Trust bar

Heritage marketing surfaces should carry a **quiet trust bar** under the hero, a single line of subdued credentials. The pattern:

```
Founded YYYY   ·   Family stewardship since YYYY   ·   $X under stewardship   ·   State / federal regulator
```

Worked example:

```
Founded 1987   ·   Family stewardship since 1962   ·   $2.4B under stewardship   ·   PA chartered trust company · SEC RIA
```

- Render in 12–13px sans Medium, `hsl(220 9% 47%)` on ivory, `hsl(220 9% 67%)` on dark.
- Dot separators with a full em of space either side.
- Never use peer logos (Bessemer, JPMorgan, Pictet) as a trust bar. Heritage's trust is conferred by its own credentials, not by a neighbor's wordmark.

---

## Component patterns, copy-pasteable

### CSS tokens

```css
:root {
  /* fonts */
  --font-display: 'Source Serif 4', 'Source Serif 4', Georgia, serif;
  --font-sans:    'Inter', system-ui, -apple-system, sans-serif;
  --font-mono:    'JetBrains Mono', ui-monospace, monospace;

  /* surfaces */
  --page:           hsl(36 40% 97%);   /* #FAF7F2 */
  --surface:        hsl(0 0% 100%);    /* #FFFFFF */
  --surface-2:      hsl(38 22% 92%);   /* #F2EDE3, tinted panel */
  --navy:           hsl(218 57% 14%);  /* #0F1E36, the single dark */
  --navy-deep:      hsl(220 44% 11%);  /* #0A1628, the inset band */

  /* ink + text */
  --ink:            hsl(218 27% 14%);  /* #1B2230 */
  --text-muted:     hsl(220 11% 41%);  /* #5C6573 */
  --text-on-dark:   hsl(44 36% 93%);   /* #F4F0E6 */
  --text-on-dark-muted: hsl(220 9% 67%);

  /* details — NO burgundy, NO red */
  --bronze:         hsl(35 26% 43%);   /* #8C7351, 1px hairlines only */
  --state:          hsl(214 50% 34%);  /* #2C5282, focus / active only */

  /* hairlines */
  --rule:           hsl(38 22% 85%);   /* #E2DCD0, warm hairline on ivory */
  --rule-dark:      hsl(218 27% 28%);  /* hairline on navy */

  --nav-height: 72px;
}

body {
  background: var(--page-bg);
  color: var(--ink);
  font-family: var(--font-sans);
  font-size: 16px;
  font-weight: 400;
  line-height: 1.6;
  margin: 0;
  min-height: 100vh;
}
```

### Nav bar (with real logo)

```html
<nav class="nav" aria-label="Heritage Strategies brand navigation">
  <a class="lockup" href="/" aria-label="Heritage Strategies LLC home">
    <img src="./heritage-logo.webp" alt="Heritage Strategies LLC" height="40" width="auto">
  </a>
  <ul class="nav-links">
    <li><a href="#mark">Mark</a></li>
    <li><a href="#typography">Type</a></li>
    <li><a href="#color">Color</a></li>
    <li><a href="#components">Components</a></li>
    <li><a href="#prompt">Prompt</a></li>
  </ul>
</nav>
<div class="hairline-bronze" role="presentation"></div>
```

```css
.nav {
  height: var(--nav-height);
  display: flex; align-items: center; justify-content: space-between;
  padding: 0 clamp(20px, 4vw, 48px);
  background: var(--page-bg);
  position: sticky; top: 0; z-index: 50;
}
.lockup img { display: block; height: 40px; width: auto; }
.nav-links { display: flex; gap: clamp(20px, 3vw, 36px); list-style: none; margin: 0; padding: 0; }
.nav-links a {
  font-family: var(--font-sans);
  font-size: 12px; font-weight: 500;
  letter-spacing: 0.18em; text-transform: uppercase;
  color: var(--ink); text-decoration: none;
  transition: color 200ms ease-out;
}
.nav-links a:hover { opacity: 0.55; }
.hairline-bronze { height: 1px; background: var(--bronze); opacity: 0.45; width: 100%; }
```

### Primary button (filled navy, one per page)

```html
<button class="btn btn-primary" type="button">Request a Stewardship Conversation</button>
```

```css
.btn-primary {
  display: inline-flex; align-items: center; justify-content: center;
  padding: 14px 26px;
  background: var(--navy);
  color: var(--page);
  border: 1px solid var(--navy);
  border-radius: 3px;
  font-family: var(--font-sans);
  font-weight: 500; font-size: 13px; letter-spacing: 0.14em;
  text-transform: uppercase; text-decoration: none; cursor: pointer;
  transition: background-color 200ms ease-out, border-color 200ms ease-out;
}
.btn-primary:hover { background: var(--navy-deep); border-color: var(--navy-deep); }
```

### Secondary button (navy outline, navy text on ivory)

```html
<button class="btn btn-secondary" type="button">Speak with a Partner</button>
```

```css
.btn-secondary {
  display: inline-flex; align-items: center; justify-content: center;
  padding: 14px 26px;
  background: transparent;
  color: var(--navy);
  border: 1px solid var(--navy);
  border-radius: 3px;
  font-family: var(--font-sans);
  font-weight: 500; font-size: 13px; letter-spacing: 0.14em;
  text-transform: uppercase; text-decoration: none; cursor: pointer;
  transition: background-color 200ms ease-out, color 200ms ease-out;
}
.btn-secondary:hover { background: var(--navy); color: var(--page); }
```

### Card on light

```html
<article class="card">
  <p class="card-eyebrow">STEWARDSHIP NOTE</p>
  <h3 class="card-title">Generational Continuity</h3>
  <p class="card-body">Three generations of stewardship across the principal's holdings, structured through a discretionary trust with a perpetuity reserve.</p>
</article>
```

```css
.card {
  background: var(--surface);
  border: 1px solid var(--rule);
  border-radius: 4px;
  padding: 32px;
}
.card-eyebrow {
  font-family: var(--font-sans);
  font-size: 11px; font-weight: 500; letter-spacing: 0.22em;
  color: var(--bronze); text-transform: uppercase;
  margin: 0 0 16px 0;
}
.card-title {
  font-family: var(--font-display);
  font-size: 28px; font-weight: 400; line-height: 1.15;
  color: var(--navy); margin: 0 0 12px 0;
}
.card-body { color: var(--ink); margin: 0; line-height: 1.6; }
```

### Section heading (signature serif + sans pair)

```html
<header class="section-title">
  <p class="section-eyebrow">SECTION EYEBROW</p>
  <h2 class="section-heading">Heading</h2>
  <p class="section-subheading">Subheading</p>
</header>
```

### Three-way comparison card (the Roemer pattern)

```html
<div class="comparison">
  <article class="comparison-card neutral">
    <p class="comparison-label">Generic Trust Company</p>
    <ul>
      <li>Quarterly reviews</li>
      <li>Standardized portfolios</li>
      <li>Phone-tree client service</li>
    </ul>
  </article>
  <article class="comparison-card neutral">
    <p class="comparison-label">Single-Family Office</p>
    <ul>
      <li>Bespoke structures</li>
      <li>High fixed cost</li>
      <li>Single-client concentration risk</li>
    </ul>
  </article>
  <article class="comparison-card heritage">
    <div class="comparison-mark">
      <img src="./heritage-logo.webp" alt="" width="32" height="32">
    </div>
    <p class="comparison-label">Heritage Strategies</p>
    <ul>
      <li>Multi-generational stewardship</li>
      <li>Named partner per family</li>
      <li>Foreman, the firm's AI Employee, on every artifact</li>
    </ul>
  </article>
</div>
```

```css
.comparison { display: grid; grid-template-columns: repeat(3, 1fr); gap: 16px; }
.comparison-card { padding: 32px; border-radius: 4px; }
.comparison-card.neutral { background: hsl(38 22% 95%); color: var(--ink); }
.comparison-card.heritage { background: var(--navy); color: var(--text-on-dark); }
.comparison-card.heritage .comparison-label { color: var(--text-on-dark); }
.comparison-label {
  font-family: var(--font-sans);
  font-size: 11px; font-weight: 500; letter-spacing: 0.22em;
  text-transform: uppercase;
  color: var(--bronze);
  margin: 16px 0 24px 0;
}
.comparison-card ul {
  list-style: none; padding: 0; margin: 0;
  font-family: var(--font-sans); font-size: 14px; line-height: 1.7;
}
.comparison-card.neutral li::before { content: "× "; color: var(--text-muted); font-family: var(--font-mono); }
.comparison-card.heritage li::before { content: "+ "; color: var(--bronze); font-family: var(--font-mono); }
```

### Stewardship table

```html
<table class="stewardship-table">
  <thead>
    <tr>
      <th>Family</th><th>Generation</th><th>Stewardship Since</th><th class="num">Assets Under Stewardship</th>
    </tr>
  </thead>
  <tbody>
    <tr><td>Redacted A</td><td>Third</td><td>1989</td><td class="num">$420,000,000</td></tr>
    <tr><td>Redacted B</td><td>Second</td><td>2004</td><td class="num">$185,000,000</td></tr>
    <tr><td>Redacted C</td><td>Fourth</td><td>1962</td><td class="num">$1,140,000,000</td></tr>
  </tbody>
</table>
```

```css
.stewardship-table {
  width: 100%;
  border-collapse: collapse;
  font-family: var(--font-sans);
  font-size: 14px;
  font-variant-numeric: tabular-nums;
  font-feature-settings: "tnum" 1;
}
.stewardship-table th,
.stewardship-table td {
  text-align: left;
  padding: 14px 0;
  border-bottom: 1px solid var(--bronze);
  color: var(--ink);
}
.stewardship-table th {
  font-size: 11px; font-weight: 500; letter-spacing: 0.18em;
  text-transform: uppercase; color: var(--bronze);
}
.stewardship-table td.num,
.stewardship-table th.num { text-align: right; font-family: var(--font-mono); }
```

### Partner-bio module

```html
<article class="partner-bio">
  <div class="partner-portrait" aria-hidden="true"></div>
  <h3 class="partner-name">Jessica Smith-Mason</h3>
  <p class="partner-role">Senior Partner, Stewardship</p>
  <p class="partner-bio-body">Twenty-three years at Heritage, leads the multi-generational practice for families in transition.</p>
  <p class="partner-credentials">JD · LLM (Tax) · TEP</p>
</article>
```

```css
.partner-bio { max-width: 320px; }
.partner-portrait {
  aspect-ratio: 1 / 1;
  background: hsl(220 9% 80%);
  border-radius: 4px;
  margin-bottom: 24px;
}
.partner-name {
  font-family: var(--font-display);
  font-size: 24px; font-weight: 400; line-height: 1.2;
  color: var(--navy);
  margin: 0;
  padding-bottom: 10px;
  border-bottom: 1px solid var(--bronze);
}
.partner-role {
  font-family: var(--font-sans);
  font-size: 13px; font-weight: 500;
  color: var(--text-muted);
  margin: 10px 0 14px 0;
}
.partner-bio-body { font-size: 14px; line-height: 1.6; margin: 0 0 14px 0; }
.partner-credentials {
  font-family: var(--font-mono);
  font-size: 11px; letter-spacing: 0.12em;
  color: var(--bronze);
  text-transform: uppercase;
  margin: 0;
}
```

---

## shadcn/ui integration notes

If the project uses shadcn/ui, override the default theme tokens to map Heritage's palette. The CSS variables shadcn expects (in HSL component form, space-separated, no `hsl()` wrapper):

```css
:root {
  --background: 36 40% 97%;       /* page ivory */
  --foreground: 218 27% 14%;      /* ink navy */

  --card: 0 0% 100%;              /* surface white */
  --card-foreground: 218 27% 14%;

  --popover: 0 0% 100%;
  --popover-foreground: 218 27% 14%;

  --primary: 218 57% 14%;         /* Heritage Navy, used for filled CTA */
  --primary-foreground: 36 40% 97%;

  --secondary: 38 22% 95%;        /* warm cream secondary surface */
  --secondary-foreground: 218 27% 14%;

  --muted: 38 22% 95%;
  --muted-foreground: 220 9% 47%;

  --accent: 214 50% 34%;          /* reserved blue, used for hover/active state */
  --accent-foreground: 44 36% 96%;

  --destructive: 0 60% 32%;
  --destructive-foreground: 44 36% 96%;

  --border: 38 22% 88%;
  --input: 220 9% 75%;
  --ring: 214 50% 34%;            /* reserved-blue focus ring */

  --radius: 0.25rem;              /* 4px rectangles, not pills */
}

.dark {
  --background: 220 44% 11%;      /* contrast dark, used for the hero panel only, not as a full dark mode */
  --foreground: 44 36% 86%;
}
```

After mapping, the default Button variant ships filled with `--primary` (Heritage Navy on ivory text). There is no burgundy variant. There is no red variant. Destructive actions use a typed confirmation modal, not a color.

---

## Do / Don't

### Do

- **Default to the warm ivory ground.** `#FAF7F2` is the page. Cards sit on pure white. Dark panels are insets only.
- **Use the real logo file.** `heritage-logo.webp` ships with the system. Never redraw the seal as inline SVG.
- **Use exactly two display + body fonts.** Display serif + sans. Mono is for fiduciary detail only.
- **Keep all red inside the logo file.** The wax seal in `heritage-logo.webp` is the only red the brand carries. Do not introduce a burgundy CTA, link, badge, or accent.
- **Reserve Reserved Blue for state.** Active, selected, focus, info.
- **Frame the page with 1px bronze hairlines** top and bottom. Heritage's quieter version of JetHQ's gold bar.
- **Tabular figures in any dense data.** Statements, position tables, stewardship counts.
- **Show the partner.** Named, with credentials, real face, available light. Square portrait crops.
- **Use the animated luminous arc once per page,** inside the navy hero panel.
- **Numbers beat adjectives.** $X AUM, Y generations, Z years. Never "premier," "trusted," "world-class."

### Don't

- **Don't make the page background dark.** Fiduciary brands run on light grounds. Dark-only is a casino, not a trustee.
- **Don't introduce red anywhere outside the logo file.** No burgundy buttons, no burgundy links, no burgundy chart series. The wax-seal red lives inside `heritage-logo.webp` and stops there.
- **Don't paint a button burgundy, ever.** Filled navy is the primary CTA. Navy-outlined is the default. Ghost is the tertiary. Three buttons, all navy.
- **Don't redraw the logo.** Use the actual `heritage-logo.webp` file.
- **Don't carry the thick 12px bottom bar from JetHQ.** Heritage is quieter, 1px bronze hairlines only.
- **Don't use stock wealth photography.** Tarmac handshakes, sunset boardrooms, champagne flutes, hands signing in soft focus.
- **Don't write "we believe," "we are passionate about," "premier," "trusted," "world-class," "boutique," or "white-glove."** Show, never claim.
- **Don't use em dashes.** Use commas, periods, or parentheses.
- **Don't animate the AUM.** Static Source Serif 4. The number is supposed to feel old.
- **Don't use any hue between 5° and 45° at saturation >55% and lightness >35%.** That is the warning band. Heritage does not visit the warning band.
- **Don't use vendor Tailwind colors** (`bg-amber-50`, `text-rose-600`). They will not match the calibrated palette.
- **Don't use pills for buttons.** Buttons are 4px-radius rectangles. Pills are reserved for status indicators and avatars.
- **Don't add a third font, glassmorphism, animated counters, autoplay video, urgency banners, exit-intent overlays, or chatbots.** Every one reads as salesy.

---

## Common mistakes to avoid

1. **The warning-band trap.** Any hex with HSL hue between 5° and 45° at saturation >55% and lightness >35% reads as "alert" on a wealth-management surface. A wax-oxblood-style accent in this band reads as a fintech alert. High-net-worth families assigning all their assets to the firm cannot have any element reading as "warning." Heritage stays out of the band entirely.
2. **Defaulting to the dark ground.** Heritage is light by default. Every peer in the prestige wealth set (Bessemer, Pictet, BBH, Lombard Odier, Northern Trust, Rothschild & Co, JPMorgan Private Bank) runs a white or warm-off-white page. A dark-only Heritage surface reads as a hedge-fund poster.
3. **Leaking the seal red into the UI.** A burgundy button or burgundy link feels harmonious with the logo at first glance, but a fiduciary brand cannot afford a red CTA. The wax-seal red is contained inside the logo file. Use filled navy or outlined navy.
4. **Redrawing the logo as inline SVG.** The real `heritage-logo.webp` is the source of truth. Reconstructions never match the wax-seal interior typography or the bronze metallic, and they will diverge from the file Sven hands the client.
5. **Hero scale on the seal.** The seal is a detail element, 24–48px. Hero-scale seals read as a corporate-seal stamp from a 1990s annual report cover, not a contemporary stewardship brand.
6. **Em dashes in body copy.** Sven has flagged this directly. Use commas, periods, or parentheses.
7. **Counter animations on AUM.** A wealth firm's AUM is not a startup's MRR. Set the number in static Source Serif 4. The number is supposed to feel old.
8. **Stock wealth imagery.** A glossy tarmac handshake or champagne-flute boardroom will instantly drag the brand back into the category it works to escape.
9. **A thick 12px bottom bar.** Heritage is quieter than JetHQ. 1px bronze hairlines only.
10. **A third font.** Display serif + sans + mono is the entire system. A "modern" display font for the hero and a separate sans for the nav is a redesign, not a Heritage surface.

---

## Worked example, Heritage hero section (full-bleed navy panel with animated arc)

```html
<div class="page-shell">

  <nav class="nav" aria-label="Heritage Strategies brand navigation">
    <a class="lockup" href="/" aria-label="Heritage Strategies LLC home">
      <img src="./heritage-logo.webp" alt="Heritage Strategies LLC" height="40" width="auto">
    </a>
    <ul class="nav-links">
      <li><a href="#mark">Mark</a></li>
      <li><a href="#typography">Type</a></li>
      <li><a href="#color">Color</a></li>
      <li><a href="#components">Components</a></li>
    </ul>
  </nav>
  <div class="hairline-bronze" role="presentation"></div>

  <section class="hero" aria-labelledby="hero-title">

    <div class="hero-arc" aria-hidden="true">
      <svg viewBox="0 0 1440 600" preserveAspectRatio="xMidYMid slice" role="presentation">
        <defs>
          <linearGradient id="arcGrad" x1="0" y1="0" x2="1" y2="0">
            <stop offset="0%"   stop-color="#F5EFE2" stop-opacity="0"/>
            <stop offset="50%"  stop-color="#F5EFE2" stop-opacity="1"/>
            <stop offset="100%" stop-color="#C9B98A" stop-opacity="0"/>
          </linearGradient>
          <filter id="arcGlow" x="-20%" y="-20%" width="140%" height="140%">
            <feGaussianBlur stdDeviation="4" result="blur"/>
            <feMerge>
              <feMergeNode in="blur"/>
              <feMergeNode in="SourceGraphic"/>
            </feMerge>
          </filter>
        </defs>
        <path
          class="arc"
          d="M -80 460 Q 360 120 720 240 T 1520 180"
          fill="none"
          stroke="url(#arcGrad)"
          stroke-width="1.25"
          stroke-linecap="round"
          filter="url(#arcGlow)"
          pathLength="1"
        />
      </svg>
    </div>

    <div class="hero-inner">
      <p class="hero-eyebrow">STEWARDSHIP, NOT TRANSACTION</p>
      <h1 class="hero-title" id="hero-title">Three generations of stewardship.</h1>
      <p class="hero-lede">
        Heritage Strategies steward what families have built, across decades, structures, and successors.
        A single named partner. Foreman, the firm's AI Employee, on every artifact.
      </p>
      <div class="hero-actions">
        <a class="btn btn-primary" href="/contact">Request a Stewardship Conversation</a>
        <a class="btn btn-on-dark" href="/about">Speak with a Partner</a>
      </div>
      <p class="trust-bar">
        <span>Founded 1987</span>
        <span>Family stewardship since 1962</span>
        <span>$2.4B under stewardship</span>
        <span>PA chartered trust company · SEC RIA</span>
      </p>
    </div>

  </section>

</div>
```

```css
.page-shell {
  background: var(--page-bg);
  color: var(--ink);
  font-family: var(--font-sans);
  font-size: 16px;
  font-weight: 400;
  line-height: 1.6;
  min-height: 100vh;
  display: flex;
  flex-direction: column;
}

.hero {
  position: relative;
  background: var(--contrast-dark);
  color: var(--text-on-dark);
  padding: clamp(96px, 14vw, 192px) clamp(20px, 4vw, 48px);
  overflow: hidden;
}
.hero-inner {
  position: relative; z-index: 1;
  max-width: 880px;
  margin: 0 auto;
}

.hero-eyebrow {
  font-family: var(--font-sans);
  font-size: 12px; font-weight: 500;
  letter-spacing: 0.22em; text-transform: uppercase;
  color: hsl(35 26% 60%); /* bronze lifted on dark */
  margin: 0 0 32px 0;
}
.hero-title {
  font-family: var(--font-display);
  font-variation-settings: "opsz" 144;
  font-size: clamp(48px, 7vw, 88px);
  font-weight: 400; line-height: 1.05;
  color: var(--text-on-dark);
  margin: 0 0 24px 0;
}
.hero-lede {
  font-family: var(--font-sans);
  font-size: clamp(17px, 1.4vw, 20px);
  font-weight: 400; line-height: 1.55;
  color: var(--text-on-dark);
  max-width: 640px;
  margin: 0 0 40px 0;
}
.hero-actions { display: flex; gap: 14px; flex-wrap: wrap; margin-bottom: 48px; }

.btn-on-dark {
  display: inline-flex; align-items: center; justify-content: center;
  padding: 14px 24px;
  background: transparent;
  color: var(--text-on-dark);
  border: 1px solid hsl(35 26% 60%);
  border-radius: 4px;
  font-family: var(--font-sans);
  font-weight: 500; font-size: 13px; letter-spacing: 0.14em;
  text-transform: uppercase; text-decoration: none;
  transition: background-color 200ms ease-out;
}
.btn-on-dark:hover { background: hsl(35 26% 60% / 0.14); }

.trust-bar {
  font-family: var(--font-sans);
  font-size: 12px; font-weight: 500; letter-spacing: 0.06em;
  color: var(--text-on-dark-muted);
  margin: 0;
}
.trust-bar span + span::before {
  content: "·"; margin: 0 0.75em; color: var(--text-on-dark-muted);
}

*:focus-visible {
  outline: 2px solid var(--reserved-blue);
  outline-offset: 2px;
}
```

---

## One-line summary

Warm ivory ground, deep navy as the single dark, aged-bronze hairlines top and bottom, Source Serif 4 display serif, Inter sans, one animated luminous arc inside the splash-mode dark panel, the real wax-seal logo file as the only red the brand carries. Numbers beat adjectives. Show, never claim. No warning hues, no red anywhere outside the logo file, ever.
