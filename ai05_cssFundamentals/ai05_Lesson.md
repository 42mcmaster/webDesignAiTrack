# ai05 Lesson: One Stylesheet for Your Whole Site

Right now every page on your site has its own style block in the head. That is 25 copies of the same rules. In this lesson you move all of them into one file called styles.css and link it from every page. Then you add a color scheme and fonts to that one file, and the whole site changes at once.

CSS changes how a page looks. It does not change what the page says or the order it is read in.

## Step 1. Set up

All work in this lesson happens in your Music Website folder. You do not need a new folder. GitHub keeps your old version.

Tell Claude:

"Look at the style blocks in every HTML file in my Music Website folder. Tell me how many pages have one, and which rules are the same on every page and which are different."

Listen to the answer before you go on.

## Step 2. Build the stylesheet

Tell Claude:

"Make a file called styles.css in my Music Website folder. Move every rule from the style blocks into it. Keep one copy of each rule. Put a comment above each group of rules saying what it is for."

"Delete the style block from every page. In the head of every page, add a link element that points to styles.css."

"Tell me if any page had a rule that the others did not. Keep that rule in styles.css and tell me which page it was for."

## Step 3. Add your own style

Decide these before you tell Claude:

1. A color scheme: a background color, a text color, and one accent color for links and headings. Pick by mood, like dark and heavy, or warm and calm. Ask Claude to suggest three schemes that fit your music and describe each one, then pick one.
2. A font for headings and a font for body text. Ask Claude to suggest pairs that fit your site.
3. A body text size. Use rem, not px. 1rem is the size the visitor's browser is set to.

Then tell Claude something like this. Fill in your choices.

"In styles.css, style the body with my background color, text color, body font, and a font size of [your size] rem."

"Style every heading level one and level two with my heading font and my accent color. This is an element selector."

"Style the page-overview class with [what you want, like a border on the left and extra space]. This is a class selector."

"Style the main-content id with [one thing, like a maximum width]. This is an id selector."

"Style links with my accent color. Give links a different look when they are hovered over and when they have keyboard focus."

"Check the contrast between my text color and background color, and between my accent color and background color. Tell me the contrast ratio for each. If either one is under 4.5 to 1, tell me and suggest a fix."

## Step 4. Check

1. Ask Claude: "List every HTML file in my Music Website folder that does not have a link to styles.css, and every file that still has a style block or a style attribute." The answer should be none.
2. Open index.html in Chrome. Press Tab once. You should hear Skip to main content. Press Enter. You should land in main. The rules that hide the skip link until it gets focus are now in styles.css, so this proves the link to the stylesheet works.
3. Press H to move through the headings on index.html, music.html, and one release page. The headings and their order should be the same as before this lesson.
4. Press Tab through the links on one page. Each link should still be reached, in the same order as before.
5. Ask Claude: "Describe how index.html looks now, as if you were describing it to a designer. Colors, fonts, spacing, mood." Check that it matches what you asked for. If something is off, tell Claude what to change.

## Step 5. Learn

Ask Claude:

"What are the three places CSS can go, and which one wins if they disagree?"

"What is the difference between a class and an id?"

"Why use rem for font size instead of px?"

"What does a contrast ratio measure, and why is 4.5 to 1 the minimum for body text?"

"If I hide something with display none, can a screen reader still find it? How does my skip link stay hidden but still work?"

## Step 6. Make it yours

Add a style for your tables, like borders between cells or a different background for the header row. Add a style for your figures and captions. Change your accent color in styles.css and have Claude confirm every page picked up the change.

## Step 7. Push

Commit with the summary One stylesheet for the site. Push. Make sure styles.css shows up on GitHub.

## Turn in

1. styles.css and your updated pages
2. Your answers to the questions in ai05_Questions.md, shared in Google Classroom
