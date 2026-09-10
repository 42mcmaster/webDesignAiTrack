# ai06 Audio Lab: Three Ways to Hide — Only One Keeps the Meaning

Your brief's twist had Claude build a demo page with four paragraphs: one plainly visible, and three "hidden," each by a different CSS technique. On a screen, all three hidden ones look equally gone. This audit reveals that they are NOT equal — the three techniques do completely different things to the page's meaning, and telling them apart is a professional skill most developers never learn properly.

**Setup:** open the hiding-demo page. Each paragraph's content says which technique it uses (e.g., "This paragraph is hidden with display none") — so what you hear identifies itself.

---

## Step 1 — Read the whole page, top to bottom

**What you're checking:** which of the four paragraphs still exist as far as the page's meaning is concerned.

**Do this:** go to the top and read continuously to the end. Count the paragraphs you hear and note which ones they are, by their self-describing content.

**You should hear exactly two:** the visible control paragraph, and the one hidden with the sr-only technique. The `display: none` paragraph and the `visibility: hidden` paragraph should be completely absent — not announced, not reachable, not there.

**Write which paragraphs you heard:**

---

## Step 2 — The census: what each technique actually did

**What you're checking:** understanding, not just observation. Go technique by technique and write what happened plus what it means:

- **`display: none`** — absent from the audit. This doesn't hide an element from view; it removes it from the page's meaning entirely. Nothing can reach it. (You met this in ai05 — now you're seeing it used deliberately.)
- **`visibility: hidden`** — ALSO absent from the audit. So how is it different? On screen, it leaves an empty gap where the element was, as if the content were covered by a blank sticker; `display: none` closes the gap as if the element never existed. Ask Claude to confirm: "Describe the visual difference on this demo page between the display-none paragraph and the visibility-hidden paragraph." Record its answer — that gap is the entire difference between the two.
- **sr-only** — present in the audit, absent from the screen. The technique positions the element off the visible page while leaving it fully in the document. It's the only one of the three that hides something *visually* while keeping it part of the page's meaning.

**Write one sentence per technique in your own words:**

---

## Step 3 — Find sr-only in the wild

**What you're checking:** that this isn't a classroom trick — professional sites use sr-only text constantly. Common uses: "skip to main content" links, text labels tucked inside icon-only buttons, warnings like "opens in new window."

**Do this:** visit two major sites (a big retailer and a news site work well). On each, press Tab from the top of the page a few times, and pull up the links list. Listen for announced text that is clearly not part of the visible design — a "skip to content" link is the classic giveaway, since sites hide those until they're focused.

**You should find** at least one example per site. Record the site, what announced, and what job that hidden text is doing.

**Write what you found:**

---

## Step 4 — Order check on your restyled site

**What you're checking:** this unit added spacing, cards, and a sticky header to your real site — all visual work. Visual work should never change the ORDER in which content reads.

**Do this:** on your updated pages, read continuously from the top. Compare against how the pages read last week.

**You should hear:** the same content in the same order as before the styling. If anything now reads out of sequence, a layout rule moved it — describe it to Claude: "After this week's styling, the [section] now reads before the [section], but the source order shouldn't have changed. Find which rule reordered it and fix it."

**Write what you heard:**

---

## Verdict

Three sentences: which hiding technique should a developer reach for in which situation — and which one, used carelessly, silently deletes content for every screen reader user on the site?
