# ai07 Audio Lab: Visual Order vs. Reading Order

This week's build made your site responsive, and the brief's twist planted a booby trap on purpose: Claude applied a flexbox rule (`row-reverse`) that makes your nav links DISPLAY in reverse order — while the code underneath stays in the original order. This audit measures the damage, names the principle behind it, and then verifies your new page template.

---

## Step 1 — Measure the reversed nav

**What you're checking:** which order the page *reads* in versus which order it *displays* in — because right now, they disagree.

**Do this:** pull up the links list and note the order of your nav links. Then Tab through the nav and note the order again. Then ask Claude: "Describe the visual order of my nav links right now, left to right."

**You should find:** the links list and Tab both give the ORIGINAL order (Home first) — because they follow the code. Claude's description gives the REVERSED order (Home last) — because the CSS only changed the display. Write both orders side by side.

**Write what you found:**

---

## Step 2 — Name the principle

**What you're checking:** why this matters beyond a party trick. Two visitors are now experiencing two different navigations: a keyboard or screen reader user gets Home-first; someone reading the screen gets Home-last. Now imagine instructions anywhere that say "choose the last link in the menu" — the two visitors pick different links. Real sites cause real confusion exactly this way.

**Do this:** write four sentences in your own words: why the order in the CODE should stay logical, why CSS reordering should be used sparingly, and who gets hurt when display order and code order disagree. (For the record: accessibility guidelines have a rule about this — reading order must be meaningful. You just demonstrated why it exists.)

**Cleanup:** say: "Remove the row-reverse rule from my nav and save." Re-check with the links list.

**Write your four sentences:**

---

## Step 3 — The wrap check

**What you're checking:** your card row now wraps into fewer columns on narrow windows — a purely visual reflow. Visual reflow must not change reading order.

**Do this:** read continuously through the card section. Then say: "Describe how my card row looks in a wide window versus a narrow one." Record the description in your prompt log. Then ask: does anything about the reading order depend on the window width? (It shouldn't — the audit reads code order either way. Confirm by re-reading the section after asking Claude to describe the narrow layout.)

**You should hear:** identical reading order regardless of window size. The wrap is real — cards visually stack on narrow screens — but the meaning never moves.

**Write what you heard:**

---

## Step 4 — The template audit

**What you're checking:** this week you saved `template.html` — the skeleton every future page starts from. If the skeleton passes the audit while nearly empty, every page built from it starts life correct.

**Do this:** open template.html and run the full basic battery: the page announcement (a placeholder title should announce), the headings list (one placeholder heading level 1), the region walk (banner, navigation, main, content information — all four), and one Tab press (the skip link should be first).

**You should hear:** a tiny page that passes everything. If any check fails, fix it NOW with a precise request to Claude — a flaw in the template gets copied into every future page, so this is the highest-leverage fix of the semester.

**Write what you heard:**

---

## Verdict

Two sentences: what can CSS change about order, and what can it never change?
