# ai04 Audio Lab: Media Under Audit

## Step 1 — The graphics pass.

Jump graphic to graphic through the page. Record what's announced for each image. The four content images should read exactly the alt text you wrote. The decorative image should not be announced at all — if the audit stops on it, its alt isn't empty; if it announces a filename like "IMG underscore 4 4 7 2," the alt is missing entirely. Both are defects with different fixes — name the right one.

**Findings:**

## Step 2 — The two tables, cell by cell.

On the correct table: jump to it, then walk it cell by cell. Moving down a column, the column header should announce before each value. Now do the same on lazy-table.html and describe the difference — what does the audit lose when the headers are plain td cells?

**Findings:**

## Step 3 — Media elements.

Tab into the video and audio players. Can the audit reach play/pause? What is each control announced as? Record anything unreachable — an unreachable control is a defect, not a quirk.

**Findings:**

## Step 4 — The caption question.

Read a figure straight through: the alt text AND the figcaption both announce. Are they saying different, complementary things, or repeating each other? Fix any repeats (rewrite one of them — decide which).

**Findings:**

## Verdict

Three sentences: the sharpest difference this audit found between done-right and done-lazy, and which single audit move you'd teach every web developer first because of it.

*(After the lab: delete lazy-table.html before committing.)*
