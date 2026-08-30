# ai08 Audio Lab: The Forms Face-Off

Two forms, same fields: the real one and lazy-form.html. This is the most important audit of the semester — the class will reuse this protocol when html10's usability testing arrives.

## Step 1 — The real form, cold.

Tab into it. For every control, record what the screen reader announces: the label, the control type ("edit," "radio button, 1 of 3"), required state, and — entering each fieldset — the legend. A perfect run announces everything a user needs before they type a single character.

**Findings:**

## Step 2 — The lazy form, same walk.

Tab through lazy-form.html. Record what each control announces now. Placeholder text may read once and then vanish as typing starts; radio groups arrive with no context ("radio button, 1 of 3" — of WHAT?). Record the exact moment the form stops making sense.

**Findings:**

## Step 3 — Diagnose like a professional.

For each failure in the lazy form, name the missing markup and the fix, one line each:
"Radio group announces no purpose → no fieldset/legend → wrap in fieldset with legend 'Shirt size'."
Five findings minimum. This is the exact skill — and format — the html11 AI critique grades.

**Findings:**

## Step 4 — Submit behavior.

On the real form: leave a required field empty, submit, and record what happens — does focus move to the problem field? Does the error announce? Then fill everything correctly and submit. Browser-native validation has real announced behavior; describe it.

**Findings:**

## Verdict

Three sentences: the single worst thing a developer can do to a form, the one-line fix, and how long that fix actually takes. (That gap — big harm, trivial fix — is the whole accessibility story, and this audit just documented it.)

*(Delete lazy-form.html before committing.)*
