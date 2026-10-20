---
name: Maple Outdoor Builds
description: A Saint John deck-and-yard crew's site in calm paper and forest-green bands, their own deck photo up front, maple amber as the one warm fill.
colors:
  amber: "#f2a93b"
  amber-2: "#f7bd62"
  amber-ink: "#8a4b00"
  navy: "#1d4630"
  deep: "#122c1e"
  paper: "#f4f6f2"
  card: "#ffffff"
  field: "#e5ece5"
  ink: "#13301f"
  body: "#28382e"
  soft: "#4a5a50"
  on-dark: "#f4f6f1"
  on-dark-soft: "#c6d5c9"
  error: "#b3261e"
typography:
  display:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "clamp(40px, 11.4vw, 80px)"
    fontWeight: 400
    lineHeight: 1.02
    letterSpacing: "-0.005em"
  headline:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "clamp(30px, 7.6vw, 48px)"
    fontWeight: 400
    lineHeight: 1.08
    letterSpacing: "-0.005em"
  phone-display:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "clamp(30px, 9vw, 52px)"
    fontWeight: 400
    lineHeight: 1
  title:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "clamp(19px, 5.2vw, 22px)"
    fontWeight: 400
    lineHeight: 1.2
  lede:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial, sans-serif"
    fontSize: "clamp(17px, 4.6vw, 19px)"
    fontWeight: 400
    lineHeight: 1.7
  promise:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial, sans-serif"
    fontSize: "clamp(17px, 4.7vw, 20px)"
    fontWeight: 400
    lineHeight: 1.5
  close-line:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial, sans-serif"
    fontSize: "clamp(18px, 5vw, 20px)"
    fontWeight: 400
    lineHeight: 1.7
  body:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial, sans-serif"
    fontSize: "16px"
    fontWeight: 400
    lineHeight: 1.7
  label:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial, sans-serif"
    fontSize: "14px"
    fontWeight: 600
    lineHeight: 1.2
    letterSpacing: "0.08em"
  scale:
    xs: "12px"
    sm: "14px"
    note: "15px"
    base: "16px"
    md: "17px"
    md-plus: "18px"
    lg: "20px"
    step: "21px"
    xl: "22px"
    brand: "24px"
    h2-min: "30px"
    h1-min: "40px"
    h2-max: "48px"
    phone-max: "52px"
    h1-max: "80px"
rounded:
  focus: "6px"
  field: "10px"
  card: "24px"
  pill: "999px"
spacing:
  gutter: "20px"
  gutter-wide: "40px"
  container: "1160px"
  band: "64px"
  band-wide: "96px"
components:
  button-primary:
    backgroundColor: "{colors.amber}"
    textColor: "{colors.ink}"
    rounded: "{rounded.pill}"
    padding: "0 26px"
    height: "56px"
  button-primary-hover:
    backgroundColor: "{colors.amber-2}"
    textColor: "{colors.ink}"
  button-ghost:
    backgroundColor: "transparent"
    textColor: "{colors.on-dark}"
    rounded: "{rounded.pill}"
    padding: "0 26px"
    height: "56px"
  input-field:
    backgroundColor: "{colors.field}"
    textColor: "{colors.ink}"
    rounded: "{rounded.field}"
    padding: "13px 14px"
    height: "52px"
  chip:
    backgroundColor: "{colors.field}"
    textColor: "{colors.ink}"
    rounded: "{rounded.pill}"
    padding: "0 18px"
    height: "48px"
  chip-selected:
    backgroundColor: "{colors.ink}"
    textColor: "{colors.card}"
  form-card:
    backgroundColor: "{colors.card}"
    rounded: "{rounded.card}"
    padding: "clamp(20px, 5vw, 32px)"
  photo-card:
    backgroundColor: "{colors.deep}"
    textColor: "{colors.card}"
    rounded: "{rounded.card}"
  link-card:
    backgroundColor: "{colors.navy}"
    textColor: "{colors.on-dark}"
    rounded: "{rounded.card}"
    padding: "14px 16px 14px 22px"
    height: "80px"
  service-row:
    textColor: "{colors.on-dark}"
    typography: "{typography.title}"
    padding: "10px 0"
    height: "64px"
  step-badge:
    backgroundColor: "{colors.amber}"
    textColor: "{colors.ink}"
    size: "48px"
  text-float:
    backgroundColor: "{colors.amber}"
    textColor: "{colors.ink}"
    size: "60px"
---

# Design System: Maple Outdoor Builds

## Overview

**Creative North Star: "The Calm Yard"**

The page is a stack of full-width colour bands that alternate between off-white paper and two forest greens, the same green-and-cream as the crew's own profile art. Nothing competes with the work: the hero is their finished deck under a deep forest overlay, the work band is their before, after and finished photos in big rounded cards, and every band holds one heading, a short line, and one clear thing to do.

Maple amber is the only warm colour, and it shows up as a filled shape (a button, a step number, the floating text circle, a row's arrow on hover), never as a field of colour. Type is Cal Sans for anything that names or sells, and the system sans at a generous 16/1.7 for everything that explains. Motion happens once and then settles: the hero headline's letters bounce in, things below the first screen fade up 12px, and after that the page holds still.

Density is low on purpose. A visitor on a phone in Facebook's in-app browser should see one idea per screen and a big target under their thumb.

**Key Characteristics:**
- Full-width paper and forest-green bands; no boxed sections floating on a ground.
- Amber as a fill (text on it is ink); amber-ink when amber has to be text on a light background.
- Soft, generous shapes: 24px cards, pill buttons and chips, 10px fields.
- Flat surfaces. The floating text circle is the only thing with a shadow.
- Real photos only, under a forest overlay or a bottom scrim so the type stays readable.

## Colors

Two forest greens and an off-white paper carry the page; one maple amber does all the warm work.

### Primary
- **Maple Amber** (amber): fills only. Primary buttons, step-number discs, the floating text circle, a service row's arrow on hover, the accent phrase in a dark-band heading, and the focus outline on dark bands. Text on it is always Forest Ink.
- **Amber Light** (amber-2): the primary button's hover fill. Nothing else.
- **Amber Ink** (amber-ink): amber when it has to be text or an icon on light: the header phone icon, the header phone number on hover.

### Secondary
- **Forest Green** (navy): the services band, the Facebook link card, the hero's fallback ground, the brand mark, and the focus/hover outline on light surfaces (the CSS calls it `--navy` and `--focus`; it is green).
- **Deep Forest** (deep): the "how it works" band and the footer, both with a faint 135-degree line texture. It is also the hero overlay tint (at 80 to 86% opacity) and the photo-card ground behind images.

### Neutral
- **Paper** (paper): the page ground, the header, and the work band. Also the theme colour.
- **Card White** (card): the form card on paper. White is also the hero H1 and the photo captions.
- **Field Mist** (field): input and chip fills inside the white form card.
- **Forest Ink** (ink): headings on light, text on amber, the selected-chip fill. Translucent ink (6%) is the only tint used on light.
- **Body Green-Grey** (body): running text on light.
- **Soft Green-Grey** (soft): secondary text on light: ledes, hints, placeholders, the small caps under the brand name.
- **On-Dark** (on-dark): headings, rows and links on green bands.
- **On-Dark Soft** (on-dark-soft): running text and group labels on green bands (6.9:1 on Forest Green).
- **Error Red** (error): field error text and the error border. Form only.

### Named Rules
**The Amber Is a Fill Rule.** Maple amber appears as a solid shape with Forest Ink on it, or as accent text on a dark band. On a light ground, amber text becomes Amber Ink. Amber never fills a band or a card.

**The Green Bands Rule.** Every band is one of three grounds: Paper, Forest Green, or Deep Forest with its line texture. Text on green uses the on-dark pair, never the light-ground greys.

## Typography

**Display Font:** Cal Sans (with Avenir Next, Segoe UI, system-ui)
**Body Font:** the system sans (-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial)

**Character:** Cal Sans is rounded, friendly, and a little bold even at its single 400 weight, so it carries every name, heading, button and service. The system sans stays out of the way and reads well at 16/1.7 on a phone.

### Hierarchy
- **Display** (Cal Sans 400, clamp 40 to 80px, line-height 1.02, max 12ch): the hero H1 only, white on the photo overlay, with its last phrase in amber.
- **Headline** (Cal Sans 400, clamp 30 to 48px, line-height 1.08, balanced wrap): band headings. On dark bands the closing phrase is amber.
- **Phone Display** (Cal Sans 400, clamp 30 to 52px, line-height 1): the big tap-to-call number in the closing band.
- **Title** (Cal Sans 400, clamp 19 to 22px, line-height 1.2): service rows and the Facebook link card. Fixed Cal Sans steps of the same family: 21px (22px on wide screens) for step titles and the brand name (24px wide), 22px for photo captions, 20px for step numbers, 18px for buttons, 17px for field labels and the header phone (20px wide).
- **Lede / Promise** (system 400, clamp 17 to 19px and 17 to 20px): the line under a heading (Soft, max 38ch) and the hero tagline (line-height 1.5).
- **Body** (system 400, 16px, line-height 1.7): all running text.
- **Label** (system 600, 14px, 0.08em, uppercase): service group headings on green. The brand's sub-line uses the same treatment at 12px.
- **Small** (system 14 to 15px): field hints (14px), error and after-send notes (15px).

### Named Rules
**The Cal Sans Speaks Rule.** Anything a visitor reads as a name, a heading, an action or a service is Cal Sans at 400. Explanations are system sans. No other weights of Cal Sans exist; never fake-bold it.

**The Uppercase Is Rare Rule.** Uppercase with tracking appears only on the service group labels and the brand sub-line. Headings and buttons are sentence case.

## Layout

A single centred column (max 1160px) with a 20px gutter on phones, 40px from 760px up. Bands run edge to edge with 64px of vertical padding, 96px from 760px. Phone first; two breakpoints do the real work:

- **760px:** gutter widens, the hero gains height (112px top, 120px bottom), the hero photo picks up a faint blur, hero buttons sit side by side (min 240px each), and the three work photos go to three columns.
- **1024px:** service groups go two columns (64px gap), the form band splits text and form (1 : 1.2) with a sticky heading, the steps go three across, and the closing band puts the big phone number on the right.

Spacing is loose and round: 8 to 16px inside components, 20 to 36px between a heading and its content, 64px column gaps. Tiny-screen tweaks at 380px and 340px only shrink chips and the header.

## Elevation & Depth

Flat. Depth comes from the band colours, the hero photo under its overlay, and the photo scrims, not from shadows. The one exception is the floating text circle, which floats over everything and gets a soft forest shadow so it reads as above the page.

### Shadow Vocabulary
- **Float lift** (`box-shadow: 0 10px 28px rgba(10,30,18,.3)`): the floating text circle only.

### Named Rules
**The One Floating Thing Rule.** Only the floating text circle casts a shadow. Cards, buttons, fields and rows stay flat at rest and on hover.

## Shapes

Soft and round everywhere. Cards and the Facebook link card use a generous 24px corner; buttons, chips, and the floating circle are full pills or circles; fields use a smaller 10px corner so they read as places to type, not buttons. Arrows, step numbers and the float are perfect circles. Focus outlines carry a 6px corner. Photos are clipped by their card's corner. No hard corners and no visible borders at rest; the only rules are 1px hairlines between service rows on green.

## Components

### Buttons
- **Shape:** full pill (999px), 56px tall, 26px side padding, Cal Sans 18px, optional 20px icon.
- **Primary:** Maple Amber fill, Forest Ink text. Full width in the form.
- **Hover / Focus:** hover lightens to Amber Light (pointer devices only); press scales to 0.98. In the form the hover and focus add a 2px Forest Green outline.
- **Ghost:** transparent with a 2px on-dark border at 70% and on-dark text, used beside the primary on the hero. Hover brings the border to white with a 10% white wash.

### Chips
- **Style:** pill, 48px tall, Field Mist fill, ink text, 2px transparent border. They are radio choices for the job type.
- **State:** hover shows a Forest Green border; selected flips to a Forest Ink fill with white text and a drawn check mark.

### Cards / Containers
- **Corner Style:** 24px.
- **Background:** the form card is Card White on Paper; photo cards sit on Deep Forest with a bottom scrim; the Facebook link card is Forest Green.
- **Shadow Strategy:** none (see Elevation).
- **Border:** none.
- **Internal Padding:** the form scales 20 to 32px; photo captions sit 20px in from the left.

### Inputs / Fields
- **Style:** Field Mist fill, 2px transparent border, 10px corners, 52px tall (textarea 120px), 16px system text in ink, soft placeholders.
- **Focus:** the border turns Forest Green on hover and on focus; no glow.
- **Error:** the border and a 15px message turn Error Red.

### Navigation
A paper header (64px, 76px wide): the leaf-over-roofline mark in Forest Green with "Maple" in Cal Sans and "Outdoor Builds" in small uppercase beneath, and a tap-to-call number with an amber-ink phone icon top right. There is no menu. The footer is Deep Forest with line texture; its links are on-dark and turn amber on hover, each at least 44px tall.

### Service Rows
Each service is a full-width Cal Sans link row (64px minimum) with a 44px round arrow at the right, separated by faint white hairlines. Only the arrow reacts: on hover or focus it fills amber with an ink arrow. The row itself never highlights. The Facebook link card reuses the same arrow behaviour.

### Step Numbers
"How it works" numbers are 48px amber discs with a Cal Sans ink numeral, beside a Cal Sans title and a body line.

### Floating Text Circle
One 60px amber circle with an ink chat icon, fixed bottom right inside the safe area. It slides up into place (0.35s) once the hero has scrolled away. It is always a circle, never a bottom bar.

### Motion
- **Hero headline bounce-in:** each letter slides in from 50px right with a slight overshoot (1s, cubic-bezier(.34,1.56,.64,1)), 20ms apart. It runs once, only after Cal Sans has loaded (900ms limit), and is skipped under reduced motion.
- **Rise:** content below the first screen fades up 12px (0.4s ease-out), once. Nothing already on screen animates.
- **State transitions:** 0.2s for buttons and arrows, 0.15s for fields and chips.

## Do's and Don'ts

### Do:
- **Do** keep every band on Paper, Forest Green, or Deep Forest with its faint line texture.
- **Do** put Forest Ink on amber, and use Amber Ink whenever amber has to be text on a light ground.
- **Do** set names, headings, buttons and services in Cal Sans 400, and running text in the system sans at 16/1.7.
- **Do** use pill buttons (56px) and pill chips (48px), 10px fields on Field Mist, and 24px cards.
- **Do** put photos under a deep-forest overlay or a bottom scrim when text sits on them.
- **Do** make service rows react only through their round arrow.
- **Do** outline form controls in Forest Green on hover and focus; use an amber outline on dark bands.
- **Do** keep motion to the hero letter bounce-in, one 12px fade-up below the first screen, and the floating circle's slide-in, all switched off under reduced motion.

### Don't:
- **Don't** fill a band, card or large area with amber, or set amber text on Paper.
- **Don't** add shadows to cards, buttons, fields or rows; the floating text circle is the only lifted thing.
- **Don't** highlight a whole service row on hover; only the arrow changes.
- **Don't** turn the floating text circle into a bottom bar or add a second floating control.
- **Don't** use bold Cal Sans or uppercase headings.
- **Don't** add hover states for touch: hover styles live only under a real pointer.
