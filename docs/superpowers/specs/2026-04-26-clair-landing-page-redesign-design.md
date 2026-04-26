# Clair landing page redesign — design spec

**Date:** 2026-04-26
**Scope:** Recreate the pre-launch landing page at getclairapp.com (`index.html`), and bring `privacy.html` + `terms.html` into the new look.
**Driver:** Conversion overhaul. Email-only ask must feel exclusive/urgent through copy + design alone (no testimonials, no fake user counts, no incentives we can't deliver). Mixed audience: quiet thinkers, founders, therapy-curious, iOS early adopters. Personality direction: Sharp & Insightful (Linear / Notion / Granola).

## 1. Page architecture

Approach: **A — Manifesto-pivot.** Seven blocks, top to bottom:

1. **Nav** — sticky, frosted on scroll. Wordmark left, single CTA right (`Get notified` → scrolls to closing form). No `How It Works` or `Features` links.
2. **Hero** — type-led, email form above the fold, ambient pulsing waveform underneath. No phone mockup, no hero card grid.
3. **Manifesto** — full-viewport-height typographic statement on white. The page's identity moment.
4. **Sample reads** — three poetry-formatted "what Clair sounds like" blocks on a soft (`#FAFAFA`) background. New section. The most powerful proof on the page because it shows what Clair says, not what it looks like.
5. **Three-up screenshots** — `01 Talk · 02 Read · 03 Ask` with terse labels and short copy above each. Real screenshot PNGs (placeholder boxes for now, swap in later).
6. **Founder note** — narrow column letter from the maker. Replaces fake testimonials as the trust load.
7. **Closing dark band** — single statement on near-black + email form again.
8. **Footer** — minimal: wordmark, tagline, Privacy / Terms, copyright. (Block 8, but functionally part of the closing.)

**Cut from current page:** "Three steps to clarity," 6-card "More features" carousel, "Your Story, Preserved" feature row, hero card grid (4 cards), nav links other than the primary CTA.

## 2. Copy (locked)

### Nav
- Wordmark: `Clair`
- CTA: `Get notified`

### Hero
- Eyebrow: `A VOICE JOURNAL · iOS`
- Headline (2 lines): `Untangle` (iOS blue `#007AFF`, no underline) / `your thoughts.` (yellow background highlight)
- Subhead: *Most journals wait for you to be clear before you write. Clair listens while you're not — and finds the one thing worth your focus today.*
- Form: email input + dark `Get notified` button
- Helper line: `No marketing. One email when Clair is ready.`

### Manifesto
> Most apps want your *data.*
> Clair listens for the **thing you couldn't quite name** —
> and tells it back to you.

Subline (smaller, gray, below): *No prompts, no templates, no productivity scaffolding. Just you, talking out loud, and a quiet read at the end of the day.*

Highlight: `thing you couldn't quite name` — purple tint background.

### Sample reads
Eyebrow: `SAMPLE READS`
Heading: `What Clair sounds like at the end of a day.`

Three blocks, each: meta-line (uppercase) + italic quote + bold-prefixed `Today:` follow-up.

**Read 1**
- Meta: `TUESDAY MORNING · WORK · FAMILY`
- Quote: *"Your drive didn't falter — but your clarity now lies in [what you allow yourself to set down], not what you keep adding."* (pink highlight on bracketed phrase)
- Today: Name your two "must do" areas. Let the rest pause without guilt.

**Read 2**
- Meta: `SATURDAY EVENING · FAITH · HEALTH`
- Quote: *"Three Saturdays in a row, you've described feeling 'behind.' But the people you love haven't asked you for more — [only you have]."* (orange highlight)
- Today: Sit with the gap between your standards and theirs. Pick one to soften.

**Read 3**
- Meta: `WEDNESDAY LATE · SIDE PROJECT`
- Quote: *"You keep returning to one tension: caring deeply about output while [resenting how much you've taken on]."* (green highlight)
- Today: One thing on the list is doing the work of two. Cut it, or rename it honestly.

### Three-up screenshots
Eyebrow: `HOW IT WORKS`
Heading: `Talk. Read. Ask.`

| # | Sub-eyebrow | Headline | Copy |
|---|-------------|----------|------|
| 01 | `VOICE-FIRST` | Talk, don't [type]. (blue highlight on `type`) | The walk, the commute, the 2am brain dump. Open the app and speak — no prompts, no templates. |
| 02 | `DAILY READ` | Reads between your [lines]. (yellow highlight on `lines`) | Each day Clair returns the day's signal: patterns underneath, open loops you forgot, one thing worth your focus. |
| 03 | `ASK CLAIR` | Your journal [talks back]. (pink highlight on `talks back`) | Ask Clair anything about your past entries — patterns, themes, what you wrote about last week. |

Each card: label row (number + sub-eyebrow), headline, copy, then a screenshot placeholder labeled `screenshot · <name>`.

### Founder note
Eyebrow: `A NOTE FROM THE MAKER`

> There was too much going on in my head—more than I could carry. I was forgetting the things that mattered, getting stuck on what to prioritize, and the clutter wasn't clearing just by writing it down. What I needed was someone to read it back to me and tell me what I'd missed.
>
> Clair is that. A journal you talk—[one that listens] and gives back the one thing your own mind was trying to say. (blue highlight on bracketed phrase)
>
> — Erick · Founder

### Closing dark band
- Heading: `Your mind is worth understanding.`
- Form: same as hero
- Helper: same as hero

### Footer
- Left: `Clair · Untangle Your Thoughts™ · © 2026`
- Right: `Privacy` · `Terms`

## 3. Design system

### Colors
| Token | Hex | Use |
|-------|-----|-----|
| `--bg` | `#FFFFFF` | Page background |
| `--soft` | `#FAFAFA` | Sample-reads section background; form input fill |
| `--ink` | `#09090B` | Primary text, button background |
| `--ink-2` | `#3F3F46` | Body sub-text |
| `--ink-3` | `#71717A` | Eyebrow labels, helper text |
| `--line` | `#E4E4E7` | Borders, dividers |
| `--accent` | `#007AFF` | Brand blue — used on `Untangle` headline word and one other small accent only |
| `--green` | `#34C759` | Highlight tint on Read 3 |
| `--purple` | `#AF52DE` | Highlight tint on Manifesto key phrase |
| `--orange` | `#FF9500` | Highlight tint on Read 2 |
| `--pink` | `#FF2D55` | Highlight tint on Read 1 + 03/Ask Clair headline |
| `--teal` | `#5AC8FA` | Reserved (not used in v1) |
| `--red` | `#FF3B30` | Reserved for error states |

**Highlight tints** (background-only, mimicking marker highlight):
- `--hl-yellow: rgba(255, 225, 0, 0.45)`
- `--hl-blue: rgba(0, 122, 255, 0.14)`
- `--hl-purple: rgba(175, 82, 222, 0.16)`
- `--hl-orange: rgba(255, 149, 0, 0.22)`
- `--hl-pink: rgba(255, 45, 85, 0.14)`
- `--hl-green: rgba(52, 199, 89, 0.18)`

Closing dark band uses `#0A0A0A` background, white text, `rgba(255,255,255,0.06)` form fill.

### Typography
**Single font: Inter** (Google Fonts, weights 300–800, with `font-feature-settings: 'cv11', 'ss01'` for refined ligatures). No second font. JetBrains Mono is **not** used.

| Role | Style |
|------|-------|
| Hero H1 | Inter 800, fluid `clamp(56px, 9vw, 116px)`, line-height 0.94, tracking -0.045em |
| Manifesto statement | Inter 700, fluid `clamp(40px, 6.5vw, 88px)`, line-height 1.05, tracking -0.035em |
| Section H2 | Inter 700, fluid `clamp(32px, 4vw, 56px)`, line-height 1.05, tracking -0.03em |
| Closing dark H2 | Inter 700, fluid `clamp(40px, 6vw, 88px)`, line-height 1.0, tracking -0.04em |
| Subhead / hero sub | Inter 400, fluid `clamp(18px, 1.6vw, 22px)`, line-height 1.45 |
| Sample-read quote | Inter 400 italic, 18px, line-height 1.4, tracking -0.005em |
| Founder lede | Inter 400, 26px, line-height 1.4, tracking -0.01em |
| Founder body | Inter 400, 19px, line-height 1.7, tracking -0.005em |
| Body small / helper | Inter 400, 13–14px, line-height 1.5 |
| Eyebrow / labels | Inter 500, 11–12px, uppercase, tracking 0.18em |

### Spacing
- Container max-width: 1180px, horizontal padding 32px (24px on mobile)
- Vertical rhythm: 96–140px between major sections (responsive collapse to 56–80px on mobile)
- Form padding: 6px wrapper, 10–14px inner

### Shapes & shadows
- Form wrapper: 12px radius
- Buttons: 8px radius
- Pill CTAs (nav): 999px radius
- Screenshot placeholders: 20px radius
- No shadows. Borders only (`1px solid var(--line)`).

### Background treatment (page-wide, blended)
The page uses a **single continuous canvas** approach — no section is its own slab with hard borders. Three layers, bottom to top:

1. **Subtle dot grid** (fixed) — Faint 1px dots on a 24px grid (`rgba(0,0,0,0.06)`) covering the page. Top and bottom softly fade out via mask gradient so the grid never reads as hard texture.
2. **Page-wide aurora** — Five soft blurred color blobs (`filter: blur(110px)`) spread vertically down the entire page in an absolute-positioned wrapper that overflows the viewport. They drift slowly across the whole experience, so each section sits in front of a different aurora moment and the backgrounds flow into each other:
  - Blue (`--accent`) — 560px, hero top-right, opacity 0.20, 18s drift
  - Orange (`--orange`) — 460px, hero/manifesto left, opacity 0.14, 22s drift
  - Pink (`--pink`) — 420px, sample reads right, opacity 0.12, 26s drift
  - Purple (`--purple`) — 480px, three-up area left, opacity 0.10, 30s drift (reverse)
  - Green (`--green`) — 380px, founder area right, opacity 0.10, 24s drift (reverse)
3. **Section content** sits at z-index 1–2 above both layers.

### Section blending rules
- **No hard borders** between consecutive sections. Sections do not have their own background colors that snap on/off.
- **Sample reads**: Cards are individual glass surfaces (`background: rgba(255,255,255,0.55) + backdrop-filter: blur(8px)`) on the continuous page canvas — *not* a soft-bg slab with top/bottom borders.
- **Hero form** + **closing form** + **screenshot placeholders** all use the same glass-card treatment so the visual language stays consistent.
- **Closing dark band** is the page's only tonal pivot. It transitions from the light canvas via a 180px gradient bridge (`linear-gradient(180deg, transparent 0%, rgba(10,10,10,0.4) 60%, rgba(10,10,10,1) 100%)`) above the section, so the dark moment arrives gradually instead of cutting.
- **Footer** shares the closing band's `#0a0a0a` background — they read as one unified dark "ground" at the end of the page, not two separate elements.

### Motion (Tier-1 polish, all rigorously respecting `prefers-reduced-motion`)
- **Headline entrance** — On first paint, the word `Untangle` "untangles": SVG of 4–5 thin curves uncross and snap into the letterforms over ~1.4s, then static. Plays once per pageview.
- **Ambient hero waveform** — 16 small bars under the form, infinite pulse on a 1.6s ease-in-out cycle, staggered delays (0.0s → 1.5s), opacity 0.35. Suggests "listening." Pauses if `prefers-reduced-motion`.
- **Aurora drift** — Three blurred color blobs in the hero background drift on slow loops (18s / 22s / 26s). Pauses if `prefers-reduced-motion`.
- **Scroll-reveal manifesto** — Words in the manifesto sentence fade up one beat at a time as the section enters the viewport (IntersectionObserver, 50ms stagger).
- **Screenshot fade-up** — Each screenshot card translates up 12px and fades in when scrolled into view (IntersectionObserver, ease-out 600ms).
- **Hover** — Buttons darken by ~6% on hover (150ms). Nav CTA scales 1.02 on hover. No other hover effects.

### Layout & responsive
- Mobile-first (≤768px): single column, sample reads stack, three-up stacks, manifesto compresses to ~70vh
- Tablet (≥768px): two-column where natural (founder note stays single column for readability)
- Desktop (≥1024px): three-column for sample reads + three-up
- Tested breakpoints: 375 / 768 / 1024 / 1440px
- No horizontal scroll at any width. No fixed pixel widths above 1180.

## 4. Behavior

### Email form
- Backend: existing Web3Forms integration (no change). Two forms on the page (hero + closing band) post to the same endpoint.
- Submit: button shows pending state; on success, swap form for the existing notify-status confirmation; on error, inline error message below the form.
- Validation: HTML5 `type="email" required`. No client-side regex.

### Anchor / scroll
- Nav `Get notified` CTA → smooth scroll to `#notify` (closing band)
- Skip link for accessibility (existing pattern, kept)
- Sticky nav: transparent above fold, frosted (`backdrop-filter: blur(20px)`, `background: rgba(255,255,255,0.7)`) once scrolled

### Accessibility
- Contrast: `--ink` on `--bg` ≥ 16:1; `--ink-3` on `--bg` ≥ 4.6:1 (passes AA)
- Focus rings on all interactive elements (2px solid `--accent`, 2px offset)
- Keyboard navigation: tab order matches visual order
- Reduced motion: all animations disabled, ambient waveform stilled, fades become instant
- ARIA: `aria-hidden="true"` on the decorative waveform; `aria-live="polite"` on form status; `aria-label` on icon-only controls (none currently planned)

## 5. Constraints (from session)

- **Tech**: Single-file static `index.html` deployable to GitHub Pages. No build step.
- **Email backend**: Web3Forms, unchanged.
- **Screenshots**: Real PNGs only — no recreated UIs. Page ships with placeholder boxes labeled `screenshot · <name>`. User swaps in real PNGs by replacing files (likely an `images/` folder).
- **Privacy / Terms** (`privacy.html`, `terms.html`): Same fonts, colors, header/footer treatment as new index.html. Content is unchanged.

## 6. Anti-patterns (do not introduce)

- Purple/pink gradients (color tints used here are flat-background highlights only, not gradients)
- Testimonials, customer logos, "trusted by" strips
- Fake user counters or waitlist counts ("1,247 thinkers")
- Stock photos of people meditating / journaling / generic happy people
- iPhone bezel mockups around recreated UIs
- Generic "Coming soon" countdown timers
- 6-card feature carousel
- Three-step "How it works" diagrams that mirror the three product moments
- Multiple body fonts; serif heading paired with sans body; mono labels mixed with sans copy

## 7. Pre-delivery checklist

Visual quality
- [ ] No emojis as icons (SVG only)
- [ ] Inter loaded and applied to all text (verify in DevTools)
- [ ] Highlights render correctly across browsers (no white space artifacts in `<span>` background)
- [ ] Screenshot placeholders are clearly labeled (so the user knows what to replace)
- [ ] `Untangle` is the iOS blue (`#007AFF`), not the muted ink

Interaction
- [ ] Both email forms submit to Web3Forms successfully
- [ ] Nav CTA scrolls smoothly to closing band
- [ ] Hover/focus states visible on all interactive elements
- [ ] Touch targets ≥ 44×44px on mobile

Light mode
- [ ] `--ink` on `--bg` contrast ≥ 4.5:1 (verified)
- [ ] `--ink-3` (helper / eyebrow) on `--bg` contrast ≥ 4.5:1
- [ ] Closing dark band: white on `#0A0A0A` ≥ 16:1
- [ ] Highlight tint colors don't reduce readability of overlaid text

Layout
- [ ] No horizontal scroll at 320px (smallest realistic mobile)
- [ ] Verified at 375 / 768 / 1024 / 1440px
- [ ] Vertical rhythm (96–140px between sections) holds on desktop, compresses cleanly on mobile

Motion
- [ ] All animations gated by `prefers-reduced-motion: reduce`
- [ ] Headline "Untangle" entrance plays once per pageview, doesn't loop
- [ ] Ambient waveform pauses when reduced-motion is set
- [ ] No animation longer than 2s

Accessibility
- [ ] Skip link present and works with keyboard
- [ ] All decorative SVGs have `aria-hidden="true"`
- [ ] Form fields have visible labels (or aria-labels) — not just placeholders
- [ ] Heading hierarchy: one h1, then h2s (manifesto / sample reads / three-up / closing)

Out-of-scope (for this redesign)
- App Store badge (no app yet) — keep email form as the only ask
- Analytics tracking beyond what's already wired
- A/B testing infrastructure
- Localization
