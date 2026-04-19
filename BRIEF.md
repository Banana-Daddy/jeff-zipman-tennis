# Jeff Zipman Tennis — Design Brief

## Brand Synopsis
Jeff Zipman is a Vancouver-based tennis coach with 30 years of experience and a Tennis Canada Coach 1 (Club Professional 1) certification. He offers private and group lessons for all levels, with a standout differentiator: free video analysis of every student's game, complete with personalized follow-up exercises. He also offers discounts for seniors and multi-session bookings.

Jeff has minimal online presence — no website, no social media coaching profiles. This mockup is his first digital footprint, designed to project the credibility and premium quality that 30 years of experience deserves. The brand positioning is intentionally upscale: this isn't a rec center flyer, it's a private coaching experience.

## Design Decisions

### Direction: Club Racquet (v4 · PRO-MAX)
- **Mood**: Prep-school blazer meets Vogue serif. Ralph Lauren courtside, not tech SaaS. Member-only, heritage, unhurried.
- **Fonts**: Bodoni Moda (display, italic-forward serif) + Manrope (body, clean sans) + JetBrains Mono (telephone / monospace details)
  - Display: https://fonts.google.com/specimen/Bodoni+Moda
  - Body: https://fonts.google.com/specimen/Manrope
- **Colors**:
  - `#F4EEE0` — Oxford cream (primary background)
  - `#0E1C36` — Blazer navy (dark sections, CTAs, footer)
  - `#A8823A` / `#C09A4E` — Brass (accent rules, CTAs, highlight type)
  - `#EFE6D0` — Parchment (elevated muted surface)
  - `#1A1A1A` — Ink (body type on cream)
- **Layout**: Three-act editorial flow — Hero lockup + framed portrait → credentials marquee (navy band, italic serif) → pull-quote essay with drop cap → bento lesson cards on navy → editorial video-analysis spread (portrait image + process column) → rates strip → navy contact crescendo ("Let's play.").
- **Signature element**: Oversized italic Bodoni **"Z" monogram** used as a brand crest in the nav, repeated as a translucent watermark on every major section, and anchored into the selector card. Brass hairline rules mark every section break.
- **Trends used**:
  - Editorial / magazine grid — asymmetric 12-col lockups, section dateline, act numerals
  - Kinetic italic typography — oversized Bodoni display with staggered word reveal on hero
  - Bento grid with liquid-glass cards — 3 service cards over navy with brass-tinted glass surfaces
  - Brass hairline rules — custom dividers replacing standard borders on every section
  - Marquee ticker — italic serif credentials strip on navy
- **Workflow**: PRO-MAX MODE — direction generated via the `ui-ux-pro-max` skill's `--design-system` search (Liquid Glass + editorial base), translated into a bespoke "Club Racquet" brief distinct from v1/v2/v3. Two fresh Grok images (no asset recycling from prior builds).

### Direction: Midnight Gold
- **Mood**: Private club invitation. Quiet confidence that lets the credentials speak.
- **Fonts**: Cormorant Garamond (display, serif — elegant weight) + Outfit (body, sans — clean modern)
  - Display: https://fonts.google.com/specimen/Cormorant+Garamond
  - Body: https://fonts.google.com/specimen/Outfit
- **Colors**:
  - `#0A0A0F` — Midnight (background)
  - `#141419` — Surface (cards, elevated elements)
  - `#C9A96E` — Gold (primary accent, CTAs, highlights)
  - `#F5F0EB` — Cream (body text, warm white)
  - `#6B6B7B` — Muted (secondary text, subtle elements)
- **Layout**: Single-page flow — cinematic hero → credentials strip → glass service cards → video analysis feature → pricing info → contact CTA
- **Signature element**: Gold court-line accents — thin gold lines positioned like tennis court markings that frame sections and create visual continuity. Combined with glassmorphism cards for premium depth.
- **Trends used**:
  - Glassmorphism (mature) — service cards with backdrop-blur and translucent borders
  - Kinetic typography — hero name reveal with staggered translateY animation
  - Floating glass nav — pill-shaped, centered, backdrop-blur, detached from header
  - Marquee text strip — oversized ghosted text separating content zones
  - Layered shadows — multi-layer box-shadow on card hover for volumetric depth

## Content Inventory
- **Images pulled**: None available — no existing website or CDN
- **Images generated**: 5 via Grok Imagine (see IMAGE_LOG.md)
  - v1 set (Midnight Gold): hero.jpg, coach-portrait.jpg, video-analysis.jpg
  - v4 set (Club Racquet / PRO-MAX): promax-portrait.jpg, promax-video.jpg
  - No recycling between builds — each direction is served by its own fresh assets
- **Key copy**: All written for Jeff — taglines, descriptions, CTAs. Flagged in ACCURACY.md for review.
- **Links preserved**:
  - Phone: tel:604-340-5424
  - Email: mailto:jzipman@hotmail.com

## Image Generation Prompts
All 3 images were auto-generated via Grok Imagine during the build. See IMAGE_LOG.md for full details, QA scores, and costs.

### Image 1 — Hero Background
- **Slot**: Full-width hero section background (20% opacity with gradient overlay)
- **Aspect ratio**: 16:9
- **Status**: Generated ✓ | Attempt 1/4

### Image 2 — Coach Portrait
- **Slot**: About section, right column (4:5 portrait)
- **Aspect ratio**: 3:4
- **Status**: Generated ✓ | Attempt 1/4

### Image 3 — Video Analysis
- **Slot**: Video Analysis feature section, left column (16:9 landscape)
- **Aspect ratio**: 16:9
- **Status**: Generated ✓ | Attempt 1/4

## Suggested Next Mockups
- **Booking page** with session types, availability calendar, and online payment
- **Testimonials page** with student progress stories and before/after video analysis screenshots
- **About/Bio page** with Jeff's coaching philosophy, certifications, and career highlights
- **Programs page** detailing junior programs, senior sessions, group clinics, and seasonal camps
- **FAQ page** covering logistics — where Jeff teaches, what to bring, cancellation policy

## Build Timing
| Phase | Duration |
|---|---|
| Step 1: READ (web search) | ~45s |
| Step 2: DIRECTION | ~10s |
| Step 3: BUILD (HTML) | ~90s |
| Image Generation (3 images) | ~24s |
| Image QA (3 Grok vision calls) | ~45s |
| Step 4: VERIFY | ~15s |
| Step 5: BRIEF + docs | ~30s |
| Step 6: PUBLISH | ~30s |
| **Total: Prompt to Live Link** | **~7m 43s** |

## Production Notes
To build this into a real site, use Claude Code (Opus, high effort). Recommended stack: static site with a booking integration (Calendly or Acuity for session scheduling). Could remain a single-page site with an embedded booking widget, or expand to 3-4 pages. Hosting on GitHub Pages or Netlify is fine — no backend needed unless Jeff wants a client portal for video analysis delivery. Consider adding a simple contact form via Formspree or Tally.
