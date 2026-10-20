# Flanders Wood Floors & Construction LLC — handoff at ~60%

**Live:** https://10elizabethbell.github.io/flandersWoodFloors/ · **Repo:** https://github.com/10elizabethbell/flandersWoodFloors · **Built:** 2026-10-19 from Muse brief (run 2026-10-20)

On the Call Sheet: yes. The script printed `ADDED`, so Muse hadn't made an entry yet; it's a minimal entry with only the name and site.

## What's built
- One page, phone first, calm band style: paper header (wordmark "Flanders / Wood Floors & Construction", tap-to-call 973-252-9051 top right) → textured navy hero → deep-navy services rows → paper "care" band with the Facebook link → navy "How it works" → paper free-estimate form → navy close with the big number → deep footer.
- Palette (no logo or brand colours exist): paper #f4f6fb, navy #1e3a5c, deep #132840, honey-oak accent #d9a25a (fills only; #875016 as text on light, 6.1:1).
- Hero: plain textured navy. **No photo could be used:** the only images Muse pointed to are the Facebook group posts. Their flyer image/video sits behind a Facebook login; logged-out fetches only return the groups' cover photos (a Clinton mill in snow and a stock office-silhouette picture), which aren't their work.
- H1 "Floors laid right in Flanders, NJ." bounces in letter by letter, then restores the plain heading; `.rise` fade-up below the fold; both off under reduced motion and without JS.
- Free-estimate form: job chips (Hardwood, LVP, Tile, Kitchen, Bathroom, Deck, Something else), town (required), size, timing, notes, name. Submit composes a text to 973-252-9051; if Messages doesn't open, it shows the message with a Copy button and the number. Tapping a service row pre-ticks its chip.
- Floating oak text circle: hidden on the hero and over the services rows, shown below them, hidden while the form is on screen.
- Favicon / home-screen icon: an "F" built from three oak planks on navy (no logo to take a mark from). og image 1200×630 at `img/og.png`.

## Assumptions I made
- **Name:** "Flanders Wood Floors & Construction LLC" rests on Muse's OCR of the flyer, which I couldn't see. Check it against the flyer before showing the owner.
- **Voice "we":** the caption says "dm us", so I wrote it as a crew.
- **Area:** only "the Flanders, NJ area" is on the page. The ads ran in Morris and Hunterdon County groups, so those counties are a likely service area, but I didn't publish them.
- **Services:** hardwood, LVP and tile come from the caption; kitchens, bathrooms and decks come from the flyer (via Muse). I didn't list refinishing, sanding or stairs; they're likely but unconfirmed.
- **Copy about care** ("we lay each one like we'll be living on it ourselves… We take care with the rest of your house while we work") is my wording, not theirs; the owner should approve it. The finish reviewer had me cut "we're not done until you're happy with it" because it reads as a guarantee they never made. Add it back if the owner says it.
- **Texting:** whether the number takes texts is unknown. The page leans on texting (hero button, form, floating circle), and calling stays one tap away in the header, the form fallback, the close and the footer.
- **Facebook link** goes to the poster's personal profile (the only Facebook link known). It's labelled "Click to see more of our work." If they have or make a business page, swap it.

## Placeholders and gaps
- No work photos, no logo, no flyer image (all behind a Facebook login). **Photos wanted:** 3+ finished floors, ideally a before/after pair. With one good photo, the hero should switch to it under the navy overlay.
- Not on the page by design (unverified or unknown): NJHIC#13VH01153400, "Fully insured", owner's name, hours, years in business, email, address, reviews, prices.
- Footer has no email (none known).

## Questions for the owner
- Is the business name exactly as on the page? Do you have a logo file?
- Can customers text 973-252-9051?
- Can we show your NJ home improvement license number and "fully insured"? (Both are strong trust signals once confirmed.)
- Which towns do you cover?
- Do you do refinishing, sanding, stairs or repairs, as well as installs?
- Can you send 5–10 photos of finished jobs (and any before/afters)?
- Is there a Facebook business page, Instagram or Google listing to link?
- Should the site name you (e.g. "Martin")? Ellie's earlier builds found that naming the person helps.

## Ideas not built (yours to pick)
- **Runner-up world, opt-in motion:** a hero where the visitor "lays the floor": dragging across the navy band drops honey-oak planks in a staggered pattern that settles with a slight click, like a floor going down board by board. Other worlds considered: sawdust in a sunbeam, herringbone tiles snapping into place, grout lines drawing in, deck boards under a porch light.
- **Desktop hero right half is empty** with no photo; a real job photo would fill it best. Until then, a quiet drawn plank/herringbone panel could fill it (it must read as a real floor, per the finishing rules).
- Before/after slider module once pairs exist.
- License and insurance line as a trust row under the care copy, once verified.
- **Self-host Cal Sans** (OFL) with a font preload, so the headline appears sooner in Facebook's in-app browser. Right now it waits up to 600ms for Google Fonts, then shows the plain heading.
- A bigger desktop H1 (about 104px) to fill the hero's empty right half (Impeccable's "bolder" pass).
- **Impeccable findings kept on purpose (your calm-style choices):**
  - eyebrow pills (the craft floor bans them outright)
  - the H1 letter bounce-in (its animate and quieter modes reject bounce easing)
  - the floating text circle
  - Cal Sans
  - the diagonal band texture
  The detector's `repeating-stripes-gradient` and `flat-type-hierarchy` findings are ignored for `index.html` in `.impeccable/config.json`. The type one is a false positive: it doesn't count the fluid heading sizes.
- **Footer phone number:** Impeccable wanted it gone because it's on screen at the same time as the big closing number on small phones. I kept it, because the finishing rules let the footer repeat the number.

## Impeccable sweep
I ran 15 modes (audit, critique, harden, optimize, adapt, clarify, typeset, layout, colorize, animate, distill, quieter, bolder, delight, polish) plus the finish reviewer. I skipped live, onboard and extract.

Applied:
- one-column centred form on desktop (the old two-column layout left a dead column)
- tapping the picked "When" chip again clears it
- a no-JS fallback line in the form
- helper text moved under the submit button
- error messages linked to their fields only while showing
- landscape-phone hero sized so it fits the first screen
- header subline wraps on phones, so the number keeps its 20px gutter (it was touching the screen edge at 320–390px)
- type steps consolidated: 12px or larger everywhere, phone h2 starts at 32px
- copy: "What we do.", "Tell us about the job.", one "Free estimates" wording, step 3 no longer repeats the promise
- no accent colour in headings on paper bands
- a short pulse on the chip a service row pre-selects

Checks (Chromium and WebKit, 320–1440px, landscape 844×390):
- no sideways overflow
- tap targets 44px or larger
- inputs 16px or larger
- bounce-in offset mid-way, then settled and restored to the plain H1
- reduced motion and no-JS show everything
- floating circle hidden on the hero, over the services and over the form
- the form's error and text-compose flow works

## Not verified
- Real-device touch, the real SMS handoff on iOS and Android, and Facebook's in-app browser.
- That 973-252-9051 accepts texts.
- Frame rate of the bounce-in on old phones.
