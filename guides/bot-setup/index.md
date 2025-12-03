---
layout: guide
title: Bot Setup Guide
section: 1
next_section: /guides/server-structure/
next_title: Server Structure Guide
---

# 1. WoW TBC Discord Bot Setup Guide

## Priority System

- **🔴 CRITICAL**: Must have before launch - core functionality
- **🟡 IMPORTANT**: Significantly improves experience - implement early
- **🟢 BONUS**: Nice-to-have features - add after core is stable

---

## 🔴 CRITICAL BOTS (Install First)

### Raid-Helper / Apollo

**Purpose**: Event scheduling, RSVP management, recurring raids

**Key Features**:

- Reaction-based signups (emoji for Tank/Healer/DPS)
- Timezone-aware reminders (auto-converts to user's local time)
- Recurring event templates
- Class/role tracking
- Multi-signup support
- Discord Scheduled Events integration

**Setup**:

- Raid-Helper: https://raid-helper.dev
- Apollo: https://apollo.fyi (250k+ servers)

**TBC-Specific Configuration**:

- Create custom templates with **Shaman as distinct role** (separate from Healer/DPS) for Bloodlust/Heroism tracking
- Force users to register their spec (not just "Mage" but "Arcane" or "Frost")
- Set up templates for "Kara 10-Man," "Gruul/Mag 25-Man," "Heroic Dungeon Spam"

**Pros**:

- Automates 90% of signup workflow
- Scales to 100+ PUGs/week
- Handles multi-timezone EU base automatically
- 1M+ proven servers (Raid-Helper)
- Recurring events save setup time

**Cons**:

- Learning curve for advanced templates
- Some premium features require subscription ($5-10/mo for advanced logging)
- Embed limits on free tier

**What You Gain**: Fills raids 2x faster, eliminates manual roster management, automatic reminders reduce no-shows by 60%

---

### SoftRes.it Bot

**Purpose**: Soft reserve loot management

**Key Features**:

- Embed reserves directly in Discord
- Multi-item reservations (2 per player standard)
- Automatic roll management
- Discord authentication
- Transparent reserve tracking
- Export CSV for in-game addons

**Setup**:

- Visit https://softres.it
- Add bot to server
- Use `!softres` command in designated channel
- Link with Raid-Helper events

**Integration Workflow**:

1. Raid-Helper posts event in `#raid-signups`
2. Bot auto-DMs reserve link when players sign up
3. Players select 2 items via web interface
4. Reserves posted as embed in Discord
5. Export CSV → Import to Gargul addon in-game

**Pros**:

- Eliminates 95% of loot drama
- Transparent MS>OS system
- Free to use
- Industry standard for Classic/TBC PUGs
- Web interface is user-friendly

**Cons**:

- Requires per-raid setup (5-10 minutes)
- Players must use external link
- No automatic in-game sync without Gargul

**What You Gain**: Loot resolution in <1 minute per item, zero "ninja" accusations, clear expectations before raid starts

---

### Dyno OR Carl-bot

**Purpose**: Moderation, verification, reaction roles, utility

**Key Features**:

**Dyno**:

- Captcha verification
- Auto-moderation (spam, links, mass mentions)
- Custom commands
- Auto-role assignment
- Moderation logging
- Timed mutes/kicks/bans
- Announcement scheduling

**Carl-bot**:

- Reaction roles (best-in-class)
- Auto-roles on join
- Logging and moderation
- Starboard (highlight best messages)
- Tags (custom commands)
- Polls
- Embed creator

**Setup**:

- Dyno: https://top.gg/bot/dyno
- Carl-bot: https://carl.gg

**Recommended**: Install **both** - Dyno for moderation, Carl-bot for reaction roles

**Configuration Priority**:

1. Set up captcha/verification in welcome channel
2. Create reaction role panel in `#roles` for class/spec selection
3. Enable auto-moderation (anti-spam, content filters)
4. Set up moderation logging to `#mod-logs`
5. Configure auto-role for verified users

**Pros**:

- 10M+ proven servers (Dyno)
- Spam-free server (-99% bots/spam)
- Automated role sync
- Free tier is robust
- Web dashboard for easy management

**Cons**:

- Dashboard learning curve (30-60 minutes)
- Some features locked behind premium (MEE6 alternative has more paywalls)

**What You Gain**: Trusted PUG base, automated onboarding, 80% reduction in moderation workload

---

### MikePy

**Purpose**: Instant gear verification via Armory embeds

**Key Features**:

- Paste gear string → instant visual Armory embed
- Shows ilvl, enchants, gems, professions
- Quick verification without leaving Discord
- Free to use
- No API key required

**Setup**:

- https://mikepy.com
- Invite bot
- Use `!armory [gear string]` command in `#gear-checks`

**How Players Get Gear String**:

1. Install "DejaCharacterStats" or similar addon
2. Type `/dcstats export` in-game
3. Copy string
4. Paste in Discord with `!armory` command

**Pros**:

- Instant verification (3 seconds vs 2 minutes manual check)
- Visual clarity for raid leaders
- Filters boosted characters
- Free
- No setup complexity

**Cons**:

- Players must install addon and copy gear string
- Some players find it confusing initially
- Doesn't auto-verify (requires manual paste)

**What You Gain**: Filters 80% unsuitable players, visual ilvl confirmation, 90% faster gear checks

---

## 🟡 IMPORTANT BOTS (High Value)

### Guilds of WoW

**Purpose**: WoW-specific LFG, gear verification, log integration

**Key Features**:

- LFG post creation with RSVP sync
- Automatic gear warnings (ilvl checks)
- Warcraft Logs embeds (shows parses)
- Battle.net account integration (Tier 2)
- In-game invite reminders
- WoW armory lookup
- Recruit feed integration

**Setup**:

- https://guildsofwow.com/install
- **Cost**: $1/month Tier 1 (recommended), $3/month Tier 2 for Battle.net sync

**What Each Tier Provides**:

- **Free**: Basic LFG posts
- **Tier 1 ($1/mo)**: Gear warnings, WCL embeds, armory lookup
- **Tier 2 ($3/mo)**: Battle.net invites, advanced RSVP sync

**Recommended Tier**: Tier 1 for casual PUGs, Tier 2 if running 10+ raids/week

**Pros**:

- Auto-checks logs and gear before raid
- Sends Battle.net invites (no friend requests needed)
- WCL integration shows player history
- WoW-tailored features
- Active development for TBC

**Cons**:

- Paid subscription (budget $12-36/year)
- Requires initial setup time (1-2 hours)
- Some features overlap with other bots

**What You Gain**: Auto-rejects undergeared players, saves 20 minutes/raid on verification, professional WCL presentation

---

### Warcraft Logs Webhook

**Purpose**: Automatic log posting and performance tracking

**Setup**:

1. Go to https://classic.warcraftlogs.com
2. Navigate to Settings → Webhooks
3. Create webhook pointing to your `#warcraftlogs` channel
4. Configure to auto-post when logs uploaded

**What It Posts**:

- Full raid report link
- Top DPS/HPS/Tank performance
- Parse percentiles
- Boss kill times
- Wipe count

**Pros**:

- Fully automated (zero manual work)
- Shows player performance publicly
- Free
- Encourages competition and improvement
- Archives raid history

**Cons**:

- Requires someone to upload logs after each raid
- Public parses can create pressure/toxicity if not moderated

**What You Gain**: Performance tracking, accountability, +30% progression speed (players improve when tracked)

---

## 🟢 BONUS BOTS (Nice-to-Have)

### Gargul (In-Game Addon + Discord Integration)

**Purpose**: Advanced loot distribution synced with SoftRes

**Key Features**:

- Syncs with SoftRes.it reserves
- Imports reserve data directly in-game
- Auto-announces loot drops in chat
- Handles rolls automatically
- Supports DKP/EPGP/Loot Council if needed
- Master loot tracking

**Setup**:

1. All raiders install Gargul addon from CurseForge
2. Raid Leader exports SoftRes CSV before raid
3. Import CSV into Gargul: `/gargul softres import`
4. Configure Discord webhook (optional) for loot announcements

**Workflow**:

- Boss dies → Loot drops → Gargul auto-announces: "Dragonspine Trophy drops! Reserved by @Player1 and @Player2. Rolling..."
- Auto-rolls among reservers
- Announces winner
- Updates loot history

**Pros**:

- Zero human error on loot
- Eliminates ninja accusations (100% transparent)
- Instant loot resolution (<30 seconds)
- Supports multiple loot systems
- Free addon

**Cons**:

- **All raiders must install addon** (can be barrier for casuals)
- Raid Leader must remember to import reserves
- Slight learning curve (15-30 minutes)

**What You Gain**: Zero loot disputes, 5x faster loot resolution, professional loot management

---

### PugBot (Self-Hosted)

**Purpose**: Quick character scans with `!pug [character-server]` command

**Setup**:

- GitHub: Self-host via Docker
- Requires Blizzard API key
- Free but technical setup

**Pros**:

- Faster than MikePy for bulk checks
- Shows achievements, gear, raid experience
- Can scan entire roster at once

**Cons**:

- Requires Docker knowledge and server hosting
- API key setup (Blizzard developer account)
- No official Discord bot (must self-host)
- More complex than MikePy

**Recommendation**: Only use if you're comfortable with Docker and want batch verification. Otherwise, stick with MikePy.

---

### Jeeves

**Purpose**: WoW utility bot for price checks and item info

**Key Features**:

- AH price checks (Primal prices, consumables)
- Item database lookups
- Quest information
- WoWProgress recruitment feed
- Token price tracking

**Setup**:

- Search "Jeeves" on top.gg
- Restrict to `#market-watch` channel to avoid spam

**Pros**:

- Quick Primal/consumable price checks in Discord
- WoW-tailored features
- Useful for economy discussions

**Cons**:

- Most features need authorized WoW accounts
- Can spam channels if unrestricted
- Some features are retail-focused (ignore for Classic)

**What You Gain**: Faster gold-making discussions, easy price references, economy tracking

---

### Ticket Tool / Ticket King

**Purpose**: Support and report management

**Key Features**:

- Creates private ticket threads
- Staff-only visibility
- Ticket logging and history
- Multi-category support (Reports, Appeals, General Help)
- Auto-close inactive tickets

**Setup**:

- https://tickettool.xyz or search "Ticket King" on top.gg
- Create ticket panel in `#support`
- Configure categories (Bug Reports, Loot Disputes, Ban Appeals)

**Pros**:

- Private dispute handling (no public drama)
- Scales moderation (10+ tickets/day manageable)
- Professional appearance
- Organized support system

**Cons**:

- Requires active mod team (tickets need responses)
- Can accumulate if not monitored

**What You Gain**: Cleaner chat (-90% public arguments), professional support system, 50% faster dispute resolution

---

### Ephemeral Roles / VoiceMaster

**Purpose**: Temporary access management for PUGs

**Key Features**:

- Auto-creates temporary voice channels
- Grants temporary roles for PUG participants
- Auto-removes roles/channels when PUG ends
- Limits visibility (only PUG members see their channels)

**Setup**:

- VoiceMaster for auto voice channels
- Custom bot or Dyno for ephemeral roles

**Pros**:

- Privacy protection (no roster sniping)
- Reduces channel clutter
- Clean UI (only active PUGs visible)
- Professional for large servers

**Cons**:

- Confusing for older/less tech-savvy players
- Requires careful permission configuration
- Can break if Discord updates permissions

**Recommendation**: Only implement if running 20+ simultaneous PUGs. Otherwise, use static voice channels.

---

### Simple Poll / Poll Bot

**Purpose**: Quick voting for raid times, strategies, loot policies

**Setup**: Search "Simple Poll" on top.gg

**Use Cases**:

- "Vote for raid time: React with 🇦 for 19:00, 🇧 for 20:00, 🇨 for 21:00"
- "Should we allow GDKP runs? ✅ Yes / ❌ No"
- "Which raid should we prioritize? ⚔️ Kara / 🛡️ Gruul / 🔥 Mag"

**Pros**:

- Fast community feedback
- Built-in to Discord (can use reactions without bot)
- Free

**Cons**:

- Minor feature (Discord reactions work fine)
- Extra bot slot used

**Recommendation**: Use Discord's native poll feature (right-click in text box → Create Poll) instead of a bot.

---

### Music Bot (FredBoat / Lavalink)

**Purpose**: Background music during raid breaks

**Key Features**:

- Play music in voice channels
- YouTube/Spotify/SoundCloud support
- Queue management
- Volume control

**Setup**:

- **WARNING**: Many music bots shut down due to YouTube ToS
- Self-host Lavalink for reliability

**Pros**:

- Keeps energy high during breaks
- Morale boost (+10% retention)
- Community bonding

**Cons**:

- Voice overlap potential (can drown out raid calls)
- DMCA/ToS issues with public bots
- Self-hosting requires technical knowledge

**Recommendation**: Only add if you have a dedicated "lounge" voice channel. Keep music bot OUT of raid voice channels.

---

## Bot Integration Workflow

### Complete Raid Workflow (All Bots Working Together)

1. **Event Creation** (Raid-Helper/Apollo)
    
    - Raid Leader: `/create Karazhan PUG - Wednesday 20:00 CET`
    - Bot posts in `#raid-signups`
2. **Signup** (Raid-Helper)
    
    - Players react: 🛡️ Tank / ❤️ Healer / ⚔️ DPS
    - Bot DMs each signup: "Lock in reserves: [SoftRes link]"
3. **Soft Reserve** (SoftRes.it)
    
    - Players visit link, pick 2 items
    - Reserves posted as embed in `#softres-kara`
4. **Gear Verification** (MikePy + Guilds of WoW)
    
    - Players post: `!armory [gear string]` in `#gear-checks`
    - Guilds of WoW bot flags undergeared: "⚠️ @Player ilvl 65 (req: 70)"
5. **Pre-Raid Prep** (1 hour before)
    
    - Raid-Helper sends reminder: "Raid in 1 hour! @Tank @Healer @DPS"
    - Raid Leader exports SoftRes CSV
    - Import to Gargul addon
6. **Raid Execution** (Gargul + Voice)
    
    - Move to `#voice-raid-leader`
    - Boss dies → Gargul: "Moroes' Lucky Pocket Watch drops! Reserved by @Rogue1 @Rogue2. Rolling..."
    - Winner announced in <5 seconds
7. **Post-Raid** (WCL Webhook)
    
    - Raid Leader uploads logs
    - Webhook auto-posts to `#warcraftlogs`: "Karazhan clear! Top DPS: @Mage (98 parse)"
    - Share highlights in `#raid-highlights`

---

## Bot Budget & Priority Order

### Free Setup (Essentials Only) - $0/month

1. Raid-Helper (free tier)
2. SoftRes.it (free)
3. Dyno (free)
4. Carl-bot (free)
5. MikePy (free)
6. WCL Webhook (free)

**Total**: $0/month  
**Capability**: Run 5-10 PUGs/week efficiently

---

### Recommended Setup (High Value) - $1-3/month

All above, plus:

- Guilds of WoW Tier 1 ($1/mo) or Tier 2 ($3/mo)

**Total**: $12-36/year  
**Capability**: Run 20+ PUGs/week with auto-verification

---

### Premium Setup (Large Community) - $5-10/month

All above, plus:

- Raid-Helper Premium ($5/mo) for advanced logging
- Music bot hosting ($3-5/mo for VPS)

**Total**: $96-180/year  
**Capability**: 50+ PUGs/week, full automation, professional polish

---

## Installation Order (First 2 Hours)

1. **Hour 1**: Core Bots
    
    - [ ] Invite Dyno → Configure verification
    - [ ] Invite Carl-bot → Set up reaction roles
    - [ ] Invite Raid-Helper → Create first test event
    - [ ] Invite SoftRes.it → Test reserve flow
2. **Hour 2**: Enhancement Bots
    
    - [ ] Invite MikePy → Test gear check
    - [ ] Set up WCL Webhook
    - [ ] (Optional) Invite Guilds of WoW
3. **Week 1**: Polish
    
    - [ ] Fine-tune auto-moderation rules
    - [ ] Create recurring raid templates
    - [ ] Test full workflow with 5 friends

---

## Common Mistakes to Avoid

1. **Over-botting**: Don't install 15+ bots. Stick to 5-8 essential ones.
2. **Permission Conflicts**: Set bot roles high in hierarchy, but below Admin.
3. **No Testing**: Always test signup → reserve → raid workflow before launch.
4. **Ignoring Logs**: Set up WCL webhook early - players want performance tracking.
5. **Forgetting Mobile**: Test all bot features on mobile Discord (reaction roles work differently).

---

## Next Steps

After bot setup is complete: → See **Server Structure Guide** for channel and role configuration  
→ See **Raid Organization Workflow** for detailed raid management  
→ See **Templates Guide** for copy-paste messages