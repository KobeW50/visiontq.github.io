---
title: "Sablinova Bot Starter Guide"
description: "Essential commands for the Sablinova Discord bot, including Honeypot and Starboard."
author: bigbud
date: 2025-08-21
categories: [Discord, Bots]
tags: [Sablinova, Red-DiscordBot, Discord Bots, Guide]
hidden: true
---

> Tip: This guide covers essential commands and setup for Sablinova bot. More unique commands will be added in future updates. {: .prompt-tip}

## Introduction

The Sablinova bot is a great open-source Discord bot based on [the Red-Discord Bot GitHub](https://github.com/Cog-Creators/Red-DiscordBot). In this starter guide, Iâ€™ll explain useful, fun, and unique commands that I havenâ€™t seen in other Discord servers.

---

## Honeypot Command

**What is it?**  
Creates a channel to attract self-bots/scammers and takes action immediately (notify, mute, kick, or ban).

> Info: The honeypot is best used at the top of your server to catch scammers fast.
{: .prompt-info}

### Quick Reference

> Tip: Use this table to quickly see all key Honeypot commands.
{: .prompt-tip}

| Command | Purpose |
|---------|---------|
| `-sethoneypot createchannel` | Creates the honeypot channel |
| `-sethoneypot enabled true` | Enables the cog |
| `-sethoneypot action [none/mute/kick/ban]` | Sets action on detected self-bot/scammer |
| `-sethoneypot muterole {role}` | Assigns the mute role if action is mute |
| `-sethoneypot logschannel {#channel}` | Sets the channel for logs |
| `-sethoneypot showsettings` | Shows all current settings |

### Commands Explained

> Info: Detailed explanation of each Honeypot command.
{: .prompt-info}

- `-sethoneypot` : Set honeypot settings (server owner only)  
- `-sethoneypot action` : Set the action on detection  
- `-sethoneypot bandeletemessagedays` : Days of messages to delete when banning  
- `-sethoneypot createchannel` : Create the honeypot channel  
- `-sethoneypot enabled` : Toggle the cog  
- `-sethoneypot logschannel` : Set logs channel  
- `-sethoneypot modalconfig` : Configure settings via Discord modal  
- `-sethoneypot muterole` : Role for muting scammers  
- `-sethoneypot pingrole` : Role to ping on detection  
- `-sethoneypot resetsetting` : Reset a setting  
- `-sethoneypot showsettings` : Show all current settings  

### Setup Steps

> Tip: Follow these steps to fully configure Honeypot.
{: .prompt-tip}

1. **Create honeypot channel:**
```bash
-sethoneypot createchannel
```

2. **Enable the cog:**
```bash
-sethoneypot enabled true
```

3. **Set the action:**
```bash
-sethoneypot action none   # or mute/kick/ban
```
- Example for mute:
```bash
-sethoneypot action mute
-sethoneypot muterole {role}
```
> Tip: I set the mute role to give an Unverified role so users must re-verify. Make sure another bot removes Verified role accordingly.
{: .prompt-tip}

- Quick alternative: kick for simplicity:
```bash
-sethoneypot action kick
```

4. **Set the logs channel:**
```bash
-sethoneypot logschannel {#channelname}
```

---

## Starboard Command

**What is it?**  
A Starboard highlights messages that get enough reactions. Perfect for funny moments, replies, or anything the server wants to showcase.

> Info: Starboards encourage community engagement by showcasing popular messages.
{: .prompt-info}

### Quick Reference

> Tip: Quick overview of key Starboard commands.
{: .prompt-tip}

| Command | Purpose |
|---------|---------|
| `-starboard create <name> [channel] [emoji=â­]` | Creates a starboard |
| `-starboard threshold highlights <number>` | Sets minimum reactions for posting |
| `-starboard allowlist add <name> <channel>` | Allow specific channels |
| `-starboard blocklist add <name> <channel>` | Block specific channels |
| `-starboard selfstar <name>` | Allow self-starring messages |
| `-starboard autostar <name>` | Bot auto-reacts when starred |
| `-starboard emoji <name> <emoji>` | Changes the starboard emoji |
| `-starboard info` | Show starboard setup |
| `-starboard remove <name>` | Remove starboard |

### Setup Steps

> Tip: Follow these steps to configure your Starboard fully.
{: .prompt-tip}

1. **Create the Starboard:**
```bash
-starboard create <name> [channel] [emoji=â­]
```
Example:
```bash
-starboard create bigbudsb #starboard â­
```

2. **Set posting threshold:**
```bash
-starboard threshold highlights 3
```

3. **Customize behavior:**
- Allow specific channels/roles:
```bash
-starboard allowlist add bigbudsb #general
```
- Block channels/roles:
```bash
-starboard blocklist add bigbudsb #spam
```
- Let users self-star:
```bash
-starboard selfstar bigbudsb
```
- Auto-react when starred:
```bash
-starboard autostar bigbudsb
```

4. **Change emoji (Optional):**
```bash
-starboard emoji bigbudsb ðŸ’Ž
```

5. **View info or remove:**
```bash
-starboard info
-starboard remove bigbudsb
```

> Tip: Auto-react and threshold adjustment help popular messages stand out more.
{: .prompt-tip}

---

> Tip: Save or bookmark this guide. More useful and unique commands will be added in future updates.
{: .prompt-tip}
