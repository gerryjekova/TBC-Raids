---
layout: guide
title: Server Structure Guide
section: 2
next_section: /guides/raid-organization/
next_title: Raid Organization Guide
---

# 2. WoW TBC Discord Server Structure Guide

## Priority System

- **🔴 CRITICAL**: Must configure before launch
- **🟡 IMPORTANT**: Implement in first week
- **🟢 BONUS**: Add as community grows

---

## 🔴 Server Foundation (Setup First)

### Community Server Features

Enable these Discord features before building structure:

1. **Enable Community Server**:
    
    - Server Settings → Enable Community
    - Accept rules screening
    - Set default channels
2. **Discovery & Safety**:
    
    - Verification Level: **Medium** (email verified)
    - Explicit Content Filter: **Scan from all members**
    - 2FA Requirement for Moderators: **Enabled**
3. **AFK Settings**:
    
    - AFK Timeout: **15 minutes**
    - AFK Channel: Create and assign

---

## Channel Structure (25 Channels - Scalable)

### Principle: "If you can't find it in 3 clicks, it's too complex"

---

## 🔴 CATEGORY: 📢 WELCOME & INFO

**Purpose**: First stop for new members  
**Permissions**: Read-only for @everyone (except #verify)

### Channels:

#### `#welcome`

- **Type**: Text (read-only)
- **Purpose**: Auto-welcome message + quick navigation
- **Permissions**:
    - @everyone: Read Messages
    - @Bots: Send Messages, Embed Links
- **Content**: Welcome embed (see Templates guide)
- **Priority**: 🔴 CRITICAL

#### `#rules`

- **Type**: Text (read-only)
- **Purpose**: Server rules, behavior expectations, loot policies
- **Permissions**:
    - @everyone: Read Messages
    - @Moderator+: Send Messages
- **Must Include**:
    - Behavior rules (no toxicity, harassment)
    - Voice requirements (Push-to-Talk recommended)
    - Punctuality expectations (10 min early)
    - Loot policy (MS>OS + 2 SR)
    - Report procedure (use tickets)
- **Priority**: 🔴 CRITICAL

#### `#verify`

- **Type**: Text (interactive)
- **Purpose**: Captcha/reaction verification gate
- **Permissions**:
    - @everyone: Read Messages, Add Reactions
    - @Dyno/@Carl-bot: Manage Roles, Send Messages
- **Bot Setup**: Dyno captcha or Carl-bot reaction verification
- **Result**: Assigns @Verified role → unlocks rest of server
- **Priority**: 🔴 CRITICAL

#### `#roles`

- **Type**: Text (read-only, reactions enabled)
- **Purpose**: Self-assign class/role/faction via reactions
- **Permissions**:
    - @everyone: Read Messages, Add Reactions
    - @Carl-bot: Manage Roles, Send Messages, Embed Links
- **Reaction Panel**: (see Role Configuration section)
- **Priority**: 🔴 CRITICAL

#### `#how-to-pug`

- **Type**: Text (read-only)
- **Purpose**: Quick guide for newcomers
- **Content**:
    - How to sign up for raids
    - How to use SoftRes
    - How to post gear for verification
    - Voice expectations
    - What addons are required
- **Priority**: 🟡 IMPORTANT

---

## 🔴 CATEGORY: 📣 ANNOUNCEMENTS

**Purpose**: Important server updates  
**Permissions**: Read-only for @everyone

#### `#announcements`

- **Type**: Announcement Channel
- **Purpose**: Major server news, maintenance, policy changes
- **Permissions**:
    - @everyone: Read Messages
    - @Admin only: Send Messages, @everyone mention
- **Usage**: Sparingly (1-2 posts/week max)
- **Priority**: 🔴 CRITICAL

#### `#pug-schedule`

- **Type**: Text (read-only)
- **Purpose**: Weekly raid calendar overview
- **Permissions**:
    - @everyone: Read Messages
    - @Raid Leader+: Send Messages
- **Content**: Pin weekly schedule summary
- **Priority**: 🟡 IMPORTANT

#### `#rules-loot`

- **Type**: Text (read-only)
- **Purpose**: Detailed loot rules (pinned reference)
- **Permissions**: @everyone: Read Messages
- **Content**: MS>OS explanation, Soft Reserve guide, BoE policy
- **Priority**: 🔴 CRITICAL

---

## 🔴 CATEGORY: 💬 SOCIAL & COMMUNITY

**Purpose**: General discussion and engagement  
**Permissions**: @Verified can read/write

#### `#general`

- **Type**: Text
- **Purpose**: Main chat, WoW discussion
- **Slowmode**: None (or 3-5 seconds if spam becomes issue)
- **Priority**: 🔴 CRITICAL

#### `#off-topic`

- **Type**: Text
- **Purpose**: Non-WoW discussion, casual chat
- **Priority**: 🟡 IMPORTANT

#### `#memes`

- **Type**: Text (media-heavy)
- **Purpose**: Images, videos, humor
- **Permissions**: Enable embeds and file uploads
- **Priority**: 🟢 BONUS

#### `#tavern-chat`

- **Type**: Text
- **Purpose**: RP/lore-friendly discussion (optional)
- **Priority**: 🟢 BONUS

#### `#market-watch`

- **Type**: Text
- **Purpose**: Economy discussion, Primal prices, crafted gear, gold-making
- **Jeeves Bot Integration**: Restrict here to avoid spam
- **Priority**: 🟡 IMPORTANT

#### `#class-discussion`

- **Type**: Text or Forum Channel
- **Purpose**: Spec theory, rotations, gear advice
- **Alternative**: Separate channels per class if population >500
- **Priority**: 🟡 IMPORTANT

---

## 🔴 CATEGORY: 🔍 LFG & SIGNUPS

**Purpose**: Group finding and raid signups  
**Permissions**: @Verified can read/write

### Design Principle: One channel per raid tier/type

#### `#raid-signups`

- **Type**: Text (read-only for @everyone)
- **Purpose**: **Bot-only** Raid-Helper/Apollo event posts
- **Permissions**:
    - @Verified: Read Messages, Add Reactions
    - @Raid-Helper/@Apollo: Send Messages, Embed Links, Manage Messages
    - @Raid Leader+: Send Messages (for manual posts)
- **Slowmode**: N/A (bot-controlled)
- **Priority**: 🔴 CRITICAL

#### `#lfg-karazhan`

- **Type**: Text
- **Purpose**: Kara-specific LFG (10-man)
- **Format**: "LFM Kara - Need 1 Tank, 2 DPS - 20:00 CET - MS>OS"
- **Slowmode**: 10 seconds (prevents spam)
- **Auto-delete**: Old posts after 24 hours (use auto-mod bot)
- **Priority**: 🔴 CRITICAL

#### `#lfg-gruul`

- **Type**: Text
- **Purpose**: Gruul's Lair (25-man)
- **Slowmode**: 10 seconds
- **Priority**: 🔴 CRITICAL

#### `#lfg-magtheridon`

- **Type**: Text
- **Purpose**: Magtheridon's Lair (25-man)
- **Slowmode**: 10 seconds
- **Priority**: 🔴 CRITICAL

#### `#lfg-heroics`

- **Type**: Text
- **Purpose**: Heroic 5-man dungeons
- **Slowmode**: 5 seconds (high traffic)
- **Priority**: 🔴 CRITICAL

#### `#lfg-attunements`

- **Type**: Text
- **Purpose**: **TBC-specific** - Kara key runs, rep grinds, attunement chains
- **Example**: "LFM Black Morass for Kara key - Need healer"
- **Slowmode**: 5 seconds
- **Priority**: 🔴 CRITICAL

#### `#lfg-arenas`

- **Type**: Text (optional)
- **Purpose**: Arena team recruitment, partners
- **Priority**: 🟢 BONUS

---

## 🔴 CATEGORY: 📋 TOOLS & RESOURCES

**Purpose**: Raid support and information  
**Permissions**: @Verified can read/write (except bot-only channels)

#### `#softres-all`

- **Type**: Text (read-only for @everyone)
- **Purpose**: SoftRes.it embed posts
- **Permissions**:
    - @Verified: Read Messages
    - @SoftRes Bot: Send Messages, Embed Links
- **Priority**: 🔴 CRITICAL

#### `#warcraftlogs`

- **Type**: Text (webhook-only)
- **Purpose**: Auto-posted logs via WCL webhook
- **Permissions**: Read for @everyone, Write for Webhook only
- **Priority**: 🔴 CRITICAL

#### `#gear-checks`

- **Type**: Text
- **Purpose**: MikePy/PugBot gear verification
- **Usage**: Players post `!armory [gear string]` here
- **Slowmode**: 5 seconds
- **Priority**: 🔴 CRITICAL

#### `#guides`

- **Type**: Text or Forum Channel (read-only)
- **Purpose**: Boss strategies, consumables lists, enchants, rotation guides
- **Permissions**: @everyone: Read, @Raid Leader+: Send
- **Content to Pin**:
    - Boss strat videos (FatBoss, etc.)
    - Consumables checklist
    - Enchant priorities per slot
    - WeakAuras pack links
- **Enable**: Embeds for videos
- **Priority**: 🟡 IMPORTANT

#### `#wago-was`

- **Type**: Text
- **Purpose**: WeakAuras sharing and discussion
- **Priority**: 🟡 IMPORTANT

#### `#goldmaking`

- **Type**: Text
- **Purpose**: Farming routes, profession guides, AH flipping
- **Priority**: 🟢 BONUS

#### `#clips`

- **Type**: Text (media-heavy)
- **Purpose**: Raid highlights, funny moments, achievements
- **Starboard Integration**: Carl-bot starboard posts here
- **Priority**: 🟡 IMPORTANT

---

## 🔴 CATEGORY: 🎤 VOICE CHANNELS

**Purpose**: Voice communication for raids and socializing

### Design: Stage Channels for raids, regular voice for casual

#### `Raid Leader` (Stage Channel)

- **Type**: Stage Channel
- **Purpose**: Main raid calls (Raid Leader + Officers as speakers)
- **Permissions**:
    - @everyone: Audience (listen only)
    - @Raid Leader, @Officer: Speaker (can talk)
    - @Moderator: Request to Speak approval, mute control
- **Usage**: 25-man raids, important callouts
- **Priority**: 🟡 IMPORTANT (use regular voice if <100 members)

#### `Off-Tank 1` / `Off-Tank 2`

- **Type**: Voice Channel
- **Purpose**: Side communication for tanks, assignments
- **Permissions**: @Verified can join/speak
- **Bitrate**: 64kbps minimum (96kbps recommended)
- **Priority**: 🟡 IMPORTANT

#### `Raid Voice - Kara`

- **Type**: Voice Channel
- **Purpose**: 10-man Kara runs
- **User Limit**: 10 (enforce comp)
- **Priority**: 🔴 CRITICAL

#### `Raid Voice - 25m`

- **Type**: Voice Channel
- **Purpose**: Gruul/Mag runs
- **User Limit**: 25 (enforce comp)
- **Priority**: 🔴 CRITICAL

#### `General Voice`

- **Type**: Voice Channel
- **Purpose**: Casual hanging out
- **Priority**: 🟡 IMPORTANT

#### `AFK Lobby`

- **Type**: Voice Channel
- **Purpose**: Auto-move AFK users here
- **Settings**: Set as AFK channel (15 min timeout)
- **Priority**: 🔴 CRITICAL

#### `Music Lounge` (Optional)

- **Type**: Voice Channel
- **Purpose**: Music bot channel (keep OUT of raid voice)
- **Priority**: 🟢 BONUS

---

## 🟡 CATEGORY: 🛡️ STAFF (Hidden)

**Purpose**: Moderator/admin operations  
**Permissions**: @Moderator and above only

#### `#mod-chat`

- **Type**: Text
- **Purpose**: Officer coordination, decisions
- **Priority**: 🟡 IMPORTANT

#### `#mod-logs`

- **Type**: Text (read-only)
- **Purpose**: Auto-moderation logs (Dyno/Carl-bot)
- **Permissions**: Bots send, Mods read
- **Priority**: 🟡 IMPORTANT

#### `#tickets`

- **Type**: Text
- **Purpose**: Ticket Tool management panel
- **Priority**: 🟡 IMPORTANT (if using Ticket Bot)

#### `#vetting-logs`

- **Type**: Text
- **Purpose**: Where users post logs to get "Verified Raider" or "Pumper" role
- **Priority**: 🟢 BONUS

---

## Role Configuration

### 🔴 Role Hierarchy (Top to Bottom)

**Critical**: Roles higher in hierarchy have more power. Set carefully.

1. **@Owner** - Full permissions
2. **@Admin** - Server administration
3. **@Officer** - Event management, moderation
4. **@Raid Leader** - Event creation, role assignment
5. **@Core** - Regular raiders (invite-only, perks)
6. **@Verified** - Passed verification (unlocks channels)
7. **@70** - Level-capped players
8. **@Pumper** - High performers (optional prestige role)
9. **Class Roles** - @Warrior, @Mage, @Warlock, @Priest, @Paladin, @Druid, @Hunter, @Rogue, @Shaman
10. **Spec Roles** - @Tank, @Healer, @DPS
11. **@Horde** / **@Alliance** - Faction tags
12. **@Pug** - Temporary participants (ephemeral, optional)
13. **@Streamers** - Content creators
14. **@Muted** - Restricted from chat
15. **@Bots** - Bot accounts

---

### 🔴 Role Permissions (Critical Settings)

#### @Verified (Gatekeeper Role)

- **Granted by**: Dyno/Carl-bot after captcha
- **Permissions**:
    - Read most channels (excludes Staff)
    - Send messages in social/LFG
    - Add reactions
    - Connect to voice
    - Use voice activity
- **Purpose**: Prevents spam bots, ensures humans

#### @Raid Leader

- **Permissions**:
    - Create Events (Discord Scheduled Events)
    - Manage Messages (in #raid-signups, #lfg channels)
    - Mention @everyone (in raid channels only)
    - Move Members (voice channels)
    - Mute Members (during raids)
- **Who Gets It**: Trusted players after 3-5 successful raid leads

#### @Core

- **Permissions**: Same as @Verified
- **Perks** (via bot or manual):
    - Priority signup for raids (early access)
    - Special color in sidebar
    - Access to #core-chat (optional exclusive channel)
- **Who Gets It**: Regular raiders (10+ raids attended)

---

### 🔴 Reaction Role Panel (Carl-bot Setup)

**Location**: `#roles` channel

#### Message Content:

```
**Select Your Class & Role**

React below to assign yourself roles. This helps Raid Leaders ping the right people!

**Classes** 🏆
⚔️ = Warrior
🔮 = Mage
🔥 = Warlock
✨ = Priest
⚡ = Shaman
🌿 = Druid
🏹 = Hunter
🗡️ = Rogue
☀️ = Paladin

**Roles** 🎯
🛡️ = Tank
❤️ = Healer
⚔️ = DPS

**Faction** 🚩
🔴 = Horde
🔵 = Alliance
```

#### Carl-bot Command (in #roles):

```
!rr create
!rr add [message ID] ⚔️ @Warrior
!rr add [message ID] 🔮 @Mage
[... repeat for all classes]
!rr add [message ID] 🛡️ @Tank
!rr add [message ID] ❤️ @Healer
!rr add [message ID] ⚔️ @DPS
!rr add [message ID] 🔴 @Horde
!rr add [message ID] 🔵 @Alliance
```

**Priority**: 🔴 CRITICAL

---

### 🟡 TBC-Specific Role: @Shaman

**Why Separate Role?**

- TBC raids require 1 Shaman per 5-man group (Bloodlust/Heroism)
- Must track Resto vs Enhancement vs Elemental specs
- Different group assignments per spec

**Setup**:

- Create @Resto-Shaman, @Enhance-Shaman, @Ele-Shaman roles
- Add to reaction panel separately from general @Healer/@DPS
- Use for targeted pings: "@Resto-Shaman we need 1 more for Gruul tonight"

---

## Permission Best Practices

### 🔴 Channel Permission Templates

#### Read-Only Announcement Channel (#announcements, #rules)

- @everyone: ✅ Read Messages, ✅ Read Message History, ❌ Send Messages
- @Admin: ✅ All permissions

#### Interactive LFG Channel (#lfg-karazhan)

- @everyone: ❌ Read Messages (gated)
- @Verified: ✅ Read, ✅ Send, ✅ Add Reactions, ✅ Embed Links, ✅ Attach Files
- **Slowmode**: 10 seconds

#### Bot-Only Channel (#raid-signups, #warcraftlogs)

- @everyone/@Verified: ✅ Read, ✅ Add Reactions, ❌ Send
- @Bots: ✅ Send, ✅ Embed, ✅ Manage Messages
- @Raid Leader: ✅ Send (for manual posts)

#### Staff Channel (#mod-chat)

- @everyone: ❌ Read (hidden)
- @Moderator+: ✅ All permissions

---

## Server Settings (Essential Configuration)

### 🔴 Moderation Settings

- **Verification Level**: Medium (email required)
- **Explicit Content Filter**: Scan all members
- **DM Filter**: Enabled (filters DM spam from server)
- **2FA Requirement**: Enabled for moderators

### 🔴 Auto-Moderation (Dyno/Carl-bot)

Enable these filters:

- ✅ Mass mention spam (4+ mentions = auto-delete)
- ✅ Link spam (3+ links in 10 seconds = auto-delete)
- ✅ Zalgo text (Unicode spam)
- ✅ Repeated text (10+ same messages)
- ✅ Caps spam (80%+ caps in message)
- ✅ Emoji spam (10+ emojis)

### 🟡 Welcome Screen

Set up Community Welcome Screen:

1. Server Settings → Community → Welcome Screen
2. Enable Welcome Screen
3. Add welcome channels:
    - #rules (required read)
    - #roles (select roles)
    - #how-to-pug (quick start)
4. Add custom welcome message (50 character limit)

### 🟡 Server Boost Perks

If boosted to Level 2:

- ✅ 150 emoji slots (use for class icons)
- ✅ 1080p 60fps streaming
- ✅ Server banner
- ✅ 50MB upload limit (useful for logs/screenshots)

---

## Common Mistakes to Avoid

1. **Too Many Channels**: Don't create 50+ channels at launch. Start with 20-25, add as needed.
2. **No Verification**: Unverified servers get bot spam. Always use captcha gate.
3. **@everyone Permissions**: Never give write permissions to @everyone. Use @Verified.
4. **Ignoring Slowmode**: LFG channels without slowmode = spam hell.
5. **No AFK Channel**: Members stay in raid voice 24/7 = confusing roster.
6. **Hidden Welcome**: New members must see #rules and #roles immediately.
7. **Bot Permission Conflicts**: Set bot roles high in hierarchy (below Admin, above users).

---

## Testing Checklist (Before Launch)

- [ ] Create test account, verify full onboarding flow
- [ ] Test reaction roles in #roles (do emojis assign correctly?)
- [ ] Verify @Verified role unlocks correct channels
- [ ] Test LFG post in each #lfg channel (slowmode working?)
- [ ] Test voice channels (bitrate good? AFK timeout working?)
- [ ] Verify bots can post in their assigned channels
- [ ] Test moderation (post spam, verify auto-delete)
- [ ] Mobile test (check on phone - reaction roles work differently)

---

## Next Steps

After structure setup: → See **Bot Setup Guide** for detailed bot configuration  
→ See **Raid Organization Workflow** for raid management  
→ See **Templates Guide** for welcome messages and rules




WoW TBC Discord Server Structure Guide

## Priority System

- **🔴 CRITICAL**: Must configure before launch
- **🟡 IMPORTANT**: Implement in first week
- **🟢 BONUS**: Add as community grows

---

## 🔴 Server Foundation (Setup First)

### Community Server Features

Enable these Discord features before building structure:

1. **Enable Community Server**:
    
    - Server Settings → Enable Community
    - Accept rules screening
    - Set default channels
2. **Discovery & Safety**:
    
    - Verification Level: **Medium** (email verified)
    - Explicit Content Filter: **Scan from all members**
    - 2FA Requirement for Moderators: **Enabled**
3. **AFK Settings**:
    
    - AFK Timeout: **15 minutes**
    - AFK Channel: Create and assign

---

## Channel Structure (25 Channels - Scalable)

### Principle: "If you can't find it in 3 clicks, it's too complex"

---

## 🔴 CATEGORY: 📢 WELCOME & INFO

**Purpose**: First stop for new members  
**Permissions**: Read-only for @everyone (except #verify)

### Channels:

#### `#welcome`

- **Type**: Text (read-only)
- **Purpose**: Auto-welcome message + quick navigation
- **Permissions**:
    - @everyone: Read Messages
    - @Bots: Send Messages, Embed Links
- **Content**: Welcome embed (see Templates guide)
- **Priority**: 🔴 CRITICAL

#### `#rules`

- **Type**: Text (read-only)
- **Purpose**: Server rules, behavior expectations, loot policies
- **Permissions**:
    - @everyone: Read Messages
    - @Moderator+: Send Messages
- **Must Include**:
    - Behavior rules (no toxicity, harassment)
    - Voice requirements (Push-to-Talk recommended)
    - Punctuality expectations (10 min early)
    - Loot policy (MS>OS + 2 SR)
    - Report procedure (use tickets)
- **Priority**: 🔴 CRITICAL

#### `#verify`

- **Type**: Text (interactive)
- **Purpose**: Captcha/reaction verification gate
- **Permissions**:
    - @everyone: Read Messages, Add Reactions
    - @Dyno/@Carl-bot: Manage Roles, Send Messages
- **Bot Setup**: Dyno captcha or Carl-bot reaction verification
- **Result**: Assigns @Verified role → unlocks rest of server
- **Priority**: 🔴 CRITICAL

#### `#roles`

- **Type**: Text (read-only, reactions enabled)
- **Purpose**: Self-assign class/role/faction via reactions
- **Permissions**:
    - @everyone: Read Messages, Add Reactions
    - @Carl-bot: Manage Roles, Send Messages, Embed Links
- **Reaction Panel**: (see Role Configuration section)
- **Priority**: 🔴 CRITICAL

#### `#how-to-pug`

- **Type**: Text (read-only)
- **Purpose**: Quick guide for newcomers
- **Content**:
    - How to sign up for raids
    - How to use SoftRes
    - How to post gear for verification
    - Voice expectations
    - What addons are required
- **Priority**: 🟡 IMPORTANT

---

## 🔴 CATEGORY: 📣 ANNOUNCEMENTS

**Purpose**: Important server updates  
**Permissions**: Read-only for @everyone

#### `#announcements`

- **Type**: Announcement Channel
- **Purpose**: Major server news, maintenance, policy changes
- **Permissions**:
    - @everyone: Read Messages
    - @Admin only: Send Messages, @everyone mention
- **Usage**: Sparingly (1-2 posts/week max)
- **Priority**: 🔴 CRITICAL

#### `#pug-schedule`

- **Type**: Text (read-only)
- **Purpose**: Weekly raid calendar overview
- **Permissions**:
    - @everyone: Read Messages
    - @Raid Leader+: Send Messages
- **Content**: Pin weekly schedule summary
- **Priority**: 🟡 IMPORTANT

#### `#rules-loot`

- **Type**: Text (read-only)
- **Purpose**: Detailed loot rules (pinned reference)
- **Permissions**: @everyone: Read Messages
- **Content**: MS>OS explanation, Soft Reserve guide, BoE policy
- **Priority**: 🔴 CRITICAL

---

## 🔴 CATEGORY: 💬 SOCIAL & COMMUNITY

**Purpose**: General discussion and engagement  
**Permissions**: @Verified can read/write

#### `#general`

- **Type**: Text
- **Purpose**: Main chat, WoW discussion
- **Slowmode**: None (or 3-5 seconds if spam becomes issue)
- **Priority**: 🔴 CRITICAL

#### `#off-topic`

- **Type**: Text
- **Purpose**: Non-WoW discussion, casual chat
- **Priority**: 🟡 IMPORTANT

#### `#memes`

- **Type**: Text (media-heavy)
- **Purpose**: Images, videos, humor
- **Permissions**: Enable embeds and file uploads
- **Priority**: 🟢 BONUS

#### `#tavern-chat`

- **Type**: Text
- **Purpose**: RP/lore-friendly discussion (optional)
- **Priority**: 🟢 BONUS

#### `#market-watch`

- **Type**: Text
- **Purpose**: Economy discussion, Primal prices, crafted gear, gold-making
- **Jeeves Bot Integration**: Restrict here to avoid spam
- **Priority**: 🟡 IMPORTANT

#### `#class-discussion`

- **Type**: Text or Forum Channel
- **Purpose**: Spec theory, rotations, gear advice
- **Alternative**: Separate channels per class if population >500
- **Priority**: 🟡 IMPORTANT

---

## 🔴 CATEGORY: 🔍 LFG & SIGNUPS

**Purpose**: Group finding and raid signups  
**Permissions**: @Verified can read/write

### Design Principle: One channel per raid tier/type

#### `#raid-signups`

- **Type**: Text (read-only for @everyone)
- **Purpose**: **Bot-only** Raid-Helper/Apollo event posts
- **Permissions**:
    - @Verified: Read Messages, Add Reactions
    - @Raid-Helper/@Apollo: Send Messages, Embed Links, Manage Messages
    - @Raid Leader+: Send Messages (for manual posts)
- **Slowmode**: N/A (bot-controlled)
- **Priority**: 🔴 CRITICAL

#### `#lfg-karazhan`

- **Type**: Text
- **Purpose**: Kara-specific LFG (10-man)
- **Format**: "LFM Kara - Need 1 Tank, 2 DPS - 20:00 CET - MS>OS"
- **Slowmode**: 10 seconds (prevents spam)
- **Auto-delete**: Old posts after 24 hours (use auto-mod bot)
- **Priority**: 🔴 CRITICAL

#### `#lfg-gruul`

- **Type**: Text
- **Purpose**: Gruul's Lair (25-man)
- **Slowmode**: 10 seconds
- **Priority**: 🔴 CRITICAL

#### `#lfg-magtheridon`

- **Type**: Text
- **Purpose**: Magtheridon's Lair (25-man)
- **Slowmode**: 10 seconds
- **Priority**: 🔴 CRITICAL

#### `#lfg-heroics`

- **Type**: Text
- **Purpose**: Heroic 5-man dungeons
- **Slowmode**: 5 seconds (high traffic)
- **Priority**: 🔴 CRITICAL

#### `#lfg-attunements`

- **Type**: Text
- **Purpose**: **TBC-specific** - Kara key runs, rep grinds, attunement chains
- **Example**: "LFM Black Morass for Kara key - Need healer"
- **Slowmode**: 5 seconds
- **Priority**: 🔴 CRITICAL

#### `#lfg-arenas`

- **Type**: Text (optional)
- **Purpose**: Arena team recruitment, partners
- **Priority**: 🟢 BONUS

---

## 🔴 CATEGORY: 📋 TOOLS & RESOURCES

**Purpose**: Raid support and information  
**Permissions**: @Verified can read/write (except bot-only channels)

#### `#softres-all`

- **Type**: Text (read-only for @everyone)
- **Purpose**: SoftRes.it embed posts
- **Permissions**:
    - @Verified: Read Messages
    - @SoftRes Bot: Send Messages, Embed Links
- **Priority**: 🔴 CRITICAL

#### `#warcraftlogs`

- **Type**: Text (webhook-only)
- **Purpose**: Auto-posted logs via WCL webhook
- **Permissions**: Read for @everyone, Write for Webhook only
- **Priority**: 🔴 CRITICAL

#### `#gear-checks`

- **Type**: Text
- **Purpose**: MikePy/PugBot gear verification
- **Usage**: Players post `!armory [gear string]` here
- **Slowmode**: 5 seconds
- **Priority**: 🔴 CRITICAL

#### `#guides`

- **Type**: Text or Forum Channel (read-only)
- **Purpose**: Boss strategies, consumables lists, enchants, rotation guides
- **Permissions**: @everyone: Read, @Raid Leader+: Send
- **Content to Pin**:
    - Boss strat videos (FatBoss, etc.)
    - Consumables checklist
    - Enchant priorities per slot
    - WeakAuras pack links
- **Enable**: Embeds for videos
- **Priority**: 🟡 IMPORTANT

#### `#wago-was`

- **Type**: Text
- **Purpose**: WeakAuras sharing and discussion
- **Priority**: 🟡 IMPORTANT

#### `#goldmaking`

- **Type**: Text
- **Purpose**: Farming routes, profession guides, AH flipping
- **Priority**: 🟢 BONUS

#### `#clips`

- **Type**: Text (media-heavy)
- **Purpose**: Raid highlights, funny moments, achievements
- **Starboard Integration**: Carl-bot starboard posts here
- **Priority**: 🟡 IMPORTANT

---

## 🔴 CATEGORY: 🎤 VOICE CHANNELS

**Purpose**: Voice communication for raids and socializing

### Design: Stage Channels for raids, regular voice for casual

#### `Raid Leader` (Stage Channel)

- **Type**: Stage Channel
- **Purpose**: Main raid calls (Raid Leader + Officers as speakers)
- **Permissions**:
    - @everyone: Audience (listen only)
    - @Raid Leader, @Officer: Speaker (can talk)
    - @Moderator: Request to Speak approval, mute control
- **Usage**: 25-man raids, important callouts
- **Priority**: 🟡 IMPORTANT (use regular voice if <100 members)

#### `Off-Tank 1` / `Off-Tank 2`

- **Type**: Voice Channel
- **Purpose**: Side communication for tanks, assignments
- **Permissions**: @Verified can join/speak
- **Bitrate**: 64kbps minimum (96kbps recommended)
- **Priority**: 🟡 IMPORTANT

#### `Raid Voice - Kara`

- **Type**: Voice Channel
- **Purpose**: 10-man Kara runs
- **User Limit**: 10 (enforce comp)
- **Priority**: 🔴 CRITICAL

#### `Raid Voice - 25m`

- **Type**: Voice Channel
- **Purpose**: Gruul/Mag runs
- **User Limit**: 25 (enforce comp)
- **Priority**: 🔴 CRITICAL

#### `General Voice`

- **Type**: Voice Channel
- **Purpose**: Casual hanging out
- **Priority**: 🟡 IMPORTANT

#### `AFK Lobby`

- **Type**: Voice Channel
- **Purpose**: Auto-move AFK users here
- **Settings**: Set as AFK channel (15 min timeout)
- **Priority**: 🔴 CRITICAL

#### `Music Lounge` (Optional)

- **Type**: Voice Channel
- **Purpose**: Music bot channel (keep OUT of raid voice)
- **Priority**: 🟢 BONUS

---

## 🟡 CATEGORY: 🛡️ STAFF (Hidden)

**Purpose**: Moderator/admin operations  
**Permissions**: @Moderator and above only

#### `#mod-chat`

- **Type**: Text
- **Purpose**: Officer coordination, decisions
- **Priority**: 🟡 IMPORTANT

#### `#mod-logs`

- **Type**: Text (read-only)
- **Purpose**: Auto-moderation logs (Dyno/Carl-bot)
- **Permissions**: Bots send, Mods read
- **Priority**: 🟡 IMPORTANT

#### `#tickets`

- **Type**: Text
- **Purpose**: Ticket Tool management panel
- **Priority**: 🟡 IMPORTANT (if using Ticket Bot)

#### `#vetting-logs`

- **Type**: Text
- **Purpose**: Where users post logs to get "Verified Raider" or "Pumper" role
- **Priority**: 🟢 BONUS

---

## Role Configuration

### 🔴 Role Hierarchy (Top to Bottom)

**Critical**: Roles higher in hierarchy have more power. Set carefully.

1. **@Owner** - Full permissions
2. **@Admin** - Server administration
3. **@Officer** - Event management, moderation
4. **@Raid Leader** - Event creation, role assignment
5. **@Core** - Regular raiders (invite-only, perks)
6. **@Verified** - Passed verification (unlocks channels)
7. **@70** - Level-capped players
8. **@Pumper** - High performers (optional prestige role)
9. **Class Roles** - @Warrior, @Mage, @Warlock, @Priest, @Paladin, @Druid, @Hunter, @Rogue, @Shaman
10. **Spec Roles** - @Tank, @Healer, @DPS
11. **@Horde** / **@Alliance** - Faction tags
12. **@Pug** - Temporary participants (ephemeral, optional)
13. **@Streamers** - Content creators
14. **@Muted** - Restricted from chat
15. **@Bots** - Bot accounts

---

### 🔴 Role Permissions (Critical Settings)

#### @Verified (Gatekeeper Role)

- **Granted by**: Dyno/Carl-bot after captcha
- **Permissions**:
    - Read most channels (excludes Staff)
    - Send messages in social/LFG
    - Add reactions
    - Connect to voice
    - Use voice activity
- **Purpose**: Prevents spam bots, ensures humans

#### @Raid Leader

- **Permissions**:
    - Create Events (Discord Scheduled Events)
    - Manage Messages (in #raid-signups, #lfg channels)
    - Mention @everyone (in raid channels only)
    - Move Members (voice channels)
    - Mute Members (during raids)
- **Who Gets It**: Trusted players after 3-5 successful raid leads

#### @Core

- **Permissions**: Same as @Verified
- **Perks** (via bot or manual):
    - Priority signup for raids (early access)
    - Special color in sidebar
    - Access to #core-chat (optional exclusive channel)
- **Who Gets It**: Regular raiders (10+ raids attended)

---

### 🔴 Reaction Role Panel (Carl-bot Setup)

**Location**: `#roles` channel

#### Message Content:

```
**Select Your Class & Role**

React below to assign yourself roles. This helps Raid Leaders ping the right people!

**Classes** 🏆
⚔️ = Warrior
🔮 = Mage
🔥 = Warlock
✨ = Priest
⚡ = Shaman
🌿 = Druid
🏹 = Hunter
🗡️ = Rogue
☀️ = Paladin

**Roles** 🎯
🛡️ = Tank
❤️ = Healer
⚔️ = DPS

**Faction** 🚩
🔴 = Horde
🔵 = Alliance
```

#### Carl-bot Command (in #roles):

```
!rr create
!rr add [message ID] ⚔️ @Warrior
!rr add [message ID] 🔮 @Mage
[... repeat for all classes]
!rr add [message ID] 🛡️ @Tank
!rr add [message ID] ❤️ @Healer
!rr add [message ID] ⚔️ @DPS
!rr add [message ID] 🔴 @Horde
!rr add [message ID] 🔵 @Alliance
```

**Priority**: 🔴 CRITICAL

---

### 🟡 TBC-Specific Role: @Shaman

**Why Separate Role?**

- TBC raids require 1 Shaman per 5-man group (Bloodlust/Heroism)
- Must track Resto vs Enhancement vs Elemental specs
- Different group assignments per spec

**Setup**:

- Create @Resto-Shaman, @Enhance-Shaman, @Ele-Shaman roles
- Add to reaction panel separately from general @Healer/@DPS
- Use for targeted pings: "@Resto-Shaman we need 1 more for Gruul tonight"

---

## Permission Best Practices

### 🔴 Channel Permission Templates

#### Read-Only Announcement Channel (#announcements, #rules)

- @everyone: ✅ Read Messages, ✅ Read Message History, ❌ Send Messages
- @Admin: ✅ All permissions

#### Interactive LFG Channel (#lfg-karazhan)

- @everyone: ❌ Read Messages (gated)
- @Verified: ✅ Read, ✅ Send, ✅ Add Reactions, ✅ Embed Links, ✅ Attach Files
- **Slowmode**: 10 seconds

#### Bot-Only Channel (#raid-signups, #warcraftlogs)

- @everyone/@Verified: ✅ Read, ✅ Add Reactions, ❌ Send
- @Bots: ✅ Send, ✅ Embed, ✅ Manage Messages
- @Raid Leader: ✅ Send (for manual posts)

#### Staff Channel (#mod-chat)

- @everyone: ❌ Read (hidden)
- @Moderator+: ✅ All permissions

---

## Server Settings (Essential Configuration)

### 🔴 Moderation Settings

- **Verification Level**: Medium (email required)
- **Explicit Content Filter**: Scan all members
- **DM Filter**: Enabled (filters DM spam from server)
- **2FA Requirement**: Enabled for moderators

### 🔴 Auto-Moderation (Dyno/Carl-bot)

Enable these filters:

- ✅ Mass mention spam (4+ mentions = auto-delete)
- ✅ Link spam (3+ links in 10 seconds = auto-delete)
- ✅ Zalgo text (Unicode spam)
- ✅ Repeated text (10+ same messages)
- ✅ Caps spam (80%+ caps in message)
- ✅ Emoji spam (10+ emojis)

### 🟡 Welcome Screen

Set up Community Welcome Screen:

1. Server Settings → Community → Welcome Screen
2. Enable Welcome Screen
3. Add welcome channels:
    - #rules (required read)
    - #roles (select roles)
    - #how-to-pug (quick start)
4. Add custom welcome message (50 character limit)

### 🟡 Server Boost Perks

If boosted to Level 2:

- ✅ 150 emoji slots (use for class icons)
- ✅ 1080p 60fps streaming
- ✅ Server banner
- ✅ 50MB upload limit (useful for logs/screenshots)

---

## Common Mistakes to Avoid

1. **Too Many Channels**: Don't create 50+ channels at launch. Start with 20-25, add as needed.
2. **No Verification**: Unverified servers get bot spam. Always use captcha gate.
3. **@everyone Permissions**: Never give write permissions to @everyone. Use @Verified.
4. **Ignoring Slowmode**: LFG channels without slowmode = spam hell.
5. **No AFK Channel**: Members stay in raid voice 24/7 = confusing roster.
6. **Hidden Welcome**: New members must see #rules and #roles immediately.
7. **Bot Permission Conflicts**: Set bot roles high in hierarchy (below Admin, above users).

---

## Testing Checklist (Before Launch)

- [ ] Create test account, verify full onboarding flow
- [ ] Test reaction roles in #roles (do emojis assign correctly?)
- [ ] Verify @Verified role unlocks correct channels
- [ ] Test LFG post in each #lfg channel (slowmode working?)
- [ ] Test voice channels (bitrate good? AFK timeout working?)
- [ ] Verify bots can post in their assigned channels
- [ ] Test moderation (post spam, verify auto-delete)
- [ ] Mobile test (check on phone - reaction roles work differently)

---

## Next Steps

After structure setup: → See **Bot Setup Guide** for detailed bot configuration  
→ See **Raid Organization Workflow** for raid management  
→ See **Templates Guide** for welcome messages and rules
