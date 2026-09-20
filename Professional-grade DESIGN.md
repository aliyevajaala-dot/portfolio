# Zenith Academy — Design System

> Single source of truth for visual and interaction design across the Zenith Academy web app.
> Every UI decision (color, spacing, type, motion) should trace back to a token defined here.

---

## 1. Brand Overview

**Mission (one sentence):**
Zenith Academy makes high-quality, self-paced learning feel calm, credible, and achievable — never overwhelming.

**Design Principles**

1. **Calm over loud.** No visual noise competes with the learning content. Color, motion, and shadow are used sparingly and with intent.
2. **Clarity is respect.** Every label, state, and piece of feedback is unambiguous. If a user has to guess, we've failed.
3. **Premium through restraint.** Premium doesn't mean decorative — it means generous whitespace, precise alignment, and consistent rhythm.
4. **Progress should feel visible.** Course progress, completion, and achievement states are always legible at a glance.

**Voice and Tone**

| Do | Don't |
|---|---|
| Speak plainly: "Continue where you left off" | Don't use hype language: "Crush your goals!" |
| Encourage without pressuring: "You're 80% through this module" | Don't guilt-trip: "You're falling behind!" |
| Use precise, calm error copy: "That email is already registered" | Don't use jokey error copy: "Oops! Something broke lol" |
| Address the learner directly ("you", "your course") | Don't use corporate third-person ("users may access...") |

---

## 2. Colors

### 2.1 Primitive Palette

**Navy (Primary — brand identity, from logo wordmark)**

| Token | Hex | Usage |
|---|---|---|
| navy-50 | #F1F1F8 | Subtle brand-tinted background (selected nav item, info banner bg) |
| navy-100 | #E1E0F0 | Hover background for brand-tinted surfaces (e.g. selected list row hover) |
| navy-200 | #C2C0E2 | Focus ring color; light borders on brand-colored elements |
| navy-300 | #9895C8 | Dark-mode secondary links; disabled brand-colored icons |
| navy-400 | #6F6AA8 | Mid-tone accents; chart/data-viz series color |
| navy-500 | #4A4488 | Dark-mode focus border/ring; dark-mode "interactive-accent" fallback |
| navy-600 | #322C6E | Inline text links (light mode); secondary interactive elements |
| navy-700 | #262159 | Primary button background; active nav item; primary text links |
| navy-800 | #1C1845 | Primary button hover background; strong heading emphasis |
| navy-900 | #131032 | Primary text color (light mode); button active/pressed state; dark inverse background |

**Green (Accent — from logo dot)**

| Token | Hex | Usage |
|---|---|---|
| green-50 | #ECFDF3 | Success message/toast background (light mode) |
| green-100 | #D1FADF | Light success badge background (e.g. "Completed" tag) |
| green-200 | #A6F4C5 | Success badge border |
| green-300 | #6CE9A6 | Success icon color on dark backgrounds |
| green-400 | #32D583 | Success state in dark mode (icons, text, "interactive-accent" dark value) |
| green-500 | #12B76A | Accent interactive elements; progress bar fill; completion checkmark |
| green-600 | #039855 | Success text (light mode); "Completed" lesson label |
| green-700 | #027A48 | Success text hover/emphasis state |
| green-800 | #05603A | Success surface background (dark mode cards) |
| green-900 | #054F31 | Success message/toast background (dark mode) |

**Gray (Neutral — UI structure, text)**

| Token | Hex | Usage |
|---|---|---|
| gray-50 | #FAFAFB | Page background (light mode) |
| gray-100 | #F2F2F5 | Secondary/tertiary background; hover background for list rows |
| gray-200 | #E4E4E9 | Default border color; dividers between sections |
| gray-300 | #CFD0D6 | Disabled text/icons; placeholder text; strong dividers |
| gray-400 | #9FA1AC | Tertiary/meta text; disabled icon color |
| gray-500 | #71737E | Secondary body text; timestamps, meta labels |
| gray-600 | #52545F | Default icon color; secondary text emphasis |
| gray-700 | #3B3D47 | Dark-mode default borders; dark-mode tertiary background |
| gray-800 | #24252C | Dark-mode card/elevated surface background |
| gray-900 | #141419 | Dark-mode page background |

**Red (Error / destructive)**

| Token | Hex | Usage |
|---|---|---|
| red-50 | #FEF3F2 | Error message/toast background (light mode) |
| red-100 | #FEE4E2 | Light error badge background |
| red-200 | #FECDCA | Error badge/input border |
| red-300 | #FDA29B | Error icon color on dark backgrounds |
| red-400 | #F97066 | Error state in dark mode (icons, text, border) |
| red-500 | #F04438 | Default error icon color; destructive hover accent |
| red-600 | #D92D20 | Error text/border (light mode); danger button background |
| red-700 | #B42318 | Danger button hover background |
| red-800 | #912018 | Danger button active/pressed background |
| red-900 | #7A271A | Error message/toast background (dark mode) |

**Amber (Warning)**

| Token | Hex | Usage |
|---|---|---|
| amber-50 | #FFFAEB | Warning message/banner background (light mode) |
| amber-100 | #FEF0C7 | Light warning badge background |
| amber-200 | #FEDF89 | Warning badge/border |
| amber-300 | #FEC84B | Warning icon color on dark backgrounds |
| amber-400 | #FDB022 | Warning state in dark mode (icons, text) |
| amber-500 | #F79009 | Default warning icon color |
| amber-600 | #DC6803 | Warning text/border (light mode); "unsaved changes" indicator |
| amber-700 | #B54708 | Warning text hover/emphasis |
| amber-800 | #93370D | Warning surface background (dark mode cards) |
| amber-900 | #7A2E0E | Warning message/banner background (dark mode) |

### 2.2 Semantic Tokens

Each row: **Light mode value → Dark mode value**

**Background**

| Token | Light | Dark | Usage |
|---|---|---|---|
| bg-primary | gray-50 (#FAFAFB) | gray-900 (#141419) | Base page/app background, behind all content |
| bg-secondary | white (#FFFFFF) | gray-800 (#24252C) | Sidebar, header bar, panel backgrounds sitting above bg-primary |
| bg-tertiary | gray-100 (#F2F2F5) | gray-700 (#3B3D47) | Subtle section fills, table row stripes, input field backgrounds |
| bg-elevated (cards, modals) | white (#FFFFFF) | gray-800 (#24252C) | Cards, modals, dropdowns, popovers — any surface with a shadow |
| bg-inverse | navy-900 (#131032) | gray-50 (#FAFAFB) | Tooltips, code blocks, dark promotional banners on a light page |

**Text**

| Token | Light | Dark | Usage |
|---|---|---|---|
| text-primary | navy-900 (#131032) | gray-50 (#FAFAFB) | Headings, primary body copy, primary form labels |
| text-secondary | gray-600 (#52545F) | gray-300 (#CFD0D6) | Descriptions, supporting copy under headings |
| text-tertiary | gray-500 (#71737E) | gray-400 (#9FA1AC) | Meta info, timestamps, helper hints |
| text-disabled | gray-300 (#CFD0D6) | gray-600 (#52545F) | Disabled form labels, inactive nav/menu items |
| text-inverse | white (#FFFFFF) | navy-900 (#131032) | Text on dark or brand-colored backgrounds (e.g. inside primary buttons) |
| text-link | navy-600 (#322C6E) | navy-300 (#9895C8) | Inline hyperlinks, "Learn more" / "View details" links |

**Border**

| Token | Light | Dark | Usage |
|---|---|---|---|
| border-default | gray-200 (#E4E4E9) | gray-700 (#3B3D47) | Card borders, input borders, standard dividers |
| border-subtle | gray-100 (#F2F2F5) | gray-800 (#24252C) | Faint internal separators (e.g. between list items in a card) |
| border-strong | gray-400 (#9FA1AC) | gray-500 (#71737E) | Hover state on inputs/cards; emphasized dividers |
| border-focus | navy-500 (#4A4488) | navy-300 (#9895C8) | Focus ring/outline for keyboard accessibility |

**Interactive**

| Token | Light | Dark | Usage |
|---|---|---|---|
| interactive-primary | navy-700 (#262159) | navy-300 (#9895C8) | Primary button background, primary CTA |
| interactive-primary-hover | navy-800 (#1C1845) | navy-200 (#C2C0E2) | Primary button hover state |
| interactive-primary-active | navy-900 (#131032) | navy-100 (#E1E0F0) | Primary button pressed/active state |
| interactive-secondary | gray-100 (#F2F2F5) | gray-700 (#3B3D47) | Secondary button background |
| interactive-accent | green-500 (#12B76A) | green-400 (#32D583) | Progress bar fill, completion checkmarks, accent CTAs |
| interactive-disabled | gray-200 (#E4E4E9) | gray-700 (#3B3D47) | Background for disabled buttons and controls |

**Feedback**

| Token | Light | Dark | Usage |
|---|---|---|---|
| feedback-success | green-600 (#039855) | green-400 (#32D583) | Success text/icon color (e.g. "Lesson completed") |
| feedback-success-bg | green-50 (#ECFDF3) | green-900 (#054F31) | Success toast/banner background |
| feedback-warning | amber-600 (#DC6803) | amber-400 (#FDB022) | Warning text/icon color (e.g. "Unsaved changes") |
| feedback-warning-bg | amber-50 (#FFFAEB) | amber-900 (#7A2E0E) | Warning banner background |
| feedback-error | red-600 (#D92D20) | red-400 (#F97066) | Error text/icon color, form validation messages |
| feedback-error-bg | red-50 (#FEF3F2) | red-900 (#7A271A) | Error toast/banner background |
| feedback-info | navy-500 (#4A4488) | navy-300 (#9895C8) | Informational text/icon color (e.g. tips, hints) |
| feedback-info-bg | navy-50 (#F1F1F8) | navy-800 (#1C1845) | Informational banner background |

### 2.3 Accessibility Matrix (Contrast Ratios)

Contrast ratios below are calculated using the WCAG 2.1 relative luminance formula: `L = 0.2126R + 0.7152G + 0.0722B` (linearized channels), `ratio = (L_lighter + 0.05) / (L_darker + 0.05)`. Required minimums: **AA normal text = 4.5:1**, **AA large text (≥18pt or ≥14pt bold) = 3:1**.

Token name mapping used below: `text-on-interactive` = `text-inverse`, `interactive-bg` = `interactive-primary`, `bg-surface` = `bg-elevated`.

| Pair | Mode | Foreground | Background | Ratio | Required | Result |
|---|---|---|---|---|---|---|
| text-primary / bg-primary | Light | navy-900 `#131032` | gray-50 `#FAFAFB` | **17.5:1** | AA normal 4.5:1 | ✅ Passed |
| text-primary / bg-primary | Dark | gray-50 `#FAFAFB` | gray-900 `#141419` | **17.6:1** | AA normal 4.5:1 | ✅ Passed |
| text-secondary / bg-primary | Light | gray-600 `#52545F` | gray-50 `#FAFAFB` | **7.2:1** | AA normal 4.5:1 | ✅ Passed |
| text-secondary / bg-primary | Dark | gray-300 `#CFD0D6` | gray-900 `#141419` | **11.9:1** | AA normal 4.5:1 | ✅ Passed |
| text-on-interactive / interactive-bg | Light | white `#FFFFFF` | navy-700 `#262159` | **14.5:1** | AA normal 4.5:1 | ✅ Passed |
| text-on-interactive / interactive-bg | Dark | navy-900 `#131032` | navy-300 `#9895C8` | **6.5:1** | AA normal 4.5:1 | ✅ Passed |
| text-primary / bg-surface | Light | navy-900 `#131032` | white `#FFFFFF` | **18.3:1** | AA normal 4.5:1 | ✅ Passed |
| text-primary / bg-surface | Dark | gray-50 `#FAFAFB` | gray-800 `#24252C` | **14.6:1** | AA normal 4.5:1 | ✅ Passed |

**Notes:**

- All 8 pairs pass AA for normal text. No token value changes were required — the palette was built with WCAG margins in mind from the start (primary-vs-background pairs sit well above 10:1, giving headroom even if a future theme adjustment shifts a shade slightly).
- The tightest pair is `text-on-interactive / interactive-bg` in **Dark mode** (6.5:1) — the dark-mode primary button (`navy-300` background) is a light tint, so it needs a dark foreground (`navy-900`) rather than white. If this button's background token is ever swapped to a lighter/higher-lightness value, re-run this check — that pair has the smallest safety margin of the eight.
- `text-secondary / bg-primary` in Light mode (7.2:1) also has less margin than the others; if `gray-600` were lightened for any reason, it must not drop below `4.5:1`.
- Any *new* semantic pair introduced later (e.g. a token added for tags, badges, or charts) must be added to this table and calculated before shipping — this matrix is the accessibility gate for the whole system, not a one-time check.

### 2.4 Theming Anchor

**`navy-700` (#262159) is the single brand anchor primitive:** every semantic token that carries brand identity (`interactive-primary`, `interactive-primary-hover`, `interactive-primary-active`, `text-link`, `border-focus`, `feedback-info`, `bg-inverse`) is a reference into the Navy scale, not a hardcoded hex — so regenerating the Navy 50–900 scale from a new base hue at `navy-700` alone re-themes every button, link, focus ring, and inverse surface across both Light and Dark mode with zero other token edits.

---

## 3. Typography

**Font families**

- **Heading font:** `Manrope` (semi-geometric sans, gives premium/editorial weight to headings) — fallback: `-apple-system, "Segoe UI", sans-serif`
- **Body/UI font:** `Inter` (neutral, highly legible at small sizes) — fallback: `-apple-system, "Segoe UI", sans-serif`
- **Mono (code snippets in course content):** `"JetBrains Mono", ui-monospace, monospace`

**Type Scale**

| Token | Size | Line-height | Weight | Usage |
|---|---|---|---|---|
| display-lg | 56px | 64px | 700 (Bold) | Marketing/landing hero only |
| display-sm | 40px | 48px | 700 (Bold) | Section hero headers |
| h1 | 32px | 40px | 700 (Bold) | Page title (e.g. Course title) |
| h2 | 26px | 34px | 600 (SemiBold) | Section headers (e.g. "Modules") |
| h3 | 22px | 30px | 600 (SemiBold) | Card/module titles |
| h4 | 18px | 26px | 600 (SemiBold) | Sub-section, list group headers |
| body-lg | 17px | 26px | 400 (Regular) | Lesson/article body text |
| body-md | 15px | 22px | 400 (Regular) | Default UI text, descriptions |
| body-sm | 13px | 18px | 400 (Regular) | Secondary/meta text, timestamps |
| caption | 12px | 16px | 500 (Medium) | Labels, badges, form hints |
| overline | 11px | 14px | 600 (SemiBold), uppercase, +0.06em tracking | Category tags, eyebrow text |

**Heading Rules**

- Only one `h1` per page.
- Headings always use the Heading font (Manrope); never mix body font into headings.
- Heading color is always `text-primary`; never use `text-secondary` for headings.
- Do not skip heading levels for styling purposes (e.g. don't use h3 styling under an h1 just because it "looks right") — use the scale token that matches actual hierarchy.

---

## 4. Spacing

**Base unit: 4px**

| Token | Value | Usage |
|---|---|---|
| space-0 | 0px | Reset margin/padding; touching/adjacent elements with no gap |
| space-1 | 4px | Icon-to-label gap; tight inline spacing (e.g. badge internal padding) |
| space-2 | 8px | Gap between a label and its input; spacing inside compact buttons |
| space-3 | 12px | Gap between stacked form fields; icon padding inside buttons |
| space-4 | 16px | Default gap between related UI elements; compact card padding |
| space-5 | 20px | Gap between list items (e.g. lesson list rows) |
| space-6 | 24px | Card default internal padding; grid gap between cards |
| space-8 | 32px | Gap between sub-sections within a page |
| space-10 | 40px | Page padding on tablet; gap between major form groups |
| space-12 | 48px | Gap between distinct page blocks (e.g. hero and content) |
| space-16 | 64px | Page padding on desktop; gap between major page sections |
| space-20 | 80px | Large vertical spacing on marketing/landing sections |
| space-24 | 96px | Hero section spacing; largest vertical rhythm on landing pages |

**Layout Rules**

- **Page padding:** `space-6` (24px) on mobile, `space-10` (40px) on tablet+, `space-16` (64px) on desktop (≥1280px).
- **Section padding (vertical):** `space-16` (64px) between major page sections; `space-8` (32px) between sub-sections.
- **Card internal padding:** `space-6` (24px) default, `space-4` (16px) for compact/dense cards (e.g. sidebar lesson list items).
- **Grid gap:** `space-6` (24px) for card grids (course catalog); `space-4` (16px) for tightly related items (form fields, button groups).
- **Stack spacing (vertical rhythm between text elements):** `space-2` between label and input, `space-4` between paragraphs, `space-3` between a heading and its immediate body text.

---

## 5. Border Radius

| Token | Value | Usage |
|---|---|---|
| radius-none | 0px | Full-bleed images, dividers |
| radius-sm | 6px | Badges, tags, small chips |
| radius-md | 10px | Inputs, buttons, small cards |
| radius-lg | 16px | Cards, modals, panels |
| radius-xl | 24px | Hero banners, large feature cards |
| radius-full | 9999px | Avatars, pill buttons, progress dots |

---

## 6. Shadows

Shadows are kept subtle and cool-toned (navy-tinted, not pure black) to preserve the "calm/premium" feel.

| Token | Value | Usage |
|---|---|---|
| shadow-xs | `0 1px 2px rgba(19, 16, 50, 0.04)` | Input default state, subtle separation |
| shadow-sm | `0 2px 4px rgba(19, 16, 50, 0.06)` | Buttons, list items on hover |
| shadow-md | `0 4px 12px rgba(19, 16, 50, 0.08)` | Cards at rest (course cards) |
| shadow-lg | `0 8px 24px rgba(19, 16, 50, 0.12)` | Dropdowns, popovers, hover-elevated cards |
| shadow-xl | `0 16px 48px rgba(19, 16, 50, 0.16)` | Modals, dialogs |

Dark mode: reduce opacity by ~half and increase blur radius slightly (dark backgrounds need less contrast to read as "elevated").

---

## 7. Breakpoints

| Token | Min-width | Target device |
|---|---|---|
| sm | 640px | Large phones (landscape) |
| md | 768px | Tablets (portrait) |
| lg | 1024px | Tablets (landscape) / small laptops |
| xl | 1280px | Standard laptop/desktop |
| 2xl | 1536px | Large desktop monitors |

Design mobile-first: base styles target < 640px, then progressively enhance upward.

---

## 8. Components

### 8.1 Button

**Variants:** `primary` · `secondary` · `ghost` · `danger`
**Sizes:** `sm` (32px height) · `md` (40px height) · `lg` (48px height)

| State | Primary | Secondary | Ghost |
|---|---|---|---|
| Default | bg `interactive-primary`, text white, `radius-md` | bg `interactive-secondary`, text `text-primary`, border `border-default` | bg transparent, text `text-primary` |
| Hover | bg `interactive-primary-hover` | bg `gray-200`, border `border-strong` | bg `bg-tertiary` |
| Active | bg `interactive-primary-active` | bg `gray-300` | bg `gray-100` |
| Focus | `shadow: 0 0 0 3px navy-200`, visible outline (never remove `:focus-visible`) | same focus ring pattern | same focus ring pattern |
| Disabled | bg `interactive-disabled`, text `text-disabled`, no pointer events | opacity 50%, no pointer events | opacity 40%, no pointer events |
| Loading | spinner replaces label, button width stays fixed (no layout shift), disabled interactions | same pattern | same pattern |

**Rules:** Primary button appears once per view/section (never two primary buttons competing). Danger variant (red-600 bg) reserved exclusively for destructive actions (delete course, cancel subscription) and always paired with a confirmation step.

### 8.2 Card

**Variants:** `default` (flat, bordered) · `elevated` (shadow, no border) · `outlined` (border only, no shadow)
**Sizes:** follows content — no fixed size tokens, but internal padding uses `space-6` default / `space-4` compact

| State | Behavior |
|---|---|
| Default | `bg-elevated`, `border-default` (default variant only), `radius-lg` |
| Hover (if clickable) | `shadow-md` → `shadow-lg`, subtle `translateY(-2px)` |
| Active (if clickable) | `translateY(0)`, `shadow-sm` |
| Focus (if clickable, keyboard nav) | `border-focus` ring, 2px offset |
| Disabled (e.g. locked course) | opacity 60%, `bg-tertiary` overlay, lock icon shown, no hover elevation |
| Loading (skeleton) | animated gray-200/gray-300 shimmer placeholder matching card's real layout |

**Rules:** A card is only interactive (hover/active states) if the whole card is clickable. If only a button inside the card is clickable, the card itself must not show hover elevation.

### 8.3 Input

**Variants:** `text` · `textarea` · `select`
**Sizes:** `sm` (32px) · `md` (40px, default) · `lg` (48px)

| State | Style |
|---|---|
| Default | `border-default`, `bg-secondary`, `radius-md`, `text-primary` |
| Hover | `border-strong` |
| Focus | `border-focus`, `shadow: 0 0 0 3px navy-100` |
| Filled | same as default, value in `text-primary` (vs. placeholder in `text-tertiary`) |
| Disabled | `bg-tertiary`, `text-disabled`, cursor not-allowed |
| Error | `border: feedback-error`, helper text below in `feedback-error`, error icon in field |
| Success (e.g. validated field) | `border: feedback-success`, checkmark icon in field |

**Rules:** Every input has a visible label (no placeholder-only labels — fails accessibility). Error message always explains *what to do*, not just *what's wrong* ("Password needs at least 8 characters" not "Invalid password").

---

## 9. Animation

**Timing Tokens**

| Token | Duration | Usage |
|---|---|---|
| duration-instant | 100ms | Micro-feedback (checkbox tick, button press) |
| duration-fast | 150ms | Hover states, small UI transitions |
| duration-base | 250ms | Default transitions (modals opening, dropdowns) |
| duration-slow | 400ms | Page-level transitions, large panel slides |

**Easing**

| Token | Curve | Usage |
|---|---|---|
| ease-standard | `cubic-bezier(0.4, 0, 0.2, 1)` | Default for most transitions |
| ease-out | `cubic-bezier(0, 0, 0.2, 1)` | Elements entering the screen |
| ease-in | `cubic-bezier(0.4, 0, 1, 1)` | Elements leaving the screen |

**Rules**

- Motion is used to clarify, not decorate: transitions communicate state change (e.g. a card lifting on hover confirms it's clickable), never purely ornamental.
- No bouncing/spring easing — conflicts with the calm/premium brand feel.
- **Reduced motion:** Respect `prefers-reduced-motion: reduce` — disable transform-based animations (slides, scales, parallax) and replace with instant or opacity-only transitions (max 100ms fade). Progress indicators (e.g. course completion bars) may still animate functionally but should skip decorative easing.

---

## 10. Iconography

- **Style:** Outline icons only (not filled/solid), consistent 1.5px stroke weight, rounded line caps — matches the calm, precise brand tone. Recommended source: Phosphor Icons or Lucide (regular weight).
- **Sizes:** 16px (inline with body-sm text), 20px (inline with body-md, default UI icon size), 24px (standalone action icons, nav icons), 32px (feature/empty-state illustrations use up to this size before switching to full illustrations).
- **Touch target:** Minimum 44×44px tappable area around any icon-only interactive element, even if the icon itself renders at 20–24px — the extra space is padding, not visible icon size.
- **Color:** Icons inherit `text-secondary` by default; active/selected state icons use `interactive-primary` or `interactive-accent` (green) only when indicating success/completion.

---

## 11. Grid and Layout

- **Columns:** 12-column grid on `lg` and above; collapses to 4-column grid on mobile (`< 640px`).
- **Gutter:** `space-6` (24px) between columns on desktop; `space-4` (16px) on mobile.
- **Margin (container edge to viewport edge):** matches page padding — `space-6` mobile, `space-10` tablet, `space-16` desktop.
- **Max container width:** `1280px`, centered, with fluid padding beyond that on ultra-wide screens.
- **Course catalog grid:** 3 cards per row at `lg`, 2 at `md`, 1 at base/mobile.
- **Lesson/reading layout:** content column capped at `680px` max-width for optimal reading line-length, regardless of viewport size.
