---
name: image-analysis
description: >
  Analyze a user-provided image and reconstruct it as a Nano Banana 2 prompt, then generate
  clone or variant prompts based on the original. Use when the user uploads or references an
  image and asks to "clone", "copy this style", "làm tương tự", "tạo biến thể", "nhân vật giống",
  "phân tích ảnh", "reverse prompt", "recreate this", "analyze this image", "tạo thêm ảnh kiểu này",
  "giống ảnh này", "variant", "style này", or wants to replicate/adapt an existing visual.
metadata:
  version: "0.1.0"
---

# Image Analysis & Variant Generator

Analyze any reference image, reconstruct it as a production-ready Nano Banana 2 prompt, then generate clones or custom variants on demand.

---

## Phase 1: Analyze the Image

When the user provides an image, systematically read it across these dimensions and write down your observations internally before presenting:

### Analysis Dimensions

**Subject**
- Who/what is in the frame (person, product, scene, food...)
- Age range, gender, ethnicity/skin tone if applicable
- Expression, gaze direction, body language
- Key identifying features (hair style/color, distinguishing details)

**Clothing / Product**
- Fabric type and texture (silk, linen, denim, knit...)
- Color with precise qualifier (dusty rose, warm camel, cool slate grey...)
- Fit and silhouette (oversized, tailored, structured...)
- Specific design details (collar type, hem, pattern, logo visibility)

**Environment / Setting**
- Location type and specific details
- Time of day implied by light
- Atmospheric elements (mist, particles, rain, bokeh type)
- Props and supporting elements

**Lighting**
- Direction (upper-left, side, back, overhead...)
- Quality (soft diffused, harsh directional, dappled, rim light)
- Color temperature (warm golden, cool daylight, tungsten orange)
- Named setup if identifiable (Rembrandt, butterfly, clamshell, window light)

**Camera & Lens**
- Estimated focal length feel (wide environmental, standard, portrait compression, telephoto)
- Aperture feel (bokeh amount → estimated f-stop range)
- Shooting angle (eye-level, slightly low, high, top-down)
- Framing (full-length, 3/4, medium, close-up, extreme close-up)

**Color Grade & Film Stock**
- Overall color palette (warm/cool, saturated/desaturated, high/low contrast)
- Closest film stock match (Kodak Portra 400, Fujifilm Pro 400H, CineStill 800T...)
- Any notable grade characteristics (lifted blacks, teal shadows, skin warmth...)

**Composition**
- Rule of thirds / centered / diagonal / symmetrical
- Negative space placement and amount
- Leading lines or framing elements

**Style & Mood**
- Overall aesthetic (editorial, UGC, commercial, lifestyle, luxury, raw...)
- Emotional tone (warm, aspirational, intimate, bold, dreamy...)

---

## Phase 2: Present the Analysis & Reconstructed Prompt

Present findings in two blocks:

### Block 1 — Visual Analysis Summary
Write a concise breakdown (bullet points per dimension). Keep it readable — this helps the user understand what was detected and correct any misreads.

### Block 2 — Reconstructed Nano Banana 2 Prompt
Build the prompt using the standard formula:
```
[Subject] + [Action/Pose] + [Clothing/Product Detail] + [Environment/Setting] + [Lighting] + [Camera/Lens/Aperture] + [Film Stock/Color Grade] + [Composition/Framing] + [Style/Mood] + [Exclusions]
```

Present in a code block. Note confidence level on uncertain elements (e.g., *"lens estimated 85mm — adjust if needed"*).

---

## Phase 3: Understand Variant Intent

After presenting the analysis, ask what the user wants to do next using AskUserQuestion:

**Option framing (suggest these, don't force):**

- **Clone** — Reproduce as close as possible to the original
- **Style transfer** — Keep the visual DNA, change the subject/product
- **Scene variant** — Same subject, different setting or time of day
- **Lighting variant** — Same scene, different lighting mood (golden hour → overcast, studio → natural)
- **Outfit/color variant** — Same person and setting, change clothing details
- **Mood variant** — Same composition, shift the color grade or film stock
- **Format variant** — Adapt for a different aspect ratio or platform (square, 9:16, banner)
- **Series** — Generate N variants with a consistent element (same model, different outfits)

Ask: *"Bạn muốn clone y hệt, hay thay đổi gì? (ví dụ: đổi outfit, background, lighting, nhân vật khác nhưng cùng style...)"*

---

## Phase 4: Generate Variant Prompts

Based on user intent, generate the variant prompt(s):

### Clone
Use the reconstructed prompt from Phase 2 verbatim. Add note: *"Add your own model/product description to replace bracketed elements."*

### Style / Subject Swap
Keep: lighting setup, camera specs, film stock, composition, mood keywords.
Replace: subject description, clothing, environment as requested.

### Lighting / Mood Variant
Keep: subject, clothing, composition.
Replace: lighting direction + quality + color temperature + film stock to match the new mood.

### Series (multiple variants)
For N variants, present each as a numbered prompt. Identify the **locked elements** (consistent across all) and **variable elements** (what changes per variant) at the top so the user understands the system.

```
LOCKED:   [subject DNA] + [camera specs] + [film stock] + [composition]
VARIABLE: [element changing per variant]

Variant 1: ...
Variant 2: ...
Variant N: ...
```

---

## Confidence & Correction Loop

If the image is ambiguous on any dimension (e.g., can't determine exact focal length or film stock), flag it explicitly and offer two options rather than guessing silently:

*"Lighting looks like either window light or a large softbox — does the original have a specific setup you know of?"*

After the user tries the reconstructed prompt in Nano Banana 2, invite feedback:
*"Kết quả có gần giống chưa? Nếu chưa, bạn thấy khác nhau ở điểm nào — mình sẽ tinh chỉnh prompt."*

---

## When to Suggest Other Skills

- If the variant requires maintaining the same character across multiple images → suggest **character-consistency** skill
- If the user wants to animate the result → suggest **video-motion** skill
- If the variant is for a TikTok ad → hand off to **tiktok-ad-creator** skill with the reconstructed prompt as the brief
