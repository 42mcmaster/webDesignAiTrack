# ai05 Audio Lab: The Invisibility Proof

This week you styled your whole site with a stylesheet. This audit proves something that sounds strange at first: **done correctly, all that styling changes nothing a screen reader reports.** CSS is the presentation layer — colors, fonts, spacing — and the audit reads the structure layer underneath it. Proving that boundary, and then finding the one exception that crosses it, is the whole lab.

---

## Step 1 — Baseline, before the stylesheet

**What you're checking:** a snapshot of the page's structure with no styling attached, so you have something to compare against.

**Do this:** ask Claude: "Temporarily remove the stylesheet link from my home page and save it — we're running an experiment; we'll put it right back." Open the page and run three moves you know well: the headings list, the region walk, and the links list. Record the results — counts, names, order.

**Write what you heard:**

---

## Step 2 — Attach the stylesheet and run the identical audit

**What you're checking:** whether full styling changes anything the audit can detect.

**Do this — prediction first:** before touching anything, write one sentence predicting what will change. Then say: "Put the stylesheet link back and save." Reload and run the exact same three moves.

**You should hear:** exactly what you heard in Step 1. Same headings, same regions, same links, same order. The page now has colors, fonts, and spacing — and none of it registers, because styling and structure are separate layers. That separation is the entire point of CSS, and you just proved it experimentally.

**If something DID change,** the stylesheet is doing something beyond styling — that's a real finding. Describe the difference to Claude and have it explain which CSS rule caused it before deciding on a fix.

**Write what you heard, and whether your prediction held:**

---

## Step 3 — The exception that proves the rule

**What you're checking:** the one CSS property that crosses the boundary. `display: none` doesn't make an element invisible — it removes it from the page's meaning entirely, screen readers included.

**Do this:** say: "In the stylesheet only — don't touch the HTML — add a rule that sets the footer to display none. Save." Reload and run the region walk.

**You should hear:** banner, navigation, main... and no footer. Gone from the walk. The HTML file still contains every word of that footer; one line of CSS erased it from what the page communicates. Write three sentences: what this proves about `display: none`, and why a stylesheet therefore can never be dismissed as "just decoration."

**Cleanup:** "Remove that display-none rule and save." Re-run the region walk to confirm the footer is back.

**Write your findings:**

---

## Step 4 — The specification audit

**What you're checking:** whether the styling you directed actually got built — verified by tracing claims to code, the way a code review works.

**Do this:** in the brief's twist you saved Claude's detailed description of the styled site. Pick its two most concrete claims — say, "headings are dark green" and "links underline when hovered." For each, say to Claude: "Read me the exact CSS rule that makes this true: [the claim]. Quote the selector and the properties."

**You should hear:** a real rule for each claim — for the heading color, a rule selecting headings with a color property; for the hover, a rule using the hover state. If Claude can't produce a rule matching a claim, then the description was embellished and the site doesn't actually do what the description said — which is a defect in either the site or the description. Direct whichever fix is right: build the missing rule, or correct the description in your prompt log.

**Write the two claims you traced and what you found:**

---

## Verdict

Two sentences: what does CSS change, what does it never change — and which single property broke that rule in this lab?
