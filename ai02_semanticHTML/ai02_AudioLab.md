# ai02 Audio Lab: Does the Structure Survive the Audit?

Run this audit on the page Claude built. Record findings under each step. If a step fails, direct Claude to fix the markup, re-run, and note what changed — the fix cycle is the best part of the lab, not a detour.

## Step 1 — Pull up the headings list.

The headings list alone should tell the page's story — what this page is and what's in it. Record: how many headings, their levels, and whether the story makes sense. Exactly one h1? Levels never skip (no h1 straight to h3)?

**Findings:**

## Step 2 — Walk the regions, from the top of the page.

The region walk should land on: banner (header), navigation, main, and footer — in that order. Record every region announced. If the walk skips something you know is on the page, that content is probably living in a plain div — that's a defect. Name it and send it back.

**Findings:**

## Step 3 — Read the sections straight through.

The lists should announce themselves ("list of five items"), and each list's type should match its content's logic. Does the ordered list actually contain sequenced content?

**Findings:**

## Step 4 — Break it on purpose.

Tell Claude: "Replace the main element and both section elements with plain divs. Save it as broken.html." Run steps 1–2 on broken.html and write 3–4 sentences: what changed in what the audit could find, and what that says about why semantic elements exist. Delete broken.html after (don't commit it).

**Findings:**

## Verdict

Two or three sentences: is this page's structure trustworthy by audit? What was the most important fix you made Claude do?
