# ai08 Lesson: A Contact Form for Your Site

Right now your Contact page has your email address. In this lesson you add a form that visitors can fill out to ask you about collaboration, production, or a booking. You use every kind of form control the class learns in Lesson 08, and you make sure each one is labeled and grouped so it is easy to fill out.

All work in this lesson happens in your Music Website folder, on contact.html.

## Step 1. Plan the form

Decide these before you tell Claude:

1. What the form is for. For example: a request to work with you.
2. The kinds of requests a visitor can pick from. Three or four, like collaboration, production, booking, or other. These become radio buttons, because a visitor picks only one.
3. Three or more things a visitor can check, like the genres they are interested in. These become checkboxes, because a visitor can pick more than one.
4. A question with a list of answers, like how the visitor heard about you. This becomes a dropdown.
5. Which fields are required. At least the name, the email, and the message.
6. The words on the submit button. Something better than Submit, like Send Request.

## Step 2. Build the form

Tell Claude something like this. Fill in your plan.

"On contact.html, after the Get In Touch section, add a section called [your form name] with a form. The form has action set to a number sign, because there is no server yet, and method get."

"Group the form into three fieldsets, each with a legend: About You, Your Request, and Your Message."

"In About You, add a text input for the visitor's name and an email input for their email. Both are required."

"In Your Request, add a group of radio buttons for the kind of request: [your choices]. They all share the same name, so only one can be picked. Put the radio buttons in their own fieldset with the legend Kind of request. Then add checkboxes for [your choices], in a fieldset with the legend [your legend]. Then add a select dropdown for [your question] with these options: [your options]."

"In Your Message, add a textarea for the message. It is required."

"Give every input, select, and textarea a label element. Connect each label to its control with a for attribute that matches the control's id. Give every control a name attribute."

"At the end, add a submit button that says [your button words], and a reset button that says Clear Form."

"Do not use placeholder text in place of labels, and do not add any tabindex attributes."

## Step 3. Style the form

Tell Claude:

"In styles.css, style the form to match my site. Give each fieldset padding, a border, and margin between them. Put each label on its own line above its control, except for radio buttons and checkboxes, which have the label right after the control. Make the text inputs, select, and textarea the full width of the form, with my body font."

"Give every input, select, textarea, and button a focus style that is easy to see, using my accent color. Give the buttons the same hover and focus look as my nav links."

"On a phone, make the buttons full width."

## Step 4. Check

1. Open contact.html in Chrome. Press F to jump to the first form field. You should hear the label, the kind of field, and that it is required, like Name, edit, required.
2. Press Tab through the whole form. You should hear every label, in the same order as the form. When you enter a fieldset, you should hear its legend. If a field has no label, tell Claude which one.
3. In the radio buttons, press the Down Arrow to move between choices. You should hear each choice and how many there are, like 2 of 4. Only one should be checked at a time.
4. In the checkboxes, press Space to check two of them. Both should stay checked.
5. Tab to the dropdown and press Alt plus Down Arrow to open it. You should hear each option.
6. Press Tab to the submit button and press Enter with the form empty. The browser should stop you and tell you which field is required.
7. Fill in everything and send it. Press Alt plus D to move to the address bar and listen to the web address. You should hear a question mark, then each name and answer, like name=your name. If one of your answers is missing, that control has no name attribute.
8. Press the Clear Form button. Tab back through the form. Everything should be empty.
9. Ask Claude: "List every form control on contact.html that is missing a label, a name, or an id, and any label whose for does not match an id." The answer should be none.

## Step 5. Learn

Ask Claude:

"How does a label get connected to its input? What does that give someone using a screen reader, and what does it give someone using a mouse?"

"What is the difference between radio buttons and checkboxes? When is each one the right choice?"

"What does a legend do for a group of radio buttons?"

"What is the difference between method get and method post? Why do real contact forms use post?"

"What does the action attribute do? What would happen on a real website when someone sends my form?"

"Why are placeholders not a good replacement for labels?"

"What does tabindex do, and why is it usually better to fix the order of the HTML instead?"

## Step 6. Make it yours

Add a date input for when the visitor wants to work together. Add a number input for how many tracks they want, with a minimum and a maximum. Add a short line under the email field that tells visitors you never share their email. Check the form again after each change.

## Step 7. Push

Commit with the summary Contact form. Push. Make sure contact.html and styles.css changed on GitHub.

## Turn in

1. contact.html and styles.css
2. Your answers to the questions in ai08_Questions.md, shared in Google Classroom
