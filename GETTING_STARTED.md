# Getting Started

## What you need running

1. **Claude desktop app** — signed in. Work by voice or keyboard, whichever is faster for you.
2. **A screen reader** — the audit tool for every AudioLab. Any screen reader works; the labs describe each step in plain English.
3. **GitHub Desktop** — this repository cloned, so you can commit and push your work.
4. A folder open where Claude saves the files it builds for you (each unit folder in this repo).

## Asking Claude to save files

When a build is right, tell Claude exactly where to put it, for example: "Save that as index.html in my ai02_semanticHTML folder." Then confirm the file exists before you commit.

## The audit moves

Every AudioLab is built from a small set of standard screen reader moves. Every screen reader has a command for each — find them in yours once, and every lab in this track is runnable:

- **Headings list** — one view of every heading on the page with its level
- **Next heading** — jump heading to heading, in order
- **Region walk** — jump between the page's landmarks: banner, navigation, main, footer
- **Links list** — every link on the page, read by its link text alone
- **Tab through** — move through every focusable element in page order
- **Next table / cell-by-cell** — jump to a data table, then walk it one cell at a time (headers announce as you move)
- **Next graphic** — jump to the next image; its alt text is what gets announced
- **Read from here** — continuous reading down the page
- **Top of page** — back to the start

## The one habit that makes everything work

After every build, before judging anything else: **pull up the headings list.** If that list alone doesn't tell the page's story, the page is wrong — no matter what else got built right.
