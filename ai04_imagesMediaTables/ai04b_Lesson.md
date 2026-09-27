# ai04b Lesson: A Page for One New Release

## Step 1. Set up

Tell Claude something like:

"Make a folder called ai04b_releasePage in my repository folder. Copy all of my site pages and image files from the folder my site is in into it. Add one more nav link on every page, pointing to release.html. The link text is the name of the release."

All work in this lesson happens in ai04b_releasePage.

## Step 2. Get your audio

A link to a music service is not a player. Those services do not let you put their player inside your own page, and there is no code that gets around that. If you want people to hear something without leaving your site, the audio file has to live in your own folder.

1. Get 30 to 60 seconds of one track as an MP3 from the software you produce in.  You can use an entire track if you like...
2. ... but a short preview is enough. It keeps the file small and keeps a full release out of a public repository.
3. Name it with lowercase letters and no spaces, like preview.mp3.

Tell Claude:

"Make a folder called audio in my ai04b_releasePage folder and put my MP3 in it."

## Step 3. Decide what to say

1. The alt text for the cover art. This is what the screen reader reads instead of the picture. Describe what the artwork looks like. One or two sentences.
2. The caption for the cover art. This is information about the release. When it came out, what it is, who worked on it. Not a second description of the picture.
3. Your track list. For each track: the name, how long it is, and anything else you want in a column.
4. The total running time of the release.

## Step 4. Build

Tell Claude something like this. Fill in with your own details/content.

"Make release.html in my ai04b_releasePage folder with the same header, nav, footer, and skip link as my other pages. The title is the name of the release. The heading level one says the name of the release."

"Add a section called About This Release with a paragraph about it."

"Add a figure element. Inside it, put the cover art image and a figcaption under it. Here is the alt text and here is the caption." Then give Claude both.

"Add a section called Listen with an audio element that has the controls attribute. The file is in my audio folder. Inside the audio element, put a sentence saying the browser cannot play the file, and a link to download it, for browsers that cannot play audio."

"Add a section called Track List with a table. The table has a caption. The header row uses th cells with scope column. Here are the columns and here are the rows." Then give Claude your track list.

"Add one more row at the bottom of the table. The first cell says Total running time and spans across the columns before the last one. The last cell has the total." Then tell Claude the total.

"On my main music page, add a link to release.html. On release.html, add a link back to the music page."

## Step 5. Check

Open release.html in Chrome.

1. Press G to move to the cover art. You should hear your alt text, not a file name.
2. Press Down Arrow after the image. You should hear the caption. It should tell you something the alt text did not. If you hear the same sentence twice, one of them needs to be rewritten.
3. Find the audio player. Press Tab to reach the play button and press Enter. Your clip should play. Press Enter again to pause. If there is no player at all, the controls attribute is missing or the file name is wrong. Tell Claude what you heard.
4. Press T to jump to the table. You should hear the caption, and the number of rows and columns.
5. Press Control plus Alt plus Right Arrow to move across a row. The screen reader should say the column header before each cell.
6. Move to the last row. The total running time should line up under the right column. If the numbers do not add up, the row spans the wrong number of columns. Tell Claude how many columns the table has.
7. Press K to go through the links. Go to the music page and back again without using the browser's back button. If you cannot get back, one of the two links is missing.

## Step 6. Learn

Ask Claude:

"Why can a link to a music service not be used as the file for an audio element?"

"What does the colspan attribute do, and how do I know what number to give it?"

"What is inside an audio element for, if the browser can play the file?"

## Step 7. Make it yours

Add a second release page. Add more columns to the table, like the format or the year. Add a link to where people can stream the full release. Check the page again after.

## Step 8. Push

Commit with the summary Release page. Push. Make sure the audio folder shows up on GitHub.

## Turn in

1. release.html and the updated pages, with the audio folder
2. Your answers to the questions in ai04b_Questions.md, shared in Google Classroom
