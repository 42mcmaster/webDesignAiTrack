# ai00 First Session: Run the Whole Loop Once

One sitting, about 45 minutes, and you'll have done everything this track ever asks — once, small, and for real. Follow it like a recipe.

## Before you start — the running check

Confirm out loud, one by one: the Claude app is open and signed in. The screen reader is running. GitHub Desktop is open and this repository is cloned. You know where the repo's folder lives. If any of those is a no, fix it first — ask for help now, not in step 4.

## Step 1 — Introduce the project (2 minutes)

Say to Claude, in your own words, something like:

> "I'm taking a web design course where I build sites by directing you and auditing the results. We'll work in my webDesignAiTrack repository. When I ask you to save files, save them where I say and confirm. Keep answers short unless I ask for detail."

That's context-setting — a professional habit. Claude works better when it knows the arrangement.

## Step 2 — Direct a tiny build (5 minutes)

> "Create a complete HTML page. Title it 'Hello from [your name]'. Give it one heading level one that says the same thing, and one paragraph about what this class is. Include an HTML comment at the top that says 'My first directed build.' Read me the structure of what you made before saving."

Listen to the read-back. Does it match what you asked? If yes:

> "Save it as hello.html in my ai00_gettingStarted folder, then list that folder's files to confirm."

## Step 3 — First audit (10 minutes)

Open hello.html in the browser and run three moves with the screen reader:

1. **The page announcement.** The first thing announced when the page opens should be its title — "Hello from [your name]." Is it?
2. **The headings list.** Pull it up. Exactly one heading, level one, matching what you directed?
3. **Read from the top.** The whole page, start to finish. Title's story, heading, paragraph — and notice what does NOT get announced: the comment. Comments are for developers, not visitors. You just verified that firsthand.

If anything failed, tell Claude the symptom and have it fix the file. Re-save, re-audit.

## Step 4 — First commit (10 minutes)

GitHub Desktop is a fixed routine — the same four moves every time, forever:

1. Switch to GitHub Desktop. It announces the changed files — hello.html should be in the changes list.
2. Move to the **Summary** field and enter a short description: "First directed build."
3. Activate **Commit to main**.
4. Activate **Push origin**.

Done means pushed. Ask Claude: "What did I just do, in plain terms, when I committed and pushed?" — and listen. (Then check your answer against the ConceptCheck later.)

## Step 5 — Close the session (5 minutes)

> "Compile everything we did this session — my requests, your key answers, any fixes — into a markdown file called ai00_PromptLog.md and save it in the ai00_gettingStarted folder."

Then commit and push again — the log is part of the turn-in. **That's the whole loop: brief, direct, save, audit, commit.** Every unit from here is this, with bigger builds and sharper audits.

## What to commit (this unit's turn-in)

- `hello.html`
- `ai00_PromptLog.md`
- Your completed `ai00_AudioLab.md` (the moves trainer) and `ai00_ConceptCheck.md`
