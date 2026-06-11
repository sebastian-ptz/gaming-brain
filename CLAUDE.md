---
---

# Claude Code Guidelines for #gaming-brain Vault

## About This Vault

**#gaming-brain** is a personal gaming wiki and knowledge base for organizing gaming notes and guides. It serves as a comprehensive reference for games and gaming topics.

### Purpose
- Centralized hub for gaming knowledge and build planning
- Personal notes on game mechanics, strategies, and builds
- Quick reference guides for games actively being played
- Repository for guides, tips, and optimization techniques

### Scope
This vault will expand over time with notes on various games. Currently focused on games that are actively played and studied, with detailed documentation for main titles. New games may be added as interest develops.

### Current Focus
- **Path of Exile 2** - Detailed build guides, mechanics, and planning tools

### Structure
Games are organized by title in top-level folders, each containing:
- Build guides and planning
- Mechanics documentation
- Strategy notes
- Tool usage guides (like Path of Building)

---

## Vault Codebase & Conventions

This document outlines best practices and automated behaviors Claude should follow when working with this Obsidian vault.

---

## List of Content in Markdown Files

### Standard Practice
**All `.md` files with multiple sections/headings (h2 level `##` or deeper) MUST include a Table of Contents at the top of the document, titled "List of Content".**

### Format

The `List of Content` section should be placed at the very top of the file (after the properties block), separated by `---` separators. If a `List of Sources` section is also present (see below), it comes **before** `List of Content`:

```markdown
---
---

# Document Title

--- 
## List of Content
- [[#Section 1]]
- [[#Section 2]]
- [[#Subsection 3]]

---

## Section 1
Content here...
```

**Important:** The first `---` on line 1 (with optional empty line after) creates the Obsidian properties tab. Always include this, even if empty.

### Guidelines

1. **Placement:** Immediately after the main title (`# Title`), before any other content (unless `List of Sources` is needed — then Sources comes first)
2. **Format:** Use wikilink format `[[#Heading]]` to allow Obsidian click-through navigation
3. **Separator:** `---` lines before and after the `List of Content` section
4. **Heading Level:** Include only h2-level headings and deeper (## and ###)
5. **Order:** Match the order of headings as they appear in the document
6. **Naming:** Use exact heading text in the wikilinks (case-sensitive for display, but Obsidian handles matching)

### When to Update

**Automatically update the List of Content whenever:**
- New sections/headings are added to the document
- Sections/headings are deleted
- Headings are renamed or reorganized

### Example Files

Reference these files for proper List of Content implementation:
- `[[01 Path of Exile/Path of Exile 2/Builds/Build Planner.md]]`
- `[[01 Path of Exile/Path of Exile 2/Builds/Path of Building.md]]`

---

## Sources Convention

### Rule: ≤ 3 Sources → Frontmatter `sources:` List Only

If a document references **3 or fewer** external sources (URLs, wikis, guides, etc.), list them directly in the YAML frontmatter under a `sources:` key. No body section needed:

```markdown
---
sources:
  - https://www.poewiki.net/wiki/Example
  - https://www.youtube.com/watch?v=example
---

# Document Title
```

### Rule: > 3 Sources → Frontmatter (top 3) + `List of Sources` Body Section

If a document references **more than 3** external sources, do **both**:
1. Keep the **3 most important/primary sources** in the frontmatter `sources:` key
2. Add a full `## List of Sources` section in the document body, placed **before** `## List of Content`, listing all sources

```markdown
---
sources:
  - https://www.poewiki.net/wiki/Example
  - https://www.youtube.com/watch?v=example
  - https://third-main-source.com
---

# Document Title

---
## List of Sources
- [PoE Wiki – Mechanic Name](https://www.poewiki.net/wiki/Example)
- [Guide Title](https://www.youtube.com/watch?v=example)
- [Third Main Source](https://third-main-source.com)
- [Additional Resource](https://example.com)
- [Another Guide](https://another.com)
- ...

---
## List of Content
- [[#Section 1]]
- [[#Section 2]]

---

## Section 1
Content here...
```

### Guidelines

1. **Sources in frontmatter** use plain URLs as list items (no markdown link syntax needed)
2. **Sources in body** (`List of Sources`) use markdown link format: `[Label](url)`
3. **Threshold is exactly 3**: ≤3 sources → frontmatter only; 4+ sources → frontmatter (top 3) + body section
4. **When >3 sources**, the 3 most relevant/primary sources must always still appear in the frontmatter
5. **Only include `sources:` if the document actually references external sources** — do not add an empty key
6. **`List of Sources` always precedes `List of Content`** when both appear as body sections

---

## File Organization Standards

### Directory Structure
- Store game-specific guides in `/01 Path of Exile/Path of Exile 2/`
- Organize by category: `Builds/`, `Mechanics/`, `Economy/`, etc.
- Use descriptive filenames (no generic "notes.md")

### Frontmatter
- Use YAML frontmatter for metadata when relevant
- Include `tags:` for categorization (e.g., `tags: [poe2, builds, guide]`)
- Include `date:` for tracking creation/updates
- Include `sources:` list for external references — always list top 3 in frontmatter; if >3 total, also add a `List of Sources` body section (see Sources Convention above)

### Internal Linking
- Use wikilink format: `[[file-name]]` or `[[folder/file-name]]`
- Use relative paths from vault root (no leading slashes)
- For referenced external resources, use markdown links: `[text](url)`

---

## Vault File Conventions

| Convention | Example | Notes |
|-----------|---------|-------|
| **List of Content** | See `Path of Building.md` | Required for multi-section docs |
| **Sources (≤3)** | `sources:` in frontmatter | Plain URL list in YAML, no body section |
| **Sources (>3)** | `sources:` (top 3) + `## List of Sources` | Top 3 in frontmatter; full list before List of Content |
| **Wikilinks** | `[[Build Planner.md]]` | Always use for internal references |
| **External Links** | `[PoE Wiki](https://poewiki.net)` | Markdown format for external URLs |
| **Relative Paths** | `01 Path of Exile/Builds/` | No leading slash, from vault root |

---

## Maintenance Checklist

When editing markdown files:

- [ ] Update List of Content if any headings changed
- [ ] Verify all internal wikilinks still work (no broken references)
- [ ] Check that heading names are unique and descriptive
- [ ] Ensure consistent heading hierarchy (don't skip levels)
- [ ] Test wikilinks in Obsidian to confirm navigation works

---

## When Claude Works on This Vault

Claude will automatically:
1. Add/update the `List of Content` when creating or editing `.md` files with multiple sections
2. Add/update `sources:` in frontmatter (and `List of Sources` body section if >3 sources)
3. Use wikilink format for internal document references
4. Verify heading hierarchy is consistent
5. Maintain proper file organization by category

Claude will ask before:
- Renaming or moving files (affects all internal links)
- Deleting content (loss of information)
- Restructuring large sections

---

## Quick Reference: Templates

### Simple (≤3 sources)

```markdown
---
sources:
  - https://source-one.com
  - https://source-two.com
---

# Document Title

---
## List of Content
- [[#Heading 1]]
- [[#Heading 2]]

---

## Heading 1
...
```

### Extended (>3 sources)

```markdown
---
sources:
  - https://primary-source.com
  - https://second-source.com
  - https://third-source.com
---

# Document Title

---
## List of Sources
- [Primary Source](https://primary-source.com)
- [Second Source](https://second-source.com)
- [Third Source](https://third-source.com)
- [Fourth Source](https://fourth-source.com)
- ...

---
## List of Content
- [[#Heading 1]]
- [[#Heading 2]]

---

## Heading 1
...
```

**Key Points:**
- Line 1+: YAML properties block — always include even if empty (`---` / `---`)
- `sources:` in frontmatter — always the top 3 (or all, if ≤3)
- `List of Sources` body section — only when total sources exceed 3; placed before `List of Content`
- `List of Content` — always present in multi-section documents

---

*Last Updated: 2026-06-11*
