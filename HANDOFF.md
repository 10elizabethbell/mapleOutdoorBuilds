# Maple Outdoor Builds — handoff at ~60%

**Live:** https://10elizabethbell.github.io/mapleOutdoorBuilds/ · **Repo:** https://github.com/10elizabethbell/mapleOutdoorBuilds · **Built:** 2026-10-17 from Muse brief 2026-10-17 (Facebook group post, Essex County Contractor Referrals)

## What's built
- **World:** an October deck in Saint John. The hero is a painted canvas deck (boards with grain, knots, screw lines) covered in maple leaves. Leaves keep falling, wind gusts sweep a lane now and then, and a finger or mouse blows them off the boards (drag works up, down and sideways on phones; the page doesn't scroll or pull-to-refresh). It ties together decks, cleanups and the maple brand.
- **Carried through:** the before/after photos are laid on the same boards as prints, with leaves that spring away from the pointer; a board strip with leaves sits above the quote form.
- **Sections:** header (leaf-over-roof mark, number top-right) → "Built right. Left clean." + 2 buttons → What we do (Decks / Yards & cleanups; each row opens a text naming the service) → Before & after + "Click to see more of our work" (Facebook) → How it works → Where we work → "Send us a photo." quote form → footer.
- **Contact:** everything goes to text at 506-607-1818 (`sms:+15066071818?&body=…`). The form composes the job, town, details and name into the text. On desktop (mouse), the hero text button scrolls to the form instead, since desktops usually can't send texts. The number only appears top-right on the first screen.
- Facebook preview image `og.jpg` (1200×630), home-screen icon, SVG favicon from the leaf mark. Photos are separate WebP files in `img/` loaded lazily (lighter than base64 on cellular).
- Tunables are named at the top of each block in the script: `HERO` (leaf counts, sizes, gust strength, blower radius, refill), `SPRING`, `DECK` (board colours).

## Assumptions I made
- **Decks first.** The brief's services came from one post caption (cleanups, junk removal, deck repairs), but their Facebook page description is "decks, repairs, railings, and extensions starting in St. John" and their profile image lists new decks, repairs & rebuilds, stairs, railings, extensions and resurfacing. I list both groups and lead with decks.
- **Green, not red.** The brief said "maple-leaf red" from 🍁 emoji, but their actual profile art is deep forest green and cream with a maple leaf over a roofline. I used green and cream, with maple red only as the hover/focus accent and the autumn leaves.
- **Logo is my redraw.** No logo file exists. Their profile image is a flyer reading "MAPLE BUILDERS" with a leaf-over-roof mark; I redrew that mark as SVG and set "MAPLE / OUTDOOR BUILDS" in the site's type. Note the name mismatch ("Maple Builders" vs page name "Maple Outdoor Builds") — I used the page name.
- **"We", not "I".** Their posts say "Send us a message" and "Our craft". Owner name is unknown, so nobody is named.
- **Service area** includes "Also Moncton, Dieppe and Riverview" because their own profile image lists them. Saint John is first, matching the brief and page.
- **Copy I wrote, to confirm with the owner:** "We look after your deck and yard like they're our own" (hero), "We tell you what it needs and what it costs before anything starts" (step 2), "Done properly, start to finish, and the yard left clean" (step 3). "Quality work, one project at a time" and "small jobs welcome" are theirs.
- Headline "Built right. Left clean." is mine (building + cleanups in one line).

## Placeholders and gaps
- **Photos:** only three stills, taken from their 2026-10-17 before/after video (720px wide, so they can't go bigger). The before and after are different shots, not the same framing, so there's no before/after slider. The photos in their profile flyer look AI-generated, so I didn't use any of them.
- No email (footer has none), no hours, no reviews, no prices, no owner name, no years in business: all left off the page.
- No Instagram or Google Maps listing.

## Questions for the owner
- More job photos, especially true before/after pairs shot from the same spot (that unlocks the drag slider).
- Your first name, so the page can say who they'll be dealing with?
- Is the business "Maple Outdoor Builds" or "Maple Builders"? Do you have a logo file?
- Email address for the footer?
- Do you really cover Moncton/Dieppe/Riverview, or mainly Saint John, Rothesay, Quispamsis, Grand Bay-Westfield?
- Which matters more right now: deck work or cleanups/junk removal? (Changes the headline and service order.)
- Insured? Any reviews from customers you could share word for word?

## Ideas not built (yours to pick)
- **Runner-up world:** plane shavings — dragging across a weathered grey board planes it back to fresh wood, curls of shavings flying off (deck resurfacing as the gesture).
- Closing headline alternative: their own flyer line "Let's build something great." (both Impeccable reviewers called it generic, so I swapped it for "Send us a photo.").
- Leaves pushed hard on the work panel could break free and blow off, like the foam bubbles on Blessed.
- A small leaf pile that gathers at the edge where you sweep, instead of leaves disappearing off the deck.
- Before/after slider once a matched pair exists.
- og image could use a painted canvas deck with leaves instead of flat CSS boards.
- A short winter variant (snow on the deck) after November, if the owner does snow clearing.

## Impeccable
- Detector: fixed all-caps body and tightened the type scale. Recorded file-scoped ignores in `.impeccable/config.json` for the system font (Ellie's house style), cream ground (client's own brand colour), repeating stripes (deck-board fallback before the canvas paints) and flat type hierarchy (detector only sees fixed sizes; headings use clamp at 34–96px).
- Finish reviewer + every mode except live/onboard/init/document/extract/shape: applied the gust fix (one gust cleared the whole phone deck), shorter phone deck so the next section peeks, 360px header, figure margins, a11y error announcements, real `sms:` hrefs in the HTML, reduced-motion behaviour (nothing moves on its own; drag still works), debounced resize, desktop headline/footer/steps layout.
- Checked by hand against `finishing-rules.md` afterwards.

## Not verified
- Real-device touch (tested with emulated touch in Chromium; layout also checked in Playwright WebKit).
- Real SMS handoff on iOS and Android, especially the multi-line form body inside Facebook's in-app browser.
- Frame rate on older phones (phone caps: 90 leaves, canvas at 1.5× pixel ratio).
