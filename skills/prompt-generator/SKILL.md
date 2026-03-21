---
name: prompt-generator
description: >
  Generate professional Nano Banana 2 image prompts from user input. Use when the user asks to
  "write a prompt", "create an image prompt", "generate a Nano Banana prompt", provides a character
  description, outfit, background, product, or any visual concept and wants a ready-to-use prompt
  for Nano Banana 2 or Gemini image generation. Also triggers when the user says "prompt cho ảnh",
  "viết prompt", "tạo prompt", or describes any visual scene they want to generate.
metadata:
  version: "0.1.0"
---

# Nano Banana 2 Prompt Generator

Generate production-ready prompts for Nano Banana 2 (Gemini 3.1 Flash Image) optimized for lifestyle, fashion, food, skincare, and commerce photography.

## Core Prompt Formula

Every prompt MUST follow this structure. Never skip components — each one dramatically affects output quality.

```
[Subject] + [Action/Pose] + [Clothing/Product Detail] + [Environment/Setting] + [Lighting] + [Camera/Lens/Aperture] + [Film Stock/Color Grade] + [Composition/Framing] + [Style/Mood] + [Exclusions]
```

## How To Generate A Prompt

### Step 1: Gather Input

Ask the user (if not already provided) using AskUserQuestion:

1. **What** — Subject (person, product, scene)?
2. **Wear/Show** — Clothing, accessories, or product details?
3. **Where** — Background/environment?
4. **Mood** — What feeling? (warm, editorial, luxurious, fresh, cozy...)
5. **Purpose** — Where will this image be used? (social media, e-commerce listing, lookbook, campaign hero, banner...)
6. **Format** — Aspect ratio or specific format needs?

### Step 2: Build The Prompt

Construct the prompt following these rules:

**Subject Description — Be extremely specific:**
- Age, gender, ethnicity/skin tone (use Fitzpatrick or NCS codes if precision needed)
- Face shape, hair (style, length, color, texture), distinguishing features
- Body type, height impression
- Expression, gaze direction

**Clothing/Product — Material-level detail:**
- Fabric type (silk, linen, cashmere, denim, leather, cotton jersey...)
- Color with qualifier (dusty rose, sage green, warm camel, cool slate grey...)
- Fit descriptor (oversized, tailored, relaxed, structured, cropped...)
- Specific design elements (notched lapel, raw hem, pleated, ribbed knit...)

**Environment — Immersive context:**
- Specific location (not just "café" → "sunlit minimalist Scandinavian café with light oak furniture and terrazzo floors")
- Time of day implied by lighting
- Atmospheric elements (morning mist, golden dust particles, rain on windows...)

**Lighting — The single most powerful variable:**
- Direction: upper-left, behind subject, overhead, side-lit
- Quality: soft diffused, harsh directional, dappled, rim light
- Color temperature: warm golden, cool daylight, tungsten orange
- Setup name: Rembrandt lighting, butterfly lighting, clamshell, natural window light

**Camera + Lens — Treat like a cinematographer brief:**
- Camera body: Sony A7III, Canon EOS R5, Hasselblad X2D, Fujifilm X-T5, Phase One XF
- Lens: 35mm (environmental), 50mm (standard), 85mm (portrait compression), 135mm (fashion telephoto)
- Aperture: f/1.2-1.8 (dreamy bokeh), f/2.8-4 (product sharp), f/5.6-8 (environmental sharp)
- Angle: eye-level, slightly low (empowering), slightly high (intimate), top-down (flat lay)

**Film Stock — Instant aesthetic control:**
- Kodak Portra 400: warm skin tones, soft contrast, fashion standard
- Kodak Portra 160: more subtle warmth, lower grain, beauty/skincare
- Fujifilm Velvia 50: vivid saturated colors, landscape/food
- Fujifilm Pro 400H: soft pastel, airy, lifestyle
- Kodak Ektar 100: punchy contrast, vivid, street/editorial
- Kodak Tri-X 400: classic black & white, gritty, editorial
- CineStill 800T: tungsten warmth, halation glow, cinematic night

**Composition:**
- Rule of thirds, centered, symmetrical, diagonal leading lines
- Negative space placement for text overlay (specify which side and percentage)
- Framing: full-length, 3/4, medium shot, close-up, extreme close-up, wide establishing

**Exclusions — Always include:**
- "No distorted fingers, no extra limbs, no watermarks, no text unless specified"
- Category-specific exclusions (see individual skill references)

### Step 3: Output Format

Present the prompt in a clean code block. Below it, provide:
- A brief explanation of key creative choices (2-3 sentences)
- Suggested variations (lighting change, different angle, alternate color palette)
- If the user wants consistency across images: remind them to use the character-consistency skill

## Prompt Length Guidelines

- **Minimum effective**: 50 words (basic scenes)
- **Optimal range**: 80-150 words (detailed professional output)
- **Maximum recommended**: 200 words (complex multi-element scenes)

## Quick Reference — Photography Terms That Work

Read `references/photography-terms.md` for the complete list of camera bodies, lenses, film stocks, lighting setups, and composition techniques that Nano Banana 2 responds well to.

## Language

Generate prompts in **English** (Nano Banana 2 performs best with English prompts). Communicate with the user in whatever language they use. If the user writes in Vietnamese, respond in Vietnamese but generate the actual prompt in English.