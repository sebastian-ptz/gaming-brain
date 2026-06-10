---
tags: [poe2, crafting, guide, overview]
date: 2026-06-10
---
## Content
- [[#Fundamentals]]
	- [[#Item Rarity & Modifier Slots]]
	- [[#Prefixes vs Suffixes]]^^
	- [[#Item Level, Mod Pools & Weights]]
	- [[#Base Types Matter]]
	- [[#Hybrid Modifiers]]
	- [[#Changing Max Prefix / Suffix Counts]]
- [[#Rolling Items – The Crafting Workflow]]
	- [[#Starting From a White Base]]
	- [[#Working a Magic (Blue) Base]]
	- [[#Working a Rare (Yellow) Base]]
	- [[#Greater & Perfect Currency Tiers]]
	- [[#When to Switch Methods]]
- [[#Ritual Omens]]
	- [[#Core Targeting Omens]]
	- [[#Greater Exaltation Omens (Double Slam)]]
	- [[#Whittling, Light & Sanctification]]
	- [[#Combining Omens]]
- [[#Abyss Desecration & Well of Souls]]
	- [[#Bone Types]]
	- [[#How Desecration Works]]
	- [[#Targeting Prefix or Suffix with Omens]]
	- [[#Replacing or Removing Desecrated Mods]]
- [[#Essences Crafting]]
	- [[#Essence Tiers]]
	- [[#Using Essences to Convert Magic to Rare]]
	- [[#Perfect & Corrupted Essences on Rares]]
	- [[#Essence Strategy Cheatsheet]]
- [[#Delirium – Liquid Emotions]]
	- [[#Enchanting with Liquid]]
	- [[#Anointing (Instilling) Amulets]]
	- [[#Best Anoint Patterns]]
- [[#Expedition – Runeforging at the Verisium Anvil]]
	- [[#Runic Ward]]
	- [[#Change Modifiers with Flux]]
	- [[#Enchanting with Alloy]]
- [[#Quality Maxing]]
- [[#Corrupting]]
	- [[#Vaal Orb Outcomes]]
	- [[#Omen of Corruption]]
	- [[#Sanctification (Divine Orb Corrupt)]]
	- [[#Pre-Corrupt Checklist]]
- [[#Profit Crafting & Tools]]
- [[#Resources & References]]

---

## Fundamentals

> Based on **GhazzyTV – "CRAFT ANYTHING YOU WANT! – PoE2 Beginner to Advanced Crafting Guide"** ([video](https://www.youtube.com/watch?v=HfFkmE_t4SA)). The principles below are the backbone for every other section.

### Item Rarity & Modifier Slots

| Rarity | Max Modifiers | Notes |
|--------|---------------|-------|
| **White (Normal)** | 0 | A "base" – the canvas for crafting. |
| **Magic (Blue)** | 1 prefix + 1 suffix | Cheap experimentation tier. |
| **Rare (Yellow)** | 3 prefixes + 3 suffixes (6 total) | Endgame target. |
| **Unique** | Fixed | Not craftable in the same way. |

**Rarity is a one-way street in PoE 2.** Once you upgrade White → Magic → Rare, you cannot go back. There is **no Orb of Scouring**. Plan carefully *before* you Regal/Alch.

### Prefixes vs Suffixes

Every modifier in the game belongs to either the **prefix** pool or the **suffix** pool. They are drawn from completely separate pools — this is the foundation of deterministic crafting.

- **Prefixes** = the "big stats". On weapons: phys/elemental damage, spirit, %spell damage. On armor: life, mana, %ES/Eva/Armor, flat ES.
- **Suffixes** = utility. Resistances (always suffix), attributes, attack/cast speed, crit chance/damage, regen.

> **Key insight:** If your item has 3/3 prefixes and 1/3 suffixes, your next Exalted Orb is *guaranteed* to add a suffix (e.g. a resistance). Look at the open pool **before** you spend currency.

You can never have two *identical* modifiers on the same item.

### Item Level, Mod Pools & Weights

Hover an item and hold **Alt** to see the **item level (iLvl)**. iLvl gates which tier of modifier can roll — it is **not** the required level for equipping.

- A `Rattling Sceptre iLvl 82` can roll the highest tier of every modifier it has access to.
- The same base at iLvl 76 cannot roll T1 `%Spirit` (needs iLvl 81) and cannot roll `+4 Level of Minion Skills` (needs iLvl 78).

Every modifier has a **weight** that determines the chance of hitting it inside the open pool. On a sceptre, `Mana` rolls have weight ~1000 while `%Spirit` has weight ~50 — random Augment Orbs are ~20× more likely to land on mana than spirit.

> Always use **[Craft of Exile (PoE 2)](https://www.craftofexile.com/?game=poe2)** to look up exact weights, T1 iLvl gates, and the prefix/suffix split for any base.

### Base Types Matter

Defensive bases gate which defensive mods can roll:

- **Pure Armor** → armor mods
- **Pure Evasion** → evasion mods
- **Pure ES** → energy shield mods
- **Hybrid (Armor/Eva, Eva/ES, Armor/ES)** → both sub-pools available, plus hybrid lines (e.g. `+%Armor and Evasion`)

Suffixes are basically identical across most bases. So your base choice mostly dictates the **defensive prefix pool**.

For **weapons**: choose the base whose iLvl-gated T1 mods match your build (e.g. minion builds buy `+4 minion skills` sceptre bases *before* crafting on them, because that mod has weight 100 and is very rare to slam).

### Hybrid Modifiers

A hybrid modifier is **one** prefix or suffix that gives **two stats** at slightly reduced values. Example: body armor can roll `+X% Armor and Evasion AND +Y Maximum Life` as a single prefix.

Because it occupies only **one** slot, you can still roll a separate flat `+Maximum Life` prefix next to it — letting you "double dip" on the same stat from two mods.

If you hold Alt and see *two lines* of "increased maximum life", that's why.

### Changing Max Prefix / Suffix Counts

The base maxima (3 prefixes / 3 suffixes) are mostly fixed by rarity, but a few mechanics interact with them:

- **Corruption / Vaal Orb**: certain corrupted *implicits* can appear "above" all six normal mods. These don't increase the cap; they slot into the implicit line above your rolled mods.
- **Sockets / Runes / Soul Cores**: runes occupy *sockets* — separate from prefix/suffix slots — and provide additional stats. Use **Lesser / Greater Jeweller's Orb** to add sockets to items.
- **Crafted/Essence/Alloy mod**: only **one** essence-/alloy-/desecration-applied modifier can exist at a time (the teal-coloured mod). It still counts toward your prefix/suffix max.
- **Fractured modifier**: a *fractured* mod still occupies a slot, but is locked in place forever (immune to Chaos / Annulment / Desecration removal).

So while the cap is always 3/3, the **effective** "stat budget" of an item grows via implicits (corrupt), socket-based stats (runes / soul cores), and quality.

---

## Rolling Items – The Crafting Workflow

### Starting From a White Base

1. **Pick the right base** – correct armor type, iLvl high enough to roll the T1 mods you want (check Craft of Exile).
2. **Orb of Transmutation** → Magic (1 mod) – cheap and the standard opener.
3. **Orb of Augmentation** → adds the 2nd mod to a magic item.
4. (Optional) Roll/swap the magic item with **Orbs of Alteration / Annulment** if needed.
5. **Regal Orb** → upgrades Magic → Rare and adds 1 new random mod, **OR**
6. **Essence** instead of Regal → upgrades Magic → Rare with a **guaranteed targeted** mod (see [[#Essences Crafting]]).
7. **Exalted Orb** → fill remaining open slots (up to 6 mods). Use **Omens** here for prefix/suffix targeting.

> *GhazzyTV's typical workflow:* `Transmute → Augment (Greater/Perfect for iLvl gating) → Essence to Rare → Desecrate one side → Greater Exalt slam with Omen of Greater Exaltation → Reveal → Sell/equip.`

### Working a Magic (Blue) Base

If you find a blue item with 1 great stat:

- **1 open slot** → use **Augmentation** (regular, Greater, or Perfect) to get the second mod.
- **Both mods bad** → annul/alteration to reroll (cheap).
- **Once happy** → **Regal** or **Essence** to convert to Rare.

> Buying a Magic base with one perfect rare mod (e.g. `+4 minion skills`) on the trade site is one of the most efficient ways to skip RNG. Then craft on it.

### Working a Rare (Yellow) Base

Rare items have **no Scouring**. Your options:

| Currency | Effect | Best for |
|----------|--------|----------|
| **Exalted Orb** | Adds 1 random modifier to an open slot. | Filling slots, use omens for control. |
| **Chaos Orb** | Removes 1 random mod and adds 1 random mod (a swap — **not** a full reroll). | Surgical mod swaps (use **Omen of Whittling** for lowest tier). |
| **Orb of Annulment** | Removes 1 random mod. | Clean up; pair with fractured base or omens. |
| **Divine Orb** | Rerolls the *numeric values* of existing mods within their tier range. | Final stat polish. |
| **Essence (Greater/Perfect/Corrupted)** | Swap a random mod for a guaranteed mod. | Targeted upgrades. |
| **Abyssal Bone (Desecration)** | Add a desecrated mod chosen from 3 random options at the Well of Souls. | Special / Abyss-exclusive mods. |
| **Alloy (Verisium Anvil)** | Removes 1 random mod, adds a guaranteed item-type-specific mod. | Runeforging mods (Runic Ward, AoE, Spirit, etc.). |
| **Flux** | Swap a random mod toward an element/theme. | Realigning elemental damage/res rolls. |
| **Vaal Orb** | Corrupt for an implicit/socket/quality, but locks the item. | End-of-craft gamble. |

### Greater & Perfect Currency Tiers

Greater and Perfect versions of `Augmentation / Regal / Exaltation` add a **"minimum modifier level"** line. The added mod *cannot* be below that level — so you skip the trash low-tier outcomes.

| Currency | Minimum Mod Level |
|----------|-------------------|
| Greater Orb (Aug/Regal/Exalt) | 44 |
| Perfect Orb (Aug/Regal/Exalt) | 70 |

**When to use:**
- **Regular orb** → cheap throwaway bases.
- **Greater orb** → mid-tier bases worth a few divines.
- **Perfect orb** → end-game bases where you cannot afford a T8 mana slam. Pair with the corresponding **Omen of Greater Exaltation** for huge currency savings.

### When to Switch Methods

| Situation | Use |
|----------|-----|
| Cheap upgrade / campaign / yellow maps | Transmute–Aug–Regal, then Exalt slam |
| Need a guaranteed stat | **Essence** (replaces the Regal step) |
| Near-perfect item with one bad slot | **Chaos + Omen of Whittling + Sinistral/Dextral Erasure** |
| Empty prefix or suffix to fill safely | **Exalted + Sinistral/Dextral Exaltation Omen** (Greater Exaltation Omen for 2 at once) |
| You want an Abyssal exclusive (Kurgal/Ulaman/Amanamu, Otherworldly, etc.) | **Desecration with Bones** (+ Necromancy Omens) |
| Final stat-rolls polish | **Divine Orb** |
| Push above 20 quality / get extra socket / corrupt implicit | **Vaal Orb (+ Omen of Corruption)** |
| Push numeric values past max | **Omen of Sanctification + Divine Orb** |

---

## Ritual Omens

> Omens are sourced exclusively from **Ritual** (bought with Tribute). They modify the behaviour of the **next applicable currency** you use. Right-click to "activate"; the omen lights up under your inventory.

### Core Targeting Omens

| Omen | Effect |
|------|--------|
| **Omen of Sinistral Exaltation** | Next Exalted Orb adds only a **Prefix**. |
| **Omen of Dextral Exaltation** | Next Exalted Orb adds only a **Suffix**. |
| **Omen of Sinistral Annulment** | Next Annulment removes only a **Prefix**. |
| **Omen of Dextral Annulment** | Next Annulment removes only a **Suffix**. |
| **Omen of Sinistral Erasure** | Next Chaos Orb only removes/adds **Prefixes**. |
| **Omen of Dextral Erasure** | Next Chaos Orb only removes/adds **Suffixes**. |
| **Omen of Sinistral Coronation** | Next Regal Orb adds a **Prefix** mod. |
| **Omen of Dextral Coronation** | Next Regal Orb adds a **Suffix** mod. |
| **Omen of Sinistral Crystallisation** | Next Perfect/Corrupted Essence removes only a **Prefix**. |
| **Omen of Dextral Crystallisation** | Next Perfect/Corrupted Essence removes only a **Suffix**. |
| **Omen of Sinistral Necromancy** | Next Desecration adds a **Prefix** desecrated mod. |
| **Omen of Dextral Necromancy** | Next Desecration adds a **Suffix** desecrated mod. |

### Greater Exaltation Omens (Double Slam)

- **Omen of Greater Exaltation** → next Exalt (regular/Greater/Perfect) adds **2 modifiers** in one slam.
- Combine with `Sinistral/Dextral Exaltation` for **2 prefixes** or **2 suffixes** in one slam.

> *GhazzyTV currency-saving example:* a Greater Exalt costs ~10 ex, the Greater Exaltation Omen ~3 ex. Two separate Greater slams = 20 ex; **one Greater slam + Omen = ~13 ex** for the same effect.

### Whittling, Light & Sanctification

| Omen | Effect |
|------|--------|
| **Omen of Whittling** | Next Chaos Orb removes the **lowest-tier modifier** (not random). Perfect for fixing a near-perfect item. |
| **Omen of Light** | Next Annulment removes the **desecrated** modifier specifically. Used to "reset" the Well of Souls slot. |
| **Omen of Sanctification** | Next **Divine Orb** sanctifies the item: every modifier value × 78–122 %. Item becomes uncraftable. How `+4 minion` sceptres become `+5`. |
| **Omen of the Ancients** | Influences high-end / Audience-with-the-King rituals. |
| **Omen of Abyssal Echoes** | At the Well of Souls, **rerolls** the 3 displayed options (one-time). |
| **Omen of Corruption** | Removes the "nothing happens" Vaal outcome (see [[#Corrupting]]). |

### Combining Omens

Multiple omens can be active simultaneously. Powerful stacks:

| Stack | Result |
|-------|--------|
| `Greater Exaltation + Sinistral Exaltation` | **+2 prefixes** in one Exalt slam |
| `Greater Exaltation + Dextral Exaltation` | **+2 suffixes** in one Exalt slam |
| `Whittling + Sinistral Erasure` | Chaos Orb removes the lowest **prefix** only |
| `Whittling + Dextral Erasure` | Chaos Orb removes the lowest **suffix** only |
| `Dextral Necromancy + Abyssal Echoes` | Guaranteed suffix desecration + reroll the 3 options |
| `Sinistral Crystallisation + Perfect Essence` | Perfect Essence only removes a prefix to inject its mod |

---

## Abyss Desecration & Well of Souls

Desecration uses **Abyssal Bones** (currency) to inject a hidden modifier into an item. You then visit the **Well of Souls** in your hideout/Ziggurat to **reveal** the mod, choosing **1 of 3** random options.

### Bone Types

Bone type is matched to the **item slot** and the **quality tier**:

| Bone | Slot Targeted |
|------|---------------|
| **Cranial** (Skull) | Helmets |
| **Vertebrae** | Body Armor |
| **Rib** | Gloves / Boots |
| **Jawbone** | Weapons / Sceptres |
| **Collarbone** | Amulets, Rings, Belts (jewellery) |
| **Femur** | Larger gear segments |

Quality / tier ladder:

| Quality | Effect |
|---------|--------|
| **Gnawed** | Only works up to **iLvl 64** (campaign tier). |
| **Preserved** | Standard endgame bone, no iLvl cap on Rares. |
| **Ancient** | Guarantees a **minimum modifier level of 40** (higher-tier outcomes). Expensive. |
| **Altered** (e.g. Altered Collarbone) | Adds a chance for **league-exclusive Abyssal modifiers** (Kurgal / Ulaman / Amanamu, Otherworldly Breach mods). Premium currency – ~98 ex per Altered Collarbone in 0.5. |

### How Desecration Works

1. Use a Bone on a Rare item → the bone removes a random modifier (only if the item is full on the matching side) and adds an **unrevealed desecrated modifier**.
2. If there is an open slot of the matching type, **nothing is removed** — the desecrated mod just slots in.
3. Walk to the **Well of Souls**, drop the item in, click **Reveal** → choose **1 of 3** random modifier options.

> Some Abyss-exclusive mods (Kurgal, Ulaman, Amanamu names) can **only** be obtained through desecration.

### Targeting Prefix or Suffix with Omens

- **Sinistral Necromancy** → forces the next desecration to add a **prefix**.
- **Dextral Necromancy** → forces the next desecration to add a **suffix**.
- If your item is **full on the targeted side**, the bone will **remove a mod from that side** — use this on purpose to clear a mod you don't want (without risking the other side).

> *GhazzyTV's `+2 minion belt` craft:* he wanted to swap a prefix, so he used **Sinistral Necromancy + Preserved Vertebrae** to force the bone to remove a prefix and replace it with a desecrated prefix, protecting his suffixes.

### Replacing or Removing Desecrated Mods

- **Omen of Light + Orb of Annulment** → guaranteed to remove the desecrated mod (clean retry without affecting other mods).
- **Fracture trick:** Fracture the item **before unveiling** the desecrated mod. Fracturing requires the item to have ≥4 mods but it **cannot fracture an unrevealed desecrated modifier**. This raises your chance of fracturing the *good* mod from 1/4 → 1/3.
- **Essence over a desecrated mod:** Essences remove a random mod of *their* affix type to add their guaranteed mod. So a *prefix-essence* on an item with full prefixes will erase a prefix (possibly your desecrated one). Use **Sinistral/Dextral Crystallisation Omens** with Perfect/Corrupted essences to keep the desired side safe.

---

## Essences Crafting

Essences are the most common deterministic crafting tool in PoE 2. There are **19 essence "types"** (Body, Command, Thawing, Insulation, Grounding, Sorcery, Enhancement, Battle, the Mind, the Infinite, Haste, etc.), each tied to a stat family.

### Essence Tiers

| Tier | What it does | Best use |
|------|--------------|----------|
| **Lesser** | Magic → Rare with 1 guaranteed low-tier mod. | Campaign filler. |
| **Normal** | Magic → Rare with 1 guaranteed mid-tier mod. | Early mapping. |
| **Greater** | Magic → Rare with 1 guaranteed **high-tier** mod (≥ T2). | The bread-and-butter for endgame crafting. |
| **Perfect** | On a **Rare** item: removes 1 random mod, adds 1 guaranteed *unique* mod (often a mod that can ONLY come from Perfect Essences). | Fix a near-perfect item with one specific high-end mod. |
| **Corrupted** | On a Rare item: removes 1 random mod, adds a guaranteed corrupted mod. **Locks the item** from further crafting. | End-of-craft enhancer (like a Vaal). |

> **0.5.0 change:** Each piece of equipment can only have **one essence-applied modifier** at a time (the small teal "crafted" coloured mod). Once present, you cannot apply another essence-class craft to that item.

### Using Essences to Convert Magic to Rare

This is the **alternative to a Regal Orb**. Workflow:

1. Get a Magic item with a great prefix or suffix already (Transmute + Augment, or buy a magic base).
2. Apply a **Greater Essence** for the stat you want guaranteed (e.g. `Greater Essence of Command` on a sceptre → guaranteed `Allies in your Presence deal 75–89% increased Damage` prefix).
3. The item is now Rare with 2 mods (your original + the essence mod), one flagged as the essence-crafted mod.
4. Fill the remaining 4 slots with **Exalted Orbs + Omens** or **Desecration**.

### Perfect & Corrupted Essences on Rares

These work *backwards*: **remove first, then add**. Because they remove a random mod, you risk losing a good mod unless you protect the side they target.

- If the essence adds a **prefix**, the item will remove a random prefix to make room (or remove a random suffix if all prefixes are open — but that's rare in practice).
- Better: use **Sinistral/Dextral Crystallisation Omens** to force the removal to a specific side.

### Essence Strategy Cheatsheet

| Goal | Essence to look at |
|------|--------------------|
| Guaranteed life | **Essence of the Body** |
| Resistances | **Essence of Thawing** (cold), **Insulation** (fire), **Grounding** (lightning) |
| Spirit / minion damage | **Essence of Command**, **Essence of the Mind** |
| Flat ES / Armor / Evasion | **Greater Essence of Enhancement** (up to 80 % AR/Eva/ES) |
| Attack speed / crit | **Essence of Battle**, **Essence of Haste** |
| Special endgame mods | **Perfect Essences** only |

> Greater Essence of Command is ~1 ex; Essence of the Body ~7 ex. They're extremely cheap relative to slamming Exalts — always essence first, slam later.

---

## Delirium – Liquid Emotions

In **0.5+** the old **Distilled Emotions** were reworked into **Liquid Emotions** with two distinct uses: **enchanting jewels/gear** and **anointing amulets**.

### Enchanting with Liquid

Liquid Emotions can now be used **like a Perfect Essence** on **Jewels** (and certain other items): they remove 1 random modifier and add a guaranteed enchant tied to the emotion type **and** the jewel base.

**Example outcomes** (from GhazzyTV — on a Sapphire Jewel):

| Liquid Emotion | Adds |
|----------------|------|
| **Liquid Iron** | Increased **Energy Shield** (prefix) |
| **Liquid Ice** | Cold Damage |
| **Liquid Suffering** | Chaos Damage |
| **Liquid Greed** | Cast Speed |
| **Liquid Disgust** | Mana Cost → Life Cost conversion |
| **Liquid Envy** | Critical strike modifiers |
| **Liquid Despair** | Damage over time |
| **Liquid Isolation** | Minion modifiers |

> Each emotion's effect depends on the **jewel base** (Sapphire/Ruby/Emerald/etc.) **and the item type**. Look it up in Craft of Exile before slamming.

**When is this useful?**
- You found a Jewel with 3 valuable mods and one trash mod — Liquid Emotion can swap the trash for a stat the jewel base supports.
- **Price example from GhazzyTV:** a `crit damage + minion damage + cold pen + minion attack speed` Sapphire worth ~40 ex jumped to **~2 div** after applying Liquid Iron because the jewel base then rolls energy shield mods.

**Best enchants depend on your build:**
- Minion ES build → **Liquid Iron** on a Sapphire (% ES).
- Crit build → **Liquid Envy** for crit chance/damage.
- DoT build → **Liquid Despair**.
- Skill/aura cost build → **Liquid Greed** (cast speed) or **Liquid Disgust** (life cost).

**Obtaining & upgrading Liquid Emotions:**
- Drop from **Delirium** encounters (Waystone fog) and **Simulacrums**. The reward counter fills as you kill in the fog.
- **Reforging Bench:** 3 emotions of one tier → 1 emotion of the next higher tier.

### Anointing (Instilling) Amulets

Anointing — officially called **Instilling** — adds a **Notable Passive Skill** to an amulet using exactly **3 Liquid Emotions** in a specific recipe.

**Workflow:**
1. Open the Passive Tree, hover the Notable you want, hold **Alt** → the recipe (3 emotion types) is shown.
2. Right-click any Liquid Emotion → opens the Instilling Bench.
3. Place the amulet + the 3 emotions → press **Instil**.
4. The amulet now grants that notable as if allocated on the tree.

### Best Anoint Patterns

Anointing decisions are build-specific, but high-value anoints come from notables that are **deep on the tree** or **expensive to path to** — anoint shortcuts the route.

Common high-value anoints:

| Notable | Why |
|---------|-----|
| **Heart of the Warrior** | +15 % maximum life |
| **Sovereignty** | Aura/reservation efficiency |
| **Resonance** | Elemental damage |
| **Ironwood** | Armor/life hybrid |
| **Charisma** / **Influence** | Aura sizing |
| **Resourcefulness** | Mana/regen |
| **Pain Attunement** | Spell damage at low life |

> Look up your build's **Recommended Anoint** in Maxroll/Mobalytics guides. Use [PoE2 Trade](https://www.pathofexile.com/trade2) anoint filters to see what top-tier amulets are running.

---

## Expedition – Runeforging at the Verisium Anvil

In **0.5 (Runes of Aldur)**, the Kalguuran expedition mechanic merged with runecrafting. After Act 4 you can use the **Verisium Anvil** with **Verisium** currency.

### Runic Ward

**Runic Ward** is a defensive buffer: when your HP would drop to 1, it absorbs incoming damage and regenerates at 5 % per second by default. It's a "last line of defence" layer that gives you time to recover.

**Where you can apply it:** non-Unique **Helmets, Body Armor, Gloves, Boots, Shields** via the Verisium Anvil.

**Cost in defenses (the trade-off you noticed):**

| Item Level | Defense Penalty |
|------------|-----------------|
| **Below iLvl 55** | Runic Ward is added with **no penalty**. Free upgrade. |
| **iLvl 55+** | Applying Runic Ward **reduces** some of the item's existing **Evasion Rating and/or Energy Shield** (and on Armor-heavy bases, some Armor). The reduction scales with iLvl and the size of the Runic Ward added. |

**How the reduction is calculated:**
- The engine essentially "converts" a slice of base defense into Ward.
- The amount removed scales with **base item level** and the **Ward magnitude**.
- On **Pure-ES gear** it tends to chew ES; on **Pure-Eva** it eats Evasion; on **hybrid pieces** it spreads across both stats; on Pure-Armor it shaves Armor.
- Concrete example: applying Runic Ward to an **Austere Garb** costs **470 Verisium** and removes some of the evasion in exchange for substantial Runic Ward.

> **Does it always happen?** Below iLvl 55 it never happens. **At iLvl 55+ it always happens** — there is no "lucky" Runeforge that doesn't take defenses on a high-iLvl item.

**When is Runic Ward worth applying?**
- **Mandatory** for builds that *consume* Runic Ward as a resource (Kalguuran skills).
- **Strongly worth it** for squishy ranged/ES/Eva builds that want an extra "oh-shit" buffer.
- **Skip** in early Act 1 — base defenses scale more linearly there, and the Anvil isn't unlocked yet anyway.
- For endgame: **quality the item first**, then **runeforge Runic Ward**, then fill remaining sockets with runes.

### Change Modifiers with Flux

**Flux Orbs** (Chilling, Blazing, Crackling, Void) swap modifiers on an item toward that element/theme. Each Flux is crafted from specific Rune combinations at the Anvil:

| Flux | Rune Recipe |
|------|-------------|
| **Chilling** | Cold + Cyclonic + Prismatic + Death + Tidal + Moon |
| **Blazing** | Fire + Earth + Prismatic + Soul + Rage + Rebirth |
| **Crackling** | Lightning + Celestial + Prismatic + Electrocuting + Oath + Tempest |
| **Void** | Toxic + Time + Adaptive + Soul + Power + Death |

**When is Flux useful?**
- You found a rare item with one "wrong-element" roll (e.g. an Ignite build has a strong piece that rolled `+Cold Damage to Spells`) — Flux can realign it.
- Repairing a resistance you don't need (e.g. swapping `+Fire Res` you're already capped on toward another mod theme).
- **Best on items that already have one strong static mod + an unwanted elemental roll** — you keep what's good and remix the bad.

### Enchanting with Alloy

**Alloys** are item-type-specific enchant currencies that **remove 1 random mod and add a guaranteed mod** tied to the alloy. They work like a Perfect Essence but for **runeforging mods** (Runic Ward, Spirit, AoE, etc.).

| Alloy | Helmet | Body | Gloves | Boots | Ring | Amulet | Belt |
|-------|--------|------|--------|-------|------|--------|------|
| **Runic Alloy** | – | – | – | – | Max Runic Ward (flat) | %Max Runic Ward | Runic Ward Regen |
| **Mystic Alloy** | Spell AoE | – | Attack AoE | Flat Spirit | – | – | – |
| **Stout Alloy** | Armor/ES | Armor | Armor/Life | – | – | – | – |

(Larger pool exists – check Craft of Exile or [poe2db](https://poe2db.tw/) for the complete list.)

**When are alloys useful?**
- You need a **specific runeforge mod** you can't get any other way (e.g. flat Spirit on boots, Spell AoE on helmet).
- Polishing a near-perfect rare to push it into "godly" tier.

**Best practices:**
- Only **one** crafted/Alloy mod can exist per item. Pick the highest-impact slot.
- Combine with **Sinistral/Dextral Crystallisation Omens** to control which side the removal lands on (Alloys behave like Essences for this).
- Alloys are unlocked after **Farrow's quest in Act 2**; they drop from **Remnants** afterwards.

---

## Quality Maxing

Quality is a separate stat (cap **20 %** without corruption) that boosts the base values of an item.

| Item Group | Quality Currency | Effect |
|------------|------------------|--------|
| **Martial Weapons** (sword, mace, bow, etc.) | **Blacksmith's Whetstone** | +1 % base physical damage per quality % (max +20 %). |
| **Armor** (helm, body, gloves, boots) | **Armorer's Scrap** | +1 % to base armor/evasion/ES per quality %. |
| **Caster Weapons / Wands / Sceptres** | **Arcanist's Etcher** | +1 % to caster mods per quality %. |
| **Flasks** | **Glassblower's Bauble** | +1 % to flask effect per quality %. |
| **Gems** | **Gemcutter's Prism** | +1 % gem stat scaling per quality %. |
| **Jewelry (Rings/Amulets/Belts)** | **Catalysts** (drop from Breach) | Quality scales a **specific mod type** based on catalyst; only 1 catalyst type per item — applying another resets quality to 0. |

**Without corrupting:** the cap is **20 %**.

**Steps to 20 %:**
1. Save quality currency until you have an endgame keeper.
2. Pour 3–6 Whetstones / Scraps / etc. into the item (higher iLvl needs more).
3. **Salvage Bench** (unlocked from Renly's *"Finding the Forge"* quest in Act 1) lets you **recover quality currency** from items with quality on them — efficient farming method.

**Catalysts (jewelry):**

| Catalyst | Boosts |
|---------|--------|
| **Xoph's Catalyst** | Fire mods |
| **Tul's Catalyst** | Cold mods |
| **Esh's Catalyst** | Lightning mods |
| **Uul-Netol's Catalyst** | Physical / Chaos mods |
| **Chayula's Catalyst** | Chaos mods |
| **Abrasive Catalyst** | Attack mods |
| **Tempering Catalyst** | Defence mods |
| **Imbued Catalyst** | Caster mods |
| **Prismatic Catalyst** | Resistance mods |
| **Fertile Catalyst** | Life / Mana mods |

Match the catalyst to your **most valuable mod** on the piece.

> Always **quality before you corrupt** — corruption locks the item.

---

## Corrupting

Corruption is the final gamble. It permanently locks the item from further crafting but can produce game-changing implicits, sockets, or quality boosts.

### Vaal Orb Outcomes

A Vaal Orb on an item rolls **one** of these (roughly equal probability before omens):

1. **Nothing happens** (most "feels-bad" outcome). Item is still corrupted and uncraftable.
2. **Add a corrupted implicit** (special mod that goes above all existing affixes — e.g. `+1 to all Skill Gems`, `Cannot be Frozen`).
3. **Reroll all modifiers** as a new random Rare (essentially a Chaos-spam reset).
4. **Add or modify a socket** (can exceed the natural socket cap — huge for martial weapons & body armor when Greater Jeweller's Orbs are expensive).
5. **Quality change ±10 %** (can push past 20 %, capped at **23 %**).

### Omen of Corruption

Activate the **Omen of Corruption** before slamming a Vaal Orb. It **removes the "nothing happens" outcome** entirely. ~60 % of remaining outcomes become positive (socket / implicit). This is the **single biggest QoL upgrade** for any meaningful Vaal slam.

### Sanctification (Divine Orb Corrupt)

- **Omen of Sanctification + Divine Orb** → randomly multiplies every numeric mod value by **78–122 %**.
- Locks the item from all further crafting (like a Vaal).
- Top-end push: this is how `+4 minion skill` sceptres become `+5 minion skill` sceptres (the multiplier crosses the integer breakpoint).
- Use it as the **very last step** when you're satisfied with mods, sockets, and quality — and just want bigger numbers.

### Pre-Corrupt Checklist

Before you Vaal, make sure you've done **all of**:

- [ ] **Filled every modifier slot** with Exalted Orbs (you cannot add mods after corrupting).
- [ ] **Capped quality** (20 %) via Whetstones/Scraps.
- [ ] **Socketed all rune sockets** you intend to use (Greater Jeweller's Orbs, then Soul Cores / Runes installed).
- [ ] **Applied Runic Ward** if relevant.
- [ ] Considered **Sanctification** instead if you only want to push numbers and you're satisfied with mods/sockets.
- [ ] (Optional) Activate **Omen of Corruption** for the slam.
- [ ] Accept that the item may brick. Only Vaal items you can replace or are gambling for an upgrade.

> Best targets: high-iLvl unique pieces with valuable corrupt implicits, maxed rare weapons / body armor for extra sockets, gems for +1 level / +23 % quality.

---

## Profit Crafting & Tools

A few takeaways from GhazzyTV on profit-crafting:

- **Don't ask "what should I craft for profit"** — once a strategy is public, the margin disappears. Instead, learn the meta and identify what **current top builds** are buying.
- Use **[poe.ninja](https://poe.ninja) → Builds → (current league, e.g. Runes of Aldur)** to see top players' gear. **Ctrl-click multiple players of the same Ascendancy** to compare their rares and find common patterns (e.g. their boots all have Evasion/ES + deflection rating + attribute suffixes, no movement speed).
- **Buy a cheap Magic base with 1 perfect prefix or suffix**, then craft on top: Essence → Desecration → Greater Exalt with Omen of Greater Exaltation → Reveal → Sell.
- **Static cost** = the price of the base. **Dynamic cost** = currency you spend during crafting. If `static + dynamic < market floor for the target outcome`, you have a profitable craft.
- Don't waste quality / sockets when selling — the buyer can do it. Sell the rare unfinished.

### Tools You Should Bookmark

| Tool | Use |
|------|-----|
| **[Craft of Exile (PoE 2)](https://www.craftofexile.com/?game=poe2)** | Mod pools, weights, iLvl gates, prefix/suffix split. The **Emulator** lets you simulate Transmute/Aug/Regal/Essence/Exalt/Desecration **without spending real currency** — the best free crafting trainer. |
| **[poe.ninja](https://poe.ninja)** | Economy, top builds, item pricing, league trends. |
| **[PoE2 Trade Site](https://www.pathofexile.com/trade2)** | Buying bases, price checking. |
| **[poe2db](https://poe2db.tw/)** | Complete modifier database (needed for Abyss desecrated mod lookup — no in-game browser). |
| **[Maxroll PoE2 Crafting Hub](https://maxroll.gg/poe2/resources/path-of-exile-2-crafting-overview)** | Mechanic explainers and crafting recipes. |
| **[Exiled Exchange 2](https://github.com/Kvan7/Awakened-PoE-Trade-PoE2)** | In-game price-check overlay. |

---

## Resources & References

### Primary video reference
- **GhazzyTV – "CRAFT ANYTHING YOU WANT! – PoE2 Beginner to Advanced Crafting Guide"** – https://www.youtube.com/watch?v=HfFkmE_t4SA *(transcript pulled and condensed throughout this note)*

### Other video guides
- DarthMicrotransaction – Currency & Crafting Tier Lists
- Zizaran / Captain Lance – Endgame Crafting deep-dives
- Tripolarbear / Subtractem – PoE 2 league-launch crafting overviews
- Goratha – Quality-of-life crafting tricks (when each currency wins)

### Web references used in this document
- [Path of Exile 2 Crafting Overview – Maxroll](https://maxroll.gg/poe2/resources/path-of-exile-2-crafting-overview)
- [PoE 2 Patch 0.5.0 Crafting Meta – Essences + Omens](https://www.poecurrency.com/news/poe-2-patch-0-5-0-new-crafting-meta-how-to-guarantee-prefixes-with-essences-omens)
- [PoE 2 Abyss Crafting Guide – Mobalytics](https://mobalytics.gg/poe-2/guides/abyss-crafting)
- [Abyss Resource – Maxroll](https://maxroll.gg/poe2/resources/abyss)
- [PoE 2 Omen Guide – Mobalytics](https://mobalytics.gg/poe-2/guides/omen-crafting)
- [PoE 2 Essences Guide – Mobalytics](https://mobalytics.gg/poe-2/guides/essences)
- [PoE 2 Distilled / Liquid Emotions – Mobalytics](https://mobalytics.gg/poe-2/guides/distilled-emotions)
- [Runeforging Guide – misti.services](https://misti.services/blog/poe-2-runeforging-guide)
- [Runeforging Guide – Fextralife wiki](https://pathofexile2.wiki.fextralife.com/Runeforging+Guide)
- [Vaal Orb Corruption Outcomes – Maxroll](https://maxroll.gg/poe2/resources/corruption-outcomes)
- [PoE 2 Item Quality Ultimate Guide – mmojugg](https://www.mmojugg.com/news/poe2-item-quality-mastery-guide-2025.html)
- [Craft of Exile (PoE 2)](https://www.craftofexile.com/?game=poe2)

### Related vault notes
- [[01 Path of Exile/Path of Exile 2/Builds/Build Planner.md]]
- [[01 Path of Exile/Path of Exile 2/Builds/Path of Building.md]]
