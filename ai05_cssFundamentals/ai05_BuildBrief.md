# ai05 Build Brief: Style Without Sight

**Pairs with html05 (CSS Fundamentals).**

## What to build

Direct Claude to style your three-page site with a single **external stylesheet**:

- One `styles.css` linked from every page — zero inline styles, zero style blocks
- A deliberate color scheme (3–4 colors) and two fonts (heading + body)
- Styled links including a `:hover` state
- Element, class, AND id selectors all used somewhere, on purpose

Here is the interesting part of this track's method: styling gets directed by *specification*, the way an art director directs a photographer — you define the palette, the mood, and the rules, and you verify by tracing claims back to code. CSS is the presentation layer, and your AudioLab this week proves it changes nothing about the page's structure or meaning.

## The must-say list

- **external stylesheet** and the `link` element that attaches it
- the three places CSS can live (inline, internal, external) — and your directions must say WHY external
- **selector** types: element, class (`.`), id (`#`)
- color values (direct specific hex codes or named colors — pick them by their descriptions; ask Claude to describe the personality of a palette)
- `font-family` with a fallback stack
- `:hover` — and note it belongs to CSS, not JavaScript

## The twist

Ask Claude: "Describe my site's appearance in full detail — colors, fonts, spacing, mood — as if writing the description for a design review." Then ask it the same question about a version with no CSS. Save both descriptions in your prompt log. Comparing them shows exactly what styling *does* — and getting precise visual descriptions out of an AI is a specification skill you'll use all year.

## What to commit

Updated site + `styles.css`, `ai05_PromptLog.md`, completed ConceptCheck and AudioLab.
