---
title: "Free Alternatives to Save Wizard for PS4/PS5 Game Saves"
date: 2025-06-01
description: "A detailed guide to free Discord-based alternatives to Save Wizard, covering features like re-signing, re-regioning, and how to use these tools for PS4 game saves."
comments: true
author: bigbud
categories: [PlayStation, Save Modding]
tags: [ps4, ps5, save wizard, re-sign, re-region, discord bot, game saves, save modding, cusa codes]
hidden: true
---

## What is Save Wizard?

For those who don't know, Save Wizard is a paid tool that lets you mod your PS4 game saves. You can do things like:

- Add infinite money
- Unlock cosmetics
- Max out XP or levels

So in everyday English, it's basically a tool to edit your save data.

---

## What are these alternatives to Save Wizard?

Basically, these are free alternatives to Save Wizard. These alternatives are available on Discord and offer similar functions for free by using Discord as their platform.

---

## Where can I find them?

They're on Discord, and there are a bunch of Discord communities that have them. Here are the communities I know so far with the bots:

- [https://discord.gg/fnntcGCC6z](https://discord.gg/fnntcGCC6z)
- [https://discord.gg/psbot](https://discord.gg/psbot)  
  If this one doesn't work, then use the Permanent Link:  
  `https://discord.gg/dyapjAPdCT`

This section will keep being updated with more links.

---

## Why is it on Discord?

Discord is a popular communication and community platform that also supports bots, which are programs that automate tasks. These bots run inside Discord, so users don’t have to install random applications - they only need Discord, which is available on PC, browser, and mobile. They just use the commands on Discord, making it accessible and easy to use for everyone.

---

## What does the bot do?

These bots help you modify PlayStation game saves by allowing you to re-sign and re-region them, among other features. They handle PS4 saves using a jailbroken PS4.

---

## What are the features of this bot?

- Re-sign saves and re-region them.
- Decrypt encrypted saves.
- Change the picture of encrypted saves.
- Change the titles of encrypted saves.
- Convert game saves from PS4 to PC or vice versa (some games require extra conversion).
- Add quick cheats to your games.
- Apply Save Wizard quick codes to your saves.
- And more.

For more information, check [https://github.com/hzhreal/HTOS/blob/main/README.md](https://github.com/hzhreal/HTOS/blob/main/README.md)

---

## Re-sign

Re-signing means taking a save file that belongs to someone else and changing its account ID or "username" so it works on your PlayStation account. 

For example, let's just say you found a save on the internet or your friend has a save with a cosmetic you want or has a lot of stuff in a game and you want to use that exact save, you cannot just copy it directly because it’s tied to their account. You must re-sign the save with your own account ID so the PlayStation system recognizes it as yours.

---

## Re-region

Re-regioning means changing the region code of a save so it matches your account's region. Basically, re-regioning changes the region of a save file. Let’s say you downloaded a save from someone who has the US version of the game, but your game is the EU version. Even though it’s the same game, it won’t load unless the region matches.

You can tell the region of the save by the CUSA code using [orbispatches](https://orbispatches.com/). It shows up like this:

```text
CUSA12345
```

Here is an example table of the same game but multiple regions/different CUSA numbers:

**Red Dead Redemption 2:**

- [CUSA08519](https://orbispatches.com/CUSA08519), [CUSA15698](https://orbispatches.com/CUSA15698) → EU
- [CUSA08568](https://orbispatches.com/CUSA08568) → JP
- [CUSA03041](https://orbispatches.com/CUSA03041) → US

They are the same game but different regions for the save. Re-signing isn't enough and won't work for your game. That's why you have to re-region it. And if you do re-region it, it doesn't matter what previous region it was. It will still work on your own region.

If your game and the save have different CUSA codes, you need to re-region it to match.

---

## Does This Really Work on PS5?

Sort of. PS5 saves can’t be copied to the USB like PS4 saves, but some games support a feature called 'cross-save'. That means the PS5 version of the game can read your PS4 save of the same game.

So you can re-sign or re-region a PS4 save, then load it into the PS5 version of a game that supports cross-save. It's limited, but it works for games that have that feature.

I'll make a separate blog or article later explaining cross-save in much detail.

---

## What You Need Before You Start

- A Discord server with one of the Save bots (There are many, and it doesn’t matter which one you use. Just make sure they support slash commands.)
- A USB flash drive to move saves between your console and phone or PC.
- If you’re on mobile: a USB adapter to connect your flash drive to your phone.
- A way to upload your saves. You can upload saves directly to the bot in Discord, but this is important: if the file is large or giving errors, just upload it to Google Drive and share the link. Make sure your link is set to "anyone with the link can view/edit".

---

# Getting Started

## Threads

Click the create thread button in the channel that the bot's message is in. Then you will get pinged or mentioned by the Discord bot in a new thread. After that, you can use the commands there.

**Disclaimer:**  
If you get "The application did not respond," it means the bot is not online. Ping the moderators or the bot admin for help.

Now, after you are in the new thread, use this command:

```text
/ping
```

to check if the bot is working and online.

Next, it depends on what you want. Do you want to re-region, re-sign, or other? Check the TOC (Table of Contents).

---

## Re-sign Command

Now type in the thread:

```text
/resign
```

There will be optional buttons that will pop up after writing the command. One of them is:

```text
playstation_id:
```

Click on it, and after you do, it should look like this:

```text
/resign playstation_id:
```


Now type in your PlayStation username.

> The bot stores you discord ID and the PSN Account ID. So even if you change your username it will still know what your ID is to use the commands on it. So if you gave thr bot your playstation username you don't have to type /reregion playstation_id: just type /reregion without the playstation_id:
 {: .prompt-info }

Then he bot will respond with:

> Please attach at least two encrypted save files that you want to upload (.bin and non-bin). Or type 'EXIT' to cancel command.

Either attach 2 save file pairs in your CUSA folder on discord or Google Drive.  
Example of a save pair: `SAVEDATASGTA50000` & `SAVEDATASGTA50000.bin`  
They are found in:

```text
PS4/SAVEDATA/{account ID}/{CUSAXXXX}/{files}
```

Now you're done.

---
## Re-region Command

```text
/reregion
```

Type that command to reregion your save. 

There will be optional buttons that will pop up after writing the command. One of them is:

```
/reregion playstation_id:
```

Now type in your PlayStation username.

>Showing the info prompt: The bot stores you discord ID and the PSN Account ID. So even if you change your username it will still know what your ID is to use the commands on it
  So if you gave thr bot your playstation username you don't have to type /reregion playstation_id: just type /reregion without the playstation_id:
{: .prompt-info }

The bot will respond with:
> **Re-region process: Upload encrypted files from YOUR region**
> Please attach two encrypted savefiles that you want to upload (.bin and non bin). Or type 'EXIT' to cancel command.

Either attach 2 save file pairs in your CUSA folder from **YOUR REGION** on discord or Google Drive.  
Example of a save pair: `SAVEDATASGTA50000` & `SAVEDATASGTA50000.bin`  
They are found in:

```text
PS4/SAVEDATA/{account ID}/{CUSAXXXX}/{files}
```

After uploading your files from your region 
