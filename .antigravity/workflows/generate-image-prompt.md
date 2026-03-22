---
description: Generate a Nano Banana 2 image prompt from a user's idea or description
---

# Generate Image Prompt

Use this workflow when the user wants to create a still image prompt for Nano Banana 2.

## Steps

1. **Identify the category** — Determine which skill best fits the user's request:
   - Fashion / lookbook / outfit → read `skills/fashion-editorial/SKILL.md`
   - Product / e-commerce / flat lay → read `skills/product-commerce/SKILL.md`
   - Food / beverage / restaurant → read `skills/food-beverage/SKILL.md`
   - Skincare / beauty / cosmetics → read `skills/skincare-beauty/SKILL.md`
   - Lifestyle / campaign / brand → read `skills/lifestyle-campaign/SKILL.md`
   - General / no specific category → read `skills/prompt-generator/SKILL.md`

2. **Read the matching SKILL.md** — Load the full skill instructions. Follow them exactly.

3. **Gather input** — Ask the user for missing details using the skill's Step 1 questions:
   - What is the subject?
   - Clothing / product details?
   - Environment / setting?
   - Mood and purpose?
   - Aspect ratio / format?

4. **Build the prompt** — Follow the Core Prompt Formula from `skills/prompt-generator/SKILL.md`:
   ```
   [Subject] + [Action/Pose] + [Clothing/Product Detail] + [Environment/Setting] + [Lighting] + [Camera/Lens/Aperture] + [Film Stock/Color Grade] + [Composition/Framing] + [Style/Mood] + [Exclusions]
   ```

5. **Output the prompt** — Present in a clean code block with:
   - Brief explanation of creative choices (2-3 sentences)
   - Suggested variations (lighting, angle, palette)
   - Reminder about `character-consistency` skill if multi-image project

6. **If the user wants video from this image** → hand off to `/animate-to-video` workflow.
