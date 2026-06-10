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

## Content Lists in Markdown Files

### Standard Practice
**All `.md` files with multiple sections/headings (h2 level `##` or deeper) MUST include a Table of Contents at the top of the document.**

### Format

Content lists should be placed at the very top of the file (after the properties block), separated by two `---` separators:

```markdown
---
---

# Document Title

--- 
## Content
- [[#Section 1]]
- [[#Section 2]]
- [[#Subsection 3]]

---

## Section 1
Content here...
```

**Important:** The first `---` on line 1 (with optional empty line after) creates the Obsidian properties tab. Always include this, even if empty.

### Guidelines

1. **Placement:** Immediately after the main title (`# Title`), before any other content
2. **Format:** Use wikilink format `[[#Heading]]` to allow Obsidian click-through navigation
3. **Separator:** Two `---` lines—one before and one after the Content section
4. **Heading Level:** Include only h2-level headings and deeper (## and ###)
5. **Order:** Match the order of headings as they appear in the document
6. **Naming:** Use exact heading text in the wikilinks (case-sensitive for display, but Obsidian handles matching)

### When to Update

**Automatically update the Content list whenever:**
- New sections/headings are added to the document
- Sections/headings are deleted
- Headings are renamed or reorganized

### Example Files

Reference these files for proper Content list implementation:
- `[[01 Path of Exile/Path of Exile 2/Builds/Build Planner.md]]`
- `[[01 Path of Exile/Path of Exile 2/Builds/Path of Building.md]]`

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

### Internal Linking
- Use wikilink format: `[[file-name]]` or `[[folder/file-name]]`
- Use relative paths from vault root (no leading slashes)
- For referenced external resources, use markdown links: `[text](url)`

---

## Vault File Conventions

| Convention | Example | Notes |
|-----------|---------|-------|
| **Content Lists** | See `Path of Building.md` | Required for multi-section docs |
| **Wikilinks** | `[[Build Planner.md]]` | Always use for internal references |
| **External Links** | `[PoE Wiki](https://poewiki.net)` | Markdown format for external URLs |
| **Relative Paths** | `01 Path of Exile/Builds/` | No leading slash, from vault root |

---

## Maintenance Checklist

When editing markdown files:

- [ ] Update Content list if any headings changed
- [ ] Verify all internal wikilinks still work (no broken references)
- [ ] Check that heading names are unique and descriptive
- [ ] Ensure consistent heading hierarchy (don't skip levels)
- [ ] Test wikilinks in Obsidian to confirm navigation works

---

## When Claude Works on This Vault

Claude will automatically:
1. Add/update Content lists when creating or editing `.md` files with multiple sections
2. Use wikilink format for internal document references
3. Verify heading hierarchy is consistent
4. Maintain proper file organization by category

Claude will ask before:
- Renaming or moving files (affects all internal links)
- Deleting content (loss of information)
- Restructuring large sections

---

## Quick Reference: Content List Template

```markdown
---
---

# Document Title

--- 
## Content
- [[#Heading 1]]
- [[#Heading 2]]
- [[#Heading 3]]

---

## Heading 1
...
```

**Key Points:**
- Line 1-2: Empty properties block (creates Obsidian properties tab)
- Line 4: Main title
- Line 6-11: Content list with `---` separators
- Line 13+: Document sections

---

*Last Updated: 2026-06-10*
