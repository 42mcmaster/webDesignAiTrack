# ai01 Audio Lab: Your First Build Under Audit

In ai00 you practiced the audit moves on a page that was already correct. Now you'll run them on a page YOU directed — which means the "right answers" come from your own build brief. Before each step, remind yourself what you asked Claude for; that's what you're listening for.

**Setup:** open your `aboutme.html` in the browser. If you're not sure how, ask Claude: "Give me steps to open aboutme.html from my ai01 folder in the browser."

---

## Step 1 — The page announcement

**What you're checking:** when a page opens, the first thing a screen reader speaks is the page's title — the one you directed Claude to put in the head of the document. This checks that the title actually made it into the code.

**Do this:** open (or reload) aboutme.html and listen to the first thing spoken.

**You should hear:** the exact title you asked for — something like "About Jordan Smith." 

**If instead you hear** a filename ("aboutme dot html") or something generic like "Untitled Document," the title is missing or wrong in the code. Say to Claude: "When I open the page, the announced title is [what you heard], but I asked for [what you wanted]. Fix the title element and save the file again." Then reload and listen again.

**Write what you heard:**

---

## Step 2 — The headings list

**What you're checking:** your brief called for exactly one heading level 1 (your name) and at least two heading level 2s for your sections. The headings list shows whether Claude delivered that outline — no extras, no missing sections, no skipped levels.

**Do this:** run your "list all headings" command. Arrow through the whole list, noting each heading's text and level.

**You should hear:** your name as "heading level 1," followed by each of your section titles as "heading level 2," in the order you asked for them. Compare it to your brief the way you'd compare a food order to the receipt.

**If something's off** — a section missing, a level wrong, two level 1s — describe it to Claude precisely: "The headings list shows two heading level 1s, but a page should have exactly one. Make my name the only h1 and change the other to an h2. Save and I'll re-check." Precision in these fix requests is a graded skill.

**Write what you heard:**

---

## Step 3 — Read the whole page

**What you're checking:** two things. First, that the paragraphs contain YOUR content — the things you dictated about yourself, not filler text. Second, that the comment you asked for is never spoken. Comments live in the code for developers; visitors never encounter them. This read-through proves both.

**Do this:** go to the top of the page and start continuous reading. Let it run to the end.

**You should hear:** your name, then each section with the sentences you actually dictated, announced as separate paragraphs. **You should NOT hear** the words from your comment ("built by direction") anywhere.

**If you hear filler** ("lorem ipsum" or generic sentences you didn't provide), say: "The paragraphs contain placeholder text. Replace them with the content I dictated earlier — read my sentences back to me first so we can confirm them." **If you hear the comment read aloud,** the comment markup is wrong — tell Claude exactly that.

**Write what you heard:**

---

## Step 4 — Break it twice, on purpose

**What you're checking:** what a correct page protects you from. You'll order two specific mistakes, hear the damage each one causes, then have them undone. Hearing the broken version once teaches more than reading about it ten times.

**Experiment A — the missing title.**
Say to Claude: "Remove the title element from aboutme.html and save it." Reload the page and listen to the opening announcement. It should now be the filename or something generic — that's what every visitor would get before reaching any content: no idea what page this is. Write down what announced and one sentence on what a missing title costs. Then say: "Put the title element back exactly as it was and save."

**Experiment B — the skipped heading level.**
Say to Claude: "Change my first heading level 2 into a heading level 4 and save." Run the headings list again. Listen for the gap: level 1, then suddenly level 4 — an outline that jumps from chapter to sub-sub-section with nothing between. Write down how the list sounded and why the page's outline got harder to trust. Then say: "Restore that heading to level 2 and save."

**Confirm the repairs:** run the headings list one final time and check it matches your brief again.

**Write your findings from both experiments:**

---

## Verdict

Answer in two or three sentences: what did this audit catch or confirm that Claude's own "done, saved it" message could never tell you? And which single move earned its keep this week?
