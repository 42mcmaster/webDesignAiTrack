# ai00 Workflow Guide: How This Track Works

In this track, you build websites by **conversation**. You describe exactly what you want, Claude writes the code, and you check the result by listening to it with a screen reader. Your voice is the keyboard and your ears are the quality department. This guide is the whole system; the FirstSession file walks you through doing it once.

## The five-step loop (every unit, every build)

1. **Brief.** Listen to (or read through) the unit's BuildBrief. Note the must-say list — the technical words your directions have to use.
2. **Direct.** Tell Claude what to build. Speak in complete requests. Use the must-say vocabulary out loud — that's the graded skill.
3. **Save.** Tell Claude exactly where to put the finished file, then ask it to confirm the file is really there.
4. **Audit.** Run the unit's AudioLab with the screen reader. If the page fails, tell Claude what failed and have it fix the markup. Repeat until it passes.
5. **Commit.** Push everything with GitHub Desktop so it's turned in.

Say the loop out loud until it's automatic: **brief, direct, save, audit, commit.**

## Talking to Claude so it actually works

Claude does exactly what you say — which means vague directions produce vague websites. Habits that make the conversation work:

- **One request at a time.** "Add a navigation region with four links" beats a paragraph asking for six things at once. Stack requests one after another; Claude keeps up.
- **Use the real names.** Say "heading level one," "nav region," "unordered list," "alt text." The technical vocabulary IS the curriculum, and Claude responds better to it too.
- **Make Claude read its work back.** After a build, say: "Describe the structure of that page, top to bottom, in plain sentences." You're checking the plan before you audit the result.
- **Ask for short answers when you want short answers.** "Answer in two sentences" or "just list the steps, one per line" keeps replies from turning into essays.
- **Interrupt freely.** If a reply is going somewhere useless, stop it and redirect. It's a tool, not a guest.
- **Never accept "done" without proof.** "List the files in my ai01 folder" after every save. Trust, but verify — by asking.

## The prompt log — end every session the same way

Before you stop working, say: **"Compile everything we did this session — my requests, your key answers, and any fixes — into a markdown file called aiNN_PromptLog.md and save it in this unit's folder."**

The log is a graded artifact: it's how the quality of your direction gets seen. Claude writes it; you just have to remember to ask.

## The tools, and what each one is for

- **Claude desktop app** — where the building happens. Voice input, dictation, or typing, whichever is fastest for you in the moment.
- **Screen reader** — the audit instrument. The AudioLabs name each move in plain English; the moves trainer in this unit teaches them all.
- **GitHub Desktop** — the turn-in machine. It's the one step that isn't a conversation: a short, fixed routine (details in FirstSession), the same every time.
- **This repository** — where everything lives. One folder per unit; your builds, logs, and completed lab files all get saved and pushed here.

## When something goes wrong

- Claude saved a file to the wrong place → "Move that file to [right place] and confirm."
- A build sounds wrong in the audit → don't debug it yourself; describe the symptom to Claude exactly ("the region walk skips the navigation") and make IT find the cause.
- You're lost mid-session → "Summarize where we are and what's left from the brief."
- GitHub Desktop says something unexpected → read the message to Claude and ask what it means. That's a legitimate professional move; developers do it all day.
