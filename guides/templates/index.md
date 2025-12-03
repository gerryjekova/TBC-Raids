---
layout: guide
title: Templates & Copy-Paste Content
section: 5
next_section: guides/macros/
next_title: In-Game Macros
---

# 8. WoW TBC Discord Templates & Copy-Paste Content

## Welcome & Rules Templates

### Welcome Embed (Pin in #welcome)

```markdown
# Welcome to [Your Server Name]! 🌙

We're building the **premier PUG community for TBC Classic EU**. Our goal: **Efficient, fair, and cleared raids without guild commitment.**

---

## 🚀 Getting Started (Required Steps)

1. **Verify** → Go to <#verify> and complete captcha
2. **Pick Roles** → Select your Class and Role in <#roles> (react with emojis)
3. **Read Rules** → Check <#rules> for behavior expectations
4. **Check Loot Rules** → Understand our system in <#rules-loot>
5. **Post Gear** → For "Verified Raider" tag, post logs in <#gear-checks>

---

## 📅 How to Join a Raid

- **Signups**: Check <#raid-signups> for upcoming events
- **React**: Use 🛡️ Tank / ❤️ Healer / ⚔️ DPS to sign up
- **Reserves**: Bot will DM you a SoftRes link - pick your 2 items
- **Requirements**: Voice (Push-to-Talk), consumables, DBM, ilvl check
- **Be On Time**: 10 minutes before start or you lose your spot

---

## 🏆 Our Community

- **Casual PUGs**: No elitism, but we expect effort (flasks, showing up, learning mechanics)
- **Fair Loot**: MS > OS + 2 Soft Reserves (transparent, bot-managed)
- **Experienced Leaders**: Raid Leaders with 100+ clears guiding every run
- **EU Timezone**: Raids typically 19:00-21:00 CET weeknights, 14:00-18:00 weekends

---

## 📖 Quick Links

- **Boss Guides**: <#guides>
- **Find Groups**: <#lfg-karazhan> <#lfg-gruul> <#lfg-heroics>
- **Economy Discussion**: <#market-watch>
- **Class Theory**: <#class-discussion>
- **Support**: <#support> (open a ticket for issues)

---

**TBC Fresh launching soon!** We're forming static dungeon groups for the 60-70 grind. Check <#lfg-attunements> to find your squad!

*Good luck in Outland!* 🔥
```

---

### Rules (Pin in #rules)

```markdown
# Server Rules

## 🛡️ Behavior

**Respect**:
✅ Treat everyone with kindness and respect
✅ Be constructive with feedback
✅ Help new players learn mechanics

**Zero Tolerance**:
❌ No toxicity, harassment, or hate speech
❌ No racism, sexism, homophobia, or discrimination
❌ No doxxing or sharing personal information
❌ No real-money trading (RMT) or gold selling

---

## 🎙️ Voice Requirements

**For Raids**:
✅ Voice **required** (listening is mandatory, talking is encouraged)
✅ Push-to-Talk **highly recommended** (prevents background noise)
✅ Keep calls short and relevant during boss fights
✅ No music, TV, keyboard spam in background

**Violations**: Warning → Mute → Kick from raid

---

## ⏰ Punctuality

- **Be online 10 minutes before raid start**
- **Late without warning = loss of spot** (bench takes your place)
- **If you can't make it**: Cancel signup 2+ hours in advance (click ❌ in signup)
- **No-shows**: 2 strikes = removed from future signup lists

---

## 💎 Loot Policy: MS > OS + 2 Soft Reserves (SR)

**How It Works** (Detailed version in <#rules-loot>):
1. Reserve **2 items** per raid via SoftRes.it link
2. If item reserved → Only reservers roll (1-100)
3. If NO reserve → Main Spec (MS) roll
4. If MS passes → Off Spec (OS) roll
5. Gargul addon handles all rolls (transparent, no ninja)

**BoE Items** (Epic world drops):
- Rolled fairly MS > OS OR sold on AH and gold split
- Decided by raid vote when it drops

**No Hard Reserves** (HR):
- Raid Leaders cannot reserve items
- Everyone has equal chance via SR system

---

## 📜 Reporting Issues

**For Loot Disputes, Toxic Behavior, or Appeals**:
1. Open a ticket in <#support>
2. Provide evidence (screenshots, timestamps)
3. Do **NOT** argue in public channels (wastes time, creates drama)
4. Staff will review and respond within 24 hours

**For Urgent Mid-Raid Issues**:
- Whisper a Moderator or Officer in-game
- Report AFTER raid ends in ticket

---

## 🚫 Consequences

**Strike System**:
1. **Warning**: Friendly reminder to follow rules
2. **Mute/Timeout**: Temporary chat/voice restriction (1-24 hours)
3. **Kick from Raid**: Removed from current raid, can rejoin future raids
4. **Server Ban**: Permanent removal (severe violations only)

**Appeals**: Open ticket in <#support> with your side of the story

---

## 🎯 Our Goal

We're here to **clear content, have fun, and build a reliable community**. No elitism, but we expect effort:
- Show up on time
- Bring consumables
- Learn mechanics
- Be respectful

*If you're willing to put in the effort, you're welcome here!* 🤝
```

---

### Loot Rules (Pin in #rules-loot)

```markdown
# Detailed Loot Policy

## MS > OS + 2 Soft Reserves (SR)

---

## What Are Soft Reserves?

**Soft Reserves (SR)** let you "claim" 2 items per raid. If your reserved item drops, you get priority to roll for it.

**Key Points**:
- **NOT exclusive**: Multiple people can reserve the same item
- **Visible to all**: Check <#softres-kara> to see what others reserved
- **Locked at raid start**: No changes once raid begins

---

## How to Reserve Items

1. **Sign up** for raid in <#raid-signups> (react with 🛡️/❤️/⚔️)
2. **Bot DMs you** a SoftRes.it link
3. **Browse available loot** (filtered by raid: Karazhan, Gruul, etc.)
4. **Select 2 items** (Example: "Dragonspine Trophy" + "Ribbon of Sacrifice")
5. **Confirm** your reserves

**Embed Updates**: Bot posts updated reserves in <#softres-kara>

**Deadline**: 30 minutes before raid start (late reserves may not count)

---

## Loot Distribution Priority

### Scenario 1: Item Reserved
**Example**: Dragonspine Trophy drops, reserved by @Rogue1, @Rogue2, @Warrior1

**Process**:
1. Gargul announces: *"Dragonspine Trophy drops! Reserved by @Rogue1, @Rogue2, @Warrior1. Rolling..."*
2. Only reservers roll (1-100)
3. Highest roll wins
4. Gargul announces winner: *"@Rogue1 wins with 87!"*

**If No Reservers Present** (they left raid or didn't show):
- Opens to Main Spec (MS) among all eligible

---

### Scenario 2: Item NOT Reserved
**Example**: Ring of Eternal Flame drops, nobody reserved it

**Process**:
1. Gargul announces: *"Ring of Eternal Flame drops! No reserves. Main Spec roll..."*
2. All eligible MS players roll (1-100)
3. Highest roll wins

**What is "Eligible"**:
- Ring = Healers and Casters (Mages, Warlocks, Shadow Priests)
- Melee weapon = Melee DPS and Tanks
- Tier token = Classes that can use it

---

### Scenario 3: Main Spec Passes
**Example**: Nobody wants the item for Main Spec

**Process**:
1. Gargul announces: *"No Main Spec rolls. Opening to Off Spec..."*
2. Anyone can roll for Off Spec (OS)
3. Highest roll wins

---

### Scenario 4: Everyone Passes
**Example**: Item is unwanted (low ilvl, bad stats)

**Process**:
- Disenchanted by Enchanter
- Materials go to guild bank (or distributed for raid repairs)

---

## Main Spec (MS) vs Off Spec (OS)

**Main Spec (MS)**:
- The role you **signed up as** (Tank, Healer, DPS)
- Gets priority for gear that improves that role

**Examples**:
- Warrior signed as Tank → Plate tank gear = MS, Plate DPS gear = OS
- Druid signed as Healer → Healing leather = MS, Feral leather = OS
- Paladin signed as Healer → Healing plate = MS, Ret/Prot plate = OS

**Rule of Thumb**: If you'd equip it right now for your signed role = MS. If it's for another spec = OS.

---

## BoE Items (Epic World Drops)

**BoE (Bind on Equip)** items are rare world drops worth 100-1000+ gold on Auction House.

**When BoE Drops**:
1. Raid Leader announces: *"BoE dropped: [Item Name]. Voting: 1 = Roll MS>OS, 2 = Vendor and split, 3 = AH and split later"*
2. Everyone types 1, 2, or 3 in raid chat
3. Majority vote wins

**Option 1: Roll It Out**:
- MS > OS roll among raid
- Winner keeps item (can equip or sell themselves)

**Option 2: Vendor Now**:
- Raid Leader vendors immediately
- Gold split 10 or 25 ways (depending on raid size)
- Everyone gets equal share (~5-50g each)

**Option 3: Auction House Later**:
- Raid Leader posts on AH
- Gold split evenly after it sells
- Risk: Might take days to sell, or not sell at all

**Default**: If no consensus, Raid Leader decides (usually Roll or Vendor)

---

## Special Cases

### Patterns and Recipes
- Profession patterns (e.g., Blacksmithing plans) = Main Spec for that profession
- If multiple people have profession → Roll
- If nobody has profession → Off Spec or guild bank

### Tier Tokens
- Tier tokens (e.g., "Helm of the Fallen Champion") = Main Spec for classes that can use it
- Tokens are NOT tradeable → Roll carefully

### Crafting Materials
- Primal materials (Nether, Fire, etc.) = Roll Off Spec or guild bank
- Exception: If someone reserved a crafted item using those materials → Discuss with raid

---

## Loot Disputes

**If You Disagree with a Roll**:
1. **DO NOT argue in raid chat** (wastes time, creates drama)
2. **Screenshot** the issue (loot window, Gargul announcement, reserves embed)
3. **Open ticket** in <#support> AFTER raid ends
4. Staff reviews with Gargul logs and SoftRes data
5. Decision within 24 hours

**Common Disputes**:
- "I reserved that but didn't get to roll" → Check if you were online and in raid
- "That item is my Main Spec but I didn't win" → Check if someone reserved it (reserves = priority)
- "Gargul gave it to wrong person" → Raid Leader can `/gargul logs` to verify

**Good Faith Policy**: If genuine mistake proven (bot error, wrong assignment), item can be mailed to correct winner if still available.

---

## Why This System?

**Transparency**: All reserves are public, all rolls logged

**Fairness**: Everyone has equal chance via reserves

**Speed**: Gargul automates 95% of loot, <1 minute per item

**No Drama**: Clear rules = fewer arguments

---

## Quick Reference

| Situation | Who Rolls? | Priority |
|-----------|------------|----------|
| Item reserved | Only reservers | Highest roll |
| Item NOT reserved | All MS-eligible | Highest roll |
| MS passes | All OS-eligible | Highest roll |
| Everyone passes | Disenchant/Bank | N/A |
| BoE drops | Vote: Roll/Vendor/AH | Majority vote |

---

**Questions?** Ask in <#general> or open a ticket!
```

---

## Raid Signup Template (Copy-Paste for Raid-Helper)

```markdown
**Event Name**: Karazhan PUG - MS>OS + 2 Soft Reserves

**Date**: Wednesday, December 11, 2025  
**Time**: 20:00 CET  
**Duration**: 3 hours (19:50 meet-up, 20:00 first pull)

---

## Requirements ✅

**Mandatory**:
- **Voice required** (Push-to-Talk recommended)
- **Consumables**: Flask OR Elixirs + Food Buff + Mana/Health Potions
- **Addons**: Deadly Boss Mods (DBM) or BigWigs, Omen Threat Meter
- **Gear**: ilvl ≥ 100 (post `!armory [gear string]` in <#gear-checks> for verification)
- **Punctuality**: Online 10 minutes before start or lose spot

**Recommended**:
- Warcraft Logs profile linked (post in <#warcraftlogs> for "Verified Raider" tag)
- WeakAuras2 for boss mechanics
- Gargul addon (syncs with our SoftRes system)

---

## Loot System 💎

**MS > OS + 2 Soft Reserves**

1. React to this message to sign up (🛡️ Tank / ❤️ Healer / ⚔️ DPS)
2. Bot will DM you a SoftRes link → Pick your 2 reserves
3. Reserves are visible in <#softres-kara>
4. Loot managed by Gargul (transparent, fast, no ninja)

**BoE Items**: Rolled or sold, decided by raid vote

---

## Raid Composition

**Slots**:
- 🛡️ **Tanks**: 0/2 (Prot Warrior/Paladin, Feral Druid)
- ❤️ **Healers**: 0/3 (Holy Paladin, Resto Druid, Resto Shaman/Priest)
- ⚔️ **DPS**: 0/5

**Prioritized DPS**:
- 1 Mage (Polymorph for Moroes)
- 1-2 Hunters (Misdirect, ranged)
- Shadow Priest (Vampiric Embrace for healer mana)
- Flex: Warlocks, Rogues, Enhancement Shaman, Ret Paladin

---

## Instructions 📋

1. **React below** to sign up (slots fill fast!)
2. **Bot DMs you** → Click SoftRes link, pick 2 items, confirm
3. **Post gear** in <#gear-checks>: `!armory [gear string from in-game addon]`
4. **Confirm 24h before**: React ✅ when bot pings (or ❌ to cancel)
5. **Be in Deadwind Pass** by 19:50 CET (summons available)
6. **Join voice**: <#raid-voice-kara> at 19:55 CET

---

## Signup Closes: 15 minutes before raid start

**Late signups**: Only accepted if spots available (bench priority first)

**Cancellations**: Click ❌ if you can't make it (2+ hours notice appreciated)

---

**Boss List**: Attumen → Moroes → Maiden → Opera → Curator → Illhoof → Shade → Netherspite → Chess → Prince → (Nightbane if time allows)

**Estimated Duration**: 2-3 hours for 10/11 bosses

---

*Questions? Ask in <#general> or whisper @RaidLeader!*

*Good luck with reserves!* 🍀
```

---

## How-to-PUG Guide (Pin in #how-to-pug)

```markdown
# How to Join a PUG Raid - Quick Start Guide

New to our server? Here's everything you need to know to join your first raid!

---

## Step 1: Get Verified ✅

1. Go to <#verify>
2. Complete the captcha (click emojis, answer question, etc.)
3. You'll automatically get the **@Verified** role
4. This unlocks all LFG and raid channels

**Why?** Prevents bots and spam accounts.

---

## Step 2: Select Your Roles 🎯

1. Go to <#roles>
2. React to the message with emojis for:
   - **Your Class** (⚔️ Warrior, 🔮 Mage, 🌿 Druid, etc.)
   - **Your Role** (🛡️ Tank, ❤️ Healer, ⚔️ DPS)
   - **Your Faction** (🔴 Horde, 🔵 Alliance)

**Why?** Raid Leaders can ping specific roles when forming groups.

---

## Step 3: Install Required Addons 🔧

**Mandatory for Raids**:

1. **Deadly Boss Mods (DBM)** or **BigWigs**
   - Download: CurseForge or WoWInterface
   - Alerts you to boss mechanics (timers, warnings)
   - Test it: Type `/dbm test` → You should see warnings

2. **Omen Threat Meter** or **KTM**
   - Shows threat (who's about to pull aggro)
   - Essential for tanks and DPS

3. **Recount** or **Details!**
   - Damage/healing meters
   - For performance tracking

**Highly Recommended**:

4. **Gargul** (Loot addon)
   - Syncs with our SoftRes system
   - Download: CurseForge → Search "Gargul"

5. **WeakAuras2**
   - Custom alerts for boss mechanics
   - Import strings from Wago.io

**Where to Download**: CurseForge or WoWInterface (Google "CurseForge WoW Classic addons")

---

## Step 4: Check LFG Channels and Sign Up 📋

### Finding a Raid

**Check these channels**:
- <#raid-signups> - Official scheduled PUGs (bot-managed)
- <#lfg-karazhan> - 10-man Kara groups
- <#lfg-gruul> - 25-man Gruul's Lair
- <#lfg-magtheridon> - 25-man Magtheridon
- <#lfg-heroics> - 5-man heroic dungeons

### Signing Up (Raid-Helper Events)

1. **Find the event** in <#raid-signups>
2. **React** with your role:
   - 🛡️ = Tank
   - ❤️ = Healer
   - ⚔️ = DPS
3. **Bot DMs you** a SoftRes link (more on this below)
4. **Confirmation**: Bot pings you 24h before → React ✅ to confirm or ❌ to cancel

---

## Step 5: Select Soft Reserves 💎

### What Are Soft Reserves?

You can "reserve" **2 items** that might drop in the raid. If your reserved item drops, you get priority to roll for it.

### How to Reserve

1. Click the **SoftRes.it link** the bot DM'd you
2. Browse available loot (filtered by raid)
3. Select **2 items** (Example: "Dragonspine Trophy" + "Ribbon of Sacrifice")
4. Click **Confirm**

**Tips**:
- Check <#guides> for BiS (Best-in-Slot) lists
- See what others reserved in <#softres-kara> (avoid overlaps if possible)
- Reserve smart: Don't reserve garbage items nobody wants

**Deadline**: 30 minutes before raid start

---

## Step 6: Verify Your Gear (First-Time Raiders) 🛡️

Raid Leaders need to see your gear to verify you meet requirements.

### How to Post Gear

1. **Install addon** "DejaCharacterStats" or similar (search "gear export addon")
2. **In-game**, type: `/dcstats export` (or addon-specific command)
3. **Copy the string** (long text with your gear data)
4. **Post in** <#gear-checks>: `!armory [paste string here]`
5. **Bot embeds** your Armory card (shows ilvl, enchants, gems)

**Guilds of WoW bot** (if installed) will flag issues:
> "⚠️ @YourName - ilvl 95 (req: 100). Missing chest enchant. 2 empty gem sockets."

**Fix issues** before raid start!

---

## Step 7: Prepare Consumables 🧪

**Mandatory for Every Raid**:

- **Flask** (2 hours, persists through death):
  - Tanks: Flask of Fortification (500 HP, 10 Defense Rating)
  - Healers: Flask of Mighty Restoration (25 MP5)
  - Casters: Flask of Pure Death (+80 Spell Damage)
  - Melee: Flask of Relentless Assault (+120 Attack Power)

**OR** (if no flask):
- **Elixirs** (1 hour, cheaper but lost on death):
  - Battle Elixir (DPS/Tank stats)
  - Guardian Elixir (Survivability)

**Also Bring**:
- **Food Buff**: Stamina/Spirit/Spell Damage food (lasts 30 min)
- **Mana Potions**: Super Mana Potions (x10+)
- **Health Potions**: Super Healing Potions (x5+)
- **Repair**: 100% durability before starting

**Where to Buy**: Auction House, or check <#market-watch> for cheapest prices

---

## Step 8: Join Voice and Meet Up 🎙️

### 10 Minutes Before Raid

1. **Be online** in-game (in Outland, preferably near the raid)
2. **Join Discord voice**: <#raid-voice-kara> (or whichever is assigned)
3. **Set Push-to-Talk** (highly recommended): Discord Settings → Voice & Video → Input Mode → Push to Talk → Set keybind

### Meeting Point

- **Karazhan**: Deadwind Pass (summons provided)
- **Gruul's Lair**: Blade's Edge Mountains (Gruul's Lair entrance)
- **Magtheridon**: Hellfire Peninsula (Magtheridon's Lair entrance)

**Summons**: Warlocks will summon. Type "sum" in raid chat if you need a summon.

---

## Step 9: Pre-Raid Checklist (Raid Leader Confirms) ✅

Before first pull, Raid Leader will do a **consumables check**:

**Type in raid chat when ready**:
- "flasked" (or "elixirs" if using elixirs)
- "fed" (food buff active)
- "repaired" (100% durability)
- "dbm" (addon installed and working)

**If you're missing anything**: "You have 5 minutes to get consumables or we pull from bench"

---

## Step 10: During Raid - Listen and Follow Instructions 👂

### Voice Etiquette

✅ **DO**:
- Listen to Raid Leader's strategy explanations
- Call out if you need help ("Need heal", "Out of mana")
- Keep calls SHORT (<5 words)
- Ask questions if confused (before pull, not during)

❌ **DON'T**:
- Talk over Raid Leader during explanations
- Open mic with background noise (music, TV, keyboard)
- Argue about strategy mid-fight
- Complain about loot in voice (use tickets after raid)

### Loot

- **Gargul automatically handles all loot** (announces drops, rolls, winners)
- **Don't spam "Need" or "Greed"** - Gargul rolls for you
- **If issue**: Screenshot and open ticket in <#support> AFTER raid (don't argue during)

---

## Step 11: Post-Raid - Logs and Feedback 📊

### Warcraft Logs

- Raid Leader uploads logs to Warcraft Logs after raid
- Auto-posted in <#warcraftlogs> via webhook
- Check your performance (DPS, HPS, mechanics)

### Feedback

- Rate the raid in <#raid-feedback> (optional)
- DM Raid Leader if you have suggestions

### Next Raid

- Recurring events auto-post every week
- Sign up early for guaranteed spot!

---

## Common Questions ❓

**Q: What if I'm late?**  
A: Bench player takes your spot. You can ask to join if someone leaves, but no guarantee.

**Q: Can I reserve the same item as someone else?**  
A: Yes! Multiple people can reserve the same item. Highest roll wins.

**Q: What if I disconnect mid-raid?**  
A: Reconnect within 60 seconds or we continue without you. No loot for bosses you miss.

**Q: Do I need to be in a guild?**  
A: No! We're a PUG community, not a guild. No guild requirements.

**Q: What's the difference between MS and OS?**  
A: Main Spec (MS) = gear for your signed role. Off Spec (OS) = gear for other roles. MS gets priority.

**Q: Can I bring my alt?**  
A: Only if alt meets gear/attunement requirements. Post `!armory` in <#gear-checks> first.

---

## Tips for Success 🏆

- **Show up on time** (10 min early)
- **Come prepared** (flasks, consumables, repaired)
- **Know mechanics** (watch videos in <#guides> before raid)
- **Be respectful** (no raging, no blaming)
- **Ask questions** (we help new raiders!)

**Good luck, and welcome to the team!** 🎉
```

---

## Quick LFG Post Templates

### Karazhan LFG Post

```
**LFM Karazhan - MS>OS + Soft Res**

**Time**: Tonight 20:00 CET (1 hour from now)  
**Req**: ilvl 100+, flasks, DBM, voice  
**Loot**: 2 SR via SoftRes.it

**Need**:
- 1 Tank (Prot Warrior/Paladin/Feral)
- 1 Healer (any spec)
- 2 DPS (prefer Mage + Hunter)

**React or DM @RaidLeader to join!**

Reserves posted after group full. Fast run, experienced RL.
```

---

### Heroic Dungeon LFG Post

```
**LFM Heroic Shadow Labyrinth**

**Time**: Now  
**Req**: Revered Consortium, key, flasks optional

**Need**:
- 1 Tank
- 1 Healer
- 1 DPS (prefer Mage for CC)

React or DM! Quick run for badges.
```

---

### Gruul/Mag LFG Post

```
**LFM Gruul's Lair + Mag (25-man) - MS>OS + SR**

**Time**: Sunday 14:00 CET  
**Req**: ilvl 105+, TBC raid experience, flasks, logs preferred

**Need**:
- 1 Tank (Prot Warrior for Maulgar)
- 3 Healers (prefer Holy Paladin + Resto Shaman)
- 8 DPS (NEED Shamans for each group - high priority)

**Special Needs**:
- 5 Shamans total (1 per group for Bloodlust)
- Shadow Priest (Vampiric Embrace for healers)
- Mages/Warlocks for High King adds

**Signup**: Check <#raid-signups> for Raid-Helper event

Both raids back-to-back (~3-4 hours total). Experienced RL, clean strats.
```

---

## Consumables Checklist (Post in #guides)

```markdown
# TBC Raid Consumables Checklist

**Copy this before every raid to verify you have everything!**

---

## 🔴 MANDATORY (Must Have)

### Flasks (Pick ONE)
- [ ] **Flask of Fortification** (Tanks: +500 HP, +10 Def Rating, 2hr)
- [ ] **Flask of Mighty Restoration** (Healers: +25 MP5, 2hr)
- [ ] **Flask of Pure Death** (Casters: +80 Spell Damage, 2hr)
- [ ] **Flask of Relentless Assault** (Melee/Hunters: +120 AP, 2hr)

**OR** (If no flask):

### Elixirs (Pick TWO - 1 Battle + 1 Guardian)
**Battle Elixirs**:
- [ ] Elixir of Major Agility (+35 Agility, Melee/Hunters)
- [ ] Elixir of Major Strength (+35 Strength, Warriors/Paladins)
- [ ] Elixir of Major Firepower (+55 Fire Damage, Mages/Warlocks)
- [ ] Elixir of Major Shadow Power (+55 Shadow Damage, Warlocks/Shadow Priests)

**Guardian Elixirs**:
- [ ] Elixir of Major Fortitude (+250 HP, Everyone)
- [ ] Elixir of Draenic Wisdom (+30 Int, +30 Spirit, Casters/Healers)
- [ ] Elixir of Major Defense (+550 Armor, Tanks)

---

### Food Buff (Pick ONE)
- [ ] **Blackened Basilisk** (+23 Spell Damage, +20 Spirit, Casters)
- [ ] **Grilled Mudfish** (+20 Agility, +20 Spirit, Melee/Hunters)
- [ ] **Fisherman's Feast** (+30 Stam, +20 Spirit, Tanks)
- [ ] **Skullfish Soup** (+20 Spirit, +23 Healing, Healers)

---

### Potions (Bring Multiple)
- [ ] **Super Mana Potion** x10+ (Casters/Healers)
- [ ] **Super Healing Potion** x5+ (Everyone, especially Tanks)
- [ ] **Haste Potion** x2 (Melee/Hunters for burst)
- [ ] **Destruction Potion** x2 (Casters for burst)

---

## 🟡 HIGHLY RECOMMENDED

### Scrolls
- [ ] **Scroll of Agility V** (+20 Agility, Melee/Hunters)
- [ ] **Scroll of Strength V** (+20 Strength, Warriors/Paladins)
- [ ] **Scroll of Intellect V** (+20 Int, Casters/Healers)
- [ ] **Scroll of Spirit V** (+20 Spirit, Healers)

### Oils/Sharpening Stones
- [ ] **Brilliant Wizard Oil** (+36 Spell Damage, +14 Crit, Casters - 1hr)
- [ ] **Adamantite Weightstone** (+12 Weapon Damage, +14 Crit, Melee - 1hr)
- [ ] **Adamantite Sharpening Stone** (+12 Weapon Damage, +14 Crit, Melee - 1hr)

---

## 🟢 BONUS (Min-Maxing)

### Resist Gear (Boss-Specific)
- [ ] **Shadow Resistance** (Magtheridon, minimum: Shadow Resist cloak)
- [ ] **Fire Resistance** (Future: Tempest Keep, Hyjal)
- [ ] **Nature Resistance** (Future: Serpentshrine Cavern)

### Special Items
- [ ] **Drums of Battle** (Leatherworkers: +80 Haste for group, 2min CD)
- [ ] **Drums of War** (Leatherworkers: +60 AP for group, 2min CD)

---

## 💰 Estimated Cost Per Raid

**Full Flask Setup**: ~50-100g per raid (Flask + Food + Potions)  
**Elixir Setup**: ~20-40g per raid (Elixirs + Food + Potions + Scrolls)

**Where to Buy**: Auction House, or check <#market-watch> for deals

---

## Repair & Bags

- [ ] **100% Repair** (Check durability before raid)
- [ ] **Empty Bag Space** (At least 10 slots for loot)

---

**Pro Tip**: Keep a "Raid Bank Alt" with consumables. Mail yourself a full stack of everything before raid night!
```

---

## Boss Strategy Quick Reference (Pin in #guides)

```markdown
# Karazhan Boss Strategy Quick Reference

**Full Video Guides**: FatBoss Gaming (YouTube)

---

## 1. Attumen the Huntsman

**Key Mechanics**:
- **Intangible Presence**: Reduces damage, Ranged spread 10 yards
- **Charge**: Charges random player, MOVE AWAY from target

**Strategy**:
- Tank Attumen in corner, face away from raid
- Midnight + Attumen merge at 95% Attumen health
- Stack behind boss for Melee cleave, Ranged spread

**Loot Highlights**: Worgen Claw Necklace, Steelhawk Crossbow

---

## 2. Moroes

**Key Mechanics**:
- **Garrote**: DoT, DISPEL IMMEDIATELY (Paladin/Priest priority)
- **Gouge**: Stuns tank, can't prevent
- **Blind**: Stuns random player, don't break it
- **Adds**: 4 adds, CC 2, kill other 2

**Strategy**:
- Tank Moroes center, face away
- CC: Mage Sheep LEFT (Moon), Hunter Trap RIGHT (Square)
- Kill order: LEFT add (Moon) → RIGHT add (Square) → Moroes
- Interrupt rotation on add heals: Rogue → Warrior → Hunter

**Loot Highlights**: Moroes' Lucky Pocket Watch (BiS trinket)

---

## 3. Maiden of Virtue

**Key Mechanics**:
- **Holy Fire**: DoT, DISPEL ASAP (Priest/Paladin)
- **Holy Wrath**: AOE damage, Spread 10 yards
- **Repentance**: AoE stun, STOP CASTING during

**Strategy**:
- Tank center, raid spread in semi-circle
- Healers spam dispel Holy Fire
- When she casts Repentance, STOP everything (casting/moving)

**Loot Highlights**: Bands of Indwelling, Shard of the Virtuous

---

## 4. Opera Event (Random: Wizard of Oz, Big Bad Wolf, or Romulo & Julianne)

**Wizard of Oz**:
- Kill order: Dorothee → Roar → Strawman → Tinhead → Tito → Crone
- Cyclone: Lifts random player, can't prevent

**Big Bad Wolf**:
- Little Red Riding Hood debuff: RUN AWAY FROM RAID (or Wolf one-shots you)
- Kill adds, burn boss

**Romulo & Julianne**:
- Kill both at same time (sync HP within 10%)
- Resurrection: If one dies first, they resurrect after 1 minute
- Burn both to 10%, then finish together

---

## 5. The Curator

**Key Mechanics**:
- **Evocation**: Channels, HUGE AOE damage, spread 15 yards
- **Astral Flare Adds**: Spawn every 10 seconds, explode on death (AOE damage)

**Strategy**:
- Ranged spread 15 yards (Evocation)
- Mage/Warlock priority DPS on Flare adds
- Casters: Evocate (mana regen spell) during boss Evocation

**Loot Highlights**: Wrynn Dynasty Greaves, Dragon-Quake Shoulderguards

**Bloodlust**: 20% boss health

---

## 6. Shade of Aran

**Key Mechanics**:
- **Flame Wreath**: RED CIRCLES, DO NOT MOVE (instant wipe if broken)
- **Blizzard**: Moves around room, stack CENTER (safe zone)
- **Arcane Explosion**: Point-blank AOE, RUN OUT 15 yards
- **Drinking Phase**: Sits and drinks at 40%, interrupt with any damage

**Strategy**:
- Tank nowhere (no tank, just DPS and dodge)
- Flame Wreath: When cast, FREEZE (wait for "Flame Wreath down" call)
- Blizzard: Stack on Aran (center safe)
- Arcane Explosion: Run out immediately
- Drinking Phase: Rogue Kick or any interrupt → Stop drinking

**Loot Highlights**: Shermanar Great-Ring, Dragonheart Flameshield

---

## 7. Terestian Illhoof

**Key Mechanics**:
- **Demon Chains**: Immobilizes player, BREAK CHAINS IMMEDIATELY
- **Kil'rek**: Demon add, Off-Tank away from raid
- **Imps**: Spawn constantly, AOE them down

**Strategy**:
- MT: Illhoof (boss)
- OT: Kil'rek (demon add, tank in corner)
- DPS: Kill Demon Chains → AOE imps → Boss
- Mage: Blizzard imps
- Warlock: Seed of Corruption imps

**Loot Highlights**: Malefic Girdle, Cord of Nature's Sustenance

---

## 8. Netherspite

**Key Mechanics**:
- **Beams**: Red (Tank), Blue (Mana), Green (Healing)
- **Beam Rotation**: Players soak beams, switch every 30 seconds
- **Void Zones**: Don't stand in them (damage + slow)

**Strategy**:
- **Red Beam**: Tank → Increases damage taken, rotate tanks
- **Blue Beam**: Caster/Healer → Mana regen, rotate
- **Green Beam**: Healer → Healing boost, rotate
- Beam phases: 60sec (beams) → 30sec (no beams, burn boss) → 60sec (beams) repeat

**Rotation Example**:
- Phase 1 (Beams): Tank1 Red, Priest1 Blue, Paladin1 Green
- Phase 2 (No Beams): Full DPS
- Phase 3 (Beams): Tank2 Red, Priest2 Blue, Paladin2 Green

**Loot Highlights**: Skulker's Greaves, Mantle of Abrahmis

---

## 9. Chess Event

**Mechanics**: Control chess pieces, defeat King

**Strategy**:
- Raid Leader assigns pieces (usually: Tank = King, DPS = Queens/Rooks)
- Move pieces strategically
- DPS King pieces when called
- Easy boss, but pay attention to RL

**Loot**: Guaranteed 2 epics (no boss fight required)

---

## 10. Prince Malchezaar

**Key Mechanics**:
- **Enfeeble**: Reduces max HP to 1, Healers top everyone after
- **Infernals**: Phase 3, adds spawn, KITE them (don't tank)
- **Axes**: Spinning axes on ground, dodge or minimize

**Strategy**:
- Phase 1-2: Tank center, raid spread 10 yards (Enfeeble)
- Phase 3: Off-Tank kites Infernals in circle
- Axes: Visual tells (spinning), move slightly to minimize hits

**Loot Highlights**: Helm of the Fallen Champion (Tier 4 token)

---

## 11. Nightbane (Optional - Requires Blackened Urn Quest)

**Key Mechanics**:
- **Air Phase**: Skeletons spawn, kill them (boss immune in air)
- **Ground Phase**: Charred Earth (fire on ground), spread
- **Fear**: Random AoE fear, Fear Ward or trinket

**Strategy**:
- Air Phase: All DPS skeletons (boss lands at 75%, 50%, 25%)
- Ground Phase: Spread for Charred Earth, don't overlap fire
- Fear Ward on tank (Dwarf Priest only)

**Loot Highlights**: Robe of the Elder Scribes, Ferocious Swift-Kickers

---

**Full Guides**: YouTube → FatBoss Gaming → Karazhan Boss Guides
```

# Welcome to [Your Server Name]! 🌙

We're building the **premier PUG community for TBC Classic EU**. Our goal: **Efficient, fair, and cleared raids without guild commitment.**

---

## 🚀 Getting Started (Required Steps)

1. **Verify** → Go to <#verify> and complete captcha
2. **Pick Roles** → Select your Class and Role in <#roles> (react with emojis)
3. **Read Rules** → Check <#rules> for behavior expectations
4. **Check Loot Rules** → Understand our system in <#rules-loot>
5. **Post Gear** → For "Verified Raider" tag, post logs in <#gear-checks>

---

## 📅 How to Join a Raid

- **Signups**: Check <#raid-signups> for upcoming events
- **React**: Use 🛡️ Tank / ❤️ Healer / ⚔️ DPS to sign up
- **Reserves**: Bot will DM you a SoftRes link - pick your 2 items
- **Requirements**: Voice (Push-to-Talk), consumables, DBM, ilvl check
- **Be On Time**: 10 minutes before start or you lose your spot

---

## 🏆 Our Community

- **Casual PUGs**: No elitism, but we expect effort (flasks, showing up, learning mechanics)
- **Fair Loot**: MS > OS + 2 Soft Reserves (transparent, bot-managed)
- **Experienced Leaders**: Raid Leaders with 100+ clears guiding every run
- **EU Timezone**: Raids typically 19:00-21:00 CET weeknights, 14:00-18:00 weekends

---

## 📖 Quick Links

- **Boss Guides**: <#guides>
- **Find Groups**: <#lfg-karazhan> <#lfg-gruul> <#lfg-heroics>
- **Economy Discussion**: <#market-watch>
- **Class Theory**: <#class-discussion>
- **Support**: <#support> (open a ticket for issues)

---

**TBC Fresh launching soon!** We're forming static dungeon groups for the 60-70 grind. Check <#lfg-attunements> to find your squad!

*Good luck in Outland!* 🔥