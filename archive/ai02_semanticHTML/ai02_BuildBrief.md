# ai02 Build Brief: A Page With Real Structure

**Pairs with html02 (Semantic HTML & Text Formatting).**

## What to build

Direct Claude to build a one-page website about a topic you actually care about — a band, a team, a game, a cause. One HTML file, no CSS yet. The page needs:

- A banner area with the site title
- A navigation area with four placeholder links
- A main content area with two distinct sections, each with its own subheading, paragraphs, and one list (one ordered, one unordered — decide which content deserves which and be ready to say why)
- A footer with contact-ish info
- At least one use of emphasis and one of strong importance inside the text

## The must-say list

Your directions to Claude must use these by name. That's the graded skill:

- `header`, `nav`, `main`, `section`, `footer`
- heading levels — one `h1`, with `h2` for section headings (say why only one h1)
- `ol` versus `ul` — and your reason for which content gets which
- `strong` versus `em` — and what each *means*, not what it looks like

## The twist (do not skip)

First drafts from AI often use generic containers where semantic elements belong. After the first build, ask Claude: "Did you use any div where a semantic element would be more appropriate? List them and fix them." Save its answer — that exchange is part of your deliverable.

## What to commit

- `index.html` — the final page
- `ai02_PromptLog.md` — your directions and the key exchanges (ask Claude to compile the transcript into this file for you)
- Your completed `ai02_AudioLab.md` and `ai02_ConceptCheck.md`
