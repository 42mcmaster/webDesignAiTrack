# ai04 Audio Lab: Media Under Audit

Your media page has four content images with alt text you wrote yourself, one decorative image that should be silent, audio and video players, and a data table. This audit checks each — and ends with a side-by-side comparison against a deliberately lazy table. Brief nearby; failures described to Claude precisely; fixes verified.

---

## Step 1 — The graphics pass

**What you're checking:** alt text — the text a screen reader speaks in place of each image. You wrote these yourself and dictated them to Claude; this step verifies they made it into the code word for word. It also checks the opposite case: your decorative image should announce NOTHING, because you directed empty alt for it, which tells screen readers "skip this, it's decoration."

**Do this:** use your "next graphic" command to jump image to image through the whole page.

**You should hear:** your four alt texts, exactly as you wrote them — and only four stops. The decorative image should not be a stop at all.

**Two different failures to listen for:** if the audit STOPS on the decorative image and says "graphic" or reads a description, its alt isn't empty — say: "The decorative divider image is announcing. Give it an empty alt attribute — alt equals two quotation marks with nothing between — and save." If any image announces a FILENAME ("IMG underscore 4 4 7 2 dot jpg"), its alt is missing entirely — different problem, different fix: "The photo of [subject] is announcing its filename, which means it has no alt attribute. Add the alt text I wrote: [your words]. Save."

**Write what you heard:**

---

## Step 2 — The correct table, cell by cell

**What you're checking:** that your data table announces its headers as you move through the data — the behavior you first heard on the ai00 practice page. That behavior comes from real header cells with scope, and a caption; your brief required both.

**Do this:** jump to the table. Listen for the caption on arrival. Then walk cell by cell down one data column.

**You should hear:** the caption when you land, and then the column's header announced with each value as you move down — "Points, 24," "Points, 31" — so every number carries its meaning with it.

**If you get bare values with no header announcements,** the header cells are probably ordinary cells: "Walking down the table columns, no headers announce with the values. Make the first row real header cells with the scope attribute, and add a caption if it's missing. Save."

**Write what you heard:**

---

## Step 3 — The lazy table, same walk

**What you're checking:** what laziness sounds like. Your brief had Claude build the same table badly on purpose in lazy-table.html: every cell ordinary, no caption. Same data, same look on screen.

**Do this:** open lazy-table.html and repeat Step 2's walk exactly.

**You should hear the difference immediately:** no caption on arrival, and bare values with nothing telling you what column you're in. Try this: walk to a cell in the middle of the table and ask yourself what the number means. In the correct table you'd know; here you'd have to count columns and memorize the top row. Write two or three sentences describing that difference — you'll reuse this comparison skill on the December exams and in html11's critique.

**Cleanup:** have Claude delete lazy-table.html (or move it out of the folder) — don't commit it.

**Write your findings:**

---

## Step 4 — Media players

**What you're checking:** that your audio and video players are actually usable. Your brief required the controls attribute, which gives each player real buttons — play, pause, volume. Buttons only help if they can be reached and announce what they are.

**Do this:** Tab into the video player, then the audio player. Listen to what each control announces as you land on it. Try play and pause on each.

**You should hear:** named controls — "play button," "mute button," a volume slider — reachable one by one, and play/pause actually working.

**If Tab skips past a player entirely or controls won't activate,** the controls attribute is likely missing: "The audio player can't be reached with Tab — check that the audio element has the controls attribute, fix it, and save."

**Write what you heard:**

---

## Step 5 — Alt versus caption

**What you're checking:** your brief put two images inside figure elements with visible captions. A screen reader announces BOTH the alt text and the caption — so if they say the same thing, the visitor hears it twice, which means one of them is wasted. Alt describes what's in the image; the caption adds context around it.

**Do this:** read continuously through both figures. Listen to the alt, then the caption, back to back.

**You should hear:** two different, complementary pieces of information — for example alt: "Three loaves of sourdough cooling on a wire rack," caption: "Saturday's first batch, gone by nine a.m."

**If they repeat each other,** decide which one to rewrite (usually the caption) and direct the change: "The second figure's caption repeats its alt text. Keep the alt, and rewrite the caption to add context instead: [your new caption]. Save."

**Write what you heard:**

---

## Verdict

Three sentences: the sharpest correct-versus-lazy difference this audit exposed, which audit move you'd teach every web developer first because of it, and the exact fix request you're proudest of this week.
