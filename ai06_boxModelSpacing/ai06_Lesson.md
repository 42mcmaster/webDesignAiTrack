# ai06 Lesson: Box Model, Hover, and a Sticky Header

You already added box model spacing to your styles.css: box-sizing, padding, borders, margins, and cards for each section. This lesson checks that work and adds three more things from Lesson 06: nav links styled as buttons with hover and focus, a header that stays at the top of the page, and the display property.

All work in this lesson happens in your Music Website folder.

## Step 1. Set up

Tell Claude:

"Read the box model section of my styles.css. For each rule, tell me which part of the box model it changes, content, padding, border, or margin, and on which sides."

"Do I already have a rule that sets a maximum width for my main content? If so, what is it?"

Listen to both answers before you go on.

## Step 2. Center the page

If you do not have a maximum width yet, tell Claude something like this. Pick your own number.

"In styles.css, give my main content a maximum width of [your number, like 60] rem. Center it with margin auto on the left and right. Add a comment saying what the two rules do."

## Step 3. Nav links as buttons

Decide how your nav links should look. For example: a thin border, rounded corners, and a little space inside each one.

Tell Claude something like this. Fill in your choices.

"In styles.css, style the links in my main navigation as buttons. Use display inline-block so padding works on all four sides. Give each one [your padding], a [your border], and rounded corners. Put [your space] of margin between them."

"Add a hover style for those links that changes the background to my accent color and the text to my background color. Give the focus style the same look, plus an outline that is easy to see."

"Also add a hover style for every other link on the site. That was missing from Lesson 5."

"Check the contrast of the hover and focus colors. Tell me the ratio. If it is under 4.5 to 1, suggest a fix."

## Step 4. Sticky header

A sticky header stays at the top of the screen while the rest of the page scrolls under it.

Tell Claude:

"Make my header sticky with position sticky and top 0. Give it a solid background color that matches my page, so text does not show through it while scrolling."

"When I press Tab on a long page, a link must never be hidden under the sticky header. Add scroll-padding-top to the html element so the page leaves room for the header. Tell me what number you used and why."

## Step 5. Check

1. Ask Claude: "List every rule in styles.css that uses padding, border, or margin shorthand, and tell me what each value does." Make sure the answer matches what you asked for.
2. Open index.html in Chrome. Press Tab to reach the Menu button and press Enter to open it. Press Tab through the nav links. You should hear the same links, in the same order, as before this lesson. Press Enter on one. The page should open.
3. Press H to move through the headings on index.html and music.html. The headings and their order should be the same as before.
4. Open music.html. Press Tab through the links in the table until you are near the bottom of the page. Then ask Claude: "With my sticky header and scroll-padding, will a link that has keyboard focus ever be hidden under the header on music.html?" The answer should be no. If it is yes, ask Claude to fix it.
5. Ask Claude: "Describe my nav links and header as someone would see them, before and after hovering over a link, and while scrolling down music.html." Check that it matches what you asked for. If something is off, tell Claude what to change.

## Step 6. Learn

Ask Claude:

"What are the four parts of the box model from the inside out, and which part does a background color fill?"

"An element is 200 pixels wide with 20 pixels of padding on each side and a 5 pixel border. How wide is it on the screen without box-sizing border-box? How wide is it with it?"

"What is the difference between display block, display inline, and display inline-block? Show me one element on my site that uses each."

"What are three ways to hide something with CSS: display none, visibility hidden, and the visually hidden technique my skip link uses? Which ones can a screen reader still find?"

"What does position sticky do, and why does a sticky header need a solid background?"

## Step 7. Make it yours

Add a hover style to the cover art on your release pages, like a brighter border. Add a short transition so the hover change fades in instead of snapping. Change the space between your section cards and have Claude tell you how it looks now.

## Step 8. Push

Commit with the summary Box model, hover, and sticky header. Push. Make sure styles.css changed on GitHub.

## Turn in

1. styles.css and any pages that changed
2. Your answers to the questions in ai06_Questions.md, shared in Google Classroom
