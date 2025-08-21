---
title: "Sablinova Bot Starter Guide"
description: "Essential commands for the Sablinova Discord bot, including Honeypot and Starboard."
author: bigbud
date: 2025-08-21
categories: [Discord, Bots]
tags: [Sablinova, Red-DiscordBot, Discord Bots, Guide]
hidden: true
---

> Tip: This guide covers essential commands and setup for Sablinova bot. More unique commands will be added in future updates.
{: .prompt-warning }

## Introduction

The Sablinova bot is a great open-source Discord bot based on [the Red-Discord Bot GitHub](https://github.com/Cog-Creators/Red-DiscordBot). In this starter guide, Iâ€™ll explain useful, fun, and unique commands that I haven't seen in other Discord servers.

---

## Honeypot Command

**What is it?**  
Creates a channel to attract self-bots/scammers and takes action immediately (notify, mute, kick, or ban).

### Setup Steps

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
> Tip: I set the mute role to give an Unverified role so users must re-verify. If you want to do that, make sure another bot removes Verified role accordingly.
{: .prompt-tip}

- Quick alternative: kicking the user is better for simplicity:
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
A Starboard highlights messages that get enough reactions. It's used for funny moments, replies, or anything the server wants to showcase.

### Setup Steps

1. **Create the Starboard:**
```bash
-starboard create <name> [channel] [emoji=⭐]
```
Example:
```bash
-starboard create bigbudsb #starboard ⭐
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
