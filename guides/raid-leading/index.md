---
layout: guide
title: Raid Leading Strategies
section: 4
next_section: /guides/templates/
next_title: Templates & Content
---

# 7. # WoW TBC Raid Leading Strategies

## The Assignment → Action → Event Method

### Core Principle: Clear, Concise, Actionable Callouts

**Format**: `[Who] → [What] → [Why/When]`

**Examples**:

- ✅ "Shammybaby - Bloodlust - NOW"
- ✅ "Everyone - Move out - Flame Wreath"
- ✅ "Healers - Dispel - Holy Fire on tanks"
- ❌ "Okay so we're gonna need the shaman to use bloodlust when the boss is low maybe around 20% or so"

**Why This Works**:

- **3-7 words max** - Fast to process under pressure
- **Name first** - Gets attention immediately
- **Action** - Clear instruction
- **Context** - Urgency or timing

---

## Pre-Raid Preparation

### 🔴 CRITICAL: Before First Pull

#### 1. Consumables Verification (5 minutes)

**Raid Leader (Voice)**:

> "Consumables check! Type in raid chat when done:
> 
> 1. Flask - type 'flasked'
> 2. Food buff - type 'fed'
> 3. Elixirs (if no flask) - type 'elixirs'
> 4. Repair 100% - type 'repaired'
> 5. DBM/BigWigs installed - type 'dbm'"

**Why**: Prevents mid-raid wipes due to missing buffs/repairs

**Follow-up**:

- If someone missing: "You have 5 minutes or we pull from bench"
- Post consumables list in #guides if recurring issue

---

#### 2. Addon Verification

**Required Addons (Post in #guides)**:

```
**REQUIRED ADDONS FOR RAIDS:**

🔴 MANDATORY:
1. Deadly Boss Mods (DBM) - Boss alerts and timers
   - Download: CurseForge / WoWInterface
   - Test: Type /dbm - you should see a menu

2. Omen Threat Meter (or KTM) - Threat tracking
   - Essential for tanks and DPS
   - Shows who's about to pull aggro

3. Recount or Details! - Damage/healing meters
   - For performance tracking
   - Don't flame others based on DPS alone

🟡 HIGHLY RECOMMENDED:
4. Grid or Healbot - Healing raid frames
   - For healers only
   - Faster dispels and target selection

5. WeakAuras2 - Custom alerts
   - Boss-specific warnings
   - Import strings from Wago.io

6. Gargul - Loot management
   - Syncs with our SoftRes system
   - Required for transparent loot

**How to Verify DBM is Working:**
- /dbm test → You should see warnings and hear sounds
- If broken, reinstall from CurseForge
```

**In-Raid Check** (Before first boss):

> "DBM check - everyone type /dbm test. If you don't see warnings on your screen, fix it NOW or you sit out."

---

#### 3. Role-Specific Assignments

**Tanks**:

```
**TANK ASSIGNMENTS - Karazhan Tonight**

@WarriorMain (Main Tank):
- Attumen/Midnight
- Moroes (boss)
- Maiden
- Curator
- Shade of Aran
- Illhoof (boss)
- Prince Malchezaar
- Nightbane (if we do)

@DruidOT (Off-Tank):
- Moroes adds (CC'd, pick up if break)
- Opera (flexibility)
- Illhoof (Kil'rek demon)
- Netherspite (beam rotation)
- Chess (DPS, no tanking)
- Prince adds (Infernals)

**Communication:**
- Taunt rotations: Call in #off-tank-1 voice
- Threat issues: "Threat high on [target]"
- Emergency: "Need taunt on [name]"
```

**Healers**:

```
**HEALER ASSIGNMENTS - Karazhan Tonight**

@PaladinHeal (Tank Healer):
- Main Tank priority (100% uptime)
- Beacon on MT if Prot Paladin
- Dispel Moroes Garrote (priority #1)

@DruidHeal (Raid Healer):
- HoT rotation on raid (Rejuv, Regrowth)
- Wild Growth on stack fights (Shade, Chess)
- Dispel poisons/curses

@ShamanHeal (Flex):
- Chain Heal on grouped players
- Mana Tide Totem on CD (in Healer group)
- Dispel Magic on Maiden Holy Fire

**Cooldown Rotation:**
- Mana consumables: Use at 50% mana
- Innervate: @DruidHeal cast on healer with lowest mana
- Mana Tide: @ShamanHeal every 5 minutes (announce)

**Emergency Protocol:**
- If healer dies: "Healer down, [Name] cover [role]"
- If OOM mid-fight: "OOM, need Innervate or Mana pot"
```

**DPS**:

```
**DPS ASSIGNMENTS - Karazhan Tonight**

@Mage1 - Crowd Control (CC):
- Moroes: Polymorph LEFT add (mark: Moon)
- Opera (Big Bad Wolf): Sheep adds
- Illhoof: AOE imps (Blizzard)
- Interrupt priority: Shade of Aran (Frostbolt)

@Hunter1 - CC + Utility:
- Moroes: Trap RIGHT add (mark: Square)
- Misdirect on MT every pull (announce: "MD ready")
- Tranq Shot: N/A (no enrage in Kara)

@Rogue1 - Interrupts:
- Moroes: Kick rotation #1 (heals)
- Shade: Kick rotation #1 (Frostbolt during drinking)
- Illhoof: Kick rotation #1 (demon casts)

@Warlock1 - AOE + Utility:
- Illhoof: Seed of Corruption on imps
- Soulstone: @PaladinHeal (pre-cast before boss)
- Healthstone: Everyone get one before raid starts

@ShadowPriest - Mana Battery:
- Vampiric Embrace on CD (healer mana)
- Shadow Word: Pain on all targets (multi-dot fights)
- Dispel Magic (backup to healers)

**DPS Priority Targets:**
- Marked targets: Skull → X → Moon → Circle
- If unmarked: Follow tank's target
- Don't switch unless called
```

---

## During Raid: Voice Communication Best Practices

### 🔴 Voice Channel Discipline

#### Main Raid Voice Rules:

```
**VOICE ETIQUETTE - READ BEFORE JOINING**

✅ DO:
- Use Push-to-Talk (PTT) [highly recommended]
- Keep calls SHORT (<5 words)
- Call out personal issues: "Need heal", "Out of mana"
- Acknowledge assignments: "Got it"

❌ DON'T:
- Open mic with background noise (music, TV, keyboard)
- Talk during boss explanations
- Argue loot during raid (use tickets after)
- Backseat raid lead ("you should have...")
- Spam memes/jokes during pulls

**Mute Status:**
- Trash: Open chat allowed
- Boss Explanations: Listen, questions after
- Boss Pulls: Essential callouts only
- After Wipes: Constructive feedback, no blame

**Violation = Warning → Mute → Kick**
```

---

### Voice Callout Templates

#### **Boss Pull Countdown**

```
Raid Leader: "Pull in 5... 4... 3... 2... 1... PULL"
[Exact timing lets DPS pre-cast]
```

#### **Mechanic Warnings (Shade of Aran)**

```
"Flame Wreath - FREEZE"
[Wait 3 seconds]
"Wreath down - move now"

"Blizzard - STACK CENTER"
"Blizzard moving - spread"

"Arcane Explosion - OUT OUT OUT"
```

#### **Interrupt Rotations**

```
"Kick rotation: Rogue - Warrior - Hunter"
[Before pull]

During fight:
"Rogue kick 1"
[After first heal]
"Warrior kick 2"
[After second heal]
"Hunter kick 3"
```

#### **Threat Management**

```
"Threat high on [DPS name] - slow DPS"
"[DPS name] - stop or pull aggro"
"Tanks swap - Taunt on 3... 2... 1... NOW"
```

#### **Healer Emergencies**

```
"Healer down - [Name2] cover tanks"
"All healers OOM - Burn cooldowns, 30 seconds"
"Lust now - push to 20%"
```

#### **Wipe Calls**

```
"Wipe it - stop DPS, let tanks die"
[If clearly unrecoverable]

"Don't release - I'll explain strat"
[After wipe, before releasing]
```

---

## Post-Pull Analysis (The 2-3 Improvement Rule)

### 🔴 CRITICAL: Never Overload Feedback

**Bad Example** (After Wipe):

> "Okay so the tank didn't position right, the DPS were too aggressive, healers were late on dispels, interrupts were missed, people stood in fire, the CC broke early, and we didn't use Bloodlust at the right time."

**Good Example** (After Wipe):

> "Three things to fix:
> 
> 1. Dispels faster on Holy Fire - Paladins, that's your only job
> 2. DPS slow down first 10 seconds - let tank build threat
> 3. I'll call Bloodlust at 25% - ignore boss health until then  
>     Questions on those three? No? Pull in 30 seconds."

**Why**: Human brains can only process 2-3 instructions under stress. More = information overload.

---

### The "Solution-Focused" Wipe Review

#### Step 1: Identify Problem (No Blame)

❌ "Mage, you screwed up Flame Wreath"  
✅ "Flame Wreath broke - let's fix it"

#### Step 2: Ask for Input

> "What happened with Flame Wreath? Anyone see?" [Let player explain - often they know what they did wrong]

#### Step 3: Provide Solution

> "Okay, so the fix: Stop all movement 2 seconds before Wreath. I'll call it earlier. Everyone freeze until I say 'move'. Got it?"

#### Step 4: Move On Quickly

> "Good. Pull in 30 seconds."

**No Dwelling**: Don't spend 5 minutes analyzing one wipe. Fix and retry.

---

## Strategy Presentation (Before Boss Pulls)

### Template for Boss Explanation (30-60 Seconds Max)

**Format**: `Role Assignments → Key Mechanics → Kill Order → Questions`

**Example: Moroes**

```
[VOICE]
"Okay, Moroes strategy - listen up:

ASSIGNMENTS:
- Warrior: Tank Moroes, face away from raid
- Mage: Sheep LEFT add, Moon marker
- Hunter: Trap RIGHT add, Square marker
- Rogues: Interrupt rotation on heals - I'll call order

MECHANICS:
- Garrote: Ticking bleed, healers dispel ASAP
- Gouge: Random stun, can't prevent
- Blind: Don't break CC, re-sheep after

KILL ORDER:
1. Kill LEFT sheeped add (Moon)
2. Kill RIGHT trapped add (Square)  
3. Burn Moroes to zero

Bloodlust at 30% boss health.

QUESTIONS? ... Good. Pull in 60 seconds."
```

**Post in Text** (While Talking):

```
#raid-signups or boss thread:

**Moroes Quick Strat:**
- CC: Sheep LEFT (Moon), Trap RIGHT (Square)
- Kill order: Moon → Square → Boss
- Interrupt heals: Rogue1 → Warrior → Hunter
- Dispel Garrote immediately
- Lust at 30%
```

**Why Dual Format**: Voice for urgency, text for reference (someone AFK, or forgot mid-fight).

---

## Handling Different Personalities in PUGs

### The "Quiet Player" (Shy/New)

**Problem**: Doesn't speak, might not understand mechanics

**Solution**:

- Whisper after explanation: "Hey, first time Kara? Let me know if you have questions"
- Assign simple job: "Just DPS boss, ignore everything else"
- Praise publicly when they do well: "Nice DPS [Name], solid job"

---

### The "Overconfident Player" (Know-it-all)

**Problem**: "I've done this 100 times, just pull"

**Solution**:

- Acknowledge experience: "Great, then you know the drill"
- Set boundary: "Still gonna explain for new folks - bear with me"
- If backseat leading: "Appreciate input, but I'm calling shots tonight. DM me after if you have ideas"

---

### The "Argumentative Player" (Challenges Every Decision)

**Problem**: "Why are we doing it this way? We should..."

**Solution**:

- First time: "Valid point, but we're sticking with this strat tonight"
- Second time: "Not gonna debate mid-raid - we'll discuss after"
- Third time: "You're muted for pulls. Focus on your role"

---

### The "Silent Underperformer" (Low DPS, Mistakes)

**Problem**: Doing 40% of expected DPS, dies to avoidable mechanics

**Solution**:

- **Don't call out publicly** (humiliating)
- Whisper after pull: "Hey, noticed your DPS is low - rotation okay? Need WeakAuras?"
- Offer help: "I can link some guides in #class-discussion after raid"
- If continues and causing wipes: "We might need to swap you out this run - let's work on gear/rotation for next time"

---

## Raid Composition Management (TBC-Specific)

### The "Shaman Game" (TBC's Unique Challenge)

**Core Rule**: 1 Shaman per 5 players (for Bloodlust/Heroism)

#### 25-Man Group Structure

**Group 1 - Melee DPS**:

- Enhancement Shaman (Windfury Totem)
- Warriors (2)
- Rogues (2) Priority: Physical DPS

**Group 2 - Caster DPS**:

- Elemental Shaman (Totem of Wrath)
- Mages (2)
- Warlocks (2) Priority: Spell DPS

**Group 3 - Ranged Physical**:

- Enhancement OR Elemental Shaman
- Hunters (3)
- Shadow Priest (Vampiric Touch) Priority: Sustained DPS

**Group 4 - Hybrid Support**:

- Resto Shaman OR Enhance (flex)
- Balance Druid (Moonkin Aura)
- Ret Paladin (buffs)
- Flex DPS

**Group 5 - Healer Mana Battery**:

- Resto Shaman (Mana Tide Totem)
- Shadow Priest (Vampiric Embrace)
- Holy Paladins (2)
- Resto Druid Priority: Healer sustainability

---

### Critical Buffs to Track

**Pre-Pull Buff Check** (Macro for Raid Leader):

```
/rw === BUFF CHECK ===
/rw Mark of the Wild - Druid
/rw Power Word: Fortitude - Priest  
/rw Arcane Intellect - Mage
/rw Blessing of Kings - Paladin (if Ret)
/rw Blessing of Might - Paladin (melee groups)
/rw Blessing of Wisdom - Paladin (healer/caster groups)
/rw Shadow Protection - Priest (if applicable)

/rw Flasks on ALL players
/rw Food buffs on ALL players
```

**Missing Buff Protocol**:

- Buff bots: Assign one person per buff to check
- @mention class if missing: "@Druid - Mark of the Wild missing"
- Don't pull until all major buffs present

---

## Loot Management (Minimizing Drama)

### 🔴 Pre-Raid Loot Announcement

**Every Raid, Before First Pull** (Voice):

> "Quick loot reminder:
> 
> - MS > OS + 2 Soft Reserves
> - Your reserves are in #softres-kara - check now if unsure
> - Gargul handles all rolls automatically
> - If you have issues, open ticket AFTER raid, not during
> - BoE items: We'll roll or sell AH and split - I'll call it when it drops  
>     Questions? ... Good, let's go"

---

### During Raid: Loot Best Practices

#### When Gargul Announces Winner

**Raid Leader** (Voice):

> "Congrats [Winner], [Item Name]"

**Why**: Public acknowledgment → transparency → trust

#### If Dispute Occurs

**Immediate Response**:

1. Pause looting
2. Ask in voice: "What's the issue?"
3. Check SoftRes embed (screenshot proof)
4. Check Gargul logs: `/gargul logs`

**If Error Proven**:

> "My bad, reassigning to [CorrectWinner]. Gargul had a hiccup."

**If Player Lying**:

> "Checked logs - you didn't reserve this. It's correct. Next boss."

**If Still Arguing**:

> "Not debating mid-raid. Open ticket after, we'll review with screenshots. Moving on."

---

### BoE Item Protocol

**When BoE Drops** (e.g., Krol Blade world drop):

```
[VOICE]
"BoE dropped: [Item Name]. Here's the deal:
- Option 1: Roll MS > OS among us (winner keeps or sells)
- Option 2: I vendor it now, gold split 25 ways (1g each)
- Option 3: Post AH, gold split later (risky, might not sell)

Voting now: React in chat
1 = Roll it out
2 = Vendor now
3 = AH and split

Most votes wins. 30 seconds."
```

**Why Democratic**: Prevents accusations of favoritism

---

## Dealing with Wipes (The "3 Strikes" Rule)

### Attempt 1: Learn Mechanics

**After Wipe**:

> "Okay, that's what the fight looks like. Now we know. Fixing: [2-3 things]. Pull in 60 seconds."

### Attempt 2: Refine Execution

**After Wipe**:

> "Better! We got to 40%. Same plan, tighter execution. DPS throttle first 10 seconds. Pull in 60."

### Attempt 3: Final Adjustments

**After Wipe**:

> "Alright, this is our attempt. All cooldowns, flasks, everything. If we wipe again, we'll take a 5-min break and rethink strategy."

### Attempt 4+: Strategy Pivot

**After 3rd Wipe**:

> "We're stuck. 5-minute break. I'm gonna research alternate strat. Meanwhile:
> 
> - Tanks: Check your resist gear, make sure capped
> - Healers: Review mana consumption, using consumables?
> - DPS: Check your buff uptime, WeakAuras working?  
>     Back in 5."

**During Break**: Post in Discord

```
#raid-signups or #guides:
"Stuck on [Boss]. Researching. If anyone has experience, DM me strat suggestions. Checking YouTube for alternate methods."
```

**Why Break After 3**: Prevents tilt. Players make worse decisions when frustrated.

---

## Recognizing and Rewarding Performance

### Mid-Raid Shoutouts (Morale Boost)

**After Clean Kill**:

> "Clean! Shoutout to [Healer] - zero deaths, perfect dispels. [DPS] - topped charts. Great job everyone."

**Why**: Positive reinforcement → people want to perform well next boss

### Post-Raid Highlights

**In #raid-highlights** (Copy-Paste Template):

```
🏆 **Karazhan MVP - December 11, 2025**

**Top Performers:**
- @Mage1: 98 parse on Shade of Aran (2,450 DPS)
- @Priest1: 96 parse overall (12,500 HPS)
- @WarriorMain: Zero deaths, perfect interrupts

**Clean Execution:**
- Nightbane: One-shot (first time in weeks!)
- Moroes: Flawless CC, no breaks

**Funny Moments:**
- @Rogue1 solo'd last 2% of Prince after raid died (clutch Evasion)
- @Hunter1 Feigned Death at wrong time, pulled all adds (RIP)

**Next Raid:** Wednesday, Dec 18 - Signups open tomorrow!
```

---

## Emergency Situations

### Mid-Raid Disconnect (Tank/Healer)

**Immediate Actions**:

1. Pause DPS: "STOP"
2. Check Discord: Is player in voice?
3. Wait 60 seconds
4. If not back: "Pulling from bench - @Backup you're in"

**Macro for Raid**:

```
/rw [DISCONNECT] - STOP DPS
/rw Waiting 60 seconds for reconnect
/rw If not back, we continue with backup
```

---

### Toxic Behavior Mid-Raid

**Scenario**: Player flaming others in raid chat

**Response Sequence**:

1. **Warning** (Public): "[Name], keep it constructive"
2. **Mute** (If continues): Server-mute via Dyno (or voice mute)
3. **Kick** (If still toxic): Remove from raid, replace with bench
4. **Ban** (If extreme): Report in #mod-chat, ticket for appeal

**Script**:

> "That's strike one, [Name]. Next one and you're muted. We're here to clear content, not argue."

---

### Raid Falling Apart (6+ People Leave)

**When to Call It**:

- Below minimum comp (9 for Kara, 22 for 25-man)
- Unrecoverable role loss (both healers left)
- Constant wipes, morale destroyed (1 hour on one boss)

**Graceful Exit**:

> "We're not gonna beat our heads tonight. Calling raid here. Thanks everyone for trying. We'll regroup next week with better comp. Logs posted in #warcraftlogs."

**Follow-Up** (Discord):

```
#announcements:
"Tonight's raid canceled after [Boss]. We need to recruit more [Role]. If you know reliable players, invite them.

Next raid: [Date] - We'll reschedule tonight's run for Sunday."
```

---

## Continuous Improvement (Personal Raid Leader Skills)

### Self-Review After Each Raid

**Questions to Ask Yourself**:

1. Did I explain all mechanics clearly?
2. Were my callouts timely and concise?
3. Did I keep morale high after wipes?
4. Did I handle loot disputes fairly?
5. What can I improve next week?

**Track in Spreadsheet**:

- Raid duration (goal: <3 hours for Kara)
- Boss kill times (compare week to week)
- Player feedback (DMs or polls)
- Personal notes ("Need to call Bloodlust earlier")

---

## Essential Addons for Raid Leaders

**Beyond Standard Raider Addons**:

1. **Method Raid Tools (MRT)**
    
    - Create raid notes (assignments)
    - Timers for cooldowns
    - Share notes to raid
    - `/mrt` to open
2. **Angry Assignments**
    
    - Alternative to MRT
    - Simpler UI
    - Good for PUGs (less clutter)
3. **Exorsus Raid Tools**
    
    - Pull timers
    - Battle res tracker
    - Cooldown tracker
    - Inspect tool (check buffs/gear)
4. **Gargul** (Already Mentioned)
    
    - Loot management
    - Soft reserve sync

---

## Quick Reference: Boss Callout Cheat Sheet

### Karazhan

**Attumen**: "Charge - move away from [target]"  
**Moroes**: "Garrote on [player] - dispel NOW"  
**Maiden**: "Holy Fire - dispel dispel dispel"  
**Opera (Wolf)**: "[Player] is Little Red - RUN AWAY"  
**Curator**: "Flare up - AOE NOW"  
**Shade**: "Flame Wreath - FREEZE... Clear, move now"  
**Illhoof**: "Chains on [player] - BREAK THEM"  
**Netherspite**: "Beam swap in 5... 4... 3... 2... 1... SWAP"  
**Prince**: "Infernal - KITE don't tank"  
**Nightbane**: "Air phase - kill skeletons only"

---

## Next Steps

After mastering raid leading: → See **Raid Organization Workflow** for full raid management  
→ See **Templates Guide** for copy-paste content  
→ Train backup raid leaders (delegate 50% of raids for burnout prevention)
