# ai03 Lesson: Three Pages That Link Together

You turn your home page into a three-page site. Every page has the same nav. The links all work. You add jump links, an email link, a download link, and a skip link.

## Step 1. Set up

Tell Claude:

"Copy index.html from my ai02_semanticHTML folder into my ai03_linksAndNav folder."

All work in this lesson happens in ai03_linksAndNav.

## Step 2. Build the pages

Tell Claude this. Fill in your content.

"Make two more pages in my ai03_linksAndNav folder, about.html and music.html. Give them the same header, nav, and footer as index.html. The nav on every page has three links: Home to index.html, About to about.html, Music to music.html. Use relative links."

"On about.html, put a heading level one that says About [your name], then three sections with heading level twos. At the top of main, put a small list of three links that jump to those three sections on the same page. Here is the content." Then give Claude the three section names and a paragraph for each.

"On music.html, put a heading level one that says My Music, and a section for each of three tracks. Each section has a heading level two with the track name and a paragraph about it."

"On every page, put a skip link as the first thing in the body. The link text is Skip to main content, and it jumps to the main element."

"In the footer of every page, add an email link to [your email address] with the subject line Question about your music. Add a download link to a file called bio.txt. Create bio.txt with a short bio I will give you." Then tell Claude your two-sentence bio.

## Step 3. Check

Open index.html in Chrome.

1. Press Tab once. The first thing you hear should be the skip link. Press Enter. You should land in main.
2. Press K to go through the nav links. Press Enter on About. The about page should open. Press Insert plus F7 to open the links list and check that Home, About, and Music are all there. Do this on all three pages.
3. On about.html, press Enter on one of the jump links. You should land on that section's heading.
4. In the footer, press Enter on the email link. Your email program should open with the subject filled in. Close it.
5. Press Enter on the download link. bio.txt should download.

If any link does nothing, tell Claude which page and which link. Have it fix the file.

## Step 4. Learn

Ask Claude:

"What is the difference between a relative link and an absolute link? Which one keeps working if I move my whole site to a new folder?"

"How does a jump link work? What does the link need and what does the target need?"

## Step 5. Make it yours

Add a fourth page, or more tracks, or more jump links. Keep every nav the same on every page.

## Step 6. Push

Commit with the summary Three page site. Push.

## Turn in

1. index.html, about.html, music.html, bio.txt
2. ai03_Questions.md with your answers
