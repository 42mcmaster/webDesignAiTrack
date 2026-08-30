# ai06 Audio Lab: Three Ways to Hide — Only One Keeps the Meaning

Run this audit on the hiding-demo page from the brief's twist. Four paragraphs: one visible, one hidden with `display: none`, one with `visibility: hidden`, one hidden with the sr-only off-screen technique.

## Step 1 — Read the whole page straight through.

How many of the four paragraphs does the audit find? Record which ones, by their content.

**Findings:**

## Step 2 — The census.

For each hidden paragraph, write what the audit found and what that tells you:

- `display: none` — absent from the audit entirely. It isn't hidden *from view*; it's removed from the page's meaning.
- `visibility: hidden` — also absent from the audit. On screen, though, it leaves an empty GAP where the element was (ask Claude to confirm the gap in its description of the page) — that gap is the entire difference between the two.
- **sr-only** — the audit finds this one. On screen it's invisible; in the markup's meaning it's fully present. It is the only technique of the three that hides something *visually* while keeping it part of the page.

**Findings:**

## Step 3 — Find sr-only in the wild.

Real sites use sr-only constantly: "skip to main content" links, text labels on icon-only buttons, "(opens in new window)" warnings. Visit two major sites and hunt with the tab-through and links-list moves for content the audit finds that isn't part of the visible design. Record what you find — you're auditing the pros now.

**Findings:**

## Step 4 — Layout by audit.

The new spacing work is purely visual — but reading ORDER isn't. Read your restyled pages straight through: did any of the layout changes alter the order in which content is announced? (They shouldn't have. If one did, that's a finding.)

**Findings:**

## Verdict

Three sentences: which hiding technique should a developer reach for in which situation — and which one, used carelessly, silently deletes content for every screen reader user on the site?
