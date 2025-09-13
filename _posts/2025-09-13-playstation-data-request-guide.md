---
title: "PlayStation Data Request Guide"
author: bigbud
date: 2025-09-13
description: "Step-by-step guide on how to request your PlayStation data through the official Sony website and mobile app, including details on what data you receive."
tags: [PlayStation, Data, Privacy, Guide]
categories: [PlayStation, Tutorial]
image: /assets/DataRequest.png
---

## Before We Begin
This post is a written guide about how to request your PlayStation data through the mobile app/PlayStation web. The process is easy and straightforward.

The same process works on the mobile app and for the PlayStation website if you're on your PC. They are almost the same steps.


## Mobile Part

1. Open the PlayStation app.  
2. Click your profile, then select **Edit Profile**.  

![EditProfilePS](/assets/PSNApp/EditProfilePS.jpg)

> Note: you may be prompted to log in to your PSN account.


## All platforms

If you're on PC or you prefer the PlayStation web, this part is the starting point.

1. Sign in to your PlayStation account on the [PlayStation.com](https://www.playstation.com) website.  
2. After you log in, click on your profile picture/avatar and then **Account Settings**, you will be on this screen:  

   ![ThisScreenPSWeb](/assets/PSWeb/ThisScreenPSWeb.jpg)  
3. **If not**, and you're on this page in the image below, click on the 3 lines in the top left corner:  
   ![TopLeftCorner](/assets/PSWeb/TopLeftCorner.jpg)  
4. Choose **Privacy Settings**:  
   ![Privacy Settings](/assets/PSWeb/PrivacySettingsClick.jpg)  
5. You will now be on this screen:  
   ![PSSett](/assets/PSWeb/PrivacySettingsSection.jpg)  
6. Scroll down & you'll find the **Access Your Personal Information** section:  
   ![ScrollingDown](/assets/PSWeb/ScrollingDown.jpg)  
7. Click on the **Data Access Requests** button. You'll be taken to a page with instructions on what data they will send you and the email address it will go to.  

> Note: it may take a couple of hours or days depending on the account.  

Once you receive the message by email, you will have 7 days to download your data.


## Breakdown of the data you get

You will get an email from PlayStation saying *"Your personal information is ready to download"*.  

Example:  
![ReadytoDownload](/assets/PSWeb/ReadytoDownload.jpg)  

1. Click the link inside the email.  
2. You will be redirected to PlayStation's site and prompted to log in.  
3. If you log in successfully, the file will automatically download.  

The file name should look like this:

```DataReport-{USERNAME}-{random}```

Inside the zip file, you will be provided with an `.xlsx` file.  

This file includes a list of **Console ID**, **Name**, **Console Type**, and **Account ID**.


| Console Id         | Name | Console Type | Account Id         |
| ------------------ | ---- | ------------ | ------------------ |
| 0227***********897 |      | PS4          | 2649***********603 |
| 0227***********686 |      | PS3          | 2649***********603 |
| 0227***********686 |      | PS3          | 2649***********603 |
| 0327***********624 |      | PS3          | 2649***********603 |
| 0327***********624 |      | PS3          | 2649***********603 |



> Note: Duplicates may appear if you’ve logged into the same console multiple times

**Console Id:** A unique identifier assigned to each PlayStation console  

**Name:** A label for the device (I'm not sure why it's blank on my end)  

**Console Type:** The model of PlayStation linked (PS3, PS4, etc.)  

**Account Id:** Sony’s internal unique number for your PSN account


## My Final Word
At the end of this, the data you receive will mainly show how many consoles are linked to your account and what type they are. That’s basically all Sony provides through this method.

If you want a deeper look into your account, PSNTools offers more detailed data extraction. With it, you can view/extract things like how many times you’ve changed your PSN ID, what your previous IDs were, and other details.

So, if your goal is more than just checking linked consoles and useless info, then PSNTools may be the better option
