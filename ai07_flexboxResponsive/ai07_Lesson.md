# ai07 Lesson: Flexbox and a Site That Works on a Phone

Flexbox lines things up in a row or a column and decides how the space between them is shared. A media query changes the layout when the screen is small, like a phone. In this lesson you put your nav and a new row of release cards into flexbox, make the site work on a phone, and save a template page to start every new page from.

All work in this lesson happens in your Music Website folder.

## Step 1. Set up

Tell Claude:

"Check that every HTML file in my Music Website folder has the viewport meta tag in the head. List any that do not, and add it to them."

"Tell me what the viewport meta tag does on a phone, and what a phone shows if a page does not have it."

## Step 2. Flexbox nav

Tell Claude:

"In styles.css, make the list in my main navigation a flexbox row. Use display flex on the list, a gap of [your choice, like 0.75] rem between the links, and flex-wrap wrap so the links move to a new line when the screen is narrow. Remove the list bullets and the extra space on the left of the list."

"Do not change the order of the links in the HTML."

## Step 3. A row of release cards

Pick three releases you want visitors to find first.

Tell Claude something like this. Fill in your three releases.

"On music.html, right after the Current Album section, add a section called Featured Releases. Inside it, put three article elements, one for each of these releases: [your three]. Each article has the cover art with its alt text, the release name as a heading level three that links to its page, and one sentence about it."

"In styles.css, make the three articles a flexbox row with a gap between them. Give each card flex 1 so they share the row evenly, and a minimum width of 15 rem so they wrap to the next line when there is not enough room. Use the same card look as my sections."

## Step 4. Images and media that fit

Tell Claude:

"Make every image, audio player, and video on the site shrink to fit the screen. Use max-width 100 percent, and height auto for images."

"My Discography table is wide. On a small screen, it should scroll sideways inside its own box instead of making the whole page scroll sideways. Check my table-wrap class and fix it if it does not do that."

## Step 5. Media query for phones

Tell Claude:

"At the very bottom of styles.css, add a media query for screens 768 pixels wide or narrower. Inside it, stack the nav links in a column, put the release cards one per row, and use less padding on the section cards. Add a comment saying what the media query is for."

## Step 6. Save a template

A template is the empty starting point for every new page, so every page has the same parts.

Tell Claude:

"Make template.html in my Music Website folder. It has the same head as my other pages, with the viewport tag, the link to styles.css, and menu.js. It has the skip link, header, main navigation, an empty main with id main-content, and the footer. Put a comment at the top saying that every new page starts as a copy of this file."

## Step 7. Check

1. Ask Claude: "List every HTML file in my Music Website folder that is missing the viewport meta tag." The answer should be none.
2. Open music.html in Chrome. Press H to move through the headings. You should hear Featured Releases, then each release name as a level three heading, in the order you asked for.
3. Press K to move through the links in the Featured Releases section. Each card link should open the right release page.
4. Ask Claude: "Describe how music.html looks on a phone 375 pixels wide and on a laptop 1200 pixels wide. Is anything cut off, and does any part of the page make the whole screen scroll sideways?" The only thing that should scroll sideways is the Discography table, inside its own box.
5. Try the order test. Tell Claude: "Add flex-direction row-reverse to my main navigation list, but do not change the HTML." Open index.html and press Tab through the nav links. Ask Claude what order the links look like on the screen now, and compare it to the order you heard. Then tell Claude: "Take the row-reverse back out."

## Step 8. Learn

Ask Claude:

"In flexbox, what is the difference between justify-content and align-items?"

"What does flex-wrap do, and what happens to my cards without it?"

"What does max-width 768 pixels mean in a media query? What does mobile-first mean, and how is it different?"

"After the row-reverse test, why did the order I heard not match the order on the screen? Why is that a problem for a keyboard user who can also see the page?"

"In two sentences, how is CSS Grid different from flexbox?"

## Step 9. Make it yours

Make your footer a flexbox row with your name on one side and your email on the other, stacked on a phone. Add a fourth featured release and have Claude describe how the row wraps. Make your next new page by copying template.html.

## Step 10. Push

Commit with the summary Flexbox and phone layout. Push. Make sure template.html shows up on GitHub.

## Turn in

1. styles.css, music.html, template.html, and any pages that changed
2. Your answers to the questions in ai07_Questions.md, shared in Google Classroom
