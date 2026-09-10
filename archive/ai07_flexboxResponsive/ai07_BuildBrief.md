# ai07 Build Brief: Responsive — and the Order Trap

**Pairs with html07 (Flexbox & Responsive Design).**

## What to build

Direct Claude to make your site genuinely responsive:

- The viewport meta tag on every page (ask Claude to check — it may already be there; verifying beats assuming)
- A flexbox nav bar and a flexbox card row that **wraps** on narrow screens
- **Mobile-first media queries**: base styles for phones, a `min-width: 768px` query that moves to the wider layout
- The responsive image rule applied site-wide
- A saved `template.html` — your bare page skeleton (header, nav, main, footer, stylesheet link, viewport tag) that every future page starts from

## The must-say list

- **viewport meta tag** — and what breaks on phones without it
- **flexbox**: `display: flex`, `justify-content`, `align-items`, `flex-wrap`, `gap`
- **mobile-first** and **media query** with `min-width`
- `max-width: 100%` for images
- **template** (that's competency 6.5.6 — creating one is a state skill)
- Grid, once, at recognition level: ask Claude to explain in two sentences how Grid differs from flexbox; put its answer in your prompt log

## The twist

Ask Claude: "Use `flex-direction: row-reverse` on my nav so the links display in reverse order — but don't touch the HTML." Visually, the links now run backward. What does the audit report? That's the AudioLab.

## What to commit

Responsive site + `template.html`, `ai07_PromptLog.md`, completed ConceptCheck and AudioLab.
