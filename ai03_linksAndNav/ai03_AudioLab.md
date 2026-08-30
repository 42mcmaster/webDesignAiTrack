# ai03 Audio Lab: Navigation on Trial

Your site is three pages now, with a shared nav, a table of contents on the about page, an email link, a download link, and a skip link on every page. This audit tests every one of those against your brief. Keep the brief nearby; describe any failure to Claude in specific words, get the fix, re-run the step.

---

## Step 1 — The links list, on every page

**What you're checking:** whether every link's text stands on its own. The links list strips away all surrounding sentences and reads ONLY the link text — which is exactly how many people scan a page. A link that reads "click here" is meaningless in this list; a link that reads "Weekly menu" tells you everything.

**Do this:** on each of your three pages, run the "list all links" command and arrow through the whole list.

**You should hear:** every link announcing a clear destination with no other context needed — nav links by page name, the table of contents by section names, the email and download links by what they do.

**If any link fails the test:** name it precisely: "In the links list, one link just says 'here.' Rewrite its link text so it names its destination — it goes to [where] — and save."

**Write what you heard (note anything that failed, per page):**

---

## Step 2 — Round trips

**What you're checking:** that the navigation actually works in both directions, and that the skip link is doing its job. The skip link exists so keyboard users can jump straight to the main content instead of tabbing through the whole menu on every single page — but only if it's the FIRST thing Tab reaches.

**Do this, on each page:** go to the top, press Tab once, and listen. Then activate what you landed on. Then, from the home page, Tab to each nav link, activate it, and use the destination page's nav to come back.

**You should hear:** on the first Tab of every page, "Skip to main content, link" — and activating it should land you at the main content (the next thing read should be the page's main heading, not more menu). Every nav link should reach its page, and every page should get you back.

**If the first Tab lands on a nav link instead**, the skip link is missing or in the wrong place: "The first Tab stop on [page] is the Home link, not the skip link. The skip link must be the very first focusable thing inside the body. Fix it on that page and save."

**Write what you heard:**

---

## Step 3 — The table of contents, on the about page

**What you're checking:** in-page anchors — links that jump to a section further down the SAME page. Each needs two halves: the link at the top, and a marked target at the section. This step tests both halves of all three.

**Do this:** on the about page, Tab to each table-of-contents link and activate it. After each jump, listen to what reads next.

**You should hear:** immediately after each activation, the target section's heading — proof you landed in the right place. Then go to the top and run the headings list: the sections should appear in the same order the table of contents promised.

**If a jump goes nowhere** (nothing changes, or reading continues from the top): the target's marker is missing. "Activating the 'My goals' link in the table of contents doesn't move me to that section. Check that the link's address and the section's id match, fix it, and save."

**Write what you heard:**

---

## Step 4 — Email and download

**What you're checking:** two special link types from your brief. An email link should open a mail window — with the subject already filled, since you directed that. A download link should offer to save a file rather than navigate.

**Do this:** activate the email link; listen to what opens and check the subject line. Close it. Then activate the download link and listen to what the browser announces.

**You should hear:** a mail compose window with your pre-filled subject announced, and — for the download — a save/download announcement naming your file (not a navigation to a new page).

**If the email opens with a blank subject:** "The email link opens a message with no subject. Add the subject [your subject] to the mailto link and save."

**Write what you heard:**

---

## Verdict

Two or three sentences: which was the worst navigation defect in Claude's first draft, which audit step exposed it, and what exact fix request did you give? (If the first draft was genuinely clean, say which step you trusted least and re-ran to be sure.)
