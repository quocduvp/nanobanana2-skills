---
description: Analyze a reference image and generate clone or variant prompts from it
---

# Analyze Image & Generate Variants

Use this workflow when the user uploads an image and wants to clone it, create variants, reverse-engineer the prompt, or transfer the style to a new subject.

## Steps

1. **Read the analysis skill** — Load `skills/image-analysis/SKILL.md` for full instructions.

2. **Analyze the image** — Systematically read across all dimensions:
   - **Subject** — Who/what, age, gender, expression, gaze, features
   - **Clothing / Product** — Fabric, color, fit, design details
   - **Environment** — Location, time of day, atmosphere, props
   - **Lighting** — Direction, quality, color temperature, named setup
   - **Camera & Lens** — Focal length feel, aperture/bokeh, angle, framing
   - **Color Grade** — Palette, film stock match, grade characteristics
   - **Composition** — Rule of thirds, negative space, leading lines
   - **Style & Mood** — Aesthetic, emotional tone

3. **Present Visual Analysis Summary** — Bullet points per dimension.

4. **Build Reconstructed Prompt** — Using the standard formula:
   ```
   [Subject] + [Action/Pose] + [Clothing/Product Detail] + [Environment] + [Lighting] + [Camera/Lens] + [Film Stock/Color Grade] + [Composition] + [Style/Mood] + [Exclusions]
   ```
   Flag uncertain elements with confidence notes.

5. **Ask what the user wants to do next:**
   - **Clone** — Reproduce as close as possible
   - **Style transfer** — Same visual DNA, different subject/product
   - **Scene variant** — Same subject, different setting
   - **Lighting variant** — Same scene, different lighting mood
   - **Outfit/color variant** — Same person/setting, change clothing
   - **Mood variant** — Same composition, shift color grade or film stock
   - **Format variant** — Adapt for different aspect ratio or platform
   - **Series** — Generate N variants with a consistent element

6. **Generate variant prompt(s)** based on user choice:
   - For **clone**: use reconstructed prompt verbatim
   - For **style swap**: keep lighting, camera, film, composition → replace subject/environment
   - For **series**: identify LOCKED vs VARIABLE elements, present each variant numbered

7. **Feedback loop** — After user tests the prompt, ask for adjustments:
   > "Kết quả có gần giống chưa? Nếu chưa, bạn thấy khác nhau ở điểm nào — mình sẽ tinh chỉnh prompt."

8. **Cross-skill suggestions:**
   - Need consistent character across variants → `/setup-consistency`
   - Want to animate the result → `/animate-to-video`
   - For a TikTok ad with this style → `/create-tiktok-ad`
