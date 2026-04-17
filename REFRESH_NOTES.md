# Brand Refresh — Session Sign-In Sheet (Feb 2026 palette)

This branch contains a visual refresh of the Session Sign-In Sheet handout to match the **Feb 2026 brand palette** used on [collaboratingwellness.com](https://collaboratingwellness.com).

## What changed

### Visual / brand
- **Palette migrated** from retired colors (champagne `#fdfae9`, champagne gold `#e6d8a2`, dusty bg `#f4f0ed`, pale rose `#f0e8e6`, silver-gray `#D1D5DB`) to the Feb 2026 palette:
  - Deep Charcoal `#374151` (text/structure)
  - Dusty Rose `#D8A2A0` (warm accent, CTA emphasis, underlines)
  - Luminous Pearl `#F0ECF7` (highlight box backgrounds)
  - Dusty Lavender `#C4B0D8` (box borders)
  - Blush Lavender `#F5F0F8` (pull-quote / info box bg)
  - Pearl White `#F5F3F8` (page background)
  - Iris `#9B8EC4` (hover states, sparing)
  - Whisper Grey `#EEEEF2` (neutral)
  - Slate `#8B909A` (secondary text)
- **CSS variables** used throughout — future palette updates are a single-source change
- **Section underlines** now dusty rose (was silver)
- **Journal boxes** now luminous pearl + dusty lavender border (was pale rose + silver)
- **Info box** now blush lavender + dusty rose border (was champagne + gold)
- **Buttons** now branded pills (primary: dusty rose; ghost: whisper grey; danger: white with rose outline)
- **Share modal** uses branded options instead of Tailwind blue/green/purple palette
- **Gradient divider** added before the thank-you message (matches brand box-component pattern)
- **Modal backdrop** softened to charcoal at 45% with light blur (was black at 50%)
- **Softer shadows** throughout (using charcoal-tinted rgba instead of plain black)

### Structural improvements
- **Semantic HTML** — `<main>`, `<section>`, `<header>`, `<footer>`, `<aside>` where appropriate
- **Labels wrap checkboxes** for better accessibility (entire feeling word is a click target)
- **ARIA labels** added on close button and icon-only elements
- **Focus styles** explicit (dusty rose ring) for keyboard users
- **OG meta tags** added for nicer link previews when clients share the URL
- **Meta description** added
- **Print CSS polished** — cleaner output when clients print

### Content (light touch only)
- **Title** updated: "Session Sign-In Sheet — Janice LaFountaine, LMFT" (was "- Collaborating Wellness")
- **"Client Name" → "Your Name"** (warmer, client-facing voice)
- **Closing message** softened: *"What you share here helps me meet you where you are."*
- **Footer added** with attribution + link back to [collaboratingwellness.com](https://collaboratingwellness.com)
- **Em-dashes** in range labels (1–10 instead of 1-10) per brand-voice standard

### What was NOT changed
- All **81 feeling-word checkboxes** preserved verbatim
- All **clinical prompts** unchanged
- **Save / share / export / print / clear** functionality — all 15 JavaScript functions preserved
- **localStorage save system** — all `data-key` attributes preserved (94 fields intact)
- **Header logo** — same imgur image

## Testing checklist (for Janice)

- [ ] Open the GitHub Pages preview and see the new look
- [ ] Fill in several fields and reload — confirm auto-save still works
- [ ] Click each of: Share, Export, Print, Clear All — confirm they function
- [ ] Test the Share modal — Email / Clipboard / Download
- [ ] Open on a phone — verify responsive layout
- [ ] Print preview — confirm clean B&W-friendly output
- [ ] If all good → merge `brand-refresh-feb-2026` → `main` to deploy

## After merge

This becomes the reference implementation. The remaining 9 handouts can follow the same pattern.

---

*Branch created 2026-04-17 by Khnum.*
