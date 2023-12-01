---
title: Additional Tool - Question Choice Help
parent: Full Limesurvey-SuAVE Guide
nav_order: 8
---

## {{page.title}}

**Included below are the purpose of each question and question type in Limesurvey. To successfully use this, narrow down first by question type (single choice, multiple choice, etc.) and then to the specific question type (list (radio), list (dropdown), etcetera). While this guide will be useful, it is most useful to practice and get a feel for how each question type is encoded.**

**Disclaimer**: Every question has aspects of it that you can edit such as making the question mandatory, adding an “Other” option, answer validation (such as at least 100 characters). To edit these, while creating the question, look at the right tab (as shown). Look through to make the changes you want.

![Image](assets/Screenshot%202023-12-01%20at%201.29.27%20PM.png)


## Single Choice Questions
**Use this question type for questions that should only have one answer**

### 5-point choice
Use this question type for when you have a question, where the responses are 1 through 5. Using this question type is quite uncommon. A perk to this question type is that there is a “no answer” button, if needed.

### Bootstrap buttons 
This question type is typically used for stylistic reasons, where each answer choice is a big green button that you can select.  

### Image select list (Radio) 
Use this question type when each possible answer choice has a picture associated with it. To add pictures, get the picture URL and, in the space where you fill in the question text, click on the pencil next to it. Then, click on the picture image and paste the URL. Do this for every image you want to add.

### List (dropdown)
Use this question type when there are many possible answer choices, where users are to only select one. For example, this is commonly used when selecting the state/country the user is from (for appearance purposes as List (radio) would take up a lot of space on the survey whereas List (dropdown) hides the answer choices you don’t choice in the dropdown box).  

### List (radio) ** popular **
This is the most popular question type for single choice questions. It allows for an “other” option (if chosen), where you have the option to force users to specify what “other” indicates. You can also add a comment to the “other” answer.

### List with comment
Use this question type when some sort of rationale should be added to a selected answer choice. This question type allows users to write a comment that is attached to their answer choice. 

## Arrays
**Use this question type for when you want to ask the same question(s) for a series of questions such as rate x, y, and z on a scale from 1 to 7, where 1 = unsatisfied and 7 = extremely satisfied.**
### Array
Use this question type when you have multiple questions that can be answered on the same scale. You can specify the scale for this question type, unlike other array question types. The most common is a scale from 1 to 7.

### Array (5 point choice)  ** popular **
Use this question type when you have multiple questions that can be answered on the same scale, where the scale spans from 1 to 5.

### Array (10 point choice)
Use this question type when you have multiple questions that can be answered on the same scale, where the scale spans from 1 to 10.

### Array (Increase/Same/Decrease)
Use this question type when you have multiple questions that can be answered on the same scale, where the scale is Increase, Same, or Decrease.

### Array (Numbers) 
Use this question type when you have multiple questions that require multiple numerical answers. For example, for x, y, and z, specify the height, width, and length in feet.

### Array (Texts) 
Use this question type when you have multiple questions that require multiple text answers. For example, for x, y, and z, comment on the color, unique traits, and who created it.

### Array (Yes/No/Uncertain)
Use this question type when you have multiple questions that can be answered on the same scale, where the scale is Yes, No, or Uncertain.

### Array by column
This question type is uncommon as it is the same as the Array question but transposed, meaning rows are columns and columns are rows. Typically, avoid it unless you prefer its style.

### Array dual scale
Use this question type when you have multiple questions that requires two separate answers. For example, for x, y, and z label its price and weight, from very cheap/light to very expensive/heavy.

## Multiple Choice Questions
**Use this question type for when there are one or more answers for a question. This question type also allows for an exclusive “None of the Above” option.**

### Bootstrap buttons
This question type is typically used for stylistic reasons, where each answer choice is a big green button that you can select. 

### Image select multiple choice
Use this question type when each possible answer choice has a picture associated with it. To add pictures, get the picture URL and, in the space where you fill in the question text, click on the pencil next to it. Then, click on the picture image and paste the URL. Do this for every image you want to add.

### Multiple choice  ** popular **
Use this question type as the default multiple choice question type. This question type allows for exclusive “None of the above” option (if chosen, it is the only response that can be chosen) and “Other” option with specifciation of what other references.

### Multiple choice with comments
Use this question type when some sort of rationale should be added to a selected answer choice(s). This question type allows users to write a comment that is attached to each of their answer choices. 

## Text Questions
** Use this question type for when the response to a question should be written. This also include questions that should be answered by pinning a point on a map. **

### Browser Detection?
This question type is quite rare as it detects the browser the user is using to fill out the survey. Use it if you want to know this information.

### Huge Free Text
Use this question type if the question requires a very long text responses (typically multiples paragraphs or more).

### Input on demand
This question type is quite rare as it allows users to answer questions on by one. They need to click a button to access the next text box if they want to answer more.

### Long free text  ** popular **
Use this question type if the question requires a long text responses (typically a paragraph or more).

### Multiple short text  ** popular **
Use this question type if you want to ask multiple questions that require short responses (typically a paragraph or less) related to a single topic.

### Short free text  ** popular **
Use this question type if you want to ask a question that require a short response (typically a paragraph or less).

### Short free text - Map  ** popular **
Use this question type as well if you want users to pinpoint something important on a map. The map can be configured to your needs such as default point, map view type, scope of map (very zoomed in versus zoomed out), etcetera. Please explore all options to edit the map to what you would like.

## Mask Questions
** Use this question type for when the above choices do not apply to your scenario. This question type includes equations, language changes, date selection, file upload, etcetera. **

### Date/Time
Use this question type if you want user answers to a questions to be in a date format.

### Equation  ** popular **
Use this question type if previous answers in the survey can be used to fill out a specified equation (by the survey creator). This value resulting from the equation can be stored in the Google Sheets of answers.

### File Upload  ** popular **
Use this question type if you want people to upload particular files. This can be projects pdfs, images (**common for SuAVE visualizations**), or other files. You also have the option to specify acceptable file types.

### Gender
Use this question type if you want users to specify their gender. You can achieve the same result by creating a “Single Choice Question” and assigning the available response choices as the genders.

### Language switch
Use this question type if you want the survey to be able to be filled out in multiple languages.

### Multiple numerical input
Use this question type when you want multiple responses to only be numbers. It is particularly useful when uploading data. Make sure, however, to specify what units the result should be measured in if it could be unclear. Additionally, only use this option if the numerical responses somehow correlate with one another; if they do not, it could confuse the user. This question type is commonly used in tandem with “Equations”.

### Numerical input  ** popular **
Use this question type when you want a response to only be numbers. It is particularly useful when uploading data. Make sure, however, to specify what units the result should be measured in if it could be unclear. This question type is commonly used in tandem with “Equations”.

### Ranking
Use this question type when you want to rank a list of items.

### Ranking advanced
Use this question type when you want to rank a list of images. To add pictures, get the picture URL and, in the space where you fill in the question text, click on the pencil next to it. Then, click on the picture image and paste the URL. Do this for every image you want to add.

### Text display ** popular **
This question type is specifically used to display text. If you have something important to convey to those filling out the survey, use this question type.

### Yes/No
The question type is used for yes or no questions. You could achieve the same result by creating a single choice question and making the only two answers yes and no (with no “Other” option, which is the default selection). 


