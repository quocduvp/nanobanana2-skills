---
name: product-commerce
description: >
  Create Nano Banana 2 prompts for product photography and e-commerce imagery. Use when the user
  mentions "product shot", "e-commerce", "sản phẩm", "thương mại", "hero image", "flat lay",
  "product photo", "packaging", "mockup", "amazon listing", "shopee", "lazada", "product on
  white background", or needs professional product imagery for online stores, marketplaces, or
  advertising.
metadata:
  version: "0.1.0"
---

# Product & Commerce Prompt Specialist

Generate Nano Banana 2 prompts for professional product photography — hero shots, flat lays, lifestyle product, and marketplace-ready images.

## Product Photography Categories

### 1. Hero Product Shot (Clean/Studio)

Purpose: Primary listing image, website hero, advertising focal point.

Template:
```
Hero product image of [product: exact description — material, color, finish, size relative cues,
key design details, brand-style but no real logos]. Placed on [surface: polished marble / matte
concrete / brushed metal / gradient backdrop — match product premium level]. [Angle: 45-degree
product angle / straight-on / slight 3/4 turn]. Shot with [85-100mm macro lens], [f/2.8-4].
[Lighting: soft key light from upper-left with [fill/rim/accent] creating [specific shadow and
highlight behavior on the product material]]. [Background: clean gradient / solid color / subtle
texture]. 4K resolution, razor-sharp focus, accurate material rendering. [Premium/casual/tech]
product photography. No dust, no fingerprints, no color bleeding, no logo distortion, no
reflection errors.
```

Surface matching guide:
- **Luxury/beauty**: Polished marble, velvet, frosted glass
- **Tech**: Matte black surface, reflective dark glass, brushed aluminum
- **Organic/natural**: Raw wood, linen, stone
- **Fashion accessories**: Leather, suede, textured fabric
- **Food products**: Ceramic, rustic wood, slate

### 2. Flat Lay (Top-Down Arrangement)

Template:
```
Top-down flat lay of [list every item with material, color, and relative size]. Arranged with
[layout style: grid / organic scatter / diagonal flow / radial] and [spacing: generous negative
space / tightly curated / overlapping edges]. On [surface: textured linen / marble / concrete /
colored paper]. [Prop elements: dried botanicals / fabric swatches / small accessories — keep
minimal]. Soft diffused overhead lighting, minimal shadows. Shot on [camera] with [35mm f/2.8
from above]. [Color grade: neutral true-to-life / warm editorial / cool minimal]. [Negative
space in (position) for text overlay]. No overlapping main products, no wrinkles on fabric,
no color cast, no items cut off at edges.
```

Layout styles:
- **Grid**: Clean, organized, e-commerce catalog feel
- **Organic scatter**: Lifestyle, editorial, Instagram-ready
- **Diagonal flow**: Dynamic, leading the eye, campaign imagery
- **Radial**: Centered hero product with supporting items around it

### 3. Lifestyle Product (In-Use Context)

Template:
```
Lifestyle product photograph of [product with full description] [in use: being held / worn /
placed in natural setting / being interacted with by person]. [Person description if present:
hands only / partial figure / full model with outfit]. In [lifestyle environment: kitchen /
bathroom / living room / outdoor café / office desk — be specific about style: Scandinavian,
industrial, Japanese minimal, etc.]. [Natural lighting matching environment]. Shot on [camera]
with [50-85mm], [f/1.8-2.8 for bokeh separation]. [Warm / airy / cozy] color palette. Medium
close-up focused on product with [environment softly blurred behind]. Lifestyle brand
photography, [mood]. Product must be clearly identifiable and the hero of the composition.
No harsh reflections, no cluttered background, no competing focal points.
```

### 4. Multi-Angle Product Series

When generating multiple angles of the same product for a listing:

1. Start with master reference shot on plain white/neutral background
2. Generate these standard e-commerce angles:
   - Front-facing straight-on
   - 45-degree 3/4 view
   - Side profile
   - Back view
   - Detail close-up (texture/material/craftsmanship)
   - Scale shot (with hand or common object for size reference)
3. Each prompt: reference the master image and specify "maintain exact same product appearance"

### 5. Before/After & Comparison

Template:
```
Split-image product comparison showing [product] in two states: [left side: description]
and [right side: description]. Clean dividing line in center. Identical lighting setup,
identical camera angle, identical background on both sides. [Studio lighting]. Shot on
[camera with lens]. Professional comparison photography. Labels: "[LEFT LABEL]" on left,
"[RIGHT LABEL]" on right in clean sans-serif white text.
```

## E-Commerce Platform Optimization

- **White background listing** (Amazon, Shopee, Lazada style): Specify "pure white (#FFFFFF) background, product fills 85% of frame, no shadows or minimal contact shadow only"
- **Social media ad**: Include text-safe negative space, more lifestyle context, warmer mood
- **Website hero banner**: Wide 16:9 format, product on one side, negative space for headline on other side
- **Instagram square**: 1:1 composition, centered or rule-of-thirds, visually striking

## Editing Prompts for Existing Product Photos

### Background Swap
```
[Attach original product photo]
Edit: Replace the background with [new background description]. Keep the product exactly
as-is — same lighting on product, same angle, same shadows. Only change the background.
Blend naturally.
```

### Product Color Variant
```
[Attach original product photo]
Edit: Change the product color from [current] to [new color]. Maintain all other details:
same shape, same texture quality, same lighting reflections adjusted for new color, same
background. Only change the color.
```

### Add Lifestyle Context
```
[Attach clean product shot]
Place this product naturally into [lifestyle scene description]. Match the lighting of the
scene to the product — adjust shadows and reflections to look physically present in the
environment. The product should be the focal point.
```

## Reference

Read `references/surface-lighting-pairs.md` for optimal surface + lighting combinations by product category.