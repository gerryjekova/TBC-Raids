---
layout: guide
title: In-Game Macros & Templates
section: 6
next_section: /guides/weakauras/
next_title: WeakAuras Guide
---

# 9. WoW TBC In-Game Macros & Templates

## Table of Contents

1. [Raid Leader Macros](https://claude.ai/chat/44ef7b25-1d31-439c-91f7-05c868210582#raid-leader-macros)
2. [Class-Specific Raid Macros](https://claude.ai/chat/44ef7b25-1d31-439c-91f7-05c868210582#class-specific-raid-macros)
3. [Universal Utility Macros](https://claude.ai/chat/44ef7b25-1d31-439c-91f7-05c868210582#universal-utility-macros)
4. [Raid Warning Templates](https://claude.ai/chat/44ef7b25-1d31-439c-91f7-05c868210582#raid-warning-templates)
5. [Master Loot Macros](https://claude.ai/chat/44ef7b25-1d31-439c-91f7-05c868210582#master-loot-macros)
6. [Keybinding Recommendations](https://claude.ai/chat/44ef7b25-1d31-439c-91f7-05c868210582#keybinding-recommendations)

---

## Raid Leader Macros

### 🔴 Essential Raid Leader Macro Pack

#### Ready Check Macro

```
/readycheck
/rw === READY CHECK ===
/rw React when ready!
/rw Pull in 30 seconds
```

**Usage**: Before every boss pull. Ensures everyone is ready.

---

#### Buff Check Macro

```
/rw === BUFF CHECK ===
/rw Mark of the Wild - Druid
/rw Power Word: Fortitude - Priest
/rw Arcane Intellect - Mage
/rw Blessing of Kings - Paladin
/rw Blessing of Might - Paladin (Melee)
/rw Blessing of Wisdom - Paladin (Casters/Healers)
/rw Shadow Protection - Priest (if needed)
/p Check your buffs! Missing = whisper class name
```

**Usage**: After every wipe, before major pulls. Missing buffs = wipes.

---

#### Pull Timer Macro (Manual Countdown)

```
/rw === PULLING IN 10 SECONDS ===
/rw 10
/rw 9
/in 1 /rw 8
/in 2 /rw 7
/in 3 /rw 6
/in 4 /rw 5
/in 5 /rw 4
/in 6 /rw 3
/in 7 /rw 2
/in 8 /rw 1
/in 9 /rw PULL NOW - GO GO GO
```

**Note**: `/in` command requires DBM or BigWigs. Alternative: Use DBM pull timer `/dbm pull 10`

**Better Alternative**:

```
/dbm pull 10
/rw Pulling in 10 seconds - Get ready!
```

---

#### Bloodlust/Heroism Call Macro

```
/rw *** BLOODLUST / HEROISM NOW ***
/rw *** USE ALL COOLDOWNS ***
/p LUST LUST LUST
/y BLOODLUST NOW
```

**Usage**: Critical DPS burn phases (20-30% boss health, or specific mechanics).

---

#### Wipe Call Macro

```
/rw === WIPE IT ===
/rw Stop DPS - Let tanks die
/rw Don't release - Waiting for explanation
/p Wipe called - stop DPS
```

**Usage**: When pull is unrecoverable. Saves time vs slow wipe.

---

#### Break Macro

```
/rw === 10 MINUTE BREAK ===
/rw Bio, smokes, drinks - Be back at [TIME]
/rw AFK = Auto-kick from raid
/p 10 min break - back at [TIME]
```

**Usage**: After major bosses, or every 1.5 hours.

---

#### Loot Explanation Macro (Pre-Raid)

```
/rw === LOOT RULES ===
/rw MS > OS + 2 Soft Reserves
/rw Gargul handles all rolls automatically
/rw BoE items: Vote when they drop (roll/vendor/AH)
/rw Disputes: Open ticket AFTER raid, not during
/rw Questions? Ask now!
```

**Usage**: Every raid, before first pull. Prevents drama.

---

#### Raid Roster Macro (Check Composition)

```
#showtooltip
/script SendChatMessage("=== RAID COMPOSITION ===", "RAID_WARNING")
/script SendChatMessage("Tanks: "..UnitName("raid1")..", "..UnitName("raid2"), "RAID_WARNING")
/script SendChatMessage("Check roles - Missing any key buffs?", "RAID_WARNING")
```

**Note**: Basic version. For advanced, use RaidComp addon.

---

#### Mark Targets Macro (Skull/X/Moon)

```
/rw Kill Order: {Skull} > {X} > {Moon}
/rw Focus fire - No random switches
/script SetRaidTarget("target", 8)
```

**Usage**: Mark kill order for multi-target fights (Moroes adds, trash packs).

**Icons**:

- 1 = Yellow Star
- 2 = Orange Circle
- 3 = Purple Diamond
- 4 = Green Triangle
- 5 = White Moon
- 6 = Blue Square
- 7 = Red X
- 8 = White Skull

---

#### Emergency Heal Assignment Macro

```
/rw === HEALER DOWN ===
/rw [HEALER1] cover tanks
/rw [HEALER2] cover raid
/rw [HEALER3] cover both - Burn mana CDs
```

**Usage**: When a healer dies mid-fight. Quick reassignment.

---

#### Congratulations Macro (After Boss Kill)

```
/rw *** BOSS DOWN - GREAT JOB! ***
/rw Top DPS: [Name] - [DPS] DPS
/rw MVP Healer: [Name] - [HPS] HPS
/rw Break for loot - 3 minutes
/y BOSS DOWN!
/p Nice work everyone!
```

**Usage**: Morale boost after clean kills.

---

## Class-Specific Raid Macros

### Tanks

#### Main Tank Taunt Macro

```
#showtooltip Taunt
/stopcasting
/cast [@mouseover,harm,nodead] Taunt; Taunt
/y TAUNTING %t - STOP DPS
/s Taunting %t
```

**Why Mouseover**: Faster taunts in multi-target situations (doesn't change your target).

---

#### Tank Swap Announcement Macro

```
#showtooltip
/cast Taunt
/rw TAUNT SWAP - [OtherTank] I have aggro
/y SWAPPING
```

**Usage**: Boss fights requiring tank swaps (stacking debuffs).

---

#### Emergency Cooldown Macro (Warrior/Paladin)

```
#showtooltip Shield Wall
/cast Shield Wall
/use Super Healing Potion
/use Healthstone
/rw !!! SHIELD WALL USED - BIG HEALS NEEDED !!!
/y SHIELD WALL POPPED
```

**Usage**: "Oh shit" button when about to die.

---

#### Pull Announcement Macro

```
/rw Pulling in 3... 2... 1...
/y PULL
/startattack
```

**Usage**: Standardizes pulls, lets DPS prepare pre-casts.

---

### Healers

#### Innervate Whisper Macro (Druids)

```
#showtooltip Innervate
/cast [@mouseover,help,nodead] Innervate; Innervate
/w %t Innervate on you - 20 seconds of mana regen
/p Innervate used on %t
```

**Why Whisper**: Target knows to spam heals during Innervate window.

---

#### Dispel Macro (Mouseover)

```
#showtooltip Cleanse / Dispel Magic / Abolish Poison
/cast [@mouseover,help,nodead] Cleanse; Cleanse
```

**Usage**: Faster dispels without changing target (keep tank selected).

---

#### Battle Res Macro (Druids)

```
#showtooltip Rebirth
/cast [@mouseover,help,dead] Rebirth; Rebirth
/rw BATTLE REZ ON %t - Stay down until rez complete
/y REZ ON %t - DON'T RELEASE
```

**Usage**: Prevents people from releasing before rez lands.

---

#### Out of Mana Warning Macro

```
/rw OOM - Need Innervate or Mana Tide ASAP
/p OOM - Low mana
/script UIErrorsFrame:AddMessage("OUT OF MANA", 1.0, 0.0, 0.0, 1.0, UIERRORS_HOLD_TIME);
```

**Usage**: Alerts raid you can't sustain healing.

---

#### Mana Tide Totem Announcement (Shaman)

```
#showtooltip Mana Tide Totem
/cast Mana Tide Totem
/rw MANA TIDE DOWN - Casters/Healers get mana
/p Mana Tide active for 12 seconds
```

**Usage**: Lets healers/casters know to spam during window.

---

### DPS

#### Misdirect Macro (Hunters)

```
#showtooltip Misdirection
/cast [@focus,help,nodead] Misdirection; [@tank1] Misdirection
/p Misdirect on %t - Pulling in 3 sec
/in 3 /startattack
```

**Setup**: `/focus MainTankName` before raid.

---

#### Interrupt Announcement Macro

```
#showtooltip Kick / Counterspell / Earth Shock
/cast [@mouseover,harm,nodead] Kick; Kick
/p KICKED %t
/y INTERRUPT ON %t
```

**Usage**: Lets other interrupters know cooldown used (so they save theirs).

---

#### Soulstone Announcement Macro (Warlocks)

```
#showtooltip Soulstone
/cast [@mouseover,help,nodead] Soulstone; Soulstone
/w %t Soulstone on you - You can self-rez if you die
/rw Soulstone on %t (Healer) - Don't release if dead
```

**Usage**: Always Soulstone a healer before boss pulls.

---

#### Seed of Corruption AOE Spam Macro (Warlocks)

```
#showtooltip Seed of Corruption
/cast [@mouseover,harm,nodead] Seed of Corruption; Seed of Corruption
/cast Shadow Bolt
```

**Usage**: Fast Seed spam on imp packs (Illhoof), switches to Shadow Bolt on single target.

---

#### Bloodlust/Heroism Macro (Shamans)

```
#showtooltip Bloodlust
/cast Bloodlust
/rw *** BLOODLUST ACTIVE - 40 SECONDS ***
/rw *** USE ALL COOLDOWNS NOW ***
/y LUST IS UP - BURN BURN BURN
/script UIErrorsFrame:AddMessage("BLOODLUST ACTIVE", 1.0, 0.1, 0.1, 1.0, UIERRORS_HOLD_TIME);
```

**Usage**: Makes sure DPS notice and use their cooldowns.

---

#### Feign Death + Trap Macro (Hunters - CC)

```
#showtooltip Freezing Trap
/cast Feign Death
/cast [@mouseover,harm,nodead] Freezing Trap; Freezing Trap
/p Trap on %t - Don't break CC
```

**Usage**: Moroes adds, trash CC. Drops aggro + traps in one button.

---

#### Polymorph Announcement Macro (Mages)

```
#showtooltip Polymorph
/cast [@mouseover,harm,nodead] Polymorph; Polymorph
/rw SHEEP ON %t - DON'T BREAK CC
/p Poly on %t
```

**Usage**: Moroes adds, trash packs. Alerts raid not to AOE.

---

## Universal Utility Macros

### Target of Target Macro

```
/assist MainTankName
/startattack
```

**Usage**: Bind to a key. Always attacks what tank is targeting (prevents breaking CC).

---

### Mouseover Interact Macro (Chess Event, Netherspite Cubes)

```
/cast [@mouseover] Interact with Target
/click [btn:1]
```

**Usage**: Netherspite (click beams), Chess (click pieces), Magtheridon (click cubes).

---

### Consumable Use Macro (Emergency)

```
#showtooltip Super Healing Potion
/use Super Healing Potion
/use Healthstone
/use Master Healthstone
/script UIErrorsFrame:AddMessage("EMERGENCY HEAL USED", 0.0, 1.0, 0.0, 1.0, UIERRORS_HOLD_TIME);
```

**Usage**: "Oh shit" button. Uses potion + healthstone in one click (shares cooldown, but one will fire).

---

### Focus Target Macro (Set Main Tank)

```
/focus
/p %t set as focus target
```

**Usage**: Before raid, `/focus MainTankName`. Then all `[@focus]` macros work.

---

### Clear Focus Macro

```
/clearfocus
/p Focus target cleared
```

---

### Leave Group Macro (Post-Raid)

```
/rw Thanks for the run! Logs posted in Discord.
/p Good run everyone!
/y GG
/leave
```

**Usage**: Clean exit after raid ends.

---

## Raid Warning Templates (Copy-Paste into Chat)

### Boss Mechanic Callouts (Text Macros)

#### Shade of Aran - Flame Wreath

```
/rw *** FLAME WREATH - FREEZE ***
/rw DO NOT MOVE OR RAID WIPES
/in 5 /rw Wreath down - Move now
```

---

#### Prince Malchezaar - Infernals

```
/rw INFERNAL SPAWNED - KITE IT
/rw [OT Name] - Kite in circles, don't tank in place
```

---

#### Moroes - Garrote Warning

```
/rw GARROTE ON %t - DISPEL NOW
/rw Healers - Priority dispel
```

---

#### Curator - Evocation Warning

```
/rw EVOCATION IN 5 SECONDS
/rw SPREAD OUT - 15 YARDS
/in 5 /rw EVOCATION NOW - SPREAD
```

---

#### Illhoof - Demon Chains

```
/rw CHAINS ON %t
/rw BREAK CHAINS - ALL DPS SWITCH
```

---

## Master Loot Macros

### Gargul Soft Reserve Macros

#### Import Soft Reserves

```
/gargul softres import
```

**Usage**: Before raid, import CSV from SoftRes.it.

---

#### Check Soft Reserves

```
/gargul softres show
```

**Usage**: Verify reserves loaded correctly.

---

#### Manual Loot Award (Override)

```
/gargul assign [ItemLink] [PlayerName]
```

**Usage**: Force assign loot (mistakes, special cases).

---

#### Loot History

```
/gargul history
```

**Usage**: Check who won what (dispute resolution).

---

### Master Loot Announcement Macro

```
/rw [ItemLink] dropped!
/rw MS > OS roll - Type /roll 100 for Main Spec
/rw Type /roll 50 for Off Spec
```

**Usage**: If Gargul fails, manual fallback.

---

## Keybinding Recommendations

### Essential Keybinds (Priority)

**Movement** (Never rebind):

- W, A, S, D - Forward, Strafe Left, Back, Strafe Right
- Space - Jump
- Q, E - Turn (or rebind if using mouse-turn only)

**Action Bars** (High Priority):

- `1-5` - Main rotation abilities
- `Shift + 1-5` - Secondary rotation / cooldowns
- `F1-F5` - Emergency abilities (defensives, interrupts)
- `R, F, G, V, B` - Utility (mount, food, bandage, etc.)
- `Mouse Wheel Up/Down` - Common spells (healers: dispel/flash heal)
- `Middle Mouse Button` - Interrupt
- `Mouse Button 4/5` - Defensives or major cooldowns

**Raid Frames** (Healers):

- `Shift + Click` - Secondary heal
- `Ctrl + Click` - Dispel
- `Alt + Click` - Quick buff

**Targeting**:

- `Tab` - Cycle targets
- `Shift + Tab` - Cycle backwards
- `F` (if unbound) - Assist main tank
- `T` - Target of target

**Consumables**:

- `Z` - Healthstone
- `X` - Healing Potion
- `C` - Mana Potion

---

### Advanced Keybinds (For Pros)

**Camera** (If using mouse to turn):

- `Q, E` - Rebind to abilities (since you don't keyboard-turn)

**Mouseover Macros** (All healers/dispellers):

- Bind dispel to mouseover macro → Hover over raid frame, press key = instant dispel

**Focus Target Keybinds**:

- `Shift + F` - Set focus
- `Alt + F` - Target focus
- `Ctrl + F` - Clear focus

**Mark Targets**:

- `Numpad 1-8` - Raid markers (Skull, X, Moon, etc.)
- Quick marking for kill order

---

## Macro Character Limit Tips

**WoW Classic Macro Limit**: 255 characters per macro.

**How to Maximize**:

1. **Remove spaces after `/`**:
    
    - ❌ `/cast Taunt`
    - ✅ `/cast Taunt` (no extra spaces)
2. **Use short command versions**:
    
    - `/rw` instead of `/raid_warning`
    - `/p` instead of `/party`
    - `/y` instead of `/yell`
3. **Combine commands**:
    
    - ✅ `/cast Spell; Spell2` (one line)
    - ❌ `/cast Spell` + `/cast Spell2` (two lines)
4. **Remove flavor text**:
    
    - Keep callouts SHORT
    - "LUST NOW" beats "Bloodlust/Heroism is now active please use cooldowns"
5. **Use addons for complex macros**:
    
    - GSE (GnomeSequencer Enhanced) for rotation macros
    - OPie for radial menus (reduces keybind needs)

---

## Common Macro Errors & Fixes

### Error: "Unknown Unit"

**Problem**: Targeting macro fails.

**Fix**: Add `[@mouseover,harm,nodead]` or `[@focus,help,nodead]`

**Example**:

```
/cast [@mouseover,harm,nodead] Polymorph; Polymorph
```

---

### Error: "That ability is not ready yet"

**Problem**: Spamming macro triggers error messages.

**Fix**: Add at top:

```
/stopcasting
```

Or install "ErrorFilter" addon to hide spam.

---

### Error: "Invalid target"

**Problem**: Casting on wrong unit type (friendly vs hostile).

**Fix**: Use conditionals:

- `harm` = hostile
- `help` = friendly
- `nodead` = alive targets only
- `dead` = corpses (for battle res)

---

### Macro Not Firing

**Problem**: Clicking macro does nothing.

**Fix**: Check syntax. Common issues:

- Missing `#showtooltip` (icon doesn't appear)
- Misspelled spell name
- Space after `/` command

**Test**: Type `/cast SpellName` in chat first. If it works, copy exact spelling into macro.

---

## Addon-Enhanced Macros

### Require DBM/BigWigs

#### DBM Pull Timer (Better than manual countdown)

```
/dbm pull 10
```

**Result**: 10-second countdown with sound, visible to entire raid (if they have DBM).

---

#### BigWigs Timer

```
/bw pull 10
```

---

### Require OPie Addon

**OPie**: Radial menu addon. Reduces keybind clutter.

**Setup**:

- Install OPie
- Create ring: "Consumables"
- Bind ring to `Z` key
- Add: Healthstone, Potion, Food, Bandage
- Result: Press `Z`, mouse in direction of item, release = use

**Frees up** 4+ keybinds.

---

### Require WeakAuras

**WeakAuras** can trigger custom macros via `/run` commands (see WeakAuras guide for details).

---

## Raid Leader Saved Message Templates

### Create Custom Channel for Templates

**Setup**:

1. Join custom channel: `/join RaidTemplates`
2. Save messages in that channel (they persist between sessions)
3. Copy-paste from chat history into `/rw` as needed

**Example Messages to Save**:

```
=== BUFF CHECK === Mark of Wild, Fort, AI, Kings, Might, Wisdom, Shadow Prot
=== READY CHECK === Pulling in 30 seconds
=== LOOT RULES === MS > OS + 2 SR. Gargul handles rolls. BoE = vote.
Kill Order: {Skull} > {X} > {Moon}
```

**Usage**:

- `/join RaidTemplates`
- Scroll up in chat
- Copy-paste into `/rw`

---

## Pro Tips for Macro Management

1. **Name Macros Clearly**: "Tank-Taunt" not "Macro1"
2. **Use Icon Matching**: Set macro icon to match spell (easier to find on bars)
3. **Test in Duels**: Before raid, test all macros on target dummies or in duels
4. **Backup Macros**: Screenshot your macros (if game crashes, they're saved)
5. **Share with Raid**: Post useful macros in Discord #guides

---

## Essential AddOns for Macros to Work

- **DBM / BigWigs**: Required for `/dbm pull` and `/bw pull` commands
- **ErrorFilter**: Hides "ability not ready" spam when spamming macros
- **OPie**: Radial menus (reduces keybind needs)
- **Bartender4**: Better action bar management (more bars = more macro buttons)
- **Clique** (Healers): Click-cast healing (replaces many mouseover macros)

---

## Next Steps

After setting up macros: → See **WeakAuras Guide** for custom alerts and timers  
→ See **Min-Maxing Guide** for consumable optimization  
→ See **Addon Configuration** for detailed setup
