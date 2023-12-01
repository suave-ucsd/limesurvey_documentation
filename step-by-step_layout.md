---
title: Steps to Follow
parent: Full Limesurvey-SuAVE Guide
nav_order: 1
---

# Full Guide to Limesurvey

## Part 1 - Creating a Survey

Go [here]()

## Part 2 - Adding Questions

Go [here]()


## Part 3 - Encode Questions in Google Sheets

Go [here]()

## Part 4 (Optional) - Survey Logic

Survey Logic is a high level concept that manipulates the survey in a way that certain questions are only available based on answers to previous questions. If you are not familiar with this, then this may not be the best idea, unless it is very basic.

********************************************************************************************************************************************************************************************
Include exactly how to do it
********************************************************************************************************************************************************************************************

## Part 5 (Optional) - Creating SuAVE Visualization

********************************************************************************************************************************************************************************************
Copy existing stuff 
********************************************************************************************************************************************************************************************

To test if you properly synched your Limesurvey survey to the SuAVE visualization, manually enter a response to the survey in the Google Sheets. After a few minutes, navigate to the correct SuAVE visualization; it should appear now. If not, make sure you followed every step correctly. If it works fine, clear the fake entry in the Google Sheets file.

## Checkpoint

- By now you should have the **survey id** and a list of the **question codes** that pertain to the responses you would like to display in SuAVE
- Checklist
  - [ ] Completed Limesurvey survey
  - [ ] Google Sheets Mapper
  - [ ] Working SuAVE Visualization


## Part 6 - Sending Out Your Survey

When sending out your survey to get responses, you have two options: sending out personalized links based on a participants table or a registration form. If you have a list of participants that should fill out the survey (such as a class roster), follow **Part A**; if you do not have a list of participants that should fill out the survey and want anybody willing to fill out the survey to do so, follow **Part B**.

#### Part A - Defined Participants Table
********************************************************************************************************************************************************************************************
MAKE SURE ITS first name, last name, and email
FINISH THE LIST SO THAT IT IS ACCURATE
********************************************************************************************************************************************************************************************
1. Get your participants table. The table needs the following three columns at the minimum: first name, last name, and email. 
2. Export this file as a csv
3. Navigate the the Participants tab in Limesurvey
4. If prompted to, make the survey closed access and initialize a participants table (if these options do not pop up, do not worry)
5. Under the Participants tab, navigate to “Import” and upload your csv
6. Create tokens for each participant. Click “Generate Tokens” and hit “Create”
7. Now, edit your survey email templates. Navigate to “Email templates”
8. Edit these templates as you see fit. Make sure to edit both the “Invitation” and “Reminder” email templates
9. Once you are ready, go back to the “Participants” tab. Select all participants you want to send the survey to and click on “With Selected”. Click “Send Invitation”
10. Some people may not receive the email or may not acknowledge the email and fill out the survey. If this is the case, send a reminder email to individuals that do not fill out the survey at your discretion.

#### Part B - Creating a Registration Form
********************************************************************************************************************************************************************************************
Copy existing stuff 
********************************************************************************************************************************************************************************************

## Part 7 - Accessing Results

Once you have sent out your survey—via a survey registration form or personalized link—responses to your survey will start coming in. Sometimes, the Google Sheets form will not automatically update to include all responses. To manually, update the Google Sheets with responses, go to [https://limesurvey.sdsc.edu/limesurvey-update](https://limesurvey.sdsc.edu/limesurvey-update). You will be prompted for a username (**lsadmin**) and a password (**VocalMimic**). Next, enter your 6-digit survey identifier and click “Update”. Once the little gray box that says that everything has updated properly pops up, all responses should now be available in the Google Sheets.


