# ai05 Audio Lab: The Invisibility Proof

This week's audit proves a negative — and the negative IS the lesson.

## Step 1 — Baseline, before the stylesheet is attached.

Pull up the headings list, walk the regions, pull up the links list. Record the results.

## Step 2 — Attach the stylesheet. Run the identical audit.

Prediction first, in writing: what will change? Then run it. Headings, regions, links, reading order — identical or not? Record exactly what changed. (The correct answer is: nothing. If something DID change, the stylesheet did something it shouldn't have, and that's a real finding worth hunting down.)

**Findings:**

## Step 3 — The exception that proves the rule.

Tell Claude: "Add `display: none` to the footer in the stylesheet — CSS only, don't touch the HTML." Now walk the regions. The footer is gone from the audit entirely — a pure styling file just removed content from the page's meaning. Write three sentences: what this proves about `display: none`, and why a stylesheet is therefore never "just decoration" where screen reader users are concerned. Have Claude remove it after.

**Findings:**

## Step 4 — The specification audit.

Take Claude's two appearance descriptions from the brief's twist (styled vs. unstyled). Pick the two most concrete visual claims in the styled description ("headings are dark green," "links underline on hover") and verify each one by tracing it to code: ask Claude to read back the exact CSS rule that makes the claim true. Specification → rule → claim, all consistent? That's a quality check that works entirely from the code — no screenshots required, which is exactly how code review works in the real world.

**Findings:**

## Verdict

Two sentences: what does CSS change, what does it never change, and which single CSS property broke that rule?
