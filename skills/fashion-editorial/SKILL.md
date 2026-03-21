---
name: fashion-editorial
description: >
  Create Nano Banana 2 prompts specifically for fashion editorial, lookbook, streetwear, and
  runway photography. Use when the user mentions "fashion", "editorial", "lookbook", "outfit",
  "streetwear", "runway", "collection", "fashion campaign", "thời trang", "lookbook", "outfit",
  or wants to generate fashion-focused imagery with specific clothing, styling, and model direction.
metadata:
  version: "0.1.0"
---

# Fashion Editorial Prompt Specialist

Generate Nano Banana 2 prompts for professional fashion photography across editorial, lookbook, streetwear, and campaign styles.

## Fashion Photography Categories

### 1. High-Fashion Editorial

Purpose: Magazine covers, editorial spreads, brand campaigns.

Template:
```
Editorial fashion photograph of [model description: age, build, skin tone, hair, makeup style]
wearing [outfit: designer-inspired description with fabric, color, silhouette, accessories].
[Dramatic pose: specific body position, hand placement, gaze direction] in [high-concept
location or studio setup]. [Professional lighting: name the setup — Rembrandt, butterfly,
split, dramatic single softbox]. Shot on [Hasselblad X2D / Phase One XF] with [80-120mm lens],
[f/2.8-5.6]. [Color grade: crisp neutral / moody desaturated / high-contrast editorial].
[Framing: full-length / 3/4 / close-up]. High-fashion editorial style, [mood: commanding /
ethereal / provocative / minimal]. No color fringing, no distracting elements, no distorted
proportions.
```

Key elements:
- Use high-end camera bodies (Hasselblad, Phase One, Canon EOS R5)
- Lighting must be specific and dramatic
- Pose direction should be precise (not "standing nicely" → "weight on back foot, chin tilted 15 degrees right, direct confrontational gaze")
- Mention makeup style explicitly (bold red lip, dewy glass skin, graphic eyeliner, no-makeup makeup)

### 2. Lookbook / Catalog

Purpose: E-commerce clothing listings, seasonal collections, brand websites.

Template:
```
Clean lookbook photograph of [model description] wearing [full outfit description with every
visible item — top, bottom, shoes, accessories, each with fabric and color]. [Natural relaxed
pose: walking, mid-turn, hands in pockets, adjusting sleeve] in [clean environment: white
cyclorama / neutral studio / simple lifestyle location]. [Soft even lighting: large softbox
or natural window light, minimal shadows]. Shot on [Sony A7IV / Canon R6] with [50-85mm],
[f/4-5.6 for full sharpness]. True-to-life colors, no heavy color grade. [Full-length shot
showing complete outfit including shoes]. Commercial lookbook style, approachable and clean.
No harsh shadows, no dramatic angles, no cropped clothing items.
```

Key elements:
- MUST show complete outfit head-to-toe
- Colors must be true-to-life (not stylized)
- Lighting should be flat and even — clothing detail is priority
- Pose should feel natural but show the garments clearly

### 3. Streetwear / Urban

Template:
```
Streetwear [lookbook/editorial] photograph of [model: age, attitude, hair, build] wearing
[urban outfit: graphic tee, cargo pants, sneakers — brand-inspired but no logos]. [Confident
pose with urban body language] in [gritty location: alley, parking garage, concrete underpass,
rooftop]. [Lighting: overcast natural / neon ambient / golden hour side-light]. Shot on
[Leica Q3 / Fujifilm X-T5] with [28-35mm wide]. [Film-like grade: Kodak Tri-X pushed /
CineStill 800T / slightly desaturated]. [Full-length or 3/4 shot, low angle for power].
Raw street photography aesthetic, authentic mood. No over-processed skin, no artificial
bokeh, no clean studio feel.
```

### 4. Accessories Focus

Template:
```
Close-up fashion photograph focusing on [accessory: watch/jewelry/bag/sunglasses/shoes with
precise material and design description]. [Worn by / placed on: on model's wrist with outfit
context / styled on marble surface]. [Detail lighting: soft side light emphasizing texture and
material quality, catching metallic surfaces]. Shot on [macro-capable lens: 90mm macro or
100mm f/2.8], [f/2.8-4]. Shallow depth of field isolating the accessory. [Warm/cool tone
matching brand palette]. Luxury accessories photography. No dust, no fingerprints, no
reflection distortion.
```

## Model Direction Cheat Sheet

Read `references/model-direction.md` for pose vocabulary, hand positions, gaze types, and body language terms that Nano Banana 2 interprets accurately.

## Seasonal & Trend Considerations

When the user mentions a season or trend, layer these atmospheric elements:

- **Spring/Summer**: soft natural light, outdoor settings, light fabrics, movement (wind in hair, flowing skirt)
- **Autumn/Winter**: warm golden/tungsten lighting, layered textures, cozy indoor settings, moodier tones
- **Resort/Holiday**: bright tropical light, water reflections, relaxed poses, vivid colors
- **Minimalist trend**: clean lines, monochrome palette, negative space, architectural backgrounds
- **Y2K/Retro**: CineStill film stock, flash photography, slightly overexposed, vibrant pop colors

## Workflow for Multi-Look Campaigns

When generating multiple looks for the same campaign:

1. First, use the `character-consistency` skill to establish the model's Character DNA
2. Lock the Brand Style Guide (color grade, lighting style, mood)
3. Generate the hero shot first — this becomes the visual anchor
4. Each subsequent look: change ONLY the outfit and pose, keep everything else from the style guide
5. Use the previous output as reference for the next generation