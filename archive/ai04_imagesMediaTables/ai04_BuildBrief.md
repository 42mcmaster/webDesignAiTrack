# ai04 Build Brief: Images, Media & a Table That Reads Aloud Correctly

**Pairs with html04 (Images, Media & Tables).**

## What to build

Direct Claude to add a media page to your site:

- Four images relevant to your topic. **You write every alt text yourself** and dictate it to Claude — alt text is the author's voice, and outsourcing it to an AI is how the web filled up with useless alt. Decide what each image needs to say to someone experiencing the page through a screen reader.
- One purely decorative image (a divider, a flourish) with **empty alt** (`alt=""`) — so a screen reader skips it entirely
- One embedded video and one audio element, with controls
- A data table about your topic: caption, header row with proper header cells, at least four rows of data

## The must-say list

- `img`, `src`, `alt` — and the rule for decorative images (empty alt, not missing alt)
- `figure` and `figcaption`, and how a caption differs from alt text
- `audio` and `video` with the `controls` attribute
- `table`, `caption`, `thead`, `tbody`, `th` with `scope`
- image file formats: when JPG, when PNG, when SVG

## The twist

Have Claude produce the table twice: once correctly (th cells, scope, caption) and once lazily (every cell a td, no caption) as `lazy-table.html`. The AudioLab compares them cell by cell. Delete the lazy version after — don't commit it.

## What to commit

- Your media page + image/media files
- `ai04_PromptLog.md`
- Completed `ai04_AudioLab.md` and `ai04_ConceptCheck.md`
