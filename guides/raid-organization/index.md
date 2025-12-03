---
layout: guide
title: Raid Organization Workflow
section: 3
next_section: guides/raid-leading/
next_title: Raid Leading Strategies
---

# 6. WoW TBC Raid Organization Workflow

## The Golden Workflow (Complete Raid Cycle)

This workflow integrates all bots and tools into a seamless raid management system.

---

## Phase 1: Event Creation (48-72 Hours Before Raid)

### 🔴 Raid Leader Actions

#### Step 1: Create Event (Raid-Helper/Apollo)

**Command**: `/create` in #raid-signups

**Event Template Example**:

```
Event Name: Karazhan PUG - MS>OS + 2 SR
Date: Wednesday, December 11, 2025
Time: 20:00 CET
Duration: 3 hours

Requirements:
✅ Voice required (Push-to-Talk)
✅ Flasks, food, consumables ready
✅ Warcraft Logs profile linked in #gear-checks
✅ ilvl ≥ 100 (check with !armory)
✅ DBM/Deadly Boss Mods installed

Loot: Main Spec > Off Spec + 2 Soft Reserves

Slots:
🛡️ Tank: 0/2
❤️ Healer: 0/3
⚔️ DPS: 0/5

Instructions:
1. React to sign up
2. You will be DM'd a SoftRes link - select your 2 reserves
3. Post your gear in #gear-checks for verification
4. Be online 10 minutes before start time
```

#### Step 2: Configure Raid-Helper Settings

- Enable auto-reminders (24h, 3h, 30min before)
- Set signup deadline (15 minutes before raid)
- Enable bench system (allow 2 extra signups)
- Link SoftRes.it (if supported by bot)

**Result**: Event posted in #raid-signups with reaction buttons

---

## Phase 2: Signup & Verification (48h-2h Before)

### Player Actions (Automated by Bots)

#### Step 1: React to Sign Up

- Player clicks 🛡️ Tank / ❤️ Healer / ⚔️ DPS emoji
- Raid-Helper adds them to roster
- **Bot auto-DMs player**: "Thanks for signing up! Lock in your 2 Soft Reserves: [SoftRes link]"

#### Step 2: Select Soft Reserves

- Player clicks link → Opens SoftRes.it web interface
- Browses available loot (filtered by raid: Karazhan)
- Selects 2 items (e.g., "Dragonspine Trophy", "Ribbon of Sacrifice")
- Confirms reserves

**Bot Action**: Updates reserve embed in #softres-kara

#### Step 3: Gear Verification (Required for First-Time Raiders)

Player posts in #gear-checks:

```
!armory <gear string from in-game addon>
```

**How to Get Gear String**:

1. Install "DejaCharacterStats" addon (or similar)
2. Type `/dcstats export` in-game
3. Copy string
4. Paste in Discord with `!armory`

**MikePy Response**: Embeds visual Armory card showing:

- ilvl
- Enchants (missing enchants flagged)
- Gems (empty sockets flagged)
- Professions
- Spec

**Guilds of WoW (if installed)**: Auto-flags warnings

> "⚠️ @Player - ilvl 95 (requirement: 100). Missing chest enchant. 2 empty gem sockets."

### Raid Leader Actions

#### Review Roster (Daily Check)

- Check Raid-Helper signup list
- Verify class balance:
    - **Kara (10-man)**: 2 tanks, 2-3 healers, 5-6 DPS
    - **Gruul/Mag (25-man)**: 2-3 tanks, 6-8 healers, 14-17 DPS
    - **Critical**: At least 1 Shaman per 5 players (TBC requirement)

#### Approve/Reject Signups

If undergeared (flagged by Guilds of WoW):

- DM player: "Thanks for signing up! For this run we need ilvl 100+. You're currently 95. Please upgrade and try next week, or join our Heroic groups to gear up!"
- Remove from roster
- Notify backup/bench

#### 24 Hours Before: Roster Lock Check

- Verify minimum signups (8 for Kara, 20 for 25-man)
- If under-filled: @mention roles needed in #lfg-karazhan
    
    > "@Healer @DPS Kara tomorrow 20:00 CET - Need 1 Healer, 2 DPS! MS>OS + 2 SR. React in #raid-signups"
    

---

## Phase 3: Pre-Raid Preparation (1-2 Hours Before)

### 🔴 Raid Leader Actions (Critical)

#### Step 1: Export Soft Reserves (1 hour before)

1. Go to SoftRes.it → Your Event
2. Click "Export CSV"
3. Save file: `kara_reserves_2025-12-11.csv`

#### Step 2: Import to Gargul (In-Game)

1. Log into WoW
2. Type `/gargul softres import`
3. Select downloaded CSV file
4. Verify import: `/gargul softres show`

**Result**: Gargul now knows who reserved what items

#### Step 3: Send Reminders

**Raid-Helper auto-sends**: "Raid in 1 hour! @Tank @Healer @DPS - Be online in 10 minutes!"

**Manual reminder in #raid-signups**:

```
@Tank @Healer @DPS 

Karazhan raid in 1 HOUR!

✅ Check your reserves in #softres-kara
✅ Flasks, food, consumables ready
✅ Repair at 100%
✅ Be in Deadwind Pass by 19:50 CET

Voice: #raid-voice-kara
```

#### Step 4: Confirm Attendance

- Raid-Helper auto-pings: "React with ✅ to confirm or ❌ to cancel"
- Track responses
- If someone cancels late: Pull from bench or re-advertise in #lfg

#### Step 5: Review Strategy (Optional)

Post quick strategy reminder in #raid-signups or #guides:

```
**Tonight's Bosses:**
- Attumen: Tank in corner, move away from charge
- Moroes: CC 2 adds, interrupt heals
- Maiden: Dispel Holy Fire ASAP
- Opera: Will announce which event when we zone in
- Curator: Kill Flare adds, Evocate on Mage/Warlock for mana

Full strats pinned in #guides. Questions before we start?
```

---

## Phase 4: Raid Execution (Raid Time)

### 🔴 Raid Start Checklist (Raid Leader)

#### 10 Minutes Before Pull

1. **Form Raid Group** (In-Game)
    
    - Invite all signed players
    - Use `/invite <name>` or Battle.net if Guilds of WoW Tier 2
2. **Move to Voice**
    
    - @mention raid roster: "Everyone to #raid-voice-kara now"
    - Mute #raid-signups temporarily (reduce distraction)
3. **Roll Call** (Voice)
    
    - "Sound off when I say your name - Tank 1: [name]..."
    - Confirm all 10 players present
4. **Consumables Check**
    
    - "Flask check - type 'flasked' in raid chat"
    - "Food buff check"
    - If someone missing: "You have 5 minutes to get consumables or we pull from bench"
5. **Verify Gargul Sync**
    
    - `/gargul softres show` in raid chat
    - Verify reserves displayed correctly
    - If broken: Re-import CSV
6. **Boss Strategy Recap** (Voice)
    
    - Quick 30-second recap of first boss (Attumen)
    - "Any questions before pull?"

#### During Raid: Loot Management (Automated)

**Gargul Workflow**:

1. Boss dies → Loot window opens
2. **Gargul auto-announces in raid chat**:
    
    ```
    [Gargul] Moroes' Lucky Pocket Watch drops!Reserved by: [Rogue1], [Rogue2]Rolling among reservers...
    ```
    
3. **Auto-rolls** (1-100) among reservers
4. **Announces winner**:
    
    ```
    [Gargul] [Rogue1] wins with 87! Congratulations!
    ```
    
5. **Master Looter assigns item** (if ML system) OR
6. **Winner loots** (if personal loot)

**If No Reserves**:

```
[Gargul] Ring of Eternal Flame drops!
No reserves. Rolling Main Spec...
All eligible: [Mage1], [Warlock1], [Priest1]
```

**If MS Pass, Goes to OS**:

```
[Gargul] No MS rolls. Opening to Off Spec...
```

**Manual Override** (Raid Leader):

- `/gargul assign [item] [player]` - Force assign (use for special cases)

#### During Raid: Voice Management

**Raid Leader Best Practices**:

- Keep main callouts in #raid-leader Stage (if using Stage Channel)
- Tanks coordinate in #off-tank-1 voice (separate channel)
- **Clear callouts**: "Assignment → Action → Event"
    - "Shammybaby - Bloodlust - NOW"
    - "Everyone - Move out - Flame Wreath"

**Mute Control**:

- If too much chatter: "Muting non-essential during boss pulls. Whisper me if emergency."
- Use Dyno/Carl-bot to temp-mute disruptive players

#### During Raid: Strategy Adjustments

**If Wipe Occurs**:

1. **No Blame** - "Okay, what went wrong? Let's fix it."
2. **Focus on 2-3 Improvements** - Don't overload
    - "Next pull: Interrupt the heal at 50% boss health"
    - "Hunters: Misdirect to main tank at start"
3. **Post Text Summary** - In #raid-signups or dedicated raid thread
    
    ```
    **Moroes Adjustments:**- CC kill order: Paladin → Priest → Shaman- Interrupt rotation: Rogue1 (1st), Rogue2 (2nd), Warrior (3rd)- Dispel Garrote ASAP
    ```
    

#### Breaks

- **10 minutes after each boss** - "10 minute bio break, be back by 20:45"
- Use break to discuss next boss strategy
- Post strategy in text while on break

---

## Phase 5: Post-Raid (After Clear)

### 🔴 Raid Leader Actions (Critical)

#### Step 1: Upload Warcraft Logs (Immediately After)

1. Open Warcraft Logs Uploader app
2. Select raid session
3. Click "Upload"
4. **Webhook auto-posts** to #warcraftlogs:
    
    ```
    📊 Karazhan - December 11, 2025Duration: 2h 15mBosses: 11/11Top DPS: @Mage1 (98 parse - Shade of Aran)Top HPS: @Priest1 (96 parse - Overall)Full report: [WCL Link]
    ```
    

#### Step 2: Thank Raid (Voice & Text)

**Voice**: "Great job everyone! Clean run, 11/11 in 2 hours. See you next week!"

**Text in #raid-signups**:

```
✅ Karazhan CLEARED! 11/11 in 2h 15m

🏆 **Highlights:**
- @Mage1: 98 parse on Shade (monster!)
- @Priest1: 96 HPS overall (carried heals)
- Zero wipes on Nightbane (perfect execution)

📊 Logs: [WCL Link]
🎥 Highlights: Post clips in #clips

**Next Raid:** Wednesday, December 18 - Signups open tomorrow!

Thanks to everyone! 🎉
```

#### Step 3: Collect Feedback (Optional)

Post in #raid-feedback or DM:

```
Quick feedback survey:
- What went well?
- What should we improve?
- Any loot concerns?
```

Or use Simple Poll bot:

```
!poll "Rate this raid: 1⭐ Terrible | 2⭐ Meh | 3⭐ Good | 4⭐ Great | 5⭐ Perfect"
```

#### Step 4: Update Roster Notes

- Track attendance: "Mage1: 10 raids, 90% attendance"
- Note high performers for Core role consideration
- Flag issues: "Tank2 late 3 times, warned"

#### Step 5: Schedule Next Raid

- Raid-Helper: Create recurring event (auto-posts next week)
- OR manually: `/create` next raid immediately
- Advantage: Early signups = better turnout

---

## TBC-Specific Raid Compositions

### Karazhan (10-Man) - Optimal Comp

**Tanks (2)**:

- Main Tank: Protection Warrior or Protection Paladin
- Off-Tank: Feral Druid (can DPS when not tanking)

**Healers (2-3)**:

- Priority: Holy Paladin (tank healing)
- Priority: Resto Druid (HoTs for raid)
- Flex: Resto Shaman or Holy Priest

**DPS (5-6)**:

- **REQUIRED**: 1 Mage (Polymorph for Moroes)
- **REQUIRED**: 1-2 Hunters (Misdirect, ranged)
- Recommended: Shadow Priest (Vampiric Embrace for healer mana)
- Flex: Warlocks, Rogues, Enhancement Shaman

**Critical**: No hard DPS checks in Kara - bring reliable players over "meta" specs

---

### Gruul's Lair / Magtheridon (25-Man) - Optimal Comp

**Tanks (2-3)**:

- Main Tank: Protection Warrior (highest threat)
- Off-Tank 1: Feral Druid (add control)
- Off-Tank 2 (Gruul): Protection Paladin (emergency)

**Healers (6-8)**:

- **Group 5 (Healer Mana Group)**: Resto Shaman (Mana Tide) + Shadow Priest (Vampiric Embrace) + 1 other healer
- 2-3 Holy Paladins (tank healing)
- 2-3 Resto Druids (raid healing)
- 1-2 Resto Shaman (Bloodlust + Chain Heal)

**DPS (14-17)**:

**CRITICAL - Shaman Distribution** (TBC Unique Requirement):

- **Goal**: 1 Shaman per 5-man group (5 total)
- **Group 1 (Melee DPS)**: Enhancement Shaman (Windfury Totem) + Warriors/Rogues/Feral
- **Group 2 (Caster DPS)**: Elemental Shaman (Totem of Wrath) + Mages/Warlocks
- **Group 3 (Ranged Phys)**: Enhancement Shaman OR Ele (flexibility) + Hunters
- **Group 4 (Hybrid DPS)**: Ret Paladin + Shadow Priest + Flex DPS + Resto Shaman
- **Group 5 (Healers)**: Resto Shaman + Shadow Priest (mana battery) + Healers

**DPS Composition Guidelines**:

- 3-4 Warlocks (Curse of Elements, high sustained damage)
- 2-3 Mages (AoE, Polymorph utility)
- 2-3 Hunters (Misdirect, ranged)
- 2-3 Rogues (melee DPS, interrupts)
- 2-3 Warriors (melee DPS)
- 1 Shadow Priest (mandatory - Vampiric Embrace for healers)
- 1-2 Balance Druids (Moonkin Aura for casters)
- 0-1 Ret Paladin (buffs > personal DPS)

**Critical Notes**:

- **Bloodlust/Heroism**: Each group needs Shaman for this ability (TBC's most powerful raid CD)
- **Resist Gear**: Magtheridon requires Shadow Resistance gear (cloak minimum)
- **Clickers**: Assign 5 players for Magtheridon cube channels BEFORE pull

---

### Bench Policy (The 10% Rule)

**Always recruit 10% over capacity:**

- 25-man raid → Sign up 28 players
- 10-man raid → Sign up 11 players

**Bench Management**:

1. Announce bench system upfront: "We maintain a bench for reliability. Benched players get priority next week."
2. Rotate bench fairly: Track who's been benched, prioritize them next raid
3. Benched players stay in Discord voice: "Listen to raid, learn strats, you might be called in"
4. If someone leaves mid-raid → Instant swap with bench

**Raid-Helper Bench Feature**:

- Enable "Bench" role in event settings
- Excess signups auto-tagged as "Bench"
- Easy swap: Click name → Promote to Main Roster

---

## Raid Assignment Templates (Copy-Paste)

### Template 1: Karazhan Boss Assignments

**Post in #raid-signups before raid:**

```
**KARAZHAN ASSIGNMENTS - December 11, 2025**

📋 **Raid Composition:**
Tanks: @WarriorMain, @DruidOT
Healers: @PaladinHeal, @DruidHeal, @ShamanHeal
DPS: @Mage1, @Warlock1, @Rogue1, @Hunter1, @ShadowPriest

---

🎯 **Key Assignments:**

**Attumen the Huntsman:**
- MT: @WarriorMain (Attumen + Midnight)
- Ranged: Spread for Intangible Presence
- All: Move away from Charge target

**Moroes:**
- MT: @WarriorMain (Moroes)
- CC: @Mage1 Polymorph Left add, @Hunter1 Trap Right add
- Interrupt rotation: @Rogue1 → @WarriorMain → @Hunter1
- Dispels: @PaladinHeal priority on Garrote

**Maiden of Virtue:**
- Spread 10 yards (Consecration damage)
- @PaladinHeal @DruidHeal: Dispel Holy Fire IMMEDIATELY
- All: Stop casting during Repentance

**Opera Event:** (TBD - will announce when we zone in)
- Wizard of Oz: Kill Dorothee first
- Big Bad Wolf: Run out if turned into Red Riding Hood
- Romulo & Julianne: Kill at same time (10% sync)

**Curator:**
- Ranged: Spread 15 yards (Evocate)
- @Mage1 @Warlock1: Priority DPS on Flare adds
- Heroism/Bloodlust: 20% boss health

**Shade of Aran:**
- Flame Wreath: DO NOT MOVE (instant wipe if broken)
- Blizzard: Stack on Aran (center safe zone)
- Arcane Explosion: Run out 15 yards
- @Rogue1: Kick Frostbolt during drinking phase

**Terestian Illhoof:**
- MT: @WarriorMain (Illhoof)
- OT: @DruidOT (Kil'rek add)
- Imp AOE: @Mage1 Blizzard, @Warlock1 Seed of Corruption
- Priority: Kill Demon Chains IMMEDIATELY

**Netherspite:**
- MT: @WarriorMain in Red beam
- @ShadowPriest: Rotate Blue beam (mana regen)
- Healers: Rotate Green beam (healing boost)
- Beam rotation every 30 seconds (call switches)

**Chess Event:**
- Follow Raid Leader calls for piece movement
- All: DPS King pieces when available

**Prince Malchezaar:**
- Phase 1-2: MT center, raid spread 10 yards (Enfeeble)
- Phase 3: Add tank @DruidOT (Netherspite Infernals)
- Infernals: Kite, do not tank in place
- Axes: Dodge or minimize (visual tells)

**Nightbane:** (Optional - requires Blackened Urn)
- Air Phase: All DPS skeletons
- Ground Phase: Spread for Charred Earth
- @PaladinHeal: Fear Ward on MT (if available)

---

❓ Questions? Ask now before we start!
```

---

### Template 2: Loot Priority Notes

**Post in #rules-loot or #raid-signups:**

```
**LOOT PRIORITY SYSTEM - MS > OS + 2 Soft Reserves**

🎲 **How It Works:**
1. Boss dies → Gargul checks reserves
2. If item reserved → Only reservers roll (1-100)
3. If NO reserve → Main Spec (MS) rolls
4. If MS passes → Off Spec (OS) rolls
5. If OS passes → Disenchant or bank for guild

💎 **Soft Reserve Rules:**
- You reserve 2 items total per raid (via SoftRes link)
- Multiple people can reserve same item (not exclusive)
- Reserves are public (check #softres-kara)
- Once reserved, locked (no changes after raid starts)

⚔️ **Main Spec vs Off Spec:**
- MS = Your signed role (Tank/Healer/DPS)
- OS = Any other role
- Example: Warrior signed as Tank → Plate DPS gear is OS

💰 **BoE Items (Epic World Drops):**
- Rolled fairly among all (MS > OS)
- OR sold on AH and gold split (announced before roll)
- No reserves allowed on BoE (applies to raid drops only)

🚫 **NO Hard Reserves:**
- Raid Leaders cannot reserve items
- Everyone has equal chance via SR system

📜 **Dispute Process:**
- Issues? Open ticket in #support immediately
- Don't argue in raid chat (wastes time)
- Loot can be reassigned if mistake proven

---

**Tonight's Popular Reserves:**
- Dragonspine Trophy: 4 reservers (Moroes)
- Ribbon of Sacrifice: 3 reservers (Maiden)
- Helm of the Fallen Champion: 2 reservers (Prince)

Good luck! 🍀
```

---

## Automation Checklist (Set Once, Use Forever)

### Raid-Helper Recurring Events

- [ ] Create template: "Karazhan PUG - Wednesday 20:00 CET"
- [ ] Enable recurring: Every week, same time
- [ ] Auto-reminders: 24h, 3h, 30min before
- [ ] Auto-bench: 11+ signups = bench system
- [ ] Auto-close: 15 min before raid time

### SoftRes.it Webhook

- [ ] Link SoftRes bot to #softres-kara
- [ ] Enable auto-post when reserves updated
- [ ] Set reserve limit: 2 items per player
- [ ] CSV export reminder (calendar event 1h before raid)

### Warcraft Logs Webhook

- [ ] Configure WCL webhook to #warcraftlogs
- [ ] Auto-post on log upload: Full report + top parses
- [ ] Enable notifications (@Raid tag)

### Dyno/Carl-bot Auto-Moderation

- [ ] Auto-delete old LFG posts (24h timer)
- [ ] Auto-close raid signups (15 min before start)
- [ ] Auto-move AFK players to #afk-lobby (15 min)

---

## Common Raid Issues & Solutions

### Issue: Players No-Show

**Solution**:

- Always recruit 10% over (bench system)
- Raid-Helper auto-reminds 30 min before
- If chronic: Remove from future signups

### Issue: Undergeared Players Slip Through

**Solution**:

- Use Guilds of WoW auto-checks ($1/mo)
- Manually verify: `!armory` check before accepting signup
- Set clear ilvl requirements in event description

### Issue: Loot Dispute ("I reserved that!")

**Solution**:

- Gargul logs all rolls → Show proof
- SoftRes embeds are public → Screenshot
- If genuine mistake: Reassign, note in logs
- If player lying: Remove from raid, warn in #mod-chat

### Issue: Raid Takes Too Long (5+ Hours)

**Solution**:

- Over-explain fights BEFORE pull (not during)
- Limit wipes: 3 attempts → Break for strategy rework
- Skip optional bosses (Nightbane) if time-limited
- Set hard stop time: "We raid until 23:00 CET, no exceptions"

### Issue: Toxic Player in Voice

**Solution**:

- Warning: "Keep it constructive, [Name]"
- Mute: If continues, temp-mute via Dyno
- Kick: If still continues, remove from raid
- Ban: Report in #mod-chat, ticket system for appeal

---

## Next Steps

After workflow setup: → See **Raid Leading Strategies** for callout techniques  
→ See **Templates Guide** for more copy-paste content  
→ See **Bot Setup Guide** for tool configuration


