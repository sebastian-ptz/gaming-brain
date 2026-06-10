---
tags:
  - poe1
  - crafting
  - guide
  - overview
date: 2026-06-10
---

# Crafting Overview – Path of Exile 1

> PoE 1 crafting is **significantly more complex than PoE 2** because of the many overlapping deterministic mechanics (Crafting Bench, Harvest, Beast Imprints, Fossils, Metamods, Awakener's Orb, Eldritch implicits, Veiled mods, Memory Strands…). This document is the launch-pad reference for the whole crafting toolbox; deeper guides per mechanic live in their own notes.

---
## Content
- [[#Fundamentals]]
	- [[#Item Anatomy]]
	- [[#Rarity & Affix Limits]]
	- [[#Prefixes vs Suffixes]]
	- [[#Item Level, Mod Tiers & Weights]]
	- [[#Base Items & Defensive Pools]]
	- [[#Local vs Global Modifiers]]
	- [[#Special Modifier Types]]
- [[#Currency Orbs – The Building Blocks]]
- [[#Crafting Bench (Master Crafts)]]
	- [[#Multimod]]
	- [[#Metamods – Prefixes/Suffixes Cannot Be Changed]]
	- [[#Bench Blocking]]
	- [[#Socket, Link & Colour Crafts]]
- [[#Essences]]
	- [[#Essence Tiers]]
	- [[#Essence Workflows]]
- [[#Fossils & Resonators]]
	- [[#Resonator Tiers]]
	- [[#Most Useful Fossils]]
	- [[#Common Fossil Combos]]
- [[#Harvest Crafting]]
	- [[#Lifeforce Types]]
	- [[#Best Harvest Crafts]]
	- [[#Harvest + Metamod Workflow]]
- [[#Beastcrafting]]
	- [[#Imprint (Magic Item Snapshot)]]
	- [[#Aspect Skills]]
	- [[#Split Beast & Other Recipes]]
- [[#Influence & Awakener's Orb]]
	- [[#Influence Types]]
	- [[#Awakener's Orb Rules]]
	- [[#Conqueror Exalted Slams]]
- [[#Eldritch Crafting (Searing Exarch & Eater of Worlds)]]
	- [[#Ember & Ichor Tiers]]
	- [[#Orb of Conflict]]
	- [[#Eldritch Chaos/Exalt/Annul]]
- [[#Veiled Crafting (Betrayal & Aisling T4)]]
	- [[#Unveiling]]
	- [[#Aisling T4 Bench Slam]]
- [[#Vaal Corruption]]
	- [[#Vaal Orb on Items]]
	- [[#Gem Corruption + Doryani's Institute]]
	- [[#Temple Altar of Corruption (Double Corrupt)]]
	- [[#Tainted Currency]]
- [[#Quality Maxing]]
	- [[#Standard Quality Currencies]]
	- [[#Catalysts (Jewellery)]]
- [[#Memory Strands (Current 3.28 Mirage)]]
	- [[#Petals & Memory Threads]]
	- [[#Orb of Remembrance & Orb of Unravelling]]
	- [[#How to Use Strands in Crafting]]
- [[#Utility Flask Crafting]]
	- [[#Base Flask Rolling]]
	- [[#Instilling Orb – Auto-Triggers]]
	- [[#Enkindling Orb – Effect Boost]]
	- [[#Best Flask Mod Setups]]
- [[#Mageblood Belt Setup]]
- [[#Synthesis & Other Niche Mechanics]]
- [[#Profit Crafting Mindset]]
- [[#Resources & References]]

---

## Fundamentals

> Based on **GhazzyTV – "Basics of Crafting" video** ([YouTube](https://www.youtube.com/watch?v=DXDxV0pccxw)) and his updated **written guide** at [poe-vault.com/guides/crafting-basics](https://www.poe-vault.com/guides/crafting-basics) (*last updated Oct 30 2025*). Memory Strands and a few current-league items are added on top because they post-date the written guide.

### Item Anatomy

A PoE 1 item from top to bottom can have:

1. **Name + Influence icons** (Shaper / Elder / Hunter / Crusader / Redeemer / Warlord / Searing Exarch / Eater of Worlds / Synthesised).
2. **Enchant** (teal text) – Labyrinth helmet/glove/boot, Blight oil anoint on amulets/rings, Cassia oil on belts.
3. **Implicit modifier(s)** (teal line above the divider) – base, Synthesised, or Eldritch implicit.
4. **Explicit modifiers** below the divider – up to **3 prefixes + 3 suffixes**.

Hold **Alt** in-game to see item level + each mod tier + whether a mod is `prefix`, `suffix`, `crafted`, `fractured`, `synthesised`, `enchant`, `eldritch`, or `master-crafted`.

### Rarity & Affix Limits

| Rarity | Modifier Limits | Notes |
|--------|-----------------|-------|
| **Normal (White)** | 0 explicit | The "base". |
| **Magic (Blue)** | 1 prefix + 1 suffix | Cannot be bench-crafted (unless Magic-flask). |
| **Rare (Yellow)** | 3 prefixes + 3 suffixes (6 total) | The endgame target. |
| **Unique** | Fixed pool | Modifiable only with Divine (re-roll values) or Vaal (corrupt). |

Some heist/special items (Heist rings, Replica uniques) have **exceptions** clearly stated on the item itself.

### Prefixes vs Suffixes

Every explicit mod is either prefix or suffix and they pull from **completely separate pools**.

- **Prefixes** = "big numbers" (life, ES, flat damage, %damage, spirit, etc.).
- **Suffixes** = utility (**all resistances**, attributes, attack/cast speed, crit, regen).

Knowing the **open pool** before you spend currency is the single biggest lever in PoE 1 crafting (see [[#Bench Blocking]] for the mathematical follow-up).

### Item Level, Mod Tiers & Weights

Hovering an item + Alt shows **iLvl**. The iLvl gates which **tiers** of every mod can roll (e.g. T1 Life requires iLvl 54 on most armours; T1 Movement Speed requires iLvl 86 on boots).

Every mod has a **weight** that determines how likely it is to land inside the open pool. Example: on body armour, **flat ES T8 = ~1000 weight** while **T1 Life = ~50 weight** — random Exalt slams are vastly more likely to hit the cheap pool.

> **Crucial tool:** **[Craft of Exile – PoE 1](https://www.craftofexile.com/?game=poe1)** to look up: every modifier's tier table, iLvl gate, weight, prefix/suffix split, and Eldritch/Influence/Synthesis pools per base. It also has a full **Emulator** for risk-free crafting practice.

#### Calculating odds (Ghazzy's method)
```
P(desired) = sum-of-weights(desired mods) ÷ sum-of-weights(all remaining-pool mods)
```
Block the highest-weight unwanted mods at the bench to push P(desired) much higher.

### Base Items & Defensive Pools

Base type gates the **defensive prefix pool**:

| Stat req | Defensive | Example body armour |
|----------|-----------|---------------------|
| Strength | Armour | Astral Plate |
| Dexterity | Evasion | Cloud Squall |
| Intelligence | Energy Shield | Vaal Regalia |
| Str/Dex | Armour/Evasion | Triumphant Lamellar |
| Dex/Int | Evasion/Energy Shield | Sacrificial Garb |
| Str/Int | Armour/Energy Shield | Sacred Targe (Shield) |
| Str/Dex/Int | Tri-stat | Necromancer Silks (synth) |

Choose your base **deliberately**: a Vaal Regalia cannot ever roll Armour mods; a Spirit Shield (int) opens Cast Speed / Spell Damage / +Lvl gem mods that a Tower Shield cannot roll.

### Local vs Global Modifiers

- **Local** mods only affect that item (`+X Armour`, `Y% Increased Physical Damage` on a weapon, `Crit Chance` on weapons, `Adds X-Y Damage` on weapons, attack speed on weapon).
- **Global** mods affect the whole character (`+X Maximum Life`, resistances, `%Spell Damage` on a wand, `+X% Crit Chance for Spells`).

When you see a numeric mod, check whether the tooltip stats line increased — local mods *scale by quality* and other local multipliers, global mods don't.

### Special Modifier Types

| Type | Where it comes from | Removable? |
|------|---------------------|------------|
| **Implicit** | Item base / Synthesised / Eldritch | Only via Vaal corrupt, Temple, or new Eldritch slam |
| **Fractured** (dark golden) | Fracturing Orb / specific Atlas mechanics | **Never** — permanent anchor mod |
| **Synthesised implicit** | Synthesis Memory Nexus | Cannot influence further; replaceable by re-synthesis |
| **Enchant** | Labyrinth (helm/glove/boot), Blight oil (amulet/ring), Cassia oil (belt) | Lab/oil re-roll |
| **Incursion mod** | Temple of Atzoatl rooms | If removed by crafting, **lost forever** — protect or imprint |
| **Delve mod** | Niko / Delve fossils only | Same — keep it or lose it |
| **Influence mod** | Shaper/Elder/Conqueror exalts, drops | Removable but exclusive pool |
| **Eldritch implicit** | Embers / Ichors | Replaceable only by another Eldritch slam |
| **Veiled** (red Jun icon) | Betrayal / Aisling T4 | Must be unveiled at Jun |
| **Master-crafted** (teal) | Crafting Bench | One only, unless **Multimod** metamod is used |
| **Memory Strand mod** (rose petal background) | Originator memory maps (3.26 / 3.28) | See [[#Memory Strands (Current 3.28 Mirage)]] |

---

## Currency Orbs – The Building Blocks

| Orb | Effect |
|-----|--------|
| **Orb of Transmutation** | Normal → Magic with 1 mod |
| **Orb of Augmentation** | Adds 2nd mod to Magic |
| **Orb of Alteration** | Re-rolls a Magic item's mods (the *spam* orb) |
| **Orb of Alchemy** | Normal → Rare with 4-6 mods |
| **Regal Orb** | Magic → Rare adding 1 new random mod |
| **Orb of Scouring** | Rare/Magic → Normal (this is the key tool **PoE 2 deliberately removed**) |
| **Chaos Orb** | Re-rolls a Rare item's mods (4-6 new mods) |
| **Exalted Orb** | Adds 1 random mod to a Rare with an open slot |
| **Divine Orb** | Re-rolls numeric values of existing mods within tier ranges |
| **Orb of Annulment** | Removes 1 random mod |
| **Vaal Orb** | Corrupts (see [[#Vaal Corruption]]) |
| **Blessed Orb** | Re-rolls the numeric value of the **implicit** |
| **Eternal Orb** | (Legacy) Creates an imprint of a Rare. Removed from drop pool, replaced by Beast Imprint |
| **Awakener's Orb** | Combines 2 influences (see [[#Influence & Awakener's Orb]]) |
| **Sacred Orb** | Re-rolls the Sockets and Links of an item |
| **Fracturing Orb** | Fractures one random mod on an item with ≥4 mods (locks it) |
| **Hinekora's Lock** | "Foresee" the result of the next currency before applying |

Plus dozens of mechanic-specific currencies: **Essences, Fossils, Resonators, Embers, Ichors, Lifeforce, Catalysts, Bestiary Beasts, Veiled mods, Memory Strands, Orb of Remembrance, Orb of Unravelling, Instilling Orb, Enkindling Orb, Tainted variants of all the above for corrupted items**, etc.

---

## Crafting Bench (Master Crafts)

The hideout **Crafting Bench** lets you spend currency to add a single deterministic **master-crafted modifier** (teal text). Recipes are unlocked from Niko / Veiled mods / specific maps.

### Multimod

- **Recipe:** *"Can have up to 3 Crafted Modifiers"*
- **Type:** Suffix (occupies a suffix slot)
- **Cost:** ~2 Divines
- **Source:** Putrid Cloister unique map
- Unlocks adding **two extra** bench crafts on top of itself (so 3 crafted mods total — usually 2 prefix + the Multimod suffix, or 1 prefix + 1 suffix + Multimod).

### Metamods – Prefixes/Suffixes Cannot Be Changed

The single most important PoE 1 crafting tool that has no PoE 2 equivalent:

| Metamod | Effect |
|---------|--------|
| **"Prefixes Cannot Be Changed"** (suffix, ~2 div) | Locks all prefixes during a Chaos, Scour, Alteration, Harvest reforge, Essence, etc. |
| **"Suffixes Cannot Be Changed"** (prefix, ~2 div) | Same for suffixes |
| **"Cannot Roll Attack Modifiers"** | Blocks the entire attack-mod pool from rolling |
| **"Cannot Roll Caster Modifiers"** | Same for caster mods |

#### The Scour trick (PoE 1 exclusive)

```
Item has good prefixes, garbage suffixes
1. Bench-craft "Prefixes Cannot Be Changed" (eats your suffix slot)
2. Orb of Scouring → removes ALL suffixes (including the metamod itself) but KEEPS all prefixes
3. Item is now Rare with only good prefixes + 3 open suffixes
4. Alch/Chaos/Essence/Harvest the suffixes freely
```

The reverse works for prefixes. This is the backbone of *every* high-end PoE 1 craft.

### Bench Blocking

Before slamming an Exalt onto a Rare, bench-craft the **highest-weight unwanted mod** at the cheapest tier. This **removes it from the open pool** — drastically improving the odds of hitting what you want. Then either keep it or re-roll afterward.

> GhazzyTV's calculation on Vaal Regalia: removing the ~9000-weight Intelligence mod from a 47200-weight pool pushed the chance of hitting top-3 resistance tiers from ~19 % to ~24 %.

### Socket, Link & Colour Crafts

- **Off-colours:** Use the [Vorici Calculator](https://siveran.github.io/calc.html) to compare bench cost vs Chromatic spam. For very off-stat items (e.g. 4× red on int gloves), use the **"reduce to N sockets → re-add"** trick — each re-add bench craft is a fresh ~29 % chance at the off colour, often cheaper than Chromatic spam.
- **Quality first:** **20 % quality** boosts the chance for sockets and links. Always quality-max before fusing/jeweling.
- **Corrupted items:** The bench still works for sockets/links/colours, but each craft costs **the equivalent Vaal Orbs** on top of fusings/jewellers. Use **Tainted Fusings / Tainted Jewellers / Tainted Chromatics** for unpredictable but cheap re-rolls (can hit 6L corrupted from 4L, can hit 28-29 % quality with Tainted Armourer's Scrap).

---

## Essences

### Essence Tiers

| Tier | Name | Notes |
|------|------|-------|
| 1 | Whispering | Campaign filler |
| 2 | Muttering | – |
| 3 | Weeping | – |
| 4 | Wailing | – |
| 5 | **Screaming** | First tier that can re-roll a **Rare** like a Chaos Orb |
| 6 | **Shrieking** | Endgame staple |
| 7 | **Deafening** | Best regular outcome |
| – | **Corrupted essences** | Highest-tier mods (e.g. Hysteria, Insanity, Horror, Delirium, Envy). Only from corrupting a Deafening Essence Monolith with a Vaal Orb |

3 essences of one tier → 1 essence of next tier at any vendor.

### Essence Workflows

- **Magic → Rare with guaranteed mod:** Use **Screaming+** on a Magic item with a great single prefix → become Rare with the magic mod retained + the essence-guaranteed mod + a random extra. Cheaper than `Regal slam`.
- **Re-roll a Rare around a fractured anchor:** Combine a fractured item (e.g. fractured Life on gloves) with Essence spam to guarantee Minion Damage / Caster mod / Attack Speed. The fractured mod can never be lost.
- **Essence overrides metamods:** Screaming+ essences re-roll **all mods** like a Chaos, ignoring "Prefixes Cannot Be Changed". This is intentional — use it when you want full re-rolls but with one stat locked.
- **Corrupted Essences** like *Hysteria* (Attack Speed top tier) and *Horror* (Minion Damage top tier) are the staple for endgame minion/attack crafts.

---

## Fossils & Resonators

Fossils are socketed into **Chaotic Resonators** to bias the mod pool when re-rolling an item.

### Resonator Tiers

| Resonator | Sockets |
|-----------|---------|
| Primitive Chaotic Resonator | 1 |
| Potent Chaotic Resonator | 2 |
| Powerful Chaotic Resonator | 3 |
| Prime Chaotic Resonator | 4 |

### Most Useful Fossils

| Fossil | Effect (paraphrased) |
|--------|----------------------|
| **Pristine** | 10× Life mods, blocks Defence mods |
| **Dense** | 10× Defence mods (great for ES / Armour / Evasion %) |
| **Bound** | 10× Minion mods |
| **Aberrant** | 10× Chaos mods, blocks Lightning |
| **Frigid** | 10× Cold mods |
| **Scorched** | 10× Fire mods |
| **Metallic** | 10× Lightning mods |
| **Corroded** | 10× Bleed/Poison/DoT mods |
| **Jagged** | 10× Attack mods, blocks Caster |
| **Lucent** | 10× Mana mods |
| **Prismatic** | 10× Elemental Resistances |
| **Serrated** | 10× Attack mods (alternate) |
| **Shuddering** | 10× Speed mods |
| **Sanctified** | 10× Crit / 10× Quality lottery (15-30 % quality outcome) |
| **Faceted** | 10× +1 Gem mods (extreme rarity) |
| **Deafening Echo** | Greater modifier tiers |
| **Tangled** | 10× Tangled/exotic mods |
| **Encrusted / Gilded / Glyphic** | League-specific |
| **Perfect Fossil** | Re-rolls quality 15-30 % |
| **Hollow** | 10× Abyss Jewel slots |

### Common Fossil Combos

| Goal | Combo |
|------|-------|
| **High-life Stygian Vise** | Pristine + Primitive Resonator |
| **ES body armour** | Dense + Potent |
| **+1 Gem amulet** | Faceted + Primitive (very expensive) |
| **+2 Minion wand** | Bound + Faceted + Metallic + Shuddering in Prime |
| **Phys bow** | Jagged + Serrated + Shuddering + Corroded |
| **Crit / Quality push** | Sanctified solo on quality-needy items |
| **Spell crit caster** | Aberrant + Faceted + Shuddering |

> Niko sells fossils in delve city and via Azurite. **Pristine** is sometimes 1000 Azurite from him directly.

---

## Harvest Crafting

The Sacred Grove (Oshabi) drops **Crystallised Lifeforce** which you spend at the **Horticrafting Station** in your hideout. Crafts can be **stored** (banked) per slot for later.

### Lifeforce Types

| Type | Used by |
|------|---------|
| **Vivid** (purple) | "Augment + Reforge" attack / caster / fire / cold / lightning crafts |
| **Primal** (red) | Life / chaos / phys / defence crafts |
| **Wild** (green) | Speed / crit / quality / resistance crafts |
| **Sacred Crystallised Lifeforce** | Premium "Reforge Influenced" or "More Likely" tags (rare drop) |

### Best Harvest Crafts

- **Augment X then Remove Y** — adds a guaranteed mod with the chosen tag (Life, Caster, Speed, Defence, etc.) on an item with open slots. **Without** the side effects of a Reforge — the single most-used Harvest craft for endgame.
- **Reforge keeping prefixes/suffixes** — costs **Sacred Lifeforce**, guaranteed to keep one side intact (similar to scour-trick but in one click).
- **Reforge X (more likely)** — 10× weight on the chosen tag plus the guaranteed tagged mod.
- **Reforge Influenced** — re-rolls an influenced item with a guaranteed influenced mod.
- **Reforge Critical / Defence / Life / Cold / Fire / Lightning / Phys / Chaos / Attack / Caster / Speed** — Chaos-style re-roll guaranteeing one mod with the chosen tag.
- **Swap Resistance** — convert a Fire Res mod to Cold (or any combo) for **500 lifeforce** — fantastic for tri-res balancing on jewels & jewellery.
- **Change a non-X to Y modifier** — for surgical mod swaps.

### Harvest + Metamod Workflow

The classic deterministic craft:

```
1. Get a Rare item with good prefixes, bad suffixes
2. Bench-craft "Suffixes Cannot Be Changed" (prefix slot)
3. Bench-craft a placeholder open-prefix blocker  (optional, with multimod)
4. Use a Harvest "Reforge keeping prefixes" or "Augment Life then Remove" 
5. Repeat until suffixes are perfect
6. Remove metamod, slam Exalts to fill, or use Awakener's slam
```

---

## Beastcrafting

Hideout **Blood Altar** (Einhar's Menagerie) lets you sacrifice 4 captured beasts for a recipe.

### Imprint (Magic Item Snapshot)

**Recipe:** *Create an Imprint of a Magic Item* — requires a **Craicic Chimeral** (rare red beast) + 3 rare beasts.

- Creates an **Imprint** item that snapshots the Magic item exactly.
- Use additional currency to evolve the Magic item further; if the craft goes wrong, **apply the imprint to revert** the item back exactly to the snapshot point.
- The endgame use: imprint a `Magic, 1-mod fractured base` → spam Augments / Alterations to try for a 2nd perfect mod → if it bricks, revert. Repeat until done.
- **Limitation:** Only works on **Magic** items, **not Rare**.

### Aspect Skills

- The four **Spirit Beasts** (Saqawal, Farrul, Craiceann, Fenumus) each drop their **Aspect crafting recipe**.
- The recipe adds an **Aspect of the X** suffix mod to a piece of gear — Cat / Spider / Crab / Bird — granting access to a permanent aura when equipped.
- **Use case:** very common on amulets/rings/shields/helms to add a free defensive or offensive aura without slotting a gem.

### Split Beast & Other Recipes

- **Split an Item** (Fenumus Spinneret) — clones a Rare into two Rares each with ~50 % of the original mods. Mostly used in build-base reduction scenarios.
- **Add a Suffix / Add Resistance / Add Quality** beast crafts — niche but powerful.
- **Reforge Influenced** beasts add a specific influence type to a Rare (very expensive).
- **Tabula Rasa-style Magic with up to 4 sockets** (lower-end QoL).

---

## Influence & Awakener's Orb

### Influence Types

| Influence | Symbol | Notable mod themes |
|-----------|--------|--------------------|
| **Shaper** | Top-left | Cold, Spell damage, +1 gems |
| **Elder** | Top-right | Chaos, Minion mods, ES, Speed |
| **Hunter** | Right | DoT multiplier, Curse effect, Maim |
| **Crusader** | Right | Phys, Consecrated ground, Armour |
| **Redeemer** | Right | Cold, Crit, Evasion |
| **Warlord** | Right | Endurance/Rage, Armour, Phys |
| **Searing Exarch** | Top | Eldritch implicit (see below) |
| **Eater of Worlds** | Top | Eldritch implicit (see below) |

A normal item can carry **one** Conqueror/Shaper/Elder influence; an **Awakener-merged** item can carry **two**.

### Awakener's Orb Rules

- Both items must be the **same base type** and each carry **exactly one** different influence.
- **Donor:** loses its base; only **one of its influenced mods is preserved**.
- **Target:** keeps base, iLvl, sockets, links, quality, enchantments — gets **completely re-rolled** as a Rare with both influence pools, **preserving one influenced mod from each item**.
- Mutually-exclusive mods (same ModGroup) drop one at random.
- Influence icon display order is fixed: **Shaper > Elder > Crusader > Redeemer > Hunter > Warlord**.

**Classic recipe:** Hunter `+1 Curse` amulet + Warlord `+1 to all skill gems` amulet → Awakener slam → double-influenced amulet with both T1 mods intact, then craft / Harvest the rest.

### Conqueror Exalted Slams

The four Conqueror **Exalted Orbs** (Awakened Hunter's / Warlord's / Crusader's / Redeemer's Exalt) — slam a Rare with the corresponding influence + add 1 influenced mod. **Cannot be used on items with Eldritch implicits.**

---

## Eldritch Crafting (Searing Exarch & Eater of Worlds)

Applies only to **Helmets, Gloves, Boots, Body Armour** that are **not Conqueror/Shaper/Elder-influenced**.

### Ember & Ichor Tiers

| Tier | Searing Exarch | Eater of Worlds |
|------|----------------|------------------|
| 1 | Lesser Eldritch Ember | Lesser Eldritch Ichor |
| 2 | Greater Eldritch Ember | Greater Eldritch Ichor |
| 3 | Grand Eldritch Ember | Grand Eldritch Ichor |
| 4 | **Exceptional Eldritch Ember** | **Exceptional Eldritch Ichor** |

**Embers** add an Exarch implicit (above the line). **Ichors** add an Eater implicit (above the line). An item can have **one of each** simultaneously.

### Orb of Conflict

Use an **Orb of Conflict** on an item with both implicits — randomly **upgrades one tier and downgrades the other**. Spam this on tier-6 vs tier-1 implicits to maintain the keeper while the cheap one bounces.

### Eldritch Chaos / Exalt / Annul

- **Eldritch Chaos Orb** — re-rolls **prefixes** if Exarch is dominant, **suffixes** if Eater is dominant (whichever implicit is higher tier).
- **Eldritch Exalted Orb** — slams a prefix/suffix to the side that's dominant.
- **Eldritch Orb of Annulment** — annuls a mod from the dominant side.

> These are the best targeted Chaos / Exalt / Annul in the game — exclusive to Eldritch items.

---

## Veiled Crafting (Betrayal & Aisling T4)

Veiled mods drop from **Immortal Syndicate** members during Betrayal encounters. They appear as a red Jun icon on the item.

### Unveiling

- Take a Veiled item to **Jun Ortoi** at her Mastermind camp.
- Pick **1 of 3** revealed options.
- Unveiled mod is **more powerful** than the bench-craft equivalent and **does not count as a Master-Crafted mod**, so you can still bench-craft on top.
- Unveiling also **unlocks** that mod recipe on your Crafting Bench (the league-progression hook).

### Aisling T4 Bench Slam

With **Aisling Laffrey** as Mastermind Captain in **Research** (3 stars / T4), defeating the Mastermind rewards a **Crafting Bench** that removes a random mod from an item and **adds a Veiled mod**. (Updated mechanic: she now *removes first, then adds*, making her a riskier late-step craft than the old version.)

**Strategic blocking:** Bench-craft a placeholder mod you don't want to unveil before sending it to Jun. This narrows the unveil pool, raising odds of hitting your target.

---

## Vaal Corruption

### Vaal Orb on Items

Possible outcomes:

1. **Nothing visible** — item is corrupted but unchanged (still uncraftable now).
2. **Reroll all mods** as a random Rare.
3. **Convert to a Rare** (if Magic).
4. **Add a corrupted implicit** (special pool above the line — see Craft of Exile *Corrupted Implicits* tab on every base).
5. **+/- 1 to gem level or +/-X % quality** (gems only).
6. **Add a socket / change links / re-colour** (on items).
7. **Brick: turn item into a Rare with all White sockets** ("RGB" outcome).

### Gem Corruption + Doryani's Institute

- Vaal Orb on a **Lvl 20 / Q20 gem** can hit `+1 Lvl` (best), `+1-23 % quality`, become **Vaal version**, or shatter.
- The **Temple of Atzoatl → Doryani's Institute (T3)** has the **Lapidary Lens** — a *double Vaal* in one click. Pushes 20/20 gems to **21/23** outcomes much more often than two sequential Vaals (per-roll outcome distribution is the same but it's one click and one item-state).

### Temple Altar of Corruption (Double Corrupt)

- **Locus of Corruption (T3 Corruption Chamber)** has the **Altar of Corruption**: corrupts an item with **2 corrupted implicits** at once, or all **White sockets**, or bricks.
- Used for crazy double-implicit chest pieces / helmets / belts. High risk.

### Tainted Currency

For items already corrupted:

- **Tainted Fusing** — unpredictably re-roll links (only way to 6L a corrupted item without a 6L vendor recipe).
- **Tainted Jeweller's** — re-roll sockets (can exceed natural cap on some items).
- **Tainted Chromatic** — re-roll colours.
- **Tainted Armourer's Scrap / Blacksmith Whetstone** — push quality to 28-29 % on corrupted items.
- **Tainted Mythic Orb** — combine two corrupted uniques.
- **Tainted Exalted / Chaos / Divine** — equivalent currencies that work on corrupted Rares.

---

## Quality Maxing

### Standard Quality Currencies

| Item | Currency | Cap |
|------|----------|-----|
| **Weapons (Martial)** | Blacksmith's Whetstone | 20 % (30 % via Hillock / Perfect Fossil) |
| **Armour** (helm/body/gloves/boots) | Armourer's Scrap | 20 % (30 % via Hillock / Perfect Fossil) |
| **Caster weapons / wands** | Arcanist's Etcher | 20 % |
| **Flasks** | Glassblower's Bauble | 20 % |
| **Gems** | Gemcutter's Prism | 20 % (23 % via Vaal) |
| **Maps** | Cartographer's Chisel | **Removed in 3.28 Mirage** |
| **Jewellery** | Catalysts (see below) | 20 % (50 % on Breach Rings) |

**Hillock (Betrayal / Research)** can push quality to **28-30 %** depending on rank. Perfect Fossils also roll 15-30 % quality lottery.

> **Important on quality + fusings/jewellers/chromatics:** quality **increases the chance** of hitting more sockets / links / off-colours. **Always quality-max first**, then spam fusings.

### Catalysts (Jewellery)

Catalysts buff rings, amulets, and belts by adding quality that **scales mods with the matching tag**.

| Catalyst | Scales mods tagged… |
|----------|---------------------|
| **Abrasive** | Attack |
| **Accelerating** | Speed |
| **Fertile** | Life / Mana |
| **Imbued** | Caster |
| **Intrinsic** | Attribute |
| **Noxious** | Physical / Chaos |
| **Prismatic** | Resistance |
| **Tempering** | Defence |
| **Turbulent** | Elemental |
| **Unstable** | Critical |
| **Tainted** | Works on corrupted jewellery |
| **Reaver / Skittering** (3.x league) | Niche |

- 20 catalysts of one type → 20 % quality of that type on the item.
- **Breach Rings** can reach **50 % quality** (scaling explicit mods to 150 % of their value). 
- Catalyst type is exclusive per item — using a different catalyst type wipes existing quality and starts over.

---

## Memory Strands (Current 3.28 Mirage)

> **Not yet covered in Ghazzy's written guide (last updated Oct 30 2025).** Introduced in **3.26 Mercenaries of Trarthus / Secrets of the Atlas** and carried into **3.28 Mirage**. Drops on items found inside **memory-influenced maps**.

### Petals & Memory Threads

- **Items with Memory Strands** display a value **1-100** on the tooltip, with a **rose-petal background** and special symbols next to the name.
- **Petals** are collected in originator-influenced areas — they increase the **chance** that items drop with Memory Strands and increase the **strand value**.
- **Memory Threads** are the originator-area currency that pools the petal effect across maps.
- After completing the **Threads of the Originator** quest, **all maps** have a (much smaller) chance to drop strand-items.

### Orb of Remembrance & Orb of Unravelling

| Orb | Effect |
|-----|--------|
| **Orb of Remembrance** | Adds or randomises the Memory Strand value on a **Normal** item |
| **Orb of Unravelling** | Consumes **all remaining strands**, attempting to upgrade tiers of explicit modifiers; quantity consumed = upgrade attempts. May upgrade nothing if unlucky |

### How to Use Strands in Crafting

- Whenever you use a **Chaos Orb, Exalted Orb, Essence**, or comparable crafting currency on a strand-item, it **consumes a random number of strands** to **boost the tier** of the modifier being added.
- **Workflow:**
	1. Find a high-iLvl base with ≥80 strands (or use **Orb of Remembrance** on a Normal base to roll high strands).
	2. Alch / Chaos / Essence with **maximum strand value** — high probability of hitting top-tier mods.
	3. End with **Orb of Unravelling** to attempt one last tier-upgrade lottery before strands run out.

> This makes a fresh high-strand base into a **deterministic-ish** tier-1 mod factory. Pair with Bench Blocking + Metamods for best results.

**Important:** Strands deplete with each craft. Plan your bench blocks and currency order **before** you start consuming the budget.

---

## Utility Flask Crafting

### Base Flask Rolling

1. **Quality first while White** — Glassblower's Baubles applied to a Normal flask cost **5 baubles to 20 %** (Magic costs 20 baubles for the same outcome).
2. **Transmute** to Magic.
3. **Alteration spam** for the prefix you want.
4. **Augment** if only one mod rolled, to get the suffix you want.
5. **Beast-craft "Add 1 Suffix"** to surgically slot a missing immunity / immunity-style suffix.

### Best Flask Prefixes

| Prefix | Effect |
|--------|--------|
| **Alchemist's** | +25 % flask effect (the Mageblood meta) |
| **Avenger's** | Charges gained on crit |
| **Surgeon's** | Charges gained on crit (alternate) |
| **Chemist's** | -25 % charges used |
| **Experimenter's** | +35 % duration |
| **Saturated** | +50 % recovery (for life/mana flasks) |

### Best Flask Suffixes

| Suffix | Effect (immunity / status) |
|--------|-----------------------------|
| **of Staunching** | Bleed immunity |
| **of the Skink** | Shock immunity |
| **of the Walrus** | Freeze immunity |
| **of Dousing** | Ignite immunity |
| **of Heat** | Chill immunity |
| **of Curing** | Poison immunity |
| **of Warding** | Curse immunity |
| **of Adrenaline** | +20 % move speed |
| **of Reflexes** | +X % evasion during effect |
| **of Iron Skin** | +X % armour during effect |

### Instilling Orb – Auto-Triggers

The **Instilling Orb** adds an **enchantment** to a utility flask that **auto-uses** under a condition. Random enchant from the pool:

- **Used when you Hit a Rare or Unique Enemy** (boss-fight burst-flask trigger).
- **Used when an Adjacent Enemy dies**.
- **Used when you have less than X % Life/ES/Mana**.
- **Used when you are Bleeding / Ignited / Frozen / Shocked / Poisoned**.
- **Used when Charges reach Full**.

Each enchant also disables manual flask use (the cost of automation).

**Deterministic crafting (post-3.15.2):** the **Crafting Bench has recipes** for **every** Instilling enchant — costs **5 Instilling Orbs + 5 Glassblower's Baubles** per craft. Always prefer the bench over spamming raw orbs.

### Enkindling Orb – Effect Boost

The **Enkindling Orb** adds an effect-boost enchant — typically **60-70 % increased flask effect** — at the cost of **no flask charges gained during effect**. **Mandatory for the Mageblood flask setup** (you don't need charges if the flask runs forever).

### Best Flask Mod Setups

| Flask base | Suggested prefix | Suggested suffix | Enchant |
|------------|------------------|------------------|---------|
| **Quartz** | Alchemist's | of Warding | Enkindling 70 % effect |
| **Granite** | Alchemist's | of Iron Skin | Enkindling 70 % effect |
| **Jade** | Alchemist's | of Reflexes | Enkindling 70 % effect |
| **Quicksilver** | Alchemist's | of Adrenaline | Enkindling 70 % effect |
| **Silver** | Alchemist's | of Adrenaline | Enkindling 70 % effect |
| **Basalt** | Alchemist's | of Iron Skin | Enkindling 70 % effect |
| **Topaz/Sapphire/Ruby** | Alchemist's | of any element-immunity | Enkindling 70 % effect |
| **Sulphur** | Alchemist's | of Warding | Enkindling 70 % effect |
| **Gold** (rarity) | Alchemist's | of Adrenaline | Enkindling 70 % effect |
| **Life flask** | Saturated | of Staunching (or Heat) | **Instilling: Used when Low Life** |
| **Mana flask** | Saturated | of Curing | **Instilling: Used when Low Mana** |

For non-Mageblood builds, **drop the Enkindling** (you need charges) and use **Instilling** triggers instead.

---

## Mageblood Belt Setup

**Mageblood** is the unique **Heavy Belt** that makes all five equipped **Magic utility flasks apply permanently** without manual activation or charges consumed. Endgame chase item.

**Flask setup recipe (per slot):**

1. **White flask, max quality** (5 Baubles to 20 %).
2. **Transmute** to Magic.
3. **Alteration spam** until you hit `Alchemist's` (25 % flask effect prefix). Ignore the -10 % duration drawback — Mageblood doesn't care, the flask never runs out.
4. **Augment / Beast-craft Suffix** for the immunity or utility you need.
5. **Enkindling Orb** until you hit **60-70 % increased effect**. The "no charges gained" downside is irrelevant.
6. **Both the implicit and the suffix value get scaled by 95 %** in the final tooltip thanks to all flask-effect modifiers stacking multiplicatively with Alchemist's.

**Typical 5-flask Mageblood loadout:**

| Slot | Flask | Why |
|------|-------|-----|
| 1 | **Diamond** of Curing | Crit chance lucky, poison immunity |
| 2 | **Granite** of Iron Skin | Defence layer |
| 3 | **Jade** of Reflexes | Evasion layer |
| 4 | **Quicksilver / Silver** of Adrenaline | Movement speed |
| 5 | **Quartz** of Warding | Phase + curse immunity, ele dodge |

(Swap any slot for a **Ruby / Topaz / Sapphire of Heat / Skink / Walrus** if you need elemental res capping over a defence layer.)

---

## Synthesis & Other Niche Mechanics

- **Synthesis (Memory Nexus / Cavas):** combine 3 specific magic items in a Synthesiser to roll a Synthesised Rare with up to 3 synthesised implicits (a 4th implicit line above the explicit pool). Cannot be influenced afterward, but Synthesised implicits are some of the strongest in the game (e.g. `Damage Penetrates X % Elemental Resistance`, `+1 to all Skill Gems`).
- **Heist (Rogue's Marker / Compass mods):** craft contracts for specific Veiled / Replica unique outcomes; Trinkets allow modifying Heist rewards.
- **Logbook crafting (Expedition / Tujen):** gamble currency from Tujen's haggle for cheap currency / unique sources.
- **Sextants (replaced by Astrolabes in 3.28 Mirage):** affix mods to the Atlas regions for farming strategies.
- **Map crafting** — Chisels removed in 3.28; quality on maps now functions differently or is gone in your league.
- **Cluster Jewels** — rolled like rare items but with notable passive mods; same workflow (alt-aug-regal-exalt with bench blocks).
- **Watchstones / Voidstones** — passively boost map tier, not really crafted but worth a mention.

---

## Profit Crafting Mindset

Same wisdom Ghazzy preaches in both games:

- **Don't ask "what's profitable right now"** — once the formula is public, the margin is gone.
- Use **[poe.ninja → Builds](https://poe.ninja)** to see top players' rares; identify common patterns across an ascendancy; craft what they need.
- The **static cost** is the base item; the **dynamic cost** is your crafting currency expense. `static + dynamic < market floor` ⇒ profitable.
- Sell items **un-corrupted, un-qualitied, un-socketed** — most buyers prefer to finish themselves.
- The best long-term profit comes from learning **one** mechanic deeply (e.g. Aisling slams on Hunter influenced rare amulets, or 5-link Fossil chest spam) rather than dabbling.

---

## Resources & References

### Primary references
- **GhazzyTV – "Basics of Crafting" video** – https://www.youtube.com/watch?v=DXDxV0pccxw *(transcript pulled and integrated)*
- **GhazzyTV's Written Guide – "Basics of Crafting"** *(last updated Oct 30 2025)* – https://www.poe-vault.com/guides/crafting-basics
- **Craft of Exile (PoE 1)** – https://www.craftofexile.com/?game=poe1 *(modifier database + Emulator)*
- **PoE Wiki** – https://www.poewiki.net
- **PoEDB** – https://poedb.tw/us/ *(complete modifier database)*

### Mechanic-specific resources
- [Maxroll – Crafting Resources Hub](https://maxroll.gg/poe/resources/crafting-resources)
- [Maxroll – Fossils & Resonators](https://maxroll.gg/poe/crafting/fossils-resonators)
- [Maxroll – Harvest Crafting](https://maxroll.gg/poe/crafting/harvest-crafting-guide)
- [Maxroll – Veiled Crafting](https://maxroll.gg/poe/crafting/veiled-crafting)
- [Maxroll – Double Influence (Awakener's Orb)](https://maxroll.gg/poe/crafting/double-influence-crafting)
- [Maxroll – Beastcrafting](https://maxroll.gg/poe/crafting/beastcrafting)
- [Maxroll – Eldritch Implicits](https://maxroll.gg/poe/crafting/eldritch-implicits)
- [Maxroll – Metacrafting](https://maxroll.gg/poe/crafting/metacrafting)
- [Maxroll – Corruption Guide](https://maxroll.gg/poe/resources/corruption)
- [Maxroll – Essence Farming](https://maxroll.gg/poe/currency/essence-farming-guide)
- [Maxroll – Mirage 3.28 Patch Notes](https://maxroll.gg/poe/news/3-28-mirage-patch-notes)
- [PoE Wiki – Memory Strand](https://www.poewiki.net/wiki/Memory_strand)
- [PoE Wiki – Orb of Remembrance](https://www.poewiki.net/wiki/Orb_of_Remembrance)
- [PoE Wiki – Mageblood](https://www.poewiki.net/wiki/Mageblood)
- [PoE Wiki – Instilling Orb](https://www.poewiki.net/wiki/Instilling_Orb)
- [PoE Wiki – Enkindling Orb](https://www.poewiki.net/wiki/Enkindling_Orb)
- [PoE Wiki – Awakener's Orb](https://www.poewiki.net/wiki/Awakener's_Orb)
- [PoE Vault – Ultimate Flask Crafting](https://www.poe-vault.com/guides/ultimate-flask-crafting-guide)
- [Vorici Chromatic Calculator (off-colour sockets)](https://siveran.github.io/calc.html)

### Other recommended videos
- **GhazzyTV – PoE crafting series playlist** (Essence / Fossil / Meta / Harvest / Beast / Veiled / Awakener / Imprint videos)
- **EngineeringEternity** – deep-dive metacrafting walkthroughs
- **TalkativeTri** – currency efficiency and crafting-bench micro-optimisation
- **Mathil** – build-specific endgame crafting case studies
- **DarthMicrotransaction** – currency tier list and patch reactions

### Related vault notes
- [[PoE2 Crafting]] *(PoE 2 sibling note)*
