---
title: "Sablinova Bot Starter Guide"
description: "Learn how to use honeypot and starboard commands with Sablinova bot on Discord"
author: bigbud
date: 2025-08-21
categories: [Discord, Bots]
tags: [sablinova, discord, bot, honeypot, starboard]
---

> This blog is unfinished. More commands are being written, so make sure to bookmark or save this blog for future updates.
{: .prompt-warning }

## Introduction

The **Sablinova bot** is a powerful open-source Discord bot based on [Red-Discord Bot GitHub](https://github.com/Cog-Creators/Red-DiscordBot). In this starter guide, I'll explain some useful, fun, and unique commands that I haven't seen in other Discord bots or servers.

---

## Honeypot Command

> The honeypot command is a defensive tool to catch selfbots and scammers
{: .prompt-tip }

It creates a channel at the top of your server to attract selfbots/scammers and it can **notify, mute, kick, or ban** them immediately.

### How to Set Up

1. **Create the honeypot channel**

```bash
-sethoneypot createchannel
```

2. **Enable the cog**

```bash
-sethoneypot enabled true
```

3. **Set the action**\
   Choose what happens when someone messages in the honeypot channel: none, mute, kick, or ban. If you’re starting out, use `none` or `mute`.

Example for muting:

```bash
-sethoneypot action mute
-sethoneypot muterole {role}
```

> I use this to replace the user's role with `Unverified`, so they must verify again. If you do this, make sure another bot can remove the Verified role automatically.

If you prefer something simpler, you can kick the user instead:

```bash
-sethoneypot action kick
```

4. **Set up logs channel**\
   This is crucial for the bot to work correctly:

```bash
-sethoneypot logschannel {#channelname}
```

> That's it! Your honeypot command is ready to catch selfbots & scammers.

---

## Starboard

### What Is a Starboard?

A **Starboard** is like a community-powered highlight reel. When someone reacts to a message with ⭐ (or any emoji you choose) and it reaches a set threshold, the bot reposts it in a dedicated channel.

It's perfect for:

- Funny moments
- Server lore
- Anything your server wants

### How to Set It Up

#### 1. Create the Starboard

```bash
-starboard create <name> [channel] [emoji=⭐]
```

**Example:**

```bash
-starboard create bigbudsb #starboard ⭐
```

#### 2. Set the Posting Threshold

```bash
-starboard threshold highlights 3
```

> This requires `3` ⭐ reactions to feature the message.

#### 3. Customize Behavior (Optional)

- **Allow specific channels or roles**

```bash
-starboard allowlist add bigbudsb #general
```

- **Block channels or roles**

```bash
-starboard blocklist add bigbudsb #spam
```

- **Let users star their own messages**

```bash
-starboard selfstar bigbudsb
```

- **Auto-add emoji when someone stars a message**

> Note: The `autostar` command increases engagement and helps others react as well, especially if you added this feature recently on your server.

```bash
-starboard autostar bigbudsb
```

#### 4. Change the Emoji
Example:

```bash
-starboard emoji bigbudsb 💀
```

#### 5. View Info or Remove It

- **Check setup**

```bash
-starboard info
```

- **Remove it**

```bash
-starboard remove bigbudsb
```

---

> These are just some of the commands I have found. There are many more, and I'll add more guides for **useful and unique commands** soon, God willing 
{: .prompt-info }

More commands are being written and will be added in future updates.
