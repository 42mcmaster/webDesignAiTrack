# ai04 Lesson: Images, Audio, and a Table

You add a media page to your site. It has images with alt text, an audio player with one of your tracks, and a table of your tracks.

## Step 1. Set up

Tell Claude:

"Make a folder called ai04_imagesMediaTables in my repository folder. Copy index.html, about.html, music.html, and bio.txt from my ai03_linksAndNav folder into it. Add a fourth nav link on every page: Media, pointing to media.html."

## Step 2. Get your files

1. Put two or three images in a folder called images inside ai04_imagesMediaTables. Cover art you made, a photo of your gear, or a photo of you. Use lowercase file names with no spaces, like cover1.jpg.
2. Put one of your tracks as an MP3 in a folder called media. Keep it under 10 MB. Name it something like track1.mp3.
3. For each image, decide what the alt text should say. Alt text is what the screen reader reads instead of the picture. You write it. If you are not sure what a photo shows, ask someone, then write it in your own words. One short sentence each.

## Step 3. Build

Tell Claude this. Fill in your file names and alt text.

"Make media.html in my ai04_imagesMediaTables folder with the same header, nav, footer, and skip link as the other pages. The title is Media. Heading level one says Media."

"Add a section called Pictures. For each image, use a figure element with the img inside and a figcaption under it. Here are the file names, the alt text for each, and the caption for each." Then give Claude your list.

"Add one decorative divider image between sections with empty alt text so screen readers skip it." You can ask Claude to make a simple divider image for this.

"Add a section called Listen with an audio element that has controls. The file is media/track1.mp3. Put the track name in a heading level two above it."

"Add a section called Track List with a table. The table has a caption that says My Tracks. The header row uses th cells with scope column. The columns are Track, Year, Length, and Style. Here are four rows." Then give Claude four tracks.

## Step 4. Check

Open media.html in Chrome.

1. Press G to move to each image. You should hear your alt text, not a file name. The decorative image should be skipped.
2. Find the audio player. Press Tab to reach the play button and press Enter. Your track should play. Press Enter again to pause.
3. Press T to jump to the table. You should hear the caption, and the number of rows and columns.
4. Press Control plus Alt plus Right Arrow to move across a row. The screen reader should say the column header before each cell. If it only says the cell, the header row is wrong. Tell Claude to fix the th cells.

## Step 5. Learn

Ask Claude:

"What is the difference between alt text and a figcaption?"

"When should an image have empty alt text?"

"What is the difference between JPG, PNG, and SVG?"

## Step 6. Make it yours

Add more tracks to the table, more images, or a second audio player. Check the page again.

## Step 7. Push

Commit with the summary Media page. Push. Make sure the images and media folders show up on GitHub.

## Turn in

1. media.html and the updated pages, with the images and media folders
2. Your answers to the questions in ai04_Questions.md, shared in Google Classroom
