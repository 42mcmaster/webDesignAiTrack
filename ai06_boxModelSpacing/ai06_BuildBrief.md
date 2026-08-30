# ai06 Build Brief: Space, Boxes, and the Secret Third Way to Hide Things

**Pairs with html06 (Box Model & Spacing).**

## What to build

Direct Claude to give your site real layout polish:

- Consistent spacing: content padded away from edges, paragraphs breathing, a centered main column with a maximum width
- A "card" component used at least three times (a box with padding, a border, and margin between cards)
- A styled hover state on the cards (CSS, of course)
- One **sticky header** that stays put while the page scrolls

## The must-say list

- the **box model**, by its rings: content, padding, border, margin — your directions must use these words for WHERE space goes ("more padding inside the cards, more margin between them" — those are different requests!)
- `max-width` and centering with `margin: auto`
- shorthand order — if you direct "margin: 1rem 2rem," say what each value hits
- `position: sticky`
- `display` values: block, inline, none

## The twist

Ask Claude: "Show me three different ways to hide an element with CSS: `display: none`, `visibility: hidden`, and the off-screen 'sr-only' technique. Build a demo page with one paragraph hidden each way, plus one visible control paragraph." That demo page is your AudioLab specimen — and the third technique shows up on nearly every professional site on the web.

## What to commit

Updated site + the hiding-demo page, `ai06_PromptLog.md`, completed ConceptCheck and AudioLab.
