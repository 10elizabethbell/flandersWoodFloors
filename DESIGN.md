---
name: Flanders Wood Floors & Construction
description: Calm paper-and-navy bands with one honey-oak accent, for a northern-NJ flooring crew.
colors:
  navy: "#1e3a5c"
  deep: "#132840"
  oak: "#d9a25a"
  oak-light: "#e6b878"
  oak-ink: "#875016"
  paper: "#f4f6fb"
  card: "#ffffff"
  field: "#e6ecf5"
  body: "#2a3748"
  soft: "#4a5668"
  on-dark-soft: "#c8d4e4"
  error: "#b3261e"
typography:
  display:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "clamp(42px, 12vw, 84px)"
    fontWeight: 400
    lineHeight: 1.02
    letterSpacing: "-0.005em"
  headline:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "clamp(32px, 8.4vw, 48px)"
    fontWeight: 400
    lineHeight: 1.08
    letterSpacing: "-0.005em"
  title:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "clamp(21px, 5.6vw, 24px)"
    fontWeight: 400
    lineHeight: 1.2
  label:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "18px"
    fontWeight: 400
    lineHeight: 1.2
  lede:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial, sans-serif"
    fontSize: "clamp(17px, 4.6vw, 19px)"
    fontWeight: 400
    lineHeight: 1.7
  body:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial, sans-serif"
    fontSize: "16px"
    fontWeight: 400
    lineHeight: 1.7
  display-landscape:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "clamp(40px, calc(7vh + 20px), 60px)"
    fontWeight: 400
    lineHeight: 1.02
  promise:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial, sans-serif"
    fontSize: "clamp(17px, 4.7vw, 20px)"
    fontWeight: 400
    lineHeight: 1.5
  step-title-desktop:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "22px"
    fontWeight: 400
    lineHeight: 1.2
  wordmark-desktop:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "25px"
    fontWeight: 400
    lineHeight: 1
  wordmark-sub:
    fontFamily: "-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial, sans-serif"
    fontSize: "12px"
    fontWeight: 600
    lineHeight: 1
  tel-narrow:
    fontFamily: "Cal Sans, Avenir Next, Segoe UI, system-ui, sans-serif"
    fontSize: "15px"
    fontWeight: 400
    lineHeight: 1
rounded:
  focus: "6px"
  field: "10px"
  card: "24px"
  pill: "999px"
spacing:
  gutter: "20px"
  gutter-desktop: "40px"
  stack-sm: "16px"
  stack-md: "28px"
  band: "64px"
  band-desktop: "96px"
components:
  button-primary:
    backgroundColor: "{colors.oak}"
    textColor: "{colors.deep}"
    typography: "{typography.label}"
    rounded: "{rounded.pill}"
    padding: "0 26px"
    height: "56px"
  button-primary-hover:
    backgroundColor: "{colors.oak-light}"
    textColor: "{colors.deep}"
  button-ghost:
    backgroundColor: "transparent"
    textColor: "{colors.paper}"
    typography: "{typography.label}"
    rounded: "{rounded.pill}"
    padding: "0 26px"
    height: "56px"
  input-field:
    backgroundColor: "{colors.field}"
    textColor: "{colors.deep}"
    typography: "{typography.body}"
    rounded: "{rounded.field}"
    padding: "13px 14px"
    height: "52px"
  chip:
    backgroundColor: "{colors.field}"
    textColor: "{colors.deep}"
    typography: "{typography.body}"
    rounded: "{rounded.pill}"
    padding: "0 18px"
    height: "48px"
  chip-selected:
    backgroundColor: "{colors.deep}"
    textColor: "{colors.card}"
  form-card:
    backgroundColor: "{colors.card}"
    rounded: "{rounded.card}"
    padding: "clamp(20px, 5vw, 32px)"
  link-card:
    backgroundColor: "{colors.navy}"
    textColor: "{colors.paper}"
    typography: "{typography.title}"
    rounded: "{rounded.card}"
    padding: "14px 16px 14px 22px"
    height: "84px"
  arrow-circle:
    backgroundColor: "rgba(255,255,255,.1)"
    textColor: "{colors.paper}"
    rounded: "{rounded.pill}"
    size: "44px"
  arrow-circle-hover:
    backgroundColor: "{colors.oak}"
    textColor: "{colors.deep}"
  step-number:
    backgroundColor: "{colors.oak}"
    textColor: "{colors.deep}"
    rounded: "{rounded.pill}"
    size: "48px"
  float-circle:
    backgroundColor: "{colors.oak}"
    textColor: "{colors.deep}"
    rounded: "{rounded.pill}"
    size: "60px"
---

# Design System: Flanders Wood Floors & Construction

## Overview

**Creative North Star: "The Swept Job Site"**

The page should read like a finished room before the crew leaves: everything put away, nothing loud. Full-bleed bands of off-white paper and two navies stack in a calm order, so a new section is obvious without any rule lines or decoration. The only warmth is honey oak, taken from the trade because the business has no logo or brand colours. It shows up as small solid fills on the things you can press: the main button, the step numbers, the arrow on hover, the floating text circle. Cal Sans carries the headings; everything else uses the phone's own system font, so the page loads fast inside Facebook's in-app browser.

Content is sparse and set for phones first: one column, a 20px gutter, big tap targets, and a hero that only holds the claim, one promise and two buttons. There is no photography; the hero is the textured navy band, because no usable job photo could be fetched (HANDOFF.md). Motion is limited to three things: the hero H1 bounces in letter by letter, content below the first screen fades up once, and the floating text circle slides in. All three switch off under reduced motion, and none of them hides content when JS is off.

This build follows the house calm band style (`~/.claude/skills/pitch-site/references/calm-photo-style.md`). Where that file and this one disagree, this file records what the Flanders build actually ships.

**Key Characteristics:**
- Full-bleed bands, alternating paper and navy, with a faint diagonal line texture on the textured dark bands.
- One warm accent (honey oak), used as a fill. On light grounds it only appears as text in its darker oak-ink shade.
- Soft, borderless shapes: 24px cards, full pills, 10px tinted fields.
- One display webfont (Cal Sans, weight 400 only) and a system body at 16/1.7.
- Phone-first: 44px minimum tap targets, 16px inputs, a tap-to-call number always in the header.

## Colors

Cool paper and two deep navies make up nearly every surface, with one honey-oak accent that warms whatever you can tap.

### Primary
- **Harbour Navy** (navy): the main dark band. Used for the textured hero, the "How it works" band, the closing band and the Facebook link card. Also the focus and hover outline colour on the paper and white grounds.
- **Deep Navy** (deep): the darkest band (services and footer, both with the line texture). The same value is the page's ink: headings on light, text on oak fills, and the selected-chip fill.

### Secondary
- **Honey Oak** (oak): the one accent, used **only as a fill**: the primary button, step-number discs, arrow circles on hover or focus, the floating text circle, text selection, the eyebrow dot and the chip pick ring. On dark bands it also colours the accent phrase in a heading, the phone icons, and link hover. It is also the focus outline colour on dark bands.
- **Light Oak** (oak-light): hover state of the primary button only.
- **Oak Ink** (oak-ink): oak as text on light grounds (6.1:1 on paper): the accent phrase in headings on paper bands, the header phone icon, header phone hover.

### Neutral
- **Cool Paper** (paper): page ground, header, the light bands; also the main text colour on dark bands.
- **White Card** (card): the quote form card only.
- **Field Tint** (field): fill for inputs, chips and the "didn't open?" message panel on the white card. It is its own tint because paper on white measured about 1.08:1.
- **Slate Body** (body): running text on light.
- **Slate Soft** (soft): ledes, the wordmark subline, placeholders, "(optional)" hints and helper lines.
- **Mist** (on-dark-soft): running text on navy and deep navy bands.
- **Brick Error** (error): inline error sentences and the error border on a field.
- **Hairline** (`rgba(19,40,64,.12)` on light, `rgba(255,255,255,.12)` on dark): the only line in the system, used for the 1px rules between service rows.

### Named Rules
**The Oak Is a Fill Rule.** Honey oak is a fill, and text on it is always deep navy. When oak has to be text on paper or white, use oak-ink. Oak text is allowed only on the navy and deep bands.

**The No-Black Rule.** The darkest colour is deep navy. Nothing on the page is black, including the ground, text and shadows (the float shadow is a navy-black `rgba(10,20,36,.3)`).

## Typography

**Display Font:** Cal Sans, from Google Fonts with preconnect and `display=swap` (falls back to Avenir Next, Segoe UI, system-ui)
**Body Font:** the system stack (-apple-system, BlinkMacSystemFont, Segoe UI, Helvetica Neue, Arial)

**Character:** Cal Sans is round, solid and friendly without being cute, like a hand-painted van door. The system body keeps reading text native and fast. Cal Sans is only ever set at weight 400; hierarchy comes from size, never from weight.

### Hierarchy
- **Display** (400, clamp(42px, 12vw, 84px), 1.02): the hero H1 only, white, max 11ch, with the place name as the accent phrase. Landscape phones (760px+ wide, 520px or less tall) drop it to clamp(40px, 7vh + 20px, 60px) so the H1 and buttons stay on the first screen.
- **Headline** (400, clamp(32px, 8.4vw, 48px), 1.08, -0.005em, balanced wrap): section H2s. On paper the last phrase can be oak-ink; on dark bands it is oak.
- **Title** (400, clamp(21px, 5.6vw, 24px), 1.2): service rows, the Facebook card label, step titles (21px, 22px at 1024px and up).
- **Label** (400, 18px): buttons, form labels and legends, the header phone number (18px, 20px on desktop). The wordmark is the same face at 22px (25px on desktop).
- **Lede** (system, clamp(17px, 4.6vw, 19px), 1.7, soft, max about 38 to 42ch): the one supporting paragraph under a section heading. The hero promise is the dark-band version (clamp(17px, 4.7vw, 20px), 1.5, max 30ch on phones).
- **Body** (system, 16px, 1.7): running text, inputs, chips, errors, the footer. Inputs are never under 16px.
- **Small** (system, 600 weight, 12px, 0.06em, uppercase): the wordmark subline "Wood Floors & Construction" only. 14px for "(optional)" hints.

### Named Rules
**The One Display Face Rule.** Cal Sans covers headings, buttons, labels and phone numbers; the system stack covers everything else. Don't add a third family, and don't use any weight of Cal Sans other than 400.

**The Big Number Rule.** The phone number is set in the display face wherever it's a main action (the header, and the closing band at clamp(30px, 9vw, 52px)), always with `white-space: nowrap` so it never breaks.

## Layout

The page is a single column of full-bleed bands, with content held in a 1160px max wrap behind a 20px gutter (40px from 760px). Bands are padded 64px top and bottom (96px from 760px); the hero uses its own 56/64px padding (112/120px on desktop). Inside a band, a heading block is followed by its content 28 to 36px below, and grid gaps run 16, 20, 24 and 28px.

**Band order (as built):** paper header, textured navy hero, textured deep services band, paper care and Facebook band, navy "How it works", paper quote form, navy close, textured deep footer. The hero and services are adjacent dark bands told apart by tone and texture; from services on, paper and navy alternate strictly.

**Responsive steps:** 340px and 380px tighten the header (smaller number, then no phone icon) and chip padding. Below 520px the wordmark subline wraps to two lines so the number keeps its gutter. At 760px the gutter, band padding and hero padding grow, and the hero buttons sit side by side (240px minimum). At 1024px the service rows become two columns (64px column gap), the care band splits 1.2fr / 1fr, the steps run three across, the form centres at 640px, and the closing band puts the big number to the right of its text.

**The Phone First Rule.** Every layout starts as one column at 390px. Desktop only adds columns; it never adds content.

**The 44px Rule.** Every tap target is at least 44px (buttons 56px, chips 48px, fields 52px, footer links 44px).

## Elevation & Depth

The system is flat. Depth comes from the bands' tone (paper, navy, deep navy) and from the faint 135° line texture (`repeating-linear-gradient(135deg, transparent 0 22px, rgba(255,255,255,.035) 22px 23px)`) on the hero, services and footer. Cards sit on their bands by colour alone: the white form card on paper, the navy Facebook card on paper.

### Shadow Vocabulary
- **Float lift** (`box-shadow: 0 10px 28px rgba(10,20,36,.3)`): the floating text circle only, because it's the one thing that sits over other content.
- **Pick ring** (`0 0 0 0 → 0 0 0 10px` of oak at 0.9 → 0 alpha over 0.6s): a short-lived ring on a chip that a service row has just selected. It isn't a resting shadow.

### Named Rules
**The Flat Band Rule.** Surfaces never have a shadow. The only resting shadow belongs to the floating circle. Show separation by changing the band, not by lifting a card.

**The Quiet Texture Rule.** The line texture stays at 3.5% white or fainter, and only on dark bands, so it never reads as lines through the text.

## Shapes

Soft and borderless. Containers have a 24px radius (the form card, the Facebook card), fields and the message panel 10px, and every button, chip and circle is a full pill or circle. Borders appear only as a state: a 2px transparent border on buttons, fields and chips turns navy on hover or focus and brick on error. The ghost button is the one resting outline (2px paper at 70%). The only structural lines are the 1px hairlines between service rows. Focus is a 3px outline offset 3px with a 6px radius: navy on light, oak on dark.

## Components

### Buttons
Big, round and plain.
- **Shape:** full pill, 56px tall, 26px side padding, Cal Sans 18px, an optional 20px icon with a 10px gap.
- **Primary:** honey oak fill with deep navy text; full width inside the form.
- **Hover / Focus:** primary lightens to light oak (with a real pointer only). Inside the form, hover and focus add a 2px navy outline offset 2px. Pressing scales to 0.98 over 0.12s. Colour transitions take 0.2s.
- **Ghost:** transparent with a 2px paper border at 70% and paper text, used only on the hero next to the primary. On hover the border turns full white over a 10% white wash.
- **Copy button:** a 44px pill with a 2px deep-navy outline, transparent, Cal Sans 16px, used in the "didn't open?" panel.

### Chips
- **Style:** a 48px pill in the field tint with deep navy body text (16px) and 18px padding, wrapping with a 10px gap. A visually hidden checkbox or radio does the work.
- **State:** hover shows a 2px navy border. Selected fills deep navy with white text, and checkbox chips add a drawn tick. Hovering a selected chip shows a navy outline offset 2px, because a border can't be seen on the ink fill. Keyboard focus is a 3px navy outline offset 3px. A radio chip that is already selected clears when you tap it again.

### Cards / Containers
- **Form card:** white, 24px radius, padding clamp(20px, 5vw, 32px), 20px between fields, max 600px.
- **Facebook link card:** navy, 24px radius, at least 84px tall, an oak 30px Facebook mark, Title type, and an arrow circle on the right. Max 520px on desktop.
- **Message panel:** field tint, 10px radius, 16px padding. It holds the composed text in a pre-wrapped block and appears only if no messages app opened after 900ms.

### Inputs / Fields
- **Style:** field tint fill, a 2px transparent border, 10px radius, 13px 14px padding, at least 52px tall (textarea 120px, resizes vertically), 16px deep-navy text, slate-soft placeholders, navy caret.
- **Focus / Hover:** the border turns navy, with no glow.
- **Error:** an inline plain sentence in brick below the field, and a brick border that wins over focus. Errors show only after submit, and `aria-describedby` is set only while the error shows.

### Navigation
- **Header:** paper, not sticky, 64px tall (76px on desktop), respects the top safe area. On the left a two-line wordmark ("Flanders" in Cal Sans over the uppercase system subline); on the right the tap-to-call number with an oak-ink phone icon that turns oak-ink on hover. There is no menu.
- **Footer:** textured deep navy, Mist text, with the legal name, the area, the number (nowrap) and a Facebook link as a 44px tall row. Links turn oak on hover. The bottom padding (96px plus safe area) leaves room for the floating circle.

### Service Rows
The services as one long list on deep navy. Each row is a link at least 68px tall in Title type, with a hairline above (and below the last), and a 44px arrow circle on the right at 10% white. **Only the arrow reacts:** on hover or focus it fills oak with deep-navy arrow; the row itself gets no background, outline or shadow. Two columns at 1024px. Tapping a row jumps to the form, ticks the matching chip and plays the oak pick ring on it.

### Steps
A numbered list on navy: a 48px oak disc with the deep-navy number in Cal Sans 20px, a title in Title type and one line of Mist body. Stacked with a 24px gap on phones, three across with a 40px gap at 1024px.

### Hero
A textured navy band holding the H1, one promise line and at most two buttons (primary "Get a free estimate", ghost "Text us a photo" opening `sms:`). It has no call button, because the number is in the header. **H1 bounce-in:** JS waits up to 600ms for Cal Sans, then splits the H1 into letters inside nowrap word wrappers, keeping its measured line breaks. Each letter goes from `opacity:0; translateX(50px)` to rest over 1s `cubic-bezier(.34,1.56,.64,1)`, 20ms apart. The H1 carries an `aria-label` during the animation, and the plain HTML is restored on the last `animationend`. Without JS, with reduced motion, or if the font is late, the plain heading shows immediately. This is used on the hero H1 only.

### Closing Band
Navy: the business name as an H2 with "& Construction" in oak, a one-line offer in paper, a service-area line in Mist, and the big phone number in Cal Sans with an oak phone icon. The number turns oak on hover. On desktop the number sits to the right, aligned to the bottom.

### Floating Text Circle
A 60px oak circle with a deep-navy chat icon, fixed bottom-right and inset 16px plus the safe area. It opens `sms:` with a pre-filled message. It slides up from 120px below over 0.35s `cubic-bezier(.2,.8,.2,1)` once the hero has scrolled away, and hides again while the services band or the quote form is in view. While hidden it has `tabIndex=-1` and `aria-hidden`. Its focus ring is white with an 8px deep-navy halo. There is only ever this one circle, never a bottom bar.

### Fade-Up
Elements marked to rise start in place and visible. Only elements that begin below the first screen get a hidden state (opacity 0, 12px down) and ease up over 0.4s as they enter, triggered 8% before the bottom of the screen. The hidden state is removed once and never comes back. With reduced motion, without JS, or without IntersectionObserver, nothing is ever hidden.

## Do's and Don'ts

### Do:
- **Do** use honey oak only as a fill, with deep navy text on it; switch to oak-ink for oak text on paper or white.
- **Do** separate sections by changing the full-bleed band, and keep the 135° line texture at 3.5% white or fainter on dark bands only.
- **Do** keep Cal Sans at weight 400 and limit it to headings, buttons, labels, the wordmark and phone numbers; set body text in the system stack at 16/1.7.
- **Do** give fields and chips the field tint fill on the white card, and show hover and focus as a navy border or outline (oak on dark bands).
- **Do** keep every tap target at 44px or more, and inputs at 16px or more.
- **Do** keep the phone number tappable in the header and in the display face wherever it appears as an action, with `white-space: nowrap`.
- **Do** switch off the H1 bounce-in, fade-up, float slide and pick ring under `prefers-reduced-motion`, and keep everything visible without JS.

### Don't:
- **Don't** put white text on oak, or oak text on paper or white; both fail contrast.
- **Don't** add shadows to cards, rows or buttons; the floating circle's lift is the only resting shadow.
- **Don't** add hover backgrounds, outlines or lifts to service rows or the Facebook card; only the arrow circle changes.
- **Don't** give any heading other than the hero H1 a letter animation, and don't add parallax, carousels or count-up counters.
- **Don't** add a second floating control or a bottom bar, or show the floating circle while the form is on screen.
- **Don't** use black anywhere; the darkest value is deep navy.

## House-style exception: eyebrow pills

Two quiet eyebrow pills ("Free estimates", above the hero H1 and the form heading) ship by Ellie's choice (calm-photo-style.md item 5): 14px, oak dot, faint tint, no hover, no arrow, no shadow. Impeccable bans eyebrows, so they are recorded here as an exception, not a token.
