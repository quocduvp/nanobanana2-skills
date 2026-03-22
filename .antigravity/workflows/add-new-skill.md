---
description: How to add a new skill to the Nano Banana Prompt Studio plugin
---

# Add a New Skill

Use this workflow when you need to create a brand new prompt specialization skill.

## Steps

1. **Define the skill scope** — Clarify:
   - What domain does this skill cover? (e.g., architecture photography, pet portraits, automotive)
   - What trigger words should activate it? (English + Vietnamese)
   - Does it overlap with existing skills? If so, define boundaries.

2. **Create the skill folder and file:**
   ```
   skills/<skill-name>/SKILL.md
   ```
   Use kebab-case for the folder name (e.g., `pet-portraits`, `architecture-photography`).

3. **Write the SKILL.md** — Follow this structure:

   ```markdown
   ---
   name: <skill-name>
   description: >
     [1-3 sentence description of what this skill does and when to trigger it.
     Include English and Vietnamese trigger keywords.]
   metadata:
     version: "0.1.0"
   ---

   # [Skill Title]

   [1 sentence of what this skill generates.]

   ## [Category] Photography Categories

   ### 1. [Sub-category Name]

   Purpose: [When to use this template.]

   Template:
   ```
   [Full prompt template with bracketed variables]
   ```

   Key elements:
   - [Specific guidance for this sub-category]

   ### 2. [Next sub-category]
   ...

   ## [Domain-specific Reference Section]
   - Tips, cheat sheets, color palettes, etc.

   ## Reference
   Read `references/<filename>.md` for [what the reference contains].
   ```

4. **Create references (optional):**
   ```
   skills/<skill-name>/references/<reference-name>.md
   ```
   Add supplementary lookup tables, cheat sheets, or term glossaries.

5. **Register the skill in CLAUDE.md** — Add a new row to the Skill Registry table:
   ```markdown
   | **<skill-name>** | `skills/<skill-name>/SKILL.md` | [Trigger conditions] |
   ```

6. **Update skill selection rules in CLAUDE.md** if the new skill could conflict with existing ones.

7. **Update README.md** — Add the skill to the appropriate skills table.

8. **Test** — Verify that the skill triggers correctly and produces well-formatted prompts.
