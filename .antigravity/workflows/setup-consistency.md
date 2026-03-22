---
description: Set up Character DNA, Brand Style Guide, and Product Profiles for consistent multi-image/video campaigns
---

# Set Up Consistency (Character + Brand + Product)

Use this workflow when the user needs the same person, product, or visual style to appear consistently across multiple generations. **Always run this before multi-image campaigns, multi-clip ads, or series content.**

## Steps

1. **Read the consistency skill** — Load `skills/character-consistency/SKILL.md` for full instructions.

2. **Determine what needs consistency:**
   - 👤 **Person/Character** → build Character DNA (Pillar 1)
   - 🎨 **Brand/Visual style** → build Brand Style Guide (Pillar 2)
   - 📦 **Product appearance** → build Product Reference Profile (Pillar 3)
   - Most campaigns need **all three**.

### Pillar 1: Character DNA (if person involved)

3. **Gather character details** — Ask user for (or derive from reference image):
   - Physical: age, gender, ethnicity/skin tone, face shape, eyes, nose, lips, brows, distinguishing features
   - Hair: length, texture, color, style
   - Body: build, height impression
   - Default expression and gaze
   - Makeup baseline

4. **Write Character DNA block** — Format as specified in the skill.

5. **Generate Character Reference Sheet** — Use the 2x2 grid prompt:
   ```
   Character reference sheet of [full Character DNA].
   4 views in 2x2 grid: front-facing, 3/4 left, 3/4 right, back view.
   White background. Neutral expression. Simple white/grey t-shirt.
   Even studio lighting. Professional character design reference sheet.
   ```

### Pillar 2: Brand Style Guide (if campaign/series)

6. **Gather brand info** — Ask user about:
   - Photography style, color palette (3-5 colors with hex codes)
   - Film stock reference, color grade style
   - Composition rules, model styling direction
   - Environment family, mood (3 words)
   - Signature elements (always include) and anti-patterns (never include)

7. **Write Brand Style Guide block** — Format as specified in the skill.

### Pillar 3: Product Profile (if product featured)

8. **Gather product details:**
   - Type, material and finish, exact colors (with hex if possible)
   - Shape description, size reference
   - Key details (logo placement, stitching, label design)
   - Distinguishing features

9. **Write Product Reference Profile block.**

10. **Generate master Product Reference Photo** — Clean, white background, multiple angles.

### Usage in Subsequent Prompts

11. **For every subsequent image/video in the campaign:**
    - Attach reference images (character sheet, product master photo)
    - Prefix prompt with Brand Style Guide block
    - Include abbreviated Character DNA (2-3 key lines)
    - Include Product Profile
    - End with: "Maintain consistency with reference images"
    - Only change: outfit, pose, environment

12. **Return to the calling workflow** (e.g., `/generate-image-prompt`, `/create-tiktok-ad`).
