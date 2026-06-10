---
tags:
  - poe2
  - builds
  - guide
date: 2026-06-10
---
## Content
- [[#Official Documentation & Resources]]
- [[#JSON Format Syntax]]
- [[#Weapon Set Passive Allocation]]
- [[#Skills & Gem Setups]]


---
### Official Documentation & Resources

**Official Links:**
- [How to Use The In-game Build Planner - Maxroll.gg](https://maxroll.gg/poe2/getting-started/how-to-use-the-in-game-build-planner)
- [Path of Exile Developer Documentation - Game](https://www.pathofexile.com/developer/docs/game)
- [Build Planner - Path of Exile 2 Wiki (Fextralife)](https://pathofexile2.wiki.fextralife.com/Build+Planner)
- [PoE 2 Build Planner Guide - Boostmatch](https://boostmatch.gg/blog/poe-2/articles/poe2-build-planner-guide-return-of-the-ancients)

### JSON Format Syntax

Build Planner files use the `.build` extension and are JSON documents. They must be saved in:
```
Documents\My Games\Path of Exile 2\BuildPlanner\
```

**Basic Structure:**
```json
{
  "name": "Build Name",
  "author": "Author Name",
  "ascendancy": "AscendancyClass",
  "passives": [
    {
      "id": "passive_node_id",
      "weapon_set": 0  // Optional: 0 = shared, 1 = weapon set 1, 2 = weapon set 2
    }
  ],
  "skills": [
    {
      "id": "Metadata/Items/Gems/SkillGemName",
      "support_skills": [
        {
          "id": "Metadata/Items/Gems/SupportGemName"
        }
      ]
    }
  ]
}
```

**Key Fields:**
- **`name`**: Display name of the build (string)
- **`author`**: Creator/source of the build (string)
- **`ascendancy`**: Ascendancy class ID (string) - e.g., "Monk1", "Shadow2"
- **`passives`**: Array of allocated passive tree nodes
  - **`id`**: Unique identifier for each passive node
  - **`weapon_set`** (Optional): Determines which weapon set a node belongs to:
    - `0` or omitted = Shared passives (active in both weapon sets)
    - `1` = Weapon Set 1 passives only
    - `2` = Weapon Set 2 passives only
- **`skills`**: Array of gem setups with main skill and support gems
  - **`id`**: Metadata path to the skill gem
  - **`support_skills`**: Array of linked support gems (max 5 per setup)

### Weapon Set Passive Allocation

**Example 1 — Passive Tree Allocation:**
```json
{
  "name": "Build Name",
  "author": "Authors",
  "ascendancy": "Monk1",
  "passives": [
    { "id": "Nodename1", "weapon_set": 0 },
    { "id": "Nodename2", "weapon_set": 1 },
    { "id": "Nodename3", "weapon_set": 2 },

  ]
}
```

**Tree breakdown:**
- **weapon_set: 0** (white nodes) = Life + Resistance path (shared, always active)
- **weapon_set: 1** (red nodes) = Dual-wield damage/crit path (only when WS1 equipped)
- **weapon_set: 2** (green nodes) = Two-handed damage/crit path (only when WS2 equipped)

---

### Skills & Gem Setups

**Where skills go in the JSON:**
```json
"skills": [
  {
    "id": "Metadata/Items/Gems/SkillGemFireball",
    "support_skills": [
      { "id": "Metadata/Items/Gems/SupportGemControlledDestruction" },
      { "id": "Metadata/Items/Gems/SupportGemIncreasedAOE" }
    ]
  },
  {
    "id": "Metadata/Items/Gems/SkillGemFrostbolt",
    "support_skills": [
      { "id": "Metadata/Items/Gems/SupportGemLinkingSupport" }
    ]
  }
]
```

**Structure:**
- Each object = one skill gem setup (one gem in a linked socket group)
- `id` = the main skill gem (not weapon-set specific; gems work in any equipped weapon)
- `support_skills` = max 5 support gems linked to that skill (order doesn't matter in JSON)

**Workflow:**
1. **Passives** (`weapon_set` 0, 1, or 2) = stat bonuses based on equipped weapon set
2. **Skills** (no `weapon_set` field) = gem setups that work independently of weapon set (e.g., you can use Fireball with both your dual swords AND your staff)


