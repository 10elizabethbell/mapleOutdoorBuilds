---
name: Maple Outdoor Builds
description: Decks and property cleanups in Saint John, NB. An October deck you sweep clean.
colors:
  forest-night: "#132c1e"
  forest: "#173524"
  forest-lift: "#2c5c3e"
  cream: "#f5efe2"
  cream-deep: "#ebe2cf"
  cream-rule: "#d9cfb8"
  ink: "#172a1f"
  ink-soft: "#43574a"
  harvest: "#e9b48f"
  cream-on-green: "#e4dccb"
  sage-muted: "#bfc9bd"
  maple: "#c8442a"
  maple-bright: "#f08a5a"
  error-on-green: "#ffb894"
  board: "#a8743f"
  board-gap: "#2b1d12"
  print-paper: "#fbf8f1"
typography:
  display:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "clamp(44px, 13.4vw, 92px)"
    fontWeight: 900
    lineHeight: 0.92
    letterSpacing: "-0.015em"
  headline:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "clamp(34px, 9vw, 58px)"
    fontWeight: 900
    lineHeight: 0.98
    letterSpacing: "-0.01em"
  title:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "22px"
    fontWeight: 750
    lineHeight: 1.2
  body:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "17px"
    fontWeight: 400
    lineHeight: 1.55
  label:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif"
    fontSize: "15px"
    fontWeight: 800
    lineHeight: 1.2
    letterSpacing: "0.14em"
rounded:
  print: "3px"
  field: "12px"
  panel: "14px"
  pill: "999px"
spacing:
  gutter-phone: "20px"
  gutter: "32px"
  container: "1180px"
components:
  button-cream:
    backgroundColor: "{colors.cream}"
    textColor: "{colors.forest}"
    rounded: "{rounded.pill}"
    padding: "14px 24px"
    height: "56px"
  button-line:
    backgroundColor: "transparent"
    textColor: "{colors.cream}"
    rounded: "{rounded.pill}"
    padding: "14px 24px"
    height: "56px"
  button-green:
    backgroundColor: "{colors.forest}"
    textColor: "{colors.cream}"
    rounded: "{rounded.pill}"
    padding: "14px 24px"
    height: "56px"
  button-green-hover:
    backgroundColor: "{colors.forest-lift}"
  service-arrow:
    backgroundColor: "{colors.cream-deep}"
    textColor: "{colors.ink}"
    size: "40px"
  service-arrow-hover:
    backgroundColor: "{colors.maple}"
    textColor: "#ffffff"
  chip:
    backgroundColor: "transparent"
    textColor: "{colors.cream}"
    rounded: "{rounded.pill}"
    padding: "10px 16px"
    height: "46px"
  chip-selected:
    backgroundColor: "{colors.cream}"
    textColor: "{colors.forest}"
  input-on-green:
    backgroundColor: "rgba(10,25,16,.35)"
    textColor: "{colors.cream}"
    rounded: "{rounded.field}"
    padding: "14px 16px"
    height: "54px"
---

# Design System: Maple Outdoor Builds

## Overview

**Creative North Star: "The October Deck"**

A Saint John deck in autumn: fresh pressure-treated boards, maple leaves that keep falling on them, and a crew that sweeps them off. The material is the brand. Boards are painted live on canvas, leaves are physical objects you can push, and the page's two grounds are the forest green and cream of the company's own profile art (leaf over roofline). Everything else stays quiet so the deck can be the thing you touch.

Density is phone-first and generous: one column, big tap targets (44px minimum, 56px buttons), short uppercase headings set heavy. Colour is restrained; green and cream carry the page, harvest amber picks out the second line of headings on green, and maple red appears only when the visitor is pointing at something.

**Key Characteristics:**
- Two grounds: forest green (hero, close, footer) and cream (content). No third surface besides the boards.
- Real material, drawn in code: canvas deck boards with grain, knots, screws, butt joints and sunlight.
- Maple leaves as interactive sprites, in nine autumn colourways.
- Maple red is a state colour, never a resting colour.
- Heavy uppercase system type; no web fonts.

## Colors

Forest and cream from the client's own artwork, wood from the deck, maple red held back for interaction.

### Primary
- **Forest** (#173524): hero, close section, button-green, step numerals, theme-color, the roofline mark's ground.
- **Forest Night** (#132c1e): footer only; one step down so the page ends darker.
- **Forest Lift** (#2c5c3e): hover fill for button-green.

### Secondary
- **Harvest** (#e9b48f): second line of headings on green ("Left clean.", "a photo."), icons in the phone link and footer, text selection. Warm accent on green at rest.

### Tertiary (state only)
- **Maple** (#c8442a): hover/focus on cream; the service-row arrow fill, focus outline, the leaf mask after "Small jobs welcome" and inside selected chips.
- **Maple Bright** (#f08a5a): hover/focus on green; chip and input borders, focus rings, caret, phone-icon hover, send-button border.

### Neutral
- **Cream** (#f5efe2): content ground, text on green, button-cream.
- **Cream Deep** (#ebe2cf): the Before & after band; resting arrow discs.
- **Cream Rule** (#d9cfb8): 1px dividers between service rows.
- **Ink** (#172a1f) / **Ink Soft** (#43574a): text on cream; soft for supporting copy and group labels.
- **Cream on Green** (#e4dccb) for lead copy on green; **Sage Muted** (#bfc9bd) for optional/fine text on green; **Error on Green** (#ffb894) for validation.
- **Board** (#a8743f) / **Board Gap** (#2b1d12): CSS stripe fallback under every canvas deck; **Print Paper** (#fbf8f1) for the photo prints.

### Named Rules
**The Maple Is A Hand Rule.** Maple red (#c8442a on cream, #f08a5a on green) appears only on hover, focus, selection, or as the small leaf mark. Nothing rests in red. Use the bright variant on green, the deep one on cream (`.on-green` swaps the focus colour).

**The Two Grounds Rule.** Sections are either forest or cream. Wood is the only other surface, and it is always boards.

## Typography

**Display Font:** system stack (-apple-system, BlinkMacSystemFont, Segoe UI, Roboto, Helvetica Neue, Arial, sans-serif)
**Body Font:** the same stack

**Character:** One family doing two jobs. Display is weight 900, uppercase, near-solid leading; body is plain 17px (18px from 1024px) at 1.55. The system stack is Ellie's pitch-site house style, chosen for load speed on cellular in Facebook's in-app browser; the heaviness and case carry the voice, not the face.

### Hierarchy
- **Display** (900, clamp(44px, 13.4vw, 92px); clamp(56px, 4.8vw, 76px) on desktop; 0.92): the hero h1 only, two lines, second line in Harvest.
- **Headline** (900, clamp(34px, 9vw, 58px), 0.98, uppercase, text-wrap: balance): section h2s.
- **Title** (750-900, 22px): service rows, step titles, "Small jobs welcome".
- **Body** (400, 17px, 1.55, 34-44ch): promise, leads, step copy.
- **Label** (800-900, 15px, 0.14em, uppercase): service group headings and print captions.
- **Big statement** (850, clamp(26px, 7vw, 40px), 1.12, 18ch): the service-area line.

### Named Rules
**The Heavy Caps Rule.** All h1-h3 are uppercase, 900, letter-spacing -0.01em, leading under 1. Weight contrast (900 against 400) is the hierarchy; do not add a second family.

## Layout

Phone-first single column inside a 1180px container, 20px gutter (32px from 640px). Sections breathe vertically: 48-64px on phones, 90-100px on desktop. Up to 1023px the hero sizes to its content with the deck at clamp(240px, 40svh, 340px); from 1024px it becomes a two-column grid (copy left, deck right, deck capped near 880px viewport height with a 28px top-left corner). Content sections at 1024px split 4fr/7fr (heading left, content right); the close splits 5fr/6fr. Breakpoints: 374px (tight brand), 640px, 1024px.

## Elevation & Depth

Flat UI on flat grounds; depth belongs to physical objects only. The boards panel lifts off the cream band, prints sit on the boards with two-layer paper shadows, and leaves carry their own blurred-sprite shadow offset by height (z) so airborne leaves float further from their shadow. The canvas paints its own light: lit top edges, dark bottom edges, and a top-left sunlight gradient.

### Shadow Vocabulary
- **Panel lift** (`box-shadow: 0 18px 40px -18px rgba(40,25,10,.55)`): the before/after boards panel.
- **Print on wood** (`box-shadow: 0 2px 3px rgba(30,15,5,.35), 0 16px 30px -10px rgba(30,15,5,.6)`): each photo print.
- **Focus halo** (`box-shadow: 0 0 0 3px rgba(240,138,90,.3)`): inputs and chips on green, alongside the Maple Bright border.

### Named Rules
**The Only Things That Cast Shadows Rule.** Shadows are for objects on the deck (prints, leaves, the boards themselves). Buttons, rows and fields never cast one.

## Shapes

Round where hands touch, square where wood is cut. Buttons and chips are full pills (999px); fields 12px; the boards panel 14px; arrow discs and step numerals are circles; prints are near-square paper (3px). Boards are hard rectangles with 3px gaps and 1.6px butt joints. The maple leaf (a 15-point half-outline mirrored) is the one recurring silhouette: logo, favicon, CSS mask, canvas sprite.

## Components

### Buttons
- **Shape:** pill (999px), min-height 56px, 14px 24px, 800 17px, 2px border, 20px leading icon.
- **Cream** (on green, primary CTA): cream fill, forest text; hover goes white.
- **Line** (on green, secondary): transparent, cream text, border rgba(245,239,226,.55); hover full cream border plus 8% cream wash.
- **Green** (on cream): forest fill; hover Forest Lift.
- **States:** `:active` scale(.98); transitions 0.18s; full-width on phones, inline from 640px.

### Service Rows (signature)
- **Style:** 60px rows, 22px/750 ink, 1px Cream Rule dividers, under a 15px tracked label with a 2px ink rule.
- **Hover / Focus:** only the 40px arrow disc changes, Cream Deep to Maple with white arrow (0.18s). The row gets no background, outline or shadow; on keyboard focus the outline moves to the disc.
- **Behaviour:** every row is an `sms:` link with a body naming the service.

### Chips
- **Style:** 46px pills, 2px border rgba(245,239,226,.35), 700 17px cream text on green.
- **Hover / Focus:** border goes Maple Bright; focus adds the 3px halo.
- **Selected:** cream fill, forest text, a 16px Maple leaf mask before the label.

### Inputs / Fields
- **Style:** 54px (textarea 110px), 12px radius, 2px border rgba(245,239,226,.35), fill rgba(10,25,16,.35), cream text, Maple Bright caret.
- **Hover / Focus:** outlined, border goes Maple Bright; focus adds the halo. No outline ring.
- **Error:** border and message in Error on Green (#ffb894), 700 15px.

### Navigation
- Brand lockup (leaf-over-roofline mark, MAPLE 900 22px / OUTDOOR BUILDS 700 10.5px at 0.22em) left; tabular phone link top right in 800 cream with a Harvest icon that turns Maple Bright on hover. No menu.

### Canvas Deck (signature)
- **Painter:** `paintDeck(ctx, w, h, boardH, seed)` paints once per size into an offscreen canvas from a seeded RNG: boards of random length (320-940px) in hsl(27-33, 36-48%, 43-55%), wavy grain fibres, occasional cathedral arcs, 0-2 knots, edge shading, paired screws on joist lines every 96px, butt joints, top-left sunlight. Board height 44/54px (hero), 37/46px (boards panel), 35px (edge strip). DPR capped at 1.5.
- **Leaf sprites:** 96px offscreen sprites, two variants each of nine [base, light, vein] colourways (reds, oranges, golds, browns), radial fill, blotches, optional spots, veins, stem, plus one blurred shadow sprite.
- **Fallback:** each canvas sits on a CSS stripe of Board/Board Gap so boards show before paint and without JS.

### Hero Sweep
Leaves fall, rest, and get blown off by finger or mouse. Tunables in `HERO`: density 1/2300 px² (phone, cap 90) and 1/3600 (desktop, cap 260); refill 5 and trickle 0.35 per s per 100k px²; fall 34px/s, wind 14px/s; blower radius 84px (x1.4 desktop), push 2600, carry 0.55, lift 220, gravity 420; ground/air friction 3.2/1.0; idle gusts every 4.5-7.5s, 9s after the last touch, gust push 220; leaf size 34-50px phone, 42-62px desktop. Leaves leaving the deck are removed. The "Drag to sweep the leaves" hint fades after the first real drag.

### Resting Leaves
The boards panel and the 38px edge strip above the close carry leaves on springs: pushed by the pointer, they wobble home. Tunables in `SPRING`: k 38, damp 6.5, radius 90, push 1500, carry 0.35. Count w·h/16000 on the panel, w/95 on the strip. They only re-render while moving or touched.

### Prints on Boards
Before / After / finished-deck photos sit on the boards panel as paper prints: 9px Print Paper border, caption strip in the label style, rotated -2.2°, 1.8°, -0.8°, staggered on phones and three across on desktop. Prints ignore the pointer so the leaves underneath stay sweepable.

### Animation Loop
One `requestAnimationFrame` loop steps every visible scene (dt capped 0.05s); an IntersectionObserver per canvas marks visibility and the loop stops when none is on screen, restarting on re-entry. Resize re-setup is debounced 150ms and ignored if the box size is unchanged (address-bar jitter). Under reduced motion, no gusts or refill, and the loop starts only on a pointerdown on the hero deck.

## Do's and Don'ts

### Do:
- **Do** keep every surface forest, cream, or boards.
- **Do** reserve Maple (#c8442a) and Maple Bright (#f08a5a) for hover, focus, selection and the leaf mark.
- **Do** set headings 900 uppercase with leading under 1, and take the second line to Harvest (#e9b48f) on green.
- **Do** put photos on the boards as rotated prints, never as bare tiles.
- **Do** run new canvas scenes through the shared Scene and loop so they pause off screen.
- **Do** keep tap targets at 44px minimum and primary buttons at 56px.

### Don't:
- **Don't** put red on anything at rest, including headings, badges or backgrounds.
- **Don't** change a service row's background or outline on hover; the arrow is the only change.
- **Don't** ring form fields with an outline; they change border colour and gain the soft halo.
- **Don't** give buttons, rows or fields shadows.
- **Don't** add a web font or a second family.
