---
layout: guide
title: WeakAuras Complete Guide
section: 7
next_section: guides/minmaxing/
next_title: Min-Maxing Guide
---

# 10. WoW TBC WeakAuras Complete Guide

## Table of Contents

1. [What Are WeakAuras?](https://claude.ai/chat/44ef7b25-1d31-439c-91f7-05c868210582#what-are-weakauras)
2. [Installation & Setup](https://claude.ai/chat/44ef7b25-1d31-439c-91f7-05c868210582#installation--setup)
3. [Best WeakAura Packs for TBC](https://claude.ai/chat/44ef7b25-1d31-439c-91f7-05c868210582#best-weakaura-packs-for-tbc)
4. [Boss-Specific WeakAuras](https://claude.ai/chat/44ef7b25-1d31-439c-91f7-05c868210582#boss-specific-weakauras)
5. [Class-Specific WeakAuras](https://claude.ai/chat/44ef7b25-1d31-439c-91f7-05c868210582#class-specific-weakauras)
6. [Creating Custom WeakAuras](https://claude.ai/chat/44ef7b25-1d31-439c-91f7-05c868210582#creating-custom-weakauras)
7. [Optimization & Performance](https://claude.ai/chat/44ef7b25-1d31-439c-91f7-05c868210582#optimization--performance)

---

## What Are WeakAuras?

**WeakAuras** is the most powerful addon for custom alerts, timers, and visual indicators in WoW.

### What It Does:

- **Tracks buffs/debuffs** on you or targets
- **Boss mechanic warnings** (visual + audio)
- **Cooldown tracking** (know when abilities are ready)
- **Resource tracking** (mana, energy, combo points)
- **Proc alerts** (when trinkets/enchants activate)

### Why Essential for TBC:

- **DBM tells you WHAT** (Flame Wreath in 5 seconds)
- **WeakAuras shows you HOW** (Big red screen when you have Flame Wreath on you)

**TBC Raids = Mechanic-Heavy**: Missing one dispel or standing in one Flame Wreath = wipe. WeakAuras makes mechanics impossible to miss.

---

## Installation & Setup

### 🔴 Step 1: Install WeakAuras2

**Download**:

1. Go to **CurseForge** or **WoWInterface**
2. Search "WeakAuras 2 Classic"
3. Download **WeakAuras 2** (NOT WeakAuras 1 - outdated)
4. Extract to `World of Warcraft\_classic_\Interface\AddOns\`

**Or Use CurseForge App** (Easier):

1. Install CurseForge desktop app
2. Select "WoW Classic TBC"
3. Search "WeakAuras 2"
4. Click Install
5. App auto-updates addon

---

### 🔴 Step 2: Install WeakAuras Companion (Highly Recommended)

**Why?** Allows importing WeakAuras from **Wago.io** (community library) with one click.

**Download**:

1. CurseForge → Search "WeakAuras Companion"
2. Install
3. Restart WoW

**Alternative**: Manual import (copy-paste long strings) - tedious.

---

### 🔴 Step 3: First Launch Setup

1. Log into WoW
2. Type `/wa` or `/weakauras` to open interface
3. You'll see a blank screen (no WeakAuras loaded yet)

**Interface Overview**:

- **Left Panel**: List of installed WeakAuras
- **Center**: Preview of selected WeakAura
- **Right Panel**: Settings (triggers, actions, display)

---

### 🔴 Step 4: Import Your First WeakAura

**Test Import** (Simple Example):

1. Go to **Wago.io** (community WeakAuras library)
2. Search "TBC Raid"
3. Find a popular pack (e.g., "TBC Raid CDs")
4. Click **"Copy Import String"**
5. In WoW, type `/wa`
6. Click **"Import"** button (bottom-left)
7. Paste string (Ctrl+V)
8. Click **"Import"**

**Result**: WeakAura appears in left panel and on your screen.

---

## Best WeakAura Packs for TBC

### 🔴 Universal Raid Packs (Install First)

#### 1. **Causese's TBC Raid Suite** (Most Popular)

**Link**: Search "Causese TBC" on Wago.io

**What It Includes**:

- All Karazhan boss mechanics
- Gruul/Mag alerts
- SSC/TK (Phase 2 content)
- Universal raid timers (interrupts, dispels)

**Why Best**: Covers 90% of raid mechanics, constantly updated, used by top guilds.

**Installation**:

1. Wago.io → Search "Causese TBC Raid"
2. Copy import string
3. `/wa` → Import → Paste
4. Done (auto-loads for each boss)

---

#### 2. **LuckyOneUI - TBC Complete** (Comprehensive)

**Link**: Wago.io → "LuckyOneUI TBC"

**What It Includes**:

- Boss mechanics (all TBC raids)
- Class cooldown tracking (all specs)
- Buff/debuff tracking
- Interrupt/CC timers
- PvP arena alerts (bonus)

**Why Good**: If you want ONE pack for everything (raids + class + PvP).

---

#### 3. **Quazii's TBC Essentials** (Minimalist)

**Link**: Wago.io → "Quazii TBC"

**What It Includes**:

- Core boss mechanics only (no clutter)
- Optimized for performance (low FPS impact)
- Clean UI (small icons, not intrusive)

**Why Good**: If you have a slow PC or prefer minimal screen clutter.

---

### 🟡 Boss-Specific WeakAura Packs

#### Karazhan Mega-Pack

**Search**: "Karazhan WeakAuras TBC" on Wago.io

**Covers**:

- Attumen: Charge warning
- Moroes: Garrote dispel alert (healers)
- Maiden: Holy Fire dispel (priority)
- Opera: Little Red Riding Hood run-away alert (Big Bad Wolf)
- Curator: Evocation spread warning
- **Shade of Aran**: MASSIVE Flame Wreath alert (most important)
- Illhoof: Demon Chains break alert
- Netherspite: Beam rotation timer
- Prince: Infernal spawn, Enfeeble warning

**Critical**: Shade of Aran WeakAura alone prevents 80% of wipes.

---

#### Gruul/Mag Pack

**Search**: "Gruul Magtheridon WA TBC"

**Covers**:

- Gruul: Shatter spread timer (move every 30 sec)
- Gruul: Growth stacks (tank swap)
- High King Maulgar: Which add you're assigned to (color-coded)
- Magtheridon: Cube clicker assignments (who clicks when)
- Magtheridon: Blast Nova cast bar (massive raid-wide damage)

---

### 🟡 Class-Specific WeakAura Packs

#### Universal Class Tracker

**Search**: "[YourClass] TBC WeakAuras" (e.g., "Warlock TBC WeakAuras")

**What It Tracks** (Class-Dependent):

- Cooldown timers (know when abilities are ready)
- Buff/debuff uptime (e.g., Warlock Curses, Mage Arcane Intellect)
- Resource bars (Mana, Energy, Rage, Holy Power)
- Proc alerts (trinket procs, weapon enchants)

**Popular Packs by Class**:

**Tanks**:

- "TBC Tank Cooldowns" - Tracks Shield Wall, Last Stand, Shield Block
- Threat meter integration (alerts when close to pulling aggro off you)

**Healers**:

- "TBC Healer HoT Tracker" - Shows HoTs on raid frames (Druids)
- "TBC Dispel Tracker" - Highlights dispellable debuffs on raid

**DPS**:

- **Warlocks**: "TBC Warlock Rotation" - Tracks DoT duration, suggests next cast
- **Mages**: "TBC Mage Combustion" - Alerts when Combustion is ready (fire spec)
- **Hunters**: "TBC Hunter Aimed Shot" - Cast bar + auto-shot timer (shot weaving)
- **Rogues**: "TBC Rogue Energy Ticker" - Energy regen timer (optimal ability usage)

---

## Boss-Specific WeakAuras (Detailed)

### 🔴 Shade of Aran - Flame Wreath (CRITICAL)

**Most Important WeakAura in Karazhan**: Flame Wreath wipes raids instantly if anyone moves.

**What It Does**:

1. **Visual**: Entire screen turns RED when you have Flame Wreath
2. **Audio**: Plays LOUD sound ("FREEZE!" voiceover)
3. **Text**: Giant "DO NOT MOVE" message center-screen
4. **Duration Timer**: Shows exactly when wreath expires (5 seconds)

**Import**:

- Wago.io → Search "Shade Aran Flame Wreath"
- Top result (usually 1000+ downloads)
- Import → Test in raid

**How to Test** (Before Raid):

- `/wa` → Find "Flame Wreath" aura
- Click "Test" button
- Screen should turn red, play sound

---

### 🔴 Moroes - Garrote Dispel (Healers)

**What It Does**:

- Highlights raid frame of player with Garrote (glowing red)
- Plays alert sound ("Dispel now!")
- Shows Garrote stacks (if multi-dispel needed)

**Why Critical**: Garrote ticks for massive damage. Late dispel = death.

**Healer-Specific**:

- Paladins: "Cleanse" dispels Garrote (poison)
- Priests: "Dispel Magic" does NOT work (wrong dispel type)
- Shamans: "Poison Cleansing Totem" auto-dispels nearby players

---

### 🔴 Prince Malchezaar - Infernal Spawn

**What It Does**:

- Visual marker on ground where Infernal lands
- Audio alert: "Infernal spawn - move away"
- Arrow pointing away from Infernal (kiting guide)

**Why Critical**: Standing near Infernal = massive AOE damage. Tanks must kite, raid must avoid.

---

### 🟡 Curator - Evocation Warning

**What It Does**:

- 5-second countdown before Evocation
- Screen flash when Evocation starts
- Text: "SPREAD OUT - 15 YARDS"

**Why Useful**: Evocation does AOE damage. If stacked, entire raid dies. WeakAura reminds you to spread.

---

### 🟡 Netherspite - Beam Tracker

**What It Does**:

- Shows YOUR assigned beam color (Red/Blue/Green)
- Timer: "Swap in 5... 4... 3... 2... 1... SWAP NOW"
- Visual: Your beam color lights up when it's your turn

**Why Useful**: Netherspite fight = coordination-heavy. Wrong person in beam = wipe. WeakAura automates assignments.

**Setup**:

- Raid Leader assigns beams (tell WeakAura creator who's in each beam)
- WeakAura displays assignments automatically

**Advanced**: Integrates with ExRT (Exorsus Raid Tools) notes.

---

## Class-Specific WeakAuras (Detailed)

### Tanks

#### Cooldown Tracker

**What It Tracks**:

- Shield Wall (Warrior): 30min CD
- Last Stand (Warrior): 8min CD
- Shield Block (Warrior): 5sec CD
- Frenzied Regeneration (Druid): 3min CD
- Barkskin (Druid): 1min CD
- Divine Protection (Paladin): 3min CD

**Display**:

- Icons appear when cooldown is READY (glow effect)
- Timer bar shows cooldown remaining
- Audio alert when major CD (Shield Wall) is ready

**Why**: Tanks need to know cooldowns instantly (healers can't save you if Shield Wall is down and you don't use it).

---

#### Threat Meter Integration

**What It Does**:

- Shows if DPS is close to pulling threat off you
- Visual: Health bar turns yellow (80% threat), red (95% threat)
- Audio: "Threat high on [player]" alert

**Setup**:

- Requires Omen or ThreatClassic2 addon
- WeakAura reads threat data and displays warnings

---

### Healers

#### HoT Tracker (Druids)

**What It Does**:

- Displays Rejuvenation, Regrowth, Lifebloom timers on raid frames
- Color-coded by time remaining: Green (>10sec), Yellow (5-10sec), Red (<5sec)
- Sorts raid by who needs HoT refresh

**Why**: Prevents overwriting HoTs (wasted mana). Shows exactly who needs refresh.

---

#### Dispel Priority (All Healers)

**What It Does**:

- Highlights dispellable debuffs on raid frames
- Priority system: Red (kill player if not dispelled), Yellow (hurts), Green (minor)
- Audio alert for high-priority dispels (Garrote, Holy Fire)

**Customization**:

- Paladins: Only shows poison/disease (what Cleanse can dispel)
- Priests: Only shows magic (what Dispel Magic can remove)
- Shamans: Only shows poison/disease (Cure Poison/Cure Disease)

---

### DPS

#### Warlock - DoT Tracker

**What It Does**:

- Shows Corruption, Curse of Agony, Immolate, Unstable Affliction timers on target
- Bar colors: Green (>50% duration), Yellow (refresh soon), Red (expired)
- Multi-target DoT tracking (shows DoTs on all enemies)

**Why**: TBC Warlocks = DoT uptime is 70% of DPS. Letting DoTs fall off = massive DPS loss.

---

#### Hunter - Shot Weaving Timer

**What It Does**:

- Shows auto-shot timer (when next auto fires)
- Alerts when to cast Aimed Shot (between autos for max DPS)
- Clip warning (if you cancel auto-shot by casting too early)

**Why**: Shot weaving = 20-30% DPS increase for Hunters. WeakAura makes timing perfect.

---

#### Rogue - Energy Ticker

**What It Does**:

- Shows energy regen in 0.1sec increments (game shows only whole numbers)
- Predicts next finisher at 5 combo points (optimal time to Eviscerate)
- Cooldown tracker for Slice and Dice, Blade Flurry

**Why**: Rogues generate energy over time. Knowing exact energy = optimal ability usage (no wasted GCDs).

---

#### Mage - Combustion Tracker (Fire Spec)

**What It Does**:

- Tracks Combustion stacks (crit chance bonus)
- Alerts when to use Combustion (3 crit stacks = max DPS window)
- Shows Ignite damage (DoT from crits)

**Why**: Fire Mages in TBC = Combustion timing is everything. Bad timing = 50% DPS loss.

---

## Creating Custom WeakAuras

### When to Create Custom WA:

- Boss-specific mechanic not covered by existing packs
- Personal preference (want different colors, sounds, positions)
- Class ability not tracked by default packs

---

### 🔴 Basic Custom WeakAura Tutorial

#### Example: Track Your Own Buff (Power Word: Fortitude)

**Step 1: Open WeakAuras**

- Type `/wa`

**Step 2: Create New Aura**

- Click **"New"** button (bottom-left)
- Select **"Icon"** (most common)

**Step 3: Set Trigger**

- **Trigger 1**: "Aura" → "Buff" → "Player"
- **Aura Name**: Type "Power Word: Fortitude"
- **Show When**: "Active" (only shows when buff is ON you)

**Step 4: Set Display**

- **Icon**: Auto-selects Fort icon
- **Position**: Drag icon to where you want it on screen
- **Size**: Adjust slider (recommend 48x48 for buffs)

**Step 5: Add Actions (Optional)**

- **Sound**: Play sound when buff expires
    - **Actions Tab** → **On Hide** → **Play Sound** → Select "RaidWarning"
- **Text**: Show time remaining
    - **Display Tab** → **Text** → Enable → Insert `%p` (duration variable)

**Step 6: Test**

- Click **"Test"** button
- Icon should appear on screen
- Cast Fort on yourself → Icon should light up

**Step 7: Save**

- Name it: "Fort Tracker"
- Done!

---

### 🟡 Intermediate: Boss Mechanic Alert

#### Example: Shade of Aran Flame Wreath Custom

**Step 1**: New WeakAura → **"Icon"**

**Step 2: Trigger**

- **Aura** → **Debuff** → **Player**
- **Aura Name**: "Flame Wreath" (exact spelling from in-game)

**Step 3: Display**

- **Display Type**: Change to **"Texture"** (full-screen overlay)
- **Texture**: Choose solid color
- **Color**: RED (RGB: 255, 0, 0, alpha: 0.5 for semi-transparent)
- **Size**: 100% width, 100% height (covers screen)

**Step 4: Add Text**

- **Text Tab** → Enable
- **Text**: Type "DO NOT MOVE"
- **Font Size**: 72 (huge)
- **Color**: White
- **Position**: Center-screen

**Step 5: Add Sound**

- **Actions Tab** → **On Show** (when debuff appears)
- **Play Sound** → **Sound File**: Select "RaidWarning" or custom sound
- **Repeat**: Every 1 second (audio loop)

**Step 6: Test**

- Need to be in Karazhan with Shade of Aran to test for real
- Or use `/wa` → Test mode (simulates debuff)

**Result**: When you get Flame Wreath, screen turns red, giant text, alarm sound.

---

### 🟢 Advanced: Multi-Condition Aura

#### Example: Bloodlust/Heroism Alert (Only Show When Off Cooldown)

**Trigger 1**: Spell Cooldown

- **Spell**: "Bloodlust"
- **Show When**: "Ready" (not on CD)

**Trigger 2**: Unit Buff

- **Buff**: "Bloodlust"
- **Show When**: "Absent" (you DON'T have buff already)

**Trigger Logic**: "All Triggers" (both must be true)

**Display**: Icon glows when both conditions met (Lust off CD AND not already active).

**Action**: Play sound every 30 seconds (reminder to use Lust).

---

## Optimization & Performance

### WeakAuras = FPS Heavy (If Misconfigured)

**Problem**: Too many WeakAuras = lag in raids (especially 25-man).

---

### 🔴 Performance Optimization Tips

#### 1. Disable Unused WeakAuras

- `/wa` → Right-click aura → **Disable**
- Only enable what you NEED for current boss

**Example**: Disable all SSC/TK auras when doing Karazhan.

---

#### 2. Use "Load Conditions"

**What It Does**: WeakAura only loads when you're in specific raid/zone.

**Setup**:

- WeakAura → **Load Tab**
- **Zone**: Check "Karazhan"
- **Result**: This aura ONLY loads in Kara (saves RAM in other zones)

**Advanced**: Load by boss encounter

- **Encounter ID**: Shade of Aran = Encounter 16524 (check Wago.io for IDs)
- Aura only appears during that boss fight

---

#### 3. Reduce Update Frequency

**Default**: WeakAuras update every 0.1 seconds (10 times/sec) = CPU heavy.

**Optimization**:

- **Actions Tab** → **Update Frequency**: Change to 0.5 seconds
- **Result**: Updates 2 times/sec (less CPU, still responsive)

**When to Use**:

- Buff/debuff trackers that don't need instant updates
- Cooldown timers (1-second intervals are fine)

**When NOT to Use**:

- Boss mechanic alerts (need instant updates)
- Interrupt timers (0.1sec precision needed)

---

#### 4. Use Groups Efficiently

**What Are Groups?**: Collections of WeakAuras organized together.

**Problem**: 50 separate WeakAuras = cluttered list, hard to manage.

**Solution**: Group by category

- "Karazhan Bosses" group (all Kara auras inside)
- "Cooldown Tracking" group (all class CDs)
- "Buff Tracking" group (all buffs)

**How to Group**:

- `/wa` → Drag one aura onto another → Creates group
- Disable entire group with one click

---

#### 5. Delete Old/Unused Auras

**Problem**: Imported 10 WeakAura packs, now have 500 auras, game lags.

**Solution**:

- `/wa` → Sort by "Last Used"
- Delete anything not used in 30+ days
- Keep only current-tier content

---

### FPS Benchmarks

**Good Setup** (30-50 WeakAuras active):

- 60+ FPS in 25-man raids (modern PC)
- 40+ FPS (older PC)

**Bad Setup** (100+ WeakAuras, no optimization):

- <30 FPS in 25-man raids (slideshow)
- Frequent freezes during boss mechanics

**Goal**: <50 active WeakAuras at any time.

---

## Recommended WeakAura Priority by Role

### Tanks (Top 10 Essential)

1. Threat warnings (high-threat DPS)
2. Cooldown tracker (Shield Wall, Last Stand)
3. Taunt cooldown (know when ready)
4. Boss debuff stacks (tank swap alerts)
5. Healer dispel warnings (if you have cleanseable debuff)
6. Rage/Mana bar (resource tracking)
7. Skull marker auto-assist (always hit skull target)
8. Incoming damage meter (anticipate spike damage)
9. Boss cast bar (know when to use defensive)
10. Group buff tracker (are you missing buffs?)

---

### Healers (Top 10 Essential)

1. Dispellable debuff tracker (priority: red = urgent)
2. HoT tracker (Druids)
3. Mana bar + 5SR timer (know when regen starts)
4. Cooldown tracker (Innervate, Mana Tide, Divine Favor)
5. Boss mechanic alerts (Garrote, Holy Fire, etc.)
6. Incoming damage spikes (know when to pre-cast big heals)
7. Raid HP % warnings (know when to AOE heal)
8. Missing raid buffs (who doesn't have Fort?)
9. Battle res tracker (who has Soulstone/Rebirth ready?)
10. OOM warning (auto-alert raid when <10% mana)

---

### DPS (Top 10 Essential)

1. **Boss mechanic alerts** (Flame Wreath, Infernals, etc.)
2. **Cooldown tracker** (major DPS CDs)
3. **DoT/debuff tracker** (uptime %)
4. **Proc alerts** (trinket procs, weapon enchants)
5. **Interrupt tracker** (know when your interrupt is ready)
6. **Target of Target** (hitting what tank is targeting)
7. **Bloodlust timer** (know when to use CDs)
8. **Energy/Mana ticker** (resource optimization)
9. **Buff tracker** (did you flask? food buff?)
10. **DPS meter integration** (live DPS counter)

---

## WeakAuras Import Checklist

### Before Importing ANY WeakAura:

- [ ] Check **downloads + rating** on Wago.io (1000+ = trusted)
- [ ] Read **description** (what does it do?)
- [ ] Check **last updated** (outdated = might not work in TBC)
- [ ] Check **class/role** (is it for your class?)
- [ ] Check **load conditions** (does it load in right zones?)
- [ ] **Import → Test** (don't use in raid untested)
- [ ] **Position on screen** (don't block important UI)
- [ ] **Check FPS impact** (if FPS drops 10+, disable)

---

## Common WeakAura Issues & Fixes

### Issue: WeakAura Not Showing

**Cause**: Load conditions wrong (not loading in your zone/spec).

**Fix**:

- `/wa` → Select aura → **Load Tab**
- Check "Zone" (is current zone checked?)
- Check "Talent Spec" (is your spec checked?)

---

### Issue: WeakAura Blocking UI

**Cause**: Positioned in center-screen, covers important elements.

**Fix**:

- `/wa` → Select aura → **Display Tab**
- Drag preview to new position (top-right or top-center common)
- Lock position: **Actions Tab** → **Lock**

---

### Issue: Sound Too Loud/Quiet

**Cause**: WeakAura sound doesn't respect game volume.

**Fix**:

- `/wa` → Select aura → **Actions Tab** → **Play Sound**
- Adjust **Volume** slider (0-100%)
- Or change to different sound file (some are louder)

---

### Issue: WeakAura Lagging Game

**Cause**: Too many auras updating every 0.1 sec.

**Fix**:

- Disable unused auras
- Change update frequency to 0.5 sec (see Optimization section)
- Delete old auras

---

## Pro Tips

1. **Test Before Raid**: Never import WeakAura and go straight to raid. Test on dummies.
2. **Share with Guild**: Export your custom WAs → Share import string in Discord.
3. **Backup WeakAuras**: `/wa` → Options → Export All → Save string to text file (if game crashes, reimport).
4. **Update Regularly**: Check Wago.io monthly for updated boss mechanic WAs.
5. **Don't Over-WA**: More WeakAuras ≠ better. 30-50 is optimal. 100+ = lag.

---

## Next Steps

After WeakAuras setup: → See **Min-Maxing Guide** for rotation and consumable optimization  
→ See **Addon Configuration** for DBM, threat meters, and UI setup  
→ See **In-Game Macros** for integration with WeakAuras (macro-triggered WAs)


