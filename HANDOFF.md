# Maple Outdoor Builds — handoff at ~60% (calm revamp)

**Live:** https://10elizabethbell.github.io/mapleOutdoorBuilds/ · **Repo:** https://github.com/10elizabethbell/mapleOutdoorBuilds · **Built:** 2026-10-17 from Muse brief 2026-10-17 (Facebook group post, Essex County Contractor Referrals) · **Revamped:** 2026-10-19 into the calm band style

## What changed in the revamp (2026-10-19)
The business hasn't been contacted yet, so the whole site was rebuilt under the new house default (`calm-photo-style.md`, from lpmr.co.uk), starting from DPG's `index.html`.
- **Gone:** the leaf-sweeping canvas deck hero, falling leaves, gust lanes, the boards-as-prints photo frames, the board strip above the form, the cream ground, the "Built right. Left clean." headline, the separate "Where we work" band, and the desktop rule that sent the hero text button to the form.
- **New look:** off-white paper (#f4f6f2) alternating with forest green (#1d4630) and deep forest (#122c1e) with the faint diagonal line texture. One warm accent is maple amber (#f2a93b) as a fill only, with deep green text on it; #8a4b00 is used when amber has to be text on light. Headings are Cal Sans (Google Fonts) and body text the system stack at 16/1.7. Cards are 24px, buttons are pills, and inputs sit on a #e5ece5 fill.
- **New hero:** their own finished-deck photo (from the 10-17 video) under a forest-green overlay. On top: the eyebrow "Small jobs welcome", the H1 "Decks and yards, done right in Saint John." (place in amber), their tagline, and two buttons ("Get a free estimate" scrolls to the form, "Text us" opens a text).
- **New motion:**
  - The hero H1 bounces in letter by letter. It waits up to 900ms for Cal Sans so the line breaks match the settled heading, and shows the plain heading if the font is slower.
  - One 12px fade-up on sections below the first screen.
  - The floating 60px text circle (`CONFIG.FLOAT`).
  - Reduced motion and no-JS show everything at once.
- **Structure:**
  - header (leaf-over-roof mark + name, number top-right, not sticky)
  - hero
  - What we do: arrow rows on green in two groups, Decks and Yards & cleanups. Tapping a row jumps to the form with that job ticked.
  - Our work: Before / After / Finished deck photo cards, then a big "See more of our work on Facebook" row
  - How it works (3 steps, deep band)
  - Tell us about the job: a form that composes a text to 506-607-1818
  - close band: name, a care line, area, big tap-to-call number
  - footer: name, area, number, Facebook
- New `og.jpg` (1200×630, the deck photo with the headline), `favicon.svg` and `apple-touch-icon.png` (amber leaf over a cream roofline on green).
- The floating circle hides on the hero, over the service rows (it sat on their arrows) and over the form.

## Assumptions I made
- **Green + amber.** Their profile art is deep forest green and cream with a maple leaf. The calm style needs one warm accent, so I used autumn maple amber rather than the brief's "maple-leaf red" (red on green fights; amber reads as the leaf). Easy to swap: `--amber` / `--amber-ink` in `:root`.
- **Decks first.** The brief's caption lists cleanups, junk removal and deck repairs. Their Facebook page and profile image lead with decks (new decks, repairs & rebuilds, stairs, railings, extensions, resurfacing). Both groups are listed.
- **Logo is my redraw** of the leaf-over-roof mark from their profile image, set with "Maple / Outdoor Builds". Their profile image says "Maple Builders"; the page name is used.
- **"We", not "I".** Their posts say "Send us a message".
- **Copy I wrote, to confirm with the owner:**
  - H1 "Decks and yards, done right in Saint John."
  - the close line "We take one project at a time, so yours gets our full attention, big or small." (built from their tagline)
  - step 2 "You know what it needs and what it costs before we start."
  - step 3 "Properly, start to finish."
- "Quality work, one project at a time." and "Small jobs welcome" are theirs, word for word.
- **Hero photo:** it's 720×536 (the video is 720 wide; there's nothing larger). On phones it crops nicely to the stairs and railing. On desktop it's upscaled 2× under the overlay with a 1.5px blur so the softness reads as deliberate. If Ellie finds it too soft on desktop, the rule's fallback is the plain textured green band on desktop only.

## Placeholders and gaps
- **Service area cut to "Saint John, NB and surrounding areas."** The old build also listed Moncton, Dieppe and Riverview. That came only from the profile flyer, which looks AI-made, and Moncton is about 150 km away. The finish reviewer flagged it as unconfirmed, so it's off the page until the owner confirms.
- Only three photos, all stills from one video. Before and After are different shots, so there's no slider. "Finished deck" is the same photo as the hero.
- No email, so the footer has none. Also no hours, reviews, prices, owner name, years in business, or insurance info. All of these are left off the page.

## Questions for the owner
- More job photos, especially before/after pairs from the same spot (that unlocks a slider), and a wider or higher-res shot for the hero.
- Your first name, so the page can say who they'll be dealing with?
- "Maple Outdoor Builds" or "Maple Builders"? Do you have a logo file?
- Email address for the footer?
- Area: Saint John and which towns around it? Do you really go to Moncton, Dieppe or Riverview?
- Which matters more right now: deck work or cleanups and junk removal? This changes the H1 and the service order.
- Insured? Any customer reviews you could share word for word?

## Ideas not built (yours to pick)
- **Opt-in signature motion (runner-up):** bring back the 10-17 leaf-sweeping deck hero (blow maple leaves off the boards by drag; in git history at `dd3b6b5`) as a band below the hero, or as the hero for phones only. Other worlds from their trade: plane shavings curling off a weathered board (resurfacing), a junk pile that clears as you scroll, a deck that builds board by board.
- **Desktop dead space:** at 1024px+, the left column beside the form is empty under the heading. A small finished-deck photo or the three steps could sit there.
- **Impeccable flagged and I kept (Ellie's call):**
  - eyebrow pills (craft-floor bans eyebrows)
  - the H1 bounce-in and its font wait (animate/optimize: load choreography and LCP)
  - the floating circle duplicating "Text us" (distill)
  - the faint band texture (quieter)
  - Cal Sans from Google Fonts rather than self-hosted
- **Contrast:** the field fill #e5ece5 on the white form card is about 1.2:1 (WCAG 1.4.11). Fields are still identified by their labels and placeholder text, as in DPG's fix. A darker fill or a 1px border would pass.
- Alternative H1s: "Decks done right in Saint John." if decks are the main business; "Saint John's deck and cleanup crew."
- A before/after slider once a matched pair exists.

## Impeccable
- Detector: real findings fixed. File-scoped ignores were recorded for the calm texture (Ellie's style), the green-tinted on-dark text (6.9:1, not grey) and the full-bleed photo cards. The old 10-17 ignores (system font, cream, deck stripes) were removed. DESIGN.md was regenerated from this build.
- Modes run (all except live, onboard, init, shape, document, extract): critique, audit, polish, harden, clarify, adapt, optimize, typeset, layout, colorize, animate, delight, quieter, bolder, distill, overdrive, plus the finish reviewer. Fixes applied:
  - visible float focus ring
  - service group labels set apart from the rows
  - no repeated "small jobs" / "free estimate" lines
  - "estimate" not "quote"
  - Facebook row wording
  - town placeholder
  - error alerts
  - check marks on selected chips, and hover on selected chips
  - "didn't open?" note only when the page is still in view
  - tappable footer number
  - 320px header fit
  - unsupported claims cut
  - header no longer sticky, so the number shows once per screen
  - darker overlay behind the hero promise on phones
- `finishing-rules.md` checklist re-checked by hand afterwards.

## Verified
- Chromium and WebKit at 360 / 390 / 430 / 1440:
  - no sideways scroll
  - offer and primary button on the first phone screen
  - H1 split and settled with identical heights (same line breaks), restored to plain HTML
  - nothing left hidden after scrolling
- Reduced motion and JS off: the plain H1 and all content show at once.
- Floating circle: hidden on the hero, over the services and over the form; shown over work, steps and close; `aria-hidden` and `tabIndex` follow it.
- Form: a service row ticks its chip; empty submit flags the job and town and focuses the first chip. The composed text decodes to "Hi Maple Outdoor Builds! This is Sam. I'd like a free estimate for: Deck repair. The job is in Rothesay. Two boards rotted & loose."
- White hero text over the brightest photo pixels is 6.4:1 or better; amber H1 text about 5:1.

## Not verified
- Real-device tap and SMS handoff on iOS and Android, especially inside Facebook's in-app browser.
- How long Cal Sans takes on slow cellular. If it misses the 900ms wait, the H1 just appears without the bounce.
