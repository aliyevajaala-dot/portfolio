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

| Token | Hex |
|---|---|
| navy-50 | #F1F1F8 |
| navy-100 | #E1E0F0 |
| navy-200 | #C2C0E2 |
| navy-300 | #9895C8 |
| navy-400 | #6F6AA8 |
| navy-500 | #4A4488 |
| navy-600 | #322C6E |
| navy-700 | #262159 |
| navy-800 | #1C1845 |
| navy-900 | #131032 |

**Green (Accent — from logo dot)**

| Token | Hex |
|---|---|
| green-50 | #ECFDF3 |
| green-100 | #D1FADF |
| green-200 | #A6F4C5 |
| green-300 | #6CE9A6 |
| green-400 | #32D583 |
| green-500 | #12B76A |
| green-600 | #039855 |
| green-700 | #027A48 |
| green-800 | #05603A |
| green-900 | #054F31 |

**Gray (Neutral — UI structure, text)**

| Token | Hex |
|---|---|
| gray-50 | #FAFAFB |
| gray-100 | #F2F2F5 |
| gray-200 | #E4E4E9 |
| gray-300 | #CFD0D6 |
| gray-400 | #9FA1AC |
| gray-500 | #71737E |
| gray-600 | #52545F |
| gray-700 | #3B3D47 |
| gray-800 | #24252C |
| gray-900 | #141419 |

**Red (Error / destructive)**

| Token | Hex |
|---|---|
| red-50 | #FEF3F2 |
| red-100 | #FEE4E2 |
| red-200 | #FECDCA |
| red-300 | #FDA29B |
| red-400 | #F97066 |
| red-500 | #F04438 |
| red-600 | #D92D20 |
| red-700 | #B42318 |
| red-800 | #912018 |
| red-900 | #7A271A |

**Amber (Warning)**

| Token | Hex |
|---|---|
| amber-50 | #FFFAEB |
| amber-100 | #FEF0C7 |
| amber-200 | #FEDF89 |
| amber-300 | #FEC84B |
| amber-400 | #FDB022 |
| amber-500 | #F79009 |
| amber-600 | #DC6803 |
| amber-700 | #B54708 |
| amber-800 | #93370D |
| amber-900 | #7A2E0E |

### 2.2 Semantic Tokens

Each row: **Light mode value → Dark mode value**

**Background**

| Token | Light | Dark |
|---|---|---|
| bg-primary | gray-50 (#FAFAFB) | gray-900 (#141419) |
| bg-secondary | white (#FFFFFF) | gray-800 (#24252C) |
| bg-tertiary | gray-100 (#F2F2F5) | gray-700 (#3B3D47) |
| bg-elevated (cards, modals) | white (#FFFFFF) | gray-800 (#24252C) |
| bg-inverse | navy-900 (#131032) | gray-50 (#FAFAFB) |

**Text**

| Token | Light | Dark |
|---|---|---|
| text-primary | navy-900 (#131032) | gray-50 (#FAFAFB) |
| text-secondary | gray-600 (#52545F) | gray-300 (#CFD0D6) |
| text-tertiary | gray-500 (#71737E) | gray-400 (#9FA1AC) |
| text-disabled | gray-300 (#CFD0D6) | gray-600 (#52545F) |
| text-inverse | white (#FFFFFF) | navy-900 (#131032) |
| text-link | navy-600 (#322C6E) | navy-300 (#9895C8) |

**Border**

| Token | Light | Dark |
|---|---|---|
| border-default | gray-200 (#E4E4E9) | gray-700 (#3B3D47) |
| border-subtle | gray-100 (#F2F2F5) | gray-800 (#24252C) |
| border-strong | gray-400 (#9FA1AC) | gray-500 (#71737E) |
| border-focus | navy-500 (#4A4488) | navy-300 (#9895C8) |

**Interactive**

| Token | Light | Dark |
|---|---|---|
| interactive-primary | navy-700 (#262159) | navy-300 (#9895C8) |
| interactive-primary-hover | navy-800 (#1C1845) | navy-200 (#C2C0E2) |
| interactive-primary-active | navy-900 (#131032) | navy-100 (#E1E0F0) |
| interactive-secondary | gray-100 (#F2F2F5) | gray-700 (#3B3D47) |
| interactive-accent | green-500 (#12B76A) | green-400 (#32D583) |
| interactive-disabled | gray-200 (#E4E4E9) | gray-700 (#3B3D47) |

**Feedback**

| Token | Light | Dark |
|---|---|---|
| feedback-success | green-600 (#039855) | green-400 (#32D583) |
| feedback-success-bg | green-50 (#ECFDF3) | green-900 (#054F31) |
| feedback-warning | amber-600 (#DC6803) | amber-400 (#FDB022) |
| feedback-warning-bg | amber-50 (#FFFAEB) | amber-900 (#7A2E0E) |
| feedback-error | red-600 (#D92D20) | red-400 (#F97066) |
| feedback-error-bg | red-50 (#FEF3F2) | red-900 (#7A271A) |
| feedback-info | navy-500 (#4A4488) | navy-300 (#9895C8) |
| feedback-info-bg | navy-50 (#F1F1F8) | navy-800 (#1C1845) |

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

| Token | Value |
|---|---|
| space-0 | 0px |
| space-1 | 4px |
| space-2 | 8px |
| space-3 | 12px |
| space-4 | 16px |
| space-5 | 20px |
| space-6 | 24px |
| space-8 | 32px |
| space-10 | 40px |
| space-12 | 48px |
| space-16 | 64px |
| space-20 | 80px |
| space-24 | 96px |

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
