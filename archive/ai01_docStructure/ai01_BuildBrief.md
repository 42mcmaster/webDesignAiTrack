# ai01 Build Brief: The About Me Page

**Pairs with html01 (Document Structure).** Your first real build — the same About Me page the main course starts with, built by direction.

## What to build

Direct Claude to build a complete, valid About Me page:

- The full HTML5 skeleton: doctype, html, head, body
- In the head: a title (your name plus something), the charset declaration, and the viewport tag
- One heading level one — your name
- At least two heading level twos for sections (interests, goals, favorite anything)
- Real paragraphs under each — dictate actual content about yourself; a page of placeholder text is a failed build
- An HTML comment near the top with the date and "built by direction"

## The must-say list

Your directions must use these by name — this is week one of the vocabulary being the curriculum:

- **doctype** — and ask Claude what happens without it; the answer goes in your prompt log
- **head** versus **body** — direct content into the right one and say why ("put the title in the head; the heading goes in the body — they're different things")
- **title** — and how it's different from a heading level one
- **charset** and the **viewport** tag (describe-level is fine: say what each is for as you ask for it)
- **heading levels** — one h1, h2s below it, no skipping
- **paragraph** elements — not line breaks pretending to be paragraphs
- **comment**

## The twist

After the build, say: "Read me the page one line at a time, and after each line, one short sentence on what that line does." Save that annotated walk-through into your prompt log. By the end you can explain every line of an HTML document you never typed — which is the point of the whole track.

## What to commit

- `aboutme.html`
- `ai01_PromptLog.md` (including the line-by-line walk-through)
- Completed `ai01_AudioLab.md` and `ai01_ConceptCheck.md`
