# ai08 Audio Lab: The Forms Face-Off

Two forms with identical fields: the real one you directed carefully, and lazy-form.html, which the brief had Claude build badly on purpose. Forms are where a screen reader changes behavior: when you land in a form field, it switches into a mode where your typing goes INTO the field, and it announces what each field is as you arrive. That arrival announcement is everything — it's the only introduction a field gets. This audit compares what the two forms announce, then turns the differences into professional findings.

---

## Step 1 — The real form, walked cold

**What you're checking:** whether every control introduces itself completely at the moment you land on it — before you type anything. A complete introduction has up to four parts: the field's LABEL (what to enter), its TYPE ("edit" for a text box, "radio button," "combo box" for a dropdown), its position in a group ("1 of 3"), and whether it's REQUIRED. And when you enter one of your grouped sections, the group's LEGEND (its title) should announce first.

**Do this:** Tab through the entire real form, field by field, top to bottom. At each stop, before typing, note what announced: label? type? required? And at each new fieldset: did the group announce its legend?

**You should hear**, for example: entering the first group, "Contact information, grouping" — then "Full name, edit, required" — then "Email address, edit, required" — and at the radio group, "Shirt size, grouping. Small, radio button, not checked, 1 of 3." Every field self-explanatory on arrival.

**If a field announces only its type** ("edit" and nothing else), its label isn't connected. That's the single most common form defect on the web: "The phone number field announces as just 'edit' with no label. Connect its label element to the input using matching for and id attributes, and save."

**Write what each field announced (short notes per field are fine):**

---

## Step 2 — The lazy form, same walk

**What you're checking:** what the same fields sound like when the markup is lazy — placeholders instead of labels, no fieldsets, a generic button.

**Do this:** open lazy-form.html and repeat exactly the same Tab walk, noting what announces at each stop.

**You should notice:** some fields announce their placeholder text once — but try typing a character and then reviewing the field: the placeholder is gone, and with it any reminder of what the field wanted. The radio buttons arrive as "radio button, 1 of 3" — one of three WHAT? Nothing says. Record the exact moment the form stops making sense to someone who didn't design it.

**Write what you heard, and where it broke down:**

---

## Step 3 — Turn the differences into findings

**What you're checking:** your diagnosis skill. This is the exact format the html11 AI-critique uses, so practice it properly now. For each failure you found in the lazy form, write ONE line with three parts — what announced wrong, what markup is missing, what the fix is:

> "Radio group announces no purpose → no fieldset and legend → wrap the group in a fieldset with the legend 'Shirt size'."

**Do this:** write at least five findings in that arrow format. If you run out of failures, you missed some — go back to Step 2 and listen to the dropdown and the button.

**Cleanup:** have Claude delete lazy-form.html — don't commit it.

**Write your five findings:**

---

## Step 4 — Submit behavior on the real form

**What you're checking:** what the browser itself does when validation fails — behavior you get free from the required and pattern attributes your brief specified.

**Do this:** on the real form, leave a required field empty and activate the submit button. Note: did focus jump somewhere? Did a message announce? Which field is focused now? Then fix the field, submit again with everything valid, and note what happens.

**You should hear:** on the failed submit, focus moving to the first invalid field with an announcement along the lines of "Please fill out this field" — the browser blocking the submit and taking you straight to the problem. On the valid submit, the form goes through (on our class pages that may just reload the page — that's expected; there's no server yet, a fact your ConceptCheck asks about).

**Write what happened on both submits:**

---

## Verdict

Three sentences: the single worst thing a developer can do to a form, the one-line fix for it, and roughly how long that fix takes. That gap — large harm, trivial fix — is the whole accessibility story in one sentence, and this audit just documented it with evidence.
