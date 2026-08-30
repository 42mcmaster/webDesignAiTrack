# Web Design: AI-Directed Track

An alternative pathway through the 145010 Web Design course built on two professional skills: **directing an AI to build exactly what you specify**, and **auditing web pages by audio** — testing them with a screen reader, the same way professional accessibility testers do.

This is not a lighter version of the course. It runs on the same schedule, covers the same state competencies, and ends at the same December exam. It trades one skill (typing syntax into an editor) for two that are at least as marketable: precise technical specification, and quality auditing that most working developers never learn.

## How each unit works

Every unit has three files, numbered to match the main course (ai02 pairs with html02, and so on):

1. **BuildBrief** — what to get Claude to build, and the list of concepts your directions must use by name. The build is graded on the quality of your direction, not on typing.
2. **ConceptCheck** — questions about how the web technology actually works. Answer in your own words, in the file. These bank the knowledge the December exam tests.
3. **AudioLab** — the audit protocol. Each lab tells you, in plain English, what to check with the screen reader, what a correct page should sound like, and what to report. If the page fails the audit, it fails — send Claude back to fix it, and document what was wrong.

## Unit map (mirrors the main course's numbering and pacing)

- **ai02–ai04** — semantic HTML · links & nav · images/media/tables *(built)*
- **ai05–ai08** — CSS fundamentals · box model (including the sr-only technique) · flexbox/responsive (visual order vs. reading order) · forms (forms-mode auditing) *(built)*
- **ai09–ai11** — JavaScript features · site quality & publishing · Build It Three Ways *(coming — ai11 is where this track's builder becomes the class's audio auditor)*
- **ai12** — exam prep, shared with the main course's html12 materials

## The workflow

1. Open the unit's BuildBrief and the Claude desktop app.
2. Direct the build by voice or typing. Save the finished files into this repository's unit folder.
3. Run the AudioLab. Report findings in the lab file. If something fails, iterate with Claude until it passes, and keep notes on what changed.
4. Answer the ConceptCheck in the file.
5. Commit and push everything with GitHub Desktop.

## Why audit by audio?

A page can look right and still be built wrong — bad structure hides under good styling. A screen reader strips the styling away and reads what the markup actually *says*, so structural mistakes that are invisible on screen become impossible to miss. Professional accessibility teams audit exactly this way. In this track it's the standard quality gate for every build: if the audit passes, the markup is genuinely correct — not just pretty.

## Ground rule

"Make me a webpage" is not a direction — it's a wish. Every brief has a must-say list: the elements and concepts your instructions have to invoke by name. That vocabulary is the actual curriculum.
