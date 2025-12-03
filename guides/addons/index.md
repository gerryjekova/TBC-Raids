---
layout: guide
title: Addon Configuration & UI Setup
section: 9
next_section: 
next_title: 
---

# 12. WoW TBC Addon Configuration & UI Setup

## Table of Contents

1. [Essential Addon Pack](https://claude.ai/chat/44ef7b25-1d31-439c-91f7-05c868210582#essential-addon-pack)
2. [DBM/BigWigs Configuration](https://claude.ai/chat/44ef7b25-1d31-439c-91f7-05c868210582#dbmbigwigs-configuration)
3. [Threat Meter Setup](https://claude.ai/chat/44ef7b25-1d31-439c-91f7-05c868210582#threat-meter-setup)
4. [Raid Frame Configuration](https://claude.ai/chat/44ef7b25-1d31-439c-91f7-05c868210582#raid-frame-configuration)
5. [UI Optimization](https://claude.ai/chat/44ef7b25-1d31-439c-91f7-05c868210582#ui-optimization)
6. [Performance Optimization](https://claude.ai/chat/44ef7b25-1d31-439c-91f7-05c868210582#performance-optimization)

---

## Essential Addon Pack

### 🔴 The Core 8 (Must Have)

**Download Priority Order**:

1. **WeakAuras 2** + **WeakAuras Companion**
    
    - Boss mechanics, cooldown tracking, buff/debuff alerts
    - **See**: WeakAuras Guide for full setup
2. **Deadly Boss Mods (DBM)** OR **BigWigs** + **LittleWigs**
    
    - Boss timers, warnings, audio alerts
    - **Pick ONE** (don't run both, causes conflicts)
3. **Details! Damage Meter** OR **Recount**
    
    - DPS/HPS tracking, combat analysis
    - **Details!** = Better (more features), **Recount** = Lighter (lower FPS impact)
4. **Omen Threat Meter** OR **ThreatClassic2**
    
    - Threat tracking (essential for tanks and DPS)
    - **Omen** = Standard, **TC2** = More accurate
5. **Bartender4** OR **Dominos**
    
    - Action bar replacement (better keybind management)
    - **Bartender4** = More customization, **Dominos** = Simpler
6. **Bagnon** OR **AdiBags**
    
    - Bag addon (all-in-one bag view, search function)
    - **Bagnon** = Simple, **AdiBags** = Auto-sorts by category
7. **Grid2** OR **Healbot** (Healers Only)
    
    - Raid frame replacement (better for healing)
    - **Grid2** = Lightweight + mouseover macros, **Healbot** = Click-healing
8. **Gargul**
    
    - Loot management (syncs with SoftRes.it)
    - **See**: Raid Organization Workflow

---

### 🟡 Quality-of-Life Addons (Highly Recommended)

9. **Prat** - Better chat (copy-paste, clickable links, timestamps)
10. **Mapster** - Better map (bigger, movable, coords)
11. **SavedInstances** - Track lockouts (which raids you've done this week)
12. **AtlasLootClassic** - Browse raid loot tables (see what drops where)
13. **ClassicCastbars** - Enemy cast bars (see what enemies are casting)
14. **Questie** - Quest helper (shows quest givers on map)
15. **Leatrix Plus** - QoL improvements (auto-repair, auto-sell gray, faster looting)

---

### 🟢 Advanced/Niche Addons

16. **Method Raid Tools (MRT)** - Raid notes, assignments, timers (Raid Leaders)
17. **OPie** - Radial menus (reduce keybind clutter)
18. **Clique** - Click-casting for healers (click raid frame = cast heal)
19. **TellMeWhen** - Alternative to WeakAuras (simpler, less powerful)
20. **Plater** - Nameplate addon (customize enemy/friendly nameplates)

---

## DBM/BigWigs Configuration

### Which to Choose?

**Deadly Boss Mods (DBM)**:

- **Pros**: More users (easier to share timers in Discord), more voice packs, simpler setup
- **Cons**: Slightly higher resource usage, can be "noisy" (lots of alerts)

**BigWigs**:

- **Pros**: Lighter (better FPS), more customizable, cleaner UI
- **Cons**: Smaller community, requires manual configuration

**Recommendation**: **DBM** for casual raiders (easier), **BigWigs** for hardcore (better performance).

---

### 🔴 DBM Setup (Step-by-Step)

#### Step 1: Install DBM-Core + Raid Modules

**Required**:

- **DBM-Core**: Main addon
- **DBM-TBC-BurningCrusade**: TBC raid modules (Karazhan, Gruul, Mag, SSC, TK, etc.)

**Optional**:

- **DBM-VPRapture**: Voice pack (English, female voice, clear warnings)
- **DBM-VPYike**: Alternative voice pack (male voice)

**Download**: CurseForge → Search "Deadly Boss Mods" → Install all

---

#### Step 2: First-Time Setup Wizard

1. Type `/dbm` to open interface
2. **Setup Wizard** should auto-launch (if not, click "Run Setup Wizard")
3. Follow prompts:
    - **Enable Boss Warnings**: Yes
    - **Enable Audio Warnings**: Yes (choose voice pack)
    - **Bar Style**: Choose "Default" (or "BigWigs" if you prefer that style)
    - **Positioning**: Bars appear at **top-center** (adjustable later)

---

#### Step 3: Configure Alerts (Most Important)

**Goal**: Make warnings **LOUD and OBVIOUS** (you can't miss mechanics).

**Settings to Change**:

1. `/dbm` → **Options Tab** → **Alerts**
    
2. **Special Warning Sound**:
    
    - **Default**: "RaidWarning" (loud horn)
    - **Alternative**: "AirHorn" (VERY loud, can't miss)
    - **Test**: Click "Test" button → Should hear sound
3. **Special Warning Font Size**:
    
    - **Default**: 30
    - **Recommended**: **48-60** (huge text, impossible to miss)
    - **Position**: Center-screen
4. **Flash Screen**:
    
    - **Enable**: "Flash screen on important warnings"
    - **Why**: Screen flashes red when you have Flame Wreath, etc.
5. **Timer Bar Size**:
    
    - **Default**: 20 height
    - **Recommended**: **25-30** height (easier to see)
    - **Width**: 200-250 (don't make too wide, blocks UI)

---

#### Step 4: Enable Auto-Respond Features

**What It Does**: DBM auto-responds to whispers during raids (e.g., "AFK, in raid").

**Setup**:

- `/dbm` → **Options Tab** → **Auto-Respond**
- **Enable**: "Auto-respond to whispers during boss fights"
- **Message**: "In raid, will reply after"

---

#### Step 5: Boss-Specific Configuration (Advanced)

**Example: Shade of Aran - Flame Wreath**

1. `/dbm` → **Boss Mods Tab** → **Karazhan** → **Shade of Aran**
2. Find **"Flame Wreath" timer**
3. **Right-click** → **Announce to Raid Warning** (so entire raid sees it)
4. **Right-click** → **Play Special Warning Sound**
5. **Right-click** → **Flash Screen**

**Result**: When Flame Wreath cast, screen flashes red + loud sound + giant text "FREEZE!".

**Repeat for all high-priority mechanics** (Garrote on Moroes, Infernals on Prince, etc.)

---

#### Step 6: Pull Timer Setup

**Usage**: `/dbm pull 10` = 10-second countdown with audio

**Enable Sound**:

- `/dbm` → **Options Tab** → **Announce**
- **Enable**: "Play countdown sound"
- **Voice**: Select voice pack (or use default beeps)

**Test**:

- `/dbm pull 5` → Should hear "5... 4... 3... 2... 1... PULL!"

---

### 🔴 BigWigs Setup (Alternative to DBM)

#### Step 1: Install BigWigs + Modules

**Required**:

- **BigWigs**: Core addon
- **BigWigs_TBC**: TBC raid modules
- **LittleWigs**: 5-man dungeon modules (heroics)

---

#### Step 2: First Launch

1. Type `/bw` or `/bigwigs`
2. **Profile Setup**: Create new profile (Name: "Raiding")
3. **Positioning**: Bars appear at **center-top** (drag to adjust)

---

#### Step 3: Configure Alerts

**Settings**:

- `/bw` → **Bars Tab**
    
    - **Bar Height**: 22-28
    - **Bar Width**: 200-250
    - **Font Size**: 14-16
- `/bw` → **Messages Tab**
    
    - **Enable**: "Emphasize important messages"
    - **Font Size**: 36-48 (huge)
- `/bw` → **Sounds Tab**
    
    - **Enable**: "Play sounds for important warnings"
    - **Volume**: 80-100%

---

#### Step 4: Test Alerts

- `/bw test` → Simulates boss warning
- Should see timer bar + hear sound

---

### Pull Timer (BigWigs)

**Usage**: `/bw pull 10` = 10-second countdown

---

## Threat Meter Setup

### Which to Choose?

**Omen Threat Meter**:

- **Pros**: Industry standard, most users have it (easy to share threat in Discord)
- **Cons**: Slightly higher resource usage

**ThreatClassic2**:

- **Pros**: More accurate threat calculations, lighter
- **Cons**: Smaller user base

**Recommendation**: **Omen** (everyone uses it, easier to troubleshoot).

---

### 🔴 Omen Setup

#### Step 1: Install

**CurseForge** → Search "Omen Threat Meter" → Install

---

#### Step 2: Configure Display

1. Type `/omen` → Opens threat window
2. **Resize**: Drag corners to make bigger (recommended: 250x150 pixels)
3. **Position**: Place near center-bottom (easy to glance at)
4. **Lock**: Right-click title bar → "Lock Window"

---

#### Step 3: Enable Warnings

**Goal**: Alert you BEFORE you pull aggro.

**Settings**:

- Right-click Omen title bar → **Options**
- **Warning Tab**:
    - **Enable**: "Play sound when threat is high"
    - **Threshold**: 90% (warns at 90% of tank's threat)
    - **Sound**: "Raid Warning" (loud)

**Test**: Attack target dummy → Threat should build → Warning should sound at 90%.

---

#### Step 4: Configure for Role

**DPS**:

- **Display**: Show "Your threat" + "Tank threat" (2 bars)
- **Auto-hide**: Enable "Hide when not in combat"

**Tanks**:

- **Display**: Show "Top 3 threats" (see who's closest to pulling)
- **Color Code**: Red = about to pull, Yellow = close, Green = safe

**Healers**:

- **Display**: Show "Your threat" only (healers don't pull aggro often, minimize clutter)

---

### Threat Management Tips

**For DPS**:

- If threat bar turns **YELLOW** (80-90% of tank): **Slow down** (stop attacking for 1-2 GCDs)
- If threat bar turns **RED** (95%+ of tank): **STOP immediately** (or you pull aggro)
- Use threat reduction abilities:
    - Rogues: Feint (reduces threat by 50%)
    - Mages: Invisibility (drops all threat)
    - Hunters: Feign Death (drops all threat)

**For Tanks**:

- If DPS in red (about to pull): **Call it out** in voice: "Slow DPS on [Name]"
- Use threat generators:
    - Warriors: Devastate, Revenge (high threat)
    - Druids: Maul, Swipe (high threat)
    - Paladins: Consecration, Holy Shield (AOE threat)

---

## Raid Frame Configuration

### Default UI vs Addons

**Default Blizzard Raid Frames** (TBC):

- **Pros**: Lightweight, no addon required
- **Cons**: Limited customization, hard to see debuffs, no mouseover support

**Grid2 / Healbot** (Addons):

- **Pros**: Fully customizable, shows debuffs clearly, mouseover support
- **Cons**: Requires setup time, slight FPS impact

**Recommendation**: **Grid2** (all roles), **Healbot** (healers who prefer click-healing).

---

### 🔴 Grid2 Setup (For Healers and All Roles)

#### Step 1: Install

**CurseForge** → Search "Grid2" → Install

---

#### Step 2: First Launch

1. Type `/grid2` → Opens config
2. **Profile**: Create new profile (Name: "Raiding")

---

#### Step 3: Configure Frame Size & Position

**Settings**:

- `/grid2` → **Frame Tab** → **Size**
    - **Width**: 60-80 pixels
    - **Height**: 40-50 pixels
    - **Orientation**: "Vertical" (stacks downward)

**Position**:

- Drag Grid2 frames to **bottom-left** or **bottom-right** of screen
- Lock position: Right-click → "Lock Frames"

---

#### Step 4: Configure Buff/Debuff Display

**Goal**: See dispellable debuffs clearly (Garrote, Holy Fire, etc.).

**Settings**:

- `/grid2` → **Indicators Tab** → **Center Icon**
    - **Enable**: "Show debuffs"
    - **Priority**: Curse → Poison → Disease → Magic → Bleed
    - **Size**: 24-32 pixels (big enough to see clearly)

**Color Code Debuffs**:

- **Red**: Bleed (Garrote)
- **Green**: Poison
- **Purple**: Curse
- **Blue**: Magic (Holy Fire)
- **Brown**: Disease

---

#### Step 5: Configure Health Deficit

**What It Does**: Shows how much HP someone is missing (easier to prioritize heals).

**Settings**:

- `/grid2` → **Indicators Tab** → **Text**
    - **Enable**: "Show health deficit"
    - **Format**: "-5432" (negative number = HP missing)
    - **Position**: Center of frame

**Why**: See "-8000" on tank = big heal needed. See "-200" on DPS = ignore for now.

---

#### Step 6: Enable Mouseover Support

**What It Does**: Hover mouse over raid frame → Target that player (for mouseover macros).

**Settings**:

- `/grid2` → **Frame Tab** → **Mouseover**
    - **Enable**: "Highlight on mouseover"
    - **Highlight color**: Yellow (stands out)

**Combine with Mouseover Macros** (See Macro Guide):

```
#showtooltip Flash Heal
/cast [@mouseover,help,nodead] Flash Heal; Flash Heal
```

**Result**: Hover over raid frame → Press keybind → Instant heal (no clicking needed).

---

### 🟡 Healbot Setup (Alternative - Click-Healing)

#### What Is Healbot?

**Healbot** = Raid frames + click-to-heal in one addon.

**Example**:

- Left-click raid frame = Flash Heal
- Right-click raid frame = Renew
- Middle-click = Dispel

**Why**: No macros needed. Just click.

---

#### Setup

1. Install **Healbot**
    
2. Type `/hb` → Opens config
    
3. **Spells Tab**:
    
    - **Left-click**: Assign to your main heal (Flash Heal, Healing Wave, etc.)
    - **Right-click**: Assign to HoT or quick heal (Renew, Rejuvenation, etc.)
    - **Ctrl+Click**: Assign to dispel (Cleanse, Dispel Magic, etc.)
4. **Frames Tab**:
    
    - **Size**: 60x40 pixels
    - **Position**: Bottom-left
    - **Sort**: By group (keeps groups together)

---

### Raid Frame Comparison

|Feature|Default UI|Grid2|Healbot|
|---|---|---|---|
|Setup Time|0 min|15 min|10 min|
|Customization|Low|High|Medium|
|Mouseover Support|No|Yes|N/A (click-cast)|
|FPS Impact|0|Low|Medium|
|Best For|Minimal raiders|All roles|Healers only|

---

## UI Optimization

### 🔴 The "Clear Screen" Principle

**Goal**: 70% of screen should be clear (see mechanics). UI should take <30%.

---

### Screen Layout (Recommended)

```
[TOP-CENTER]
- DBM/BigWigs timers (200px wide)
- WeakAuras boss mechanic alerts

[TOP-LEFT]
- Minimap (shrink to 120x120)

[TOP-RIGHT]
- Buff/Debuff tracker (WeakAuras)

[CENTER-SCREEN]
- CLEAR (your character visible, see mechanics)

[BOTTOM-LEFT]
- Raid frames (Grid2, 300x400 area)

[BOTTOM-CENTER]
- Action bars (Bartender4, 3 rows max)
- Castbar (player + target)

[BOTTOM-RIGHT]
- Threat meter (Omen, 250x150)
- Details! meter (250x150, below threat)

[CHAT]
- Bottom-left corner (transparent background)
```

---

### 🔴 Action Bar Setup (Bartender4)

#### Step 1: Install Bartender4

**CurseForge** → "Bartender4" → Install

---

#### Step 2: Reduce Bar Count

**Default**: 7+ action bars visible (clutters screen).

**Optimal**: 3-4 action bars visible.

**Settings**:

- `/bart` → **Bar 1**: Enable (main rotation)
- `/bart` → **Bar 2**: Enable (cooldowns)
- `/bart` → **Bar 3**: Enable (consumables/utility)
- `/bart` → **Bar 4-7**: **Disable** (hide, or use for keybinds only with no visible buttons)

---

#### Step 3: Position Bars

**Layout**:

- **Bar 1**: Bottom-center (12 buttons, horizontal)
- **Bar 2**: Above Bar 1 (12 buttons, horizontal)
- **Bar 3**: Right side (6-12 buttons, vertical)

**Lock Bars**: `/bart` → **Options** → "Lock Bars"

---

#### Step 4: Keybind All Abilities

**Rule**: If ability is used in combat = MUST be keybound (no clicking).

**Keybind Method**:

- `/bart` → **Keybindings Tab**
- Hover over action bar slot → Press key → Ability assigned

**Optimal Keybinds** (See Macro Guide for details).

---

### 🔴 Bag Addon (Bagnon)

#### Setup

1. Install **Bagnon**
2. Type `/bagnon` → Auto-opens config
3. **Settings**:
    - **Enable**: "All-in-one bag" (combines all bags into one window)
    - **Enable**: "Search" (search items by name)
    - **Enable**: "Auto-vendor gray items"

**Result**: Press `B` → See all bags in one window. Type "potion" in search → Highlights potions.

---

### 🟡 Minimap (Mapster)

#### Setup

1. Install **Mapster**
2. Type `/mapster`
3. **Settings**:
    - **Scale**: 0.8-0.9 (shrink minimap)
    - **Position**: Top-left (out of way)
    - **Hide**: Calendar button, zoom buttons (clean UI)

---

## Performance Optimization

### 🔴 FPS Optimization (Low-End PCs)

**Goal**: 60+ FPS in 25-man raids.

---

### In-Game Graphics Settings

**Settings to Lower**:

1. **View Distance**: Medium or Low (biggest FPS gain)
2. **Environment Detail**: Low
3. **Texture Resolution**: Medium (Low looks bad)
4. **Particle Density**: Low (reduces spell effect clutter)
5. **Shadow Quality**: Off (10-15 FPS gain)
6. **Weather Effects**: Minimal

**Settings to Keep High**:

- **Texture Filtering**: 16x (no FPS cost, looks better)
- **Resolution**: Native (don't lower, looks blurry)

---

### Addon Optimizations

1. **Disable Combat Log** (in combat):
    
    - Type: `/console maxfps 60` (caps FPS at 60, reduces CPU)
    - Type: `/console cameraDistanceMaxZoomFactor 2.6` (zoom out more, see mechanics better)
2. **Reduce Details! Refresh Rate**:
    
    - Details! → Options → "Update frequency" → 0.5 sec (default is 0.1 sec = CPU heavy)
3. **Disable Unused WeakAuras**:
    
    - `/wa` → Disable all auras for bosses you're not fighting tonight
4. **Disable Prat/Chat Addons**:
    
    - In combat, chat addons = FPS loss. Disable if FPS <40.

---

### Weak PC Emergency Settings

**If FPS <30 in 25-man**:

1. Disable Details! (use lightweight Recount instead)
2. Disable WeakAuras (use TellMeWhen instead)
3. Lower texture resolution to Low
4. Turn off ALL shadows
5. Disable weather effects

**Result**: Gain 10-20 FPS, but UI less informative.

---

## Addon Configuration Checklist

### Print & Use (Physical Checklist)

```
===== ADDON SETUP CHECKLIST =====

CORE ADDONS (Must Install):
[ ] WeakAuras 2 + Companion
[ ] DBM-Core + TBC module (or BigWigs)
[ ] Details! (or Recount)
[ ] Omen Threat Meter
[ ] Bartender4
[ ] Bagnon
[ ] Grid2 (or Healbot if healer)
[ ] Gargul

DBM CONFIGURATION:
[ ] Voice pack installed (DBM-VPRapture)
[ ] Special warning font size: 48+
[ ] Flash screen on important warnings: ON
[ ] Pull timer tested (/dbm pull 5)
[ ] Boss mods enabled for tonight's raid

THREAT METER:
[ ] Omen installed and visible
[ ] Warning sound enabled at 90% threat
[ ] Position: center-bottom (easy to glance)
[ ] Test: Attack dummy, see threat build

RAID FRAMES:
[ ] Grid2 installed and configured
[ ] Frame size: 60x40 pixels
[ ] Debuff display enabled (center icon)
[ ] Position: bottom-left (healers)
[ ] Mouseover highlighting enabled

UI OPTIMIZATION:
[ ] Bartender4: 3 action bars visible (not 7)
[ ] All abilities keybound (no clicking)
[ ] Minimap shrunk to 120x120 (Mapster)
[ ] Bags combined (Bagnon all-in-one)
[ ] Center-screen CLEAR (70% visibility)

PERFORMANCE CHECK:
[ ] FPS test in 25-man: 40+ FPS?
[ ] If <40: Disable Details!, lower shadows
[ ] Disable unused WeakAuras
[ ] Combat log off (/console maxfps 60)

FINAL TEST:
[ ] /dbm test → See warnings + hear sound?
[ ] /wa → Test boss auras for tonight?
[ ] Omen visible + threat tracking?
[ ] All keybinds working?
[ ] FPS stable (no lag spikes)?

===================================
```

---

## Common Addon Issues & Fixes

### Issue: DBM Not Showing Timers

**Cause**: Boss module not installed or disabled.

**Fix**:

- Type `/dbm` → **Boss Mods Tab**
- Find raid (e.g., Karazhan)
- Ensure **all bosses are enabled** (green checkmarks)
- Reinstall "DBM-TBC-BurningCrusade" module if missing

---

### Issue: Omen Not Tracking Threat

**Cause**: Omen disabled or other players don't have Omen.

**Fix**:

- Type `/omen` → **Options** → Ensure "Enable Omen" is checked
- Ask raid: "Everyone install Omen Threat Meter" (needs 2+ users to sync threat)

---

### Issue: Grid2 Not Showing Debuffs

**Cause**: Debuff indicator not configured.

**Fix**:

- `/grid2` → **Indicators Tab** → **Center Icon**
- **Enable**: "Show debuffs"
- Test: Get poisoned → Should see green icon on your Grid2 frame

---

### Issue: Bartender4 Keybinds Not Working

**Cause**: Keybinds bound to wrong bar.

**Fix**:

- `/bart` → **Keybindings Tab**
- Verify keybinds match action bar slots
- Test: Press keybind → Ability should activate

---

### Issue: WeakAuras Causing FPS Lag

**Cause**: Too many auras updating every 0.1 sec.

**Fix**:

- `/wa` → Disable unused auras (only enable for tonight's bosses)
- Change update frequency to 0.5 sec (see WeakAuras Guide)

---

## Next Steps

After addon setup: → Test in a dungeon or LFR (practice before real raid)  
→ Screenshot your UI → Share in Discord for feedback  
→ Adjust based on personal preference (no "perfect" UI, find what works for you)

**Remember**: UI is personal. Copy pro setups as a starting point, then customize to your needs!