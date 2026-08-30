# ai07 Audio Lab: Visual Order vs. Reading Order

## Step 1 — The reversed nav.

With `row-reverse` applied (the brief's twist): pull up the links list and tab through the nav. What order does the audit report? Now ask Claude what order the links appear in visually. Write both orders side by side.

**Findings:**

## Step 2 — Name the principle.

You just demonstrated something WCAG has a rule about: CSS can rearrange what appears on screen without changing the source — so the audited order and the visual order disagree. Imagine instructions that say "click the last link in the menu" — which "last"? Write four sentences on why source order should stay logical and CSS reordering should be used sparingly. Then have Claude remove the row-reverse.

**Findings:**

## Step 3 — The wrap check.

The card row wraps on narrow screens — a purely visual event. Confirm by audit that wrapping changes nothing: same reading order, same content, narrow or wide. (Ask Claude to describe the two visual states so your prompt log captures both sides.)

**Findings:**

## Step 4 — Template audit.

Open `template.html` and audit it: a nearly empty page, but the SKELETON should already pass every structural check in this track — regions present on the region walk, one h1 placeholder in the headings list, skip link as the first tab stop. If the template passes, every future page starts life correct. That's the point of templates.

**Findings:**

## Verdict

Two sentences: what can CSS change about order, and what can it never change?
