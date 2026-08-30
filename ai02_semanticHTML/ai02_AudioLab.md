# ai02 Audio Lab: Does the Structure Survive the Audit?

This audit checks the page Claude built for your ai02 brief: the semantic structure (header, nav, main, sections, footer), the headings outline, and your two lists. Have your brief nearby — it's your answer key. For every step: if the page fails, describe the failure to Claude in specific words, have it fix the markup, save, and re-run the step. Note every fix in your findings; the fix cycle is the best part of this lab, not a detour.

**Setup:** open the page in your browser (ask Claude for the steps if needed).

---

## Step 1 — The headings list

**What you're checking:** the page's outline. Your brief called for one heading level 1 (the site title) and a level 2 for each of your two sections. A stranger running this one command should be able to tell what the page is and what's in it — from the list alone.

**Do this:** run your "list all headings" command and arrow through it.

**You should hear:** your site title as the only "heading level 1," then each section's title as "heading level 2," in page order, with no skipped levels.

**If it fails** — say the failure precisely: "The headings list shows [what you heard]. It should be one level 1 called [title] and level 2s called [sections]. Fix the heading elements and save."

**Write what you heard:**

---

## Step 2 — The region walk

**What you're checking:** the page's zones. Your brief required a real header, nav, main, and footer. This move reveals whether Claude used the true semantic elements — because ONLY the real elements announce as regions. Content wrapped in a plain generic container (a div) is invisible to this walk.

**Do this:** go to the top of the page, then press your "next region" command repeatedly.

**You should hear, in order:** "banner," "navigation," "main," "content information" (that's how footers usually announce).

**If a zone is missing from the walk** — say the navigation never announces — the content is probably there but built as a div instead of a nav element. That's exactly the defect this unit exists to catch. Say: "The region walk goes straight from banner to main — the navigation area isn't announcing as a region. Check whether the nav is built with a real nav element, fix it, and save."

**Write what you heard:**

---

## Step 3 — The lists, read in context

**What you're checking:** your brief called for one ordered list (numbered) and one unordered list (bulleted), each chosen to match its content. Real list elements announce themselves ("list of four items") and count along; the ordered one announces numbers.

**Do this:** read continuously through both sections, listening for the list announcements and the counts.

**You should hear:** each list introduced as a list with its item count — and for the ordered list, numbered items ("one: preheat the oven..."). Ask yourself the brief's question one more time as you listen: does the numbered content actually NEED its order? If the numbering sounds arbitrary, you may have chosen the wrong list type — that's a finding about your own direction, and those count too.

**Write what you heard:**

---

## Step 4 — Break it on purpose

**What you're checking:** what the semantic elements were doing for you all along — by taking them away.

**Do this:** say to Claude: "Make a copy of this page called broken.html. In the copy, replace the main element and both section elements with plain divs. Change nothing else. Save it in the same folder." Open broken.html and repeat Steps 1 and 2 on it.

**What you'll find:** the headings list still works (headings are their own elements) — but the region walk loses "main" entirely. Same words on the page, same look in a browser, and a chunk of the page's meaning is just gone. Write three or four sentences: what disappeared from the audit, and what that tells you about why semantic elements exist even though a purely visual check would never notice the difference between the two files.

**Cleanup:** say: "Delete broken.html" (or move it out of the folder) — don't commit it.

**Write your findings:**

---

## Verdict

Two or three sentences: is this page's structure trustworthy, and what was the most important fix you directed this week? Quote the exact fix request you gave Claude — the precision of that sentence is part of the grade.
