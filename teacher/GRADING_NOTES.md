# Teacher Notes: Grading the AI-Directed Track

No point values, consistent with the rest of the course. Three criteria per unit, graded from what's pushed to the repo:

## 1. Direction quality (from the saved transcript or prompt log)

Did the directions invoke the BuildBrief's must-say list by name? "Add a nav region with five links" earns it; "make a menu thing at the top" doesn't. Look for: correct element names, structural intent stated before details, and iteration that names the defect ("the headings jump from h1 to h3 — fix the hierarchy") rather than vibes ("make it better").

## 2. Concept accuracy (from the ConceptCheck)

Same competencies as the parallel html unit. Answers in the student's own words; depth matches what the WebXam asks at describe level.

## 3. Audit rigor (from the AudioLab findings)

Findings should be specific ("the nav is a plain div — the region walk jumps straight from banner to main"), evidenced (which audit move revealed it), and correctly diagnosed (what markup change fixes it). A lab that found zero issues on a first-draft AI build is a red flag — first drafts nearly always fail something; finding nothing usually means the audit wasn't run thoroughly.

## Reading the labs yourself

Each lab step names its screen reader move in plain English (GETTING_STARTED.md lists the full set). You don't need to run a screen reader to grade — read the student's evidence chain instead: move used → what it announced → diagnosis → fix. If the chain holds together, the audit was real.

## Alignment

ai-unit numbering tracks the html-unit numbering week for week. Where the class does peer review, an AudioLab protocol applied to a classmate's page is a full substitute — and by html10's usability-testing work, those audits become a resource for the whole class.
