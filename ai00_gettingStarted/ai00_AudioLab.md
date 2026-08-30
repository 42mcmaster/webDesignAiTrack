# ai00 Audio Lab: The Moves Trainer

Every lab in this course uses the same small set of screen reader moves. This trainer teaches them one at a time, using `ai00_PracticePage.html` — a small bakery website that is built correctly on purpose. Because the page is correct, this lab can tell you exactly what you should hear for every move. Learn the moves here, and every later lab is just using them on your own pages.

**Before you start:** open the practice page in your browser. If you're not sure how, ask Claude: "How do I open the file ai00_PracticePage.html from my ai00 folder in my browser? Give me the steps one at a time." Once the page is open, work through the moves below in order. For each one, write what you actually heard in the space provided — even if it matches perfectly. "It matched" is a finding too.

---

## Move 1 — The page announcement

**What this is:** the moment a web page opens, a screen reader speaks that page's title before anything else. The title comes from a tag in the page's code — you'll build one yourself in ai01. This move requires no command at all; it happens automatically.

**Do this:** open the practice page (or reload it if it's already open) and just listen to the very first thing spoken.

**You should hear:** "Trailhead Bakery - Practice Page" — possibly followed by the browser's name. If the first thing you heard was something like a filename ("ai00 underscore PracticePage dot html") that would mean the page has no title; this page does, so you should get the real one.

**Write what you heard:**

---

## Move 2 — The headings list

**What this is:** headings are the section titles of a page, and they come in levels — level 1 is the page's main title, level 2s are its major sections, level 3s are subsections, like an outline. Every screen reader has a command that gathers every heading on the page into one list you can arrow through, with each heading's level announced. This is the single most useful check in this whole course: a well-built page tells its whole story in this list alone.

**Do this:** find your screen reader's "list all headings" command and run it on the practice page. Arrow through the whole list, listening for each heading's text AND its level number.

**You should hear four headings:** "Trailhead Bakery, heading level 1" — "Our Breads, heading level 2" — "Hours and Location, heading level 2" — and "Weekend Specials, heading level 3." Notice the shape: one level 1 at the top, two level 2 sections, one level 3 tucked inside a section. That outline shape is what "correct" sounds like.

**Write what you heard:**

---

## Move 3 — The region walk

**What this is:** well-built pages are divided into named zones called regions (also called landmarks): a banner across the top (the site's header), a navigation area (the menu of links), a main content area, and a footer at the bottom. Screen readers have a command that jumps from one region to the next, announcing each one's name. It's how you check a page's big-picture skeleton in seconds.

**Do this:** go to the top of the page (there's a command for that too — find it), then press your "next region/landmark" command repeatedly until it wraps around or stops.

**You should hear, in order:** "banner" — "navigation" — "main" — and "content information" (screen readers usually announce the footer with that name; it's the same thing as a footer). Four zones, in the order they appear on the page.

**Write what you heard:**

---

## Move 4 — The links list

**What this is:** like the headings list, but for links — every link on the page, gathered into one list, read by its link text alone with no surrounding sentence. This matters because a link's text should make sense all by itself. A link that just says "click here" is meaningless in this list — and this list is exactly how many people move through a page.

**Do this:** find your screen reader's "list all links" command and run it. Arrow through.

**You should hear three links:** "Our breads" — "Hours and location" — "Contact the bakery." Notice every one of them tells you where it goes without any other context. That's what good link text sounds like.

**Write what you heard:**

---

## Move 5 — Tab through

**What this is:** the Tab key moves through every *interactive* element on a page — links, buttons, form fields — one at a time, in the order they appear in the page's code. It's how you check what a keyboard user can actually reach.

**Do this:** go to the top of the page, then press Tab repeatedly. Each press should land on the next interactive thing and announce it.

**You should hear:** the three links, one per Tab press, in the same order as the links list — and then nothing more, because this page has no buttons or form fields yet. (Your later pages will, and this same move is how you'll check them.)

**Write what you heard:**

---

## Move 6 — The table, cell by cell

**What this is:** data tables have their own set of commands: one to jump to the next table on the page, and one to walk through the table a single cell at a time. Here's the part that matters: in a *correctly built* table, when you move through the data, the screen reader announces the column's header along with each value — so you always know what a number means. In a lazily built table, you get bare values with no context. You'll test both kinds later in the course; today, hear the correct kind.

**Do this:** use your "next table" command to jump to the practice page's table. Listen to what announces when you land on it. Then use your table navigation commands (moving cell by cell) to walk down the second column.

**You should hear:** on arrival, the table's caption, "Weekly hours." Then, walking down the second column: "Hours" (the column header) announced with each cell's value — "Hours, 7am to 2pm," then "Hours, 8am to noon." That header-repeated-with-every-cell pattern is the sound of a table built right. Remember it.

**Write what you heard:**

---

## Move 7 — Read from here

**What this is:** continuous reading — the screen reader reads from your current position straight down the page until you stop it. This is how you experience the page the way a first-time visitor does, top to bottom, and how you check that the content's ORDER makes sense.

**Do this:** go to the top of the page and start continuous reading. Let it run all the way to the footer.

**You should hear:** everything, in this order: the bakery name, the three navigation links, the Our Breads section (with its bread list), the Weekend Specials subsection, the Hours section with the table, and finally the footer with the address and phone number. If the order told a sensible story from start to finish, the page passes.

**Write what you heard:**

---

## Move 8 — How lists announce themselves

**What this is:** not a new command — a new thing to *listen for* during the reading you just did. When a page uses a real list element in its code, the screen reader announces it as one: "list of three items," then counts along as it reads them. When a developer fakes a list with plain text and dashes, there's no announcement and no count. That announcement is the difference between structure and decoration, and later units test exactly this.

**Do this:** read through the navigation and the bread list again, listening specifically for the words "list" and the item count.

**You should hear:** the navigation announced as a list of three items, and the breads announced as a list of three items, with each item counted as you move through.

**Write what you heard:**

---

## Verdict

Answer in two or three sentences: which move gave you the most information for the least effort? Which one will you run first on every page you build from now on? (There's a strongly recommended answer to the second one — it's in the workflow guide.)
