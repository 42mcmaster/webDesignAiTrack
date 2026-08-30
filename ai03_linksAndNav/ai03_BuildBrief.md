# ai03 Build Brief: A Site You Can Actually Get Around

**Pairs with html03 (Links & Navigation).**

## What to build

Direct Claude to expand your ai02 page into a **three-page site**: home, about, and one topic page of your choice. Requirements:

- Every page shares the same nav, and every nav link works in both directions
- The about page is long enough to need **in-page anchors**: a small table of contents at the top that jumps to three sections further down
- The footer gains an **email link** that opens a mail message with a subject line already filled in, and a **download link** to a small text file
- Every page starts with a **skip link** to the main content (you know why better than anyone)

## The must-say list

- the `a` element and its `href` attribute
- **relative link** versus **absolute link** — direct Claude to use relative links between your pages, and be ready to say why that matters when the site moves
- **anchor / fragment** links: `id` on the target, `#` in the href
- `mailto:` with a subject parameter
- the `download` attribute
- link text quality: no "click here" — every link's text must say where it goes

## The twist

Ask Claude to write one nav using "click here"-style link text, run the links-list audit on it, then make Claude fix it. Keep both versions of that exchange in your prompt log — the audit makes the difference obvious, and that's the lesson.

## What to commit

- `index.html`, `about.html`, your topic page, the downloadable file
- `ai03_PromptLog.md`
- Completed `ai03_AudioLab.md` and `ai03_ConceptCheck.md`
