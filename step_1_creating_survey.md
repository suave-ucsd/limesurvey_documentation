---
title: Step 1 - Creating Survey
parent: Full Limesurvey-SuAVE Guide
nav_order: 1
---

## {{page.title}}

The first part of this tutorial begins in LimeSurvey. Here, we're going to begin setting up our survey to collect our data.

Begin by logging into your LimeSurvey account. You will see one or more actions to take. For now we're going to click on the "List Surveys" option

![Image of LimeSurvey Survey List page](assets/Untitled.png)

This is the LimeSurvey homepage. Here you can create surveys, or monitor the ones you've created.

Here we can view the surveys we have created along with their basic information such as whether or not a survey is actively taking responses or how many responses we've received thus far.


There will be a button in the top left corner of the homepage that reads "Create a new Survey." Press this to begin the survey creating process.

![Image of New Survey page](assets/Untitled%201.png)

Here we have many options to customize the functionality of our survey. You can read more about the specifics of each option [here, as part of LimeSurvey's documentation.](https://manual.limesurvey.org/Surveys_-_introduction)

To begin, enter the title of your survey. Here you can also enter a description for the survey and a welcome message, which the users will be able to read before they begin their survey response. We will revisit the "End message" soon, but first we need to save the survey in order to initialize it.

Press the "Save" button in the upper right hand corner.

### Write Down Your Survey ID

![Zoomed in image of survey title and ID](/assets/Untitled 2.png)

After saving, you should be redirected to your survey homepage. Here, you can revise the settings of the survey and make changes to it's functionality.

You should see a number in parenthesis next to the title of your survey. Write this number down as we will need to use it in the following step.

- For example, in the above picture we see that our Survey ID is 772653

### Create an End Message

Next, we're going add an end message and include an important piece of code that allows our survey to function correctly.

Select the menu item titled "Text elements" in the sidebar of your survey homepage.

![Image of survey summary with highlighted "Text elements" navigation menu item](/limesurvey_suave/assets/Untitled 3.png)

You will now see a page that looks very similar to the starting page of our survey creation.

Click on the toggle that reads "Toggle Source Code" to the right of the End Message block.

![Image of "Toggle Source mode" button](/assets/Untitled 4.png)

Your End Message block should now look like this:

![Image of blank "End Message" text box](/assets/Untitled 5.png)

Copy this block of code and paste it into the "End Message" block

```jsx
<script type="text/javascript" charset="utf-8">
              $(document).ready(function(){
                  var val = {SID}
                             $.ajax({
            url: 'https://limesurvey-flask.sdsc.edu',
            type: 'GET',
            dataType:'json',
            data: {
              survey_id: {SID},
              token: "{TOKEN}"
            },
            success: function(data){
                console.log(data);

            },
                             });
              });
</script>
```
Now it should look like this:

![Image of "End Message" script after replacing survey id](/assets/new_script.JPG)

You can then add whatever ending message you want by adding more html code, or replacing the text that says "Thank you for participating in this survey!" For example, you can enter

```jsx
<p>Thank for your submitting your information!<br>&nbsp;</p><p>To edit your responses to this survey, click <a href="https://limesurvey.sdsc.edu/limesurvey/index.php/123456?token={TOKEN}&amp;lang=en">https://limesurvey.sdsc.edu/limesurvey/index.php/123456?token={TOKEN}&amp;lang=en</a></p><p>Your access code for this survey is: {TOKEN}.</p><h3>To view survey responses in SuAVE <a href="https://suave2.sdsc.edu/main/file=surveyauthor_surveyname.csv&amp;view=grid">Click here</a></h3>
```

**Important:** Make sure you press the green save button in the top right before moving on to the next step.

After Saving, you can click the "Toggle Source Code" button again in order to preview what the ending message will look like. This is what the above source code looks like to the survey participant:

![Image of "End Message" box with "source mode" toggled off](/assets/Untitled 8.png)

- **Note:** If you want to change the end message in the future, you may have to repeat this step and paste in the code again
