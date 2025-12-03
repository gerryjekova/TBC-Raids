---
layout: guide
title: Min-Maxing Complete Guide
section: 8
next_section: /guides/addons/
next_title: Addon Configuration
---

# 11. # WoW TBC Min-Maxing Complete Guide

## Table of Contents

1. [Pre-Raid Preparation](https://claude.ai/chat/44ef7b25-1d31-439c-91f7-05c868210582#pre-raid-preparation)
2. [Consumable Optimization](https://claude.ai/chat/44ef7b25-1d31-439c-91f7-05c868210582#consumable-optimization)
3. [Rotation & DPS Optimization](https://claude.ai/chat/44ef7b25-1d31-439c-91f7-05c868210582#rotation--dps-optimization)
4. [Gear Optimization](https://claude.ai/chat/44ef7b25-1d31-439c-91f7-05c868210582#gear-optimization)
5. [Profession Min-Maxing](https://claude.ai/chat/44ef7b25-1d31-439c-91f7-05c868210582#profession-min-maxing)
6. [Raid Preparation Checklist](https://claude.ai/chat/44ef7b25-1d31-439c-91f7-05c868210582#raid-preparation-checklist)
7. [Gold Farming for Consumables](https://claude.ai/chat/44ef7b25-1d31-439c-91f7-05c868210582#gold-farming-for-consumables)

---

## Pre-Raid Preparation

### The 48-Hour Rule

**Optimal raiders prep 48 hours before raid, not 5 minutes before.**

---

### 🔴 48 Hours Before Raid

#### Check BiS List & Missing Gear

1. Go to **Wowhead TBC** or **Seventyupgrades.com**
2. Look up your spec's Phase 1 BiS list
3. Compare to your current gear: `/script for i=1,18 do print(GetInventoryItemLink("player",i) or "Empty: "..i) end`
4. Identify weakest slots (lowest ilvl, missing enchants, empty sockets)

**Priority Slots** (Biggest Stat Impact):

- Weapon (highest DPS contribution for DPS/Tanks)
- Trinkets (proc effects = huge DPS/HPS/survivability)
- Tier set pieces (set bonuses = 10-15% performance boost)

---

#### Farm Missing Enchants & Gems

**Goal**: Every slot enchanted, every socket filled.

**Quick Check**: Inspect yourself → If any slot has yellow text (missing enchant) or empty socket (gray socket) = fix immediately.

**Where to Get**:

- **Enchants**: Auction House (expensive but instant) OR Enchanter friend (bring mats)
- **Gems**: Jewelcrafter (VERY expensive in TBC, budget 50-100g per epic gem)

**Priority Enchants** (Don't skip these):

**Tanks**:

- Weapon: Mongoose (+120 Agility proc, +25 Agility static) - 300-500g
- Chest: Exceptional Health (+150 HP) - 50g
- Gloves: Threat (Feral Druids) or Crushing (Warriors) - 20-40g

**Healers**:

- Weapon: Major Healing (+81 healing) - 100-200g
- Chest: Exceptional Stats (+6 all stats) - 80g
- Rings: Healing Power (+20 healing per ring) - Enchanters only

**DPS**:

- Weapon (Melee): Mongoose or Executioner (+120 AP proc) - 300-500g
- Weapon (Caster): Soulfrost (+54 Shadow/Frost) or Sunfire (+50 Arcane/Fire) - 200-300g
- Gloves: Assault (+26 AP) or Spell Strike (+15 spell damage) - 30-50g
- Boots: Cat's Swiftness (+6 Agility + move speed) or Boar's Speed (+9 Stam + move speed) - 80-120g

---

#### Stock Up on Consumables

**48-Hour Advance**: Buy when prices LOW (Wednesday/Thursday). Avoid buying Sunday night (prices spike 30-50%).

**Budget**: 100-200g per raid night (full flask setup).

**Shopping List** (Copy-paste into notepad):

```
CONSUMABLES FOR RAID - [Your Name]

MANDATORY:
[ ] Flask of [Your Type] x1 (2 hours, 50-100g)
    OR
[ ] Battle Elixir x2 (1 hour each, 20-40g total)
[ ] Guardian Elixir x2 (1 hour each, 20-40g total)
[ ] Food Buff x10 (30min each, 20-50g total)
[ ] Super Healing Potion x10 (10-20g total)
[ ] Super Mana Potion x10 (Casters/Healers, 20-30g total)

HIGHLY RECOMMENDED:
[ ] Scroll of Agility/Strength/Intellect V x5 (20 stat, 10-20g total)
[ ] Wizard Oil / Weightstone x2 (1 hour weapon buff, 30-50g total)
[ ] Drums of Battle (Leatherworkers, 5-10g per drum, bring 5)

OPTIONAL:
[ ] Haste Potion x2 (DPS burst, 5-10g)
[ ] Destruction Potion x2 (Caster burst, 5-10g)
[ ] Dense Weightstone / Sharpening Stone (backup weapon buff, 5g)
```

---

### 🔴 24 Hours Before Raid

#### Repair & Bag Space

- **100% Repair**: Find repair NPC, repair all (costs 5-15g)
- **Empty Bags**: Minimum 10 slots free (for loot)
- **Bank Clutter**: Mail non-essential items to bank alt

---

#### Practice Rotation on Target Dummy

**Location**: Ironforge (Alliance) or Orgrimmar (Horde) - Near AH

**Goals**:

- 5 minutes on dummy
- Track DPS with Recount/Details
- Compare to sim DPS (see Rotation Optimization section)
- Practice opener (first 10 seconds = 20% of total DPS)

**Keybind Check**: Make sure all abilities are keybound (no clicking).

---

#### WeakAuras & Addon Check

- Update all addons (CurseForge app → Update All)
- `/dbm test` → Verify DBM works (timers + sound)
- `/wa` → Test WeakAuras for tonight's bosses
- Threat meter working? (Omen or ThreatClassic2)

---

### 🔴 1 Hour Before Raid

#### Log In Early & Buff

- **Location**: Be at raid entrance (or major city for summons)
- **Apply all buffs**:
    - Flask (or elixirs)
    - Food buff
    - Scroll buff
    - Weapon buff (oil/stone)
- **Summons**: Type "sum" in guild/raid chat if Warlock summons available

---

#### Discord Check

- Join voice channel 10 minutes early
- Test mic: "Mic check, can you hear me?"
- Set Push-to-Talk keybind (if not already)
- Mute Discord notifications (right-click server → Notification Settings → Suppress @everyone)

---

## Consumable Optimization

### 🔴 The Flask vs Elixir Decision

**Flasks**:

- **Pro**: Persists through death (keep buff even if you wipe)
- **Pro**: Lasts 2 hours (entire Kara run)
- **Con**: EXPENSIVE (50-100g per flask in TBC)

**Elixirs**:

- **Pro**: CHEAP (20-40g for full night)
- **Con**: Lost on death (must rebuff after wipes)
- **Con**: Lasts 1 hour (need 2-3 per raid)

**When to Flask**:

- Progression raids (many wipes expected)
- 25-man raids (deaths common)
- You're rich (200+ gold to spare)

**When to Elixir**:

- Farm content (Kara on repeat, few wipes)
- Gold-poor (<100g total)
- Your guild provides flasks

---

### 🔴 Best Consumables by Role

#### Tanks

**FLASK**:

- **Flask of Fortification**: +500 HP, +10 Defense Rating (70-100g)
    - **Best for**: Warriors, Paladins
    - **Why**: Survivability > everything for tanks

**OR ELIXIRS**:

- **Battle**: Elixir of Major Defense (+550 Armor, 15-25g)
- **Guardian**: Elixir of Major Fortitude (+250 HP, 10-20g)

**FOOD**:

- **Fisherman's Feast**: +30 Stamina, +20 Spirit (5-10g per)
    - **Why**: Stamina = bigger HP pool = fewer one-shots

**POTIONS**:

- **Super Healing Potion** x10 (2-3g per)
- **Ironshield Potion** x5 (+2500 Armor for 2 min, emergency, 5-10g per)

**WEAPON BUFF**:

- **Adamantite Weightstone**: +12 Weapon Damage, +14 Crit (Melee tanks, 3-5g)

**SCROLLS**:

- **Scroll of Protection V**: +300 Armor (stackable with elixir, 2-3g)

**BONUS** (Rich Tanks):

- **Elixir of Ironskin**: +30 Resilience (PvP stat, reduces crit chance on you, 10-15g)

---

#### Healers

**FLASK**:

- **Flask of Mighty Restoration**: +25 MP5 (mana per 5 seconds, 60-90g)
    - **Why**: Mana regen = never OOM = sustained healing

**OR ELIXIRS**:

- **Battle**: Elixir of Draenic Wisdom (+30 Int, +30 Spirit, 15-25g)
- **Guardian**: Elixir of Major Mageblood (+16 MP5, 10-20g)

**FOOD**:

- **Skullfish Soup**: +23 Healing, +20 Spirit (5-10g per)
    - **Best for**: Resto Shaman, Holy Priest
- **Blackened Basilisk**: +23 Spell Damage, +20 Spirit (Disc Priest, Holy Paladin)

**POTIONS**:

- **Super Mana Potion** x10 (3-5g per)
- **Dark Rune** x5 (instant 1200 mana, NO cooldown share with potions, 5-10g per)

**WEAPON BUFF**:

- **Brilliant Wizard Oil**: +36 Spell Damage, +14 Spell Crit (10-15g)

**SCROLLS**:

- **Scroll of Spirit V**: +20 Spirit (2-3g)

**BONUS** (Rich Healers):

- **Mana Potion Injector** (Engineering): Instant mana potion, 2min CD (separate from potion CD)

---

#### DPS (Melee)

**FLASK**:

- **Flask of Relentless Assault**: +120 Attack Power (60-90g)
    - **Why**: Pure DPS increase

**OR ELIXIRS**:

- **Battle**: Elixir of Major Agility (+35 Agility, 15-25g) OR Elixir of Major Strength (+35 Strength, 15-25g)
- **Guardian**: Elixir of Major Fortitude (+250 HP, 10-20g)

**FOOD**:

- **Grilled Mudfish**: +20 Agility, +20 Spirit (5-10g per)
    - **Best for**: Rogues, Hunters, Feral Druids

**POTIONS**:

- **Haste Potion** x2 (Melee/Ranged haste burst, 3-5g per)
- **Insane Strength Potion** x2 (+120 Strength for 15sec, 5-10g per)

**WEAPON BUFF**:

- **Adamantite Weightstone**: +12 Weapon Damage, +14 Crit (3-5g)
- **Adamantite Sharpening Stone**: +12 Weapon Damage, +14 Crit (3-5g)

**SCROLLS**:

- **Scroll of Agility V**: +20 Agility (2-3g) OR **Scroll of Strength V**: +20 Strength (2-3g)

**BONUS** (Rich DPS):

- **Drums of Battle**: +80 Haste to party for 30sec, 2min CD (Leatherworkers only, 10-15g per)
    - **Critical**: 1 Leatherworker per 5-man group with drums = 5% DPS increase raid-wide

---

#### DPS (Caster)

**FLASK**:

- **Flask of Pure Death**: +80 Spell Damage (Fire/Shadow, 60-90g)
- **Flask of Blinding Light**: +80 Spell Damage (Arcane/Holy, 60-90g)

**OR ELIXIRS**:

- **Battle**: Elixir of Major Firepower (+55 Fire Damage, 15-25g) OR Elixir of Major Shadow Power (+55 Shadow, 15-25g)
- **Guardian**: Elixir of Draenic Wisdom (+30 Int, +30 Spirit, 15-25g)

**FOOD**:

- **Blackened Basilisk**: +23 Spell Damage, +20 Spirit (5-10g per)
    - **Best for**: All casters

**POTIONS**:

- **Super Mana Potion** x10 (3-5g per)
- **Destruction Potion** x2 (+120 Spell Damage for 15sec, burst phase, 5-10g per)

**WEAPON BUFF**:

- **Brilliant Wizard Oil**: +36 Spell Damage, +14 Spell Crit (10-15g)
- **Superior Wizard Oil**: +42 Spell Damage (slightly better, 15-20g)

**SCROLLS**:

- **Scroll of Intellect V**: +20 Intellect (2-3g)

**BONUS** (Rich Casters):

- **Mana Emerald** (Jewelcrafter): Instant 2400 mana, no CD (10-15g per, can use multiple)

---

### 🟡 Niche Consumables (Situational)

#### Shadow Resistance (Magtheridon)

- **Shadow Protection Potion**: +1950 Shadow Resist for 2 min (15-25g per)
- **Elixir of Shadow Fortification**: +40 Shadow Resist (10-15g)
- **Shadow Cloak** (Tailoring): Enchant cloak +15 Shadow Resist (20-30g)

**When to Use**: Magtheridon's Blast Nova = massive shadow damage. Shadow resist = 30-40% less damage taken.

---

#### Fire Resistance (Gruul's Lair - Optional)

- **Fire Protection Potion**: +1950 Fire Resist for 2 min (10-15g per)
- **Flame Mantle of the Dawn** (Argent Dawn exalted): Shoulder enchant +5 Fire Resist

**When to Use**: Gruul's Ground Slam = fire damage. Minimal benefit (not required).

---

#### Underwater Breathing (SSC/Vashj - Phase 2 Content)

- **Elixir of Water Breathing**: 1 hour underwater (1-2g)
- **Shiny Fish Scales** (Fisherman): 1 hour underwater (free if you fish)

---

## Rotation & DPS Optimization

### 🔴 Universal DPS Principles (All Classes)

#### 1. ABC: Always Be Casting

**Never stand idle.** If main spell on cooldown, cast filler (Shadow Bolt for Warlocks, Steady Shot for Hunters).

**Goal**: 0% downtime. Track with Recount → "Time spent casting" should be 90%+.

---

#### 2. Opener = 20% of Total DPS

**First 10 seconds** = pre-pot + all cooldowns + Bloodlust window.

**Standard Opener** (Most Classes):

1. **Pre-pot** (5 seconds before pull): Destruction Potion (casters) or Haste Potion (melee)
2. **Pull countdown**: Get in position, start pre-cast (2sec before pull)
3. **On pull**: Cast biggest nuke (Shadowbolt, Aimed Shot, Frostbolt)
4. **Pop all cooldowns**: Trinkets, racial, class CDs (Bloodfury, Combustion, Arcane Power)
5. **Continue rotation**: Don't waste GCDs

**Why**: All CDs up at start + Bloodlust/Heroism active + Pre-pot buff = 30-40% DPS spike.

---

#### 3. Cooldown Tracking

**Major DPS cooldowns** should be used on cooldown (unless saving for specific phase).

**Examples**:

- **Warlocks**: Soul Fire (cooldown-based nuke, use on CD)
- **Mages**: Combustion (5min CD, use with boss CDs or Bloodlust)
- **Hunters**: Rapid Fire (5min CD, use on pull + during Bloodlust)
- **Rogues**: Blade Flurry (AOE CD, use on multi-target packs)

**Track with**: WeakAuras cooldown tracker.

---

#### 4. Don't Cap Resources

**Energy** (Rogues): Don't sit at 100 energy (wasted regen). Spend at 80-90.

**Mana** (Casters): Don't OOM too early. Track MP5 (Mana per 5 seconds). If going OOM before 50% boss health = not enough Spirit/MP5 gear.

**Rage** (Warriors/Druids): Don't cap at 100 rage (wasted generation). Spam Heroic Strike (Warriors) or Maul (Druids) to dump excess.

---

### 🔴 Class-Specific Rotation Optimization

#### Warlock (Destruction - Raid Spec)

**Pre-Pull**:

- Life Tap to ~50% HP (max mana)
- Apply Healthstone to hotbar
- Summon Imp or Succubus (Imp for bosses, Succubus for trash)

**Opener** (Single Target):

1. Pre-pot: Destruction Potion (5sec before pull)
2. Pre-cast: Shadow Bolt (2sec before pull)
3. Curse of Recklessness (or Curse of Doom if allowed)
4. Immolate
5. Shadow Bolt spam until Nightfall proc
6. When Nightfall procs: Instant Shadow Bolt
7. Continue Shadow Bolt spam

**Cooldowns**:

- Use on pull: Bloodfury (Orc racial, +AP/Spell Damage)

**AOE Rotation** (Trash/Imps):

1. Seed of Corruption on target (explodes at 1044 damage)
2. Tab to next target, Seed again
3. Wait for explosions (chain reaction)

**Mana Management**:

- Life Tap when mana <30%
- Drain Life if HP <50% (regen HP + mana)

---

#### Mage (Frost - Early TBC, Fire Later)

**Pre-Pull**:

- Evocation ready (no CD)
- Icy Veins ready (3min CD, save for pull)

**Opener** (Single Target):

1. Pre-pot: Destruction Potion
2. Pre-cast: Frostbolt (2sec before pull)
3. Icy Veins (3min CD, use immediately)
4. Frostbolt spam
5. When Water Elemental ready: Summon + command attack
6. Frostbolt spam (repeat)

**Cooldowns**:

- **Combustion** (Fire spec): Use when you have 3 crit stacks (WeakAura tracks this)

**Mana Management**:

- Evocate at 20-30% mana (channels for 8 sec, full mana)
- Mana Gem: Use on CD (instant 1200+ mana)

**AOE**:

- Blizzard on 3+ targets (channel, huge AOE damage)

---

#### Hunter (Beast Mastery - TBC Standard)

**Pre-Pull**:

- Pet on passive (don't auto-attack yet)
- Aspect of the Hawk active

**Opener**:

1. Pre-pot: Haste Potion (5sec before pull)
2. Misdirect on tank (3sec before pull)
3. Send pet to attack (1sec before pull)
4. Auto-shot + Steady Shot macro (shot weaving)
5. Kill Command (pet special, use on CD)
6. Steady Shot spam (between auto-shots)

**Shot Weaving** (Critical for Hunters):

- **Goal**: Cast Steady Shot BETWEEN auto-shots (not during)
- **How**: WeakAura "Hunter Shot Timer" shows when to cast Steady
- **Result**: 20-30% DPS increase over bad timing

**Cooldowns**:

- **Rapid Fire**: 5min CD, use on pull (40% haste for 15sec)
- **Bestial Wrath**: 2min CD, use on CD (50% pet damage increase)

**Mana Management**:

- Aspect of the Viper when mana <30% (regen mana while attacking)
- Switch back to Aspect of the Hawk when mana >80%

---

#### Rogue (Combat Swords - Raid Spec)

**Pre-Pull**:

- Poisons applied: Instant Poison (main hand), Deadly Poison (off-hand)
- Stealth (for Ambush opener)

**Opener**:

1. Stealth → Ambush from behind (huge damage + combo points)
2. Slice and Dice (5 combo points, 9sec buff, refresh before falls off)
3. Adrenaline Rush (3min CD, use on pull, energy regen boost)
4. Sinister Strike spam → Build combo points
5. Eviscerate at 5 combo points (finisher)
6. Repeat

**Energy Management**:

- Don't cap at 100 energy (waste)
- Use abilities at 80-90 energy

**Cooldowns**:

- **Blade Flurry**: AOE CD, use on 2+ targets (cleaves)
- **Evasion**: Defensive, use when taking damage

---

#### Warrior (Fury - Raid DPS)

**Pre-Pull**:

- Battle Stance (Fury uses Battle or Berserker Stance)
- Shout active (Battle Shout = +AP raid-wide)

**Opener**:

1. Charge (generates rage)
2. Bloodrage (instant 20 rage)
3. Bloodthirst (main DPS ability, use on CD)
4. Whirlwind (AOE/single target filler)
5. Heroic Strike (rage dump when >60 rage)

**Rage Management**:

- Spam Heroic Strike when rage >70 (prevents capping)
- Don't use Heroic Strike when rage <40 (starves rotation)

**Cooldowns**:

- **Recklessness**: 30min CD, use on pull (100% crit for 15sec)
- **Death Wish**: 3min CD, use on CD (+20% damage)

---

### 🟡 Simming Your DPS (Advanced)

**What is Simming?** Running 10,000 virtual fights with your exact gear/rotation to find **theoretical max DPS**.

**Tools**:

- **SimulationCraft (SimC)**: Desktop app, imports character from game
- **Raidbots.com**: Web version (easier, but may not support TBC fully)

**How to Sim** (TBC Classic):

1. Install SimC addon in-game
2. Type `/simc` → Copy output
3. Go to Raidbots.com → Paste
4. Run sim → See DPS results

**What to Compare**:

- Your **raid logs DPS** (from Warcraft Logs) vs **sim DPS**
- If raid DPS is 70-80% of sim = good (100% unrealistic due to movement/mechanics)
- If raid DPS <60% of sim = rotation issues, fix immediately

---

## Gear Optimization

### 🔴 Stat Priority by Role

#### Tanks (Survival Focus)

**Stat Priority**:

1. **Defense Rating** (Critical Capped: 490 Defense = 5.6% crit reduction from bosses = Uncrittable)
    - **Goal**: 490 Defense MINIMUM (if below, you get crit = instant death)
2. **Stamina** (HP pool, prevents one-shots)
3. **Armor** (physical damage reduction)
4. **Dodge / Parry** (avoidance, less damage taken)
5. **Block Rating** (Warriors/Paladins, blocks 30% of attacks)
6. **Resilience** (PvP stat, reduces crit damage, minor benefit in PvE)

**Secondary**:

- **Threat Stats** (Attack Power, Hit Rating, Expertise) - Only after survival stats met

**Why This Order**: Dead tank = wipe. Threat is useless if you're dead.

---

#### Healers (Mana Sustain + HPS)

**Stat Priority**:

1. **+Healing** (Holy Priests, Resto Shaman) OR **Spell Damage** (Disc Priest, Holy Paladin scales with +damage)
2. **MP5** (Mana Per 5 Seconds) - Sustain stat, prevents OOMing
3. **Intellect** (Bigger mana pool + spell crit)
4. **Spirit** (Out-of-Combat mana regen, some specs benefit in-combat)
5. **Spell Crit** (Crit heals = more HPS, but RNG)
6. **Spell Haste** (Faster casts, only good if not going OOM)

**Spec-Specific**:

- **Resto Druids**: Spirit > MP5 (Innervate scales with Spirit)
- **Holy Paladins**: Spell Crit > MP5 (Illumination talent = crit heals refund mana)
- **Resto Shamans**: MP5 > Spirit (Chain Heal spam = mana-hungry)

---

#### DPS (Melee)

**Stat Priority** (General):

1. **Hit Rating** (Until Hit Cap: 9% for Yellow attacks, 27% for White attacks)
    - **Why**: Misses = 0 DPS. Hit cap FIRST, then other stats.
2. **Attack Power** (Flat DPS increase)
3. **Crit Rating** (RNG DPS increase, 1% crit = ~20 Crit Rating)
4. **Agility** (Rogues, Hunters, Feral Druids = Agi > Strength)
5. **Strength** (Warriors, Paladins, Enhancement Shamans)
6. **Expertise** (Reduces dodge/parry, 15.77 Expertise = 1% reduction)
7. **Haste** (Faster attacks, 10 Haste = 1% speed increase)

**Hit Cap Targets**:

- **Yellow Hit Cap** (special attacks like Sinister Strike, Mortal Strike): 9% = 142 Hit Rating
- **White Hit Cap** (auto-attacks): 27% = 432 Hit Rating (unrealistic to reach, don't prioritize)

**Expertise Cap**:

- **Soft Cap**: 6.5% = 26 Expertise (dodges removed)
- **Hard Cap**: 15% = 60 Expertise (parries removed, only needed for boss tanking from front)

---

#### DPS (Caster)

**Stat Priority**:

1. **Spell Hit Rating** (Until Spell Hit Cap: 16% = 202 Hit Rating)
    - **Why**: Resists = 0 DPS. Hit cap FIRST.
2. **Spell Damage** (Flat DPS increase, best stat after hit cap)
3. **Spell Crit** (RNG DPS, 1% crit = ~22 Crit Rating)
4. **Spell Haste** (Faster casts, 10 Haste = 1% cast speed)
5. **Intellect** (Bigger mana pool + crit, secondary stat)
6. **Spirit** (Mana regen, only good for specs with talents that convert Spirit to +damage)

**Spell Hit Cap** (By Debuff):

- **No Debuff**: 16% = 202 Hit Rating
- **With Imp. Faerie Fire / Misery**: 13% = 164 Hit Rating (3% from raid debuff)

**Why Spell Hit > Everything**: 1% hit = 1% DPS increase (guaranteed). 1% crit = 0.5-1% DPS (RNG).

---

### 🔴 Gem Optimization

**TBC Gems** = EXPENSIVE (50-100g per epic gem). Prioritize smartly.

---

#### Gem Priority (General Rules)

1. **Match Socket Bonuses ONLY IF Worth It**:
    
    - **Good Bonus**: +4 Spell Damage, +6 Stamina, +3 Hit Rating
    - **Bad Bonus**: +2 Spirit, +3 Intellect
    - **Rule**: If bonus > value of pure stat gem, match. Otherwise, ignore and gem pure stat.
2. **Meta Gem Requirements**:
    
    - Meta gems (head slot) require specific gem colors (e.g., "Requires 2 Red, 1 Yellow")
    - **Must meet requirement** for Meta to activate (huge stat boost)
    - **Plan around Meta** first, then fill other sockets.

---

#### Best Gems by Role

**Tanks**:

- **Red**: Solid Star of Elune (+12 Defense Rating, 60-80g)
- **Yellow**: Enduring Talasite (+6 Defense, +9 Stamina, 40-60g)
- **Blue**: Solid Empyrean Sapphire (+12 Stamina, 30-50g)
- **Meta**: Austere Earthstorm Diamond (+32 Stamina, +2% Armor, 100-150g)

**Healers**:

- **Red**: Teardrop Living Ruby (+14 Spell Damage, 50-70g)
- **Yellow**: Luminous Noble Topaz (+7 Healing, +9 Intellect, 40-60g)
- **Blue**: Soothing Sapphire (+9 Healing, +7 MP5, 30-50g)
- **Meta**: Insightful Earthstorm Diamond (+12 Intellect, Mana Restore proc, 100-150g)

**DPS (Melee)**:

- **Red**: Bold Living Ruby (+14 Strength, 50-70g)
- **Yellow**: Inscribed Noble Topaz (+7 Strength, +9 Crit, 40-60g)
- **Blue**: Sovereign Nightseye (+7 Strength, +9 Stamina, 30-50g)
- **Meta**: Relentless Earthstorm Diamond (+12 Agility, +3% Crit Damage, 100-150g)

**DPS (Caster)**:

- **Red**: Runed Living Ruby (+14 Spell Damage, 50-70g)
- **Yellow**: Veiled Noble Topaz (+7 Spell Damage, +9 Hit, 40-60g)
- **Blue**: Glowing Nightseye (+7 Spell Damage, +9 Stamina, 30-50g)
- **Meta**: Chaotic Skyfire Diamond (+12 Crit Rating, +3% Crit Damage, 100-150g)

---

### 🔴 Enchant Priority (Most Impact per Gold)

**ROI** (Return on Investment) = Biggest stat gain per gold spent.

**Top 5 Enchants** (All Roles):

1. **Weapon Enchant** (10-20 DPS gain, 300-500g) - HIGHEST PRIORITY
2. **Gloves Enchant** (5-10 DPS/HPS gain, 30-50g) - HIGH PRIORITY
3. **Chest Enchant** (5-10 DPS/survivability, 50-80g) - MEDIUM PRIORITY
4. **Boots Enchant** (movement speed + stats, 80-120g) - MEDIUM PRIORITY
5. **Ring Enchants** (Enchanters only, +20 Healing per ring, 100-150g mats) - MEDIUM PRIORITY

**Skip These** (Low ROI):

- Bracer enchants (2-3 stat gain, 20-40g) - Save gold
- Cloak enchants (Minor benefits, 15-30g) - Unless farming resist gear

---

## Profession Min-Maxing

### 🔴 Best Professions for Raiding

#### Alchemy (Best Gold-Saver)

**Benefits**:

- **Mixology** (TBC passive): +25% effect + 2x duration on YOUR potions
    - **Example**: Your Flask of Relentless Assault = +150 AP (not +120) and lasts 3 hours (not 2)
- **Transmutes**: Turn cheap mats into expensive gems (50g profit per transmute)

**Best for**: Anyone using lots of consumables (all raiders).

---

#### Jewelcrafting (Best Personal Stats)

**Benefits**:

- **Exclusive Gems**: JC-only gems (+34 Spell Damage vs +14 normal, +28 Strength vs +12)
- **Can use 3x JC gems** (huge stat boost: +60 Spell Damage over normal gems)

**Best for**: DPS who want absolute max stats.

---

#### Enchanting (Best for Flexibility)

**Benefits**:

- **Ring Enchants**: +20 Healing or +12 Spell Damage per ring (2 rings = +40 healing or +24 spell damage total)
- **Disenchant Raid Drops**: Turn unwanted loot into mats (20-50g value per item)

**Best for**: Casters, Healers.

---

#### Leatherworking (Best Raid Utility)

**Benefits**:

- **Drums of Battle**: Party-wide Bloodlust-lite (+80 Haste for 30sec, 2min CD)
    - **CRITICAL**: 1 Leatherworker with drums per 5-man group = 5% raid DPS increase
- **Exclusive Armor Kits**: +18 Stamina vs +12 normal

**Best for**: Melee DPS, Druids, Shamans.

---

#### Engineering (Best for Parse Chasers)

**Benefits**:

- **Goblin Sapper Charge**: AOE bomb (900-1500 damage, 5min CD) - Pads trash DPS
- **Mana/Health Injectors**: Instant potion (doesn't share potion CD)
- **Rocket Boots**: Speed boost (escape mechanics, but can backfire)

**Best for**: Parse chasers, speedrunners.

---

## Raid Preparation Checklist

### Print & Laminate (Physical Checklist)

```
===== TBC RAID PREP CHECKLIST =====
Character: _______________  Date: ___________

PRE-RAID (24-48 Hours Before):
[ ] Check BiS list - Identify missing gear
[ ] Buy consumables (shop Wed/Thu for low prices)
[ ] Repair to 100% (15g cost)
[ ] Empty bags (10+ slots free)
[ ] Update addons (CurseForge → Update All)
[ ] Practice rotation on dummy (5 min)
[ ] Test WeakAuras (/wa → Test all boss auras)

GEAR CHECK:
[ ] All slots enchanted (no yellow text on inspect)
[ ] All sockets filled (no gray sockets)
[ ] Weapon buff applied (oil/stone)
[ ] Meta gem requirement met (check tooltip)

CONSUMABLES IN BAGS:
[ ] Flask x1 OR Elixirs x2 of each type
[ ] Food x10 (30min duration each)
[ ] Mana potions x10 (casters/healers)
[ ] Healing potions x10 (all roles)
[ ] Scrolls x5 (Agi/Str/Int)
[ ] Weapon buff x2 (oil/stone)
[ ] Special: Shadow Prot Potion (Mag only)

1 HOUR BEFORE RAID:
[ ] Log in, travel to raid entrance
[ ] Flask/elixirs applied (check buff bar)
[ ] Food buff applied
[ ] Scroll buff applied
[ ] Weapon buff applied (lasts 1 hour)
[ ] Join Discord voice 10 min early
[ ] Mic test ("Can you hear me?")
[ ] Push-to-Talk keybind set

IN-RAID CHECKLIST (Before First Pull):
[ ] Raid buffs active (Fort, AI, Kings, Might)
[ ] DBM test (/dbm test → See warnings?)
[ ] Threat meter visible (Omen/TC2)
[ ] Assigned to correct group (check Shaman buffs)
[ ] Gargul soft reserves imported (RL only)
[ ] Voice clear (no background noise)

POST-WIPE CHECKLIST:
[ ] Flask still active? (check buff bar, lasts 2hr)
[ ] Elixirs re-applied? (lost on death)
[ ] Food buff re-applied? (lost on death)
[ ] Repair durability >20%? (if <20%, repair now)

===================================
```

---

## Gold Farming for Consumables

### 🔴 Best Gold Farms (100-200g/hour)

#### Daily Quests (TBC Phase 2+)

- **Netherwing Dailies**: 20-30g per day (15 min)
- **Ogri'la Dailies**: 15-25g per day (15 min)
- **Skyguard Dailies**: 15-25g per day (20 min)

**Total**: 50-80g per day for 1 hour work.

---

#### Primal Farming (Elemental Plateau)

- **Location**: Nagrand, Elemental Plateau
- **Farm**: Primal Air (sells 30-50g each)
- **Method**: Kill air elementals, collect Motes of Air (10 motes = 1 primal)

**Rate**: 3-5 Primal Air/hour = 100-200g/hour.

---

#### Heroic Dungeon Spam

- **Method**: Speed-run Heroic Shadow Labs, Heroic Shattered Halls
- **Drops**: BoE epics (500-1000g), Badge of Justice (trade for gear to DE for mats)
- **Raw gold**: 20-30g per run (15-20 min per run)

**Rate**: 80-120g/hour + chance at BoE jackpot.

---

### Consumable Cost Breakdown (Per Raid Night)

**Budget Setup** (Elixir + Basic):

- Elixirs: 40g
- Food: 20g
- Potions: 30g
- **Total**: 90g/night

**Full Setup** (Flask + All Buffs):

- Flask: 80g
- Food: 20g
- Potions: 30g
- Scrolls: 15g
- Weapon buff: 15g
- **Total**: 160g/night

**Per Week** (2 raids): 180-320g

**Farm Time Required**: 2-3 hours gold farming/week covers consumables.

---

## Next Steps

After min-maxing: → See **Addon Configuration** for UI optimization  
→ See **WeakAuras Guide** for mechanic tracking  
→ See **In-Game Macros** for rotation automation

