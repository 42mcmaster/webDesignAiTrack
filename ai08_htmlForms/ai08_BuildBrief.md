# ai08 Build Brief: Forms — Your Richest Unit

**Pairs with html08 (HTML Forms).** Forms are where screen reader support is either professional or garbage, with nothing in between — and forms-mode auditing is the sharpest audit skill in this whole track.

## What to build

Direct Claude to build a real registration form for your site (pick a purpose that fits your topic):

- Three `<fieldset>` groups, each with a `<legend>` (e.g., Contact Info / Preferences / Confirmation)
- Inputs that cover: text, email, a radio group (3+ options), checkboxes (3+), a select dropdown, a textarea
- **Every input labeled** with a `<label>` connected by `for`/`id`
- Sensible `required` fields; one `pattern`-checked field (phone or ZIP)
- A submit button that says something better than "Submit"
- Styled with your stylesheet: visible focus styles (`input:focus`) — every keyboard user needs a visible marker of where focus is

## The must-say list

- `form`, `action`, and **GET vs POST** (which one for form submissions with personal data, and why)
- `label` with **`for` matching the input's `id`** — say the mechanism, not just "add labels"
- `fieldset` and `legend` — and what a legend does for a radio group specifically
- input `type` values by name; `required`; `pattern`
- `tabindex` — and why the answer is almost always "don't set it; fix the source order instead"

## The twist

Have Claude build the same form a second time, badly, as `lazy-form.html`: no labels (placeholders only), no fieldsets, generic button. Your AudioLab runs both. Delete the lazy version after — don't commit it.

## What to commit

The real form live on your site, `ai08_PromptLog.md`, completed ConceptCheck and AudioLab.
