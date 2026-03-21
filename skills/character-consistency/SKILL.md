---
name: character-consistency
description: >
  Create and manage Character DNA profiles and Brand Style Guides for consistent Nano Banana 2
  image generation across multiple shots. Use when the user mentions "consistency", "nhất quán",
  "same character", "same model", "cùng nhân vật", "character sheet", "style guide", "brand
  guide", "keep the same look", "maintain appearance", "series of images", "campaign consistency",
  or needs the same person/product/style to appear identically across multiple generated images.
metadata:
  version: "0.1.0"
---

# Character & Brand Consistency Manager

Create and maintain Character DNA profiles, Brand Style Guides, and Product Reference Profiles to ensure visual consistency across multiple Nano Banana 2 generations.

## Three Pillars of Consistency

### Pillar 1: Character DNA (Person Consistency)

Create a detailed "anchor profile" for any person who needs to appear consistently across images.

#### Step 1: Build Character DNA

Ask the user for (or derive from their reference image description):

```
CHARACTER DNA: "[Name]"

Physical:
- Age: [specific age]
- Gender: [gender]
- Ethnicity/Skin tone: [specific — e.g., "warm olive, approximately NC30" or "fair with pink undertones, NW15"]
- Face shape: [oval / round / square / heart / diamond / oblong]
- Eyes: [shape, size, color, distinguishing features — e.g., "almond-shaped dark brown with subtle monolid"]
- Nose: [shape — straight, button, aquiline, wide bridge, narrow, rounded tip]
- Lips: [shape, fullness — full with defined cupid's bow, thin, medium with natural pink]
- Eyebrows: [shape, thickness — straight thick brows, arched thin, natural bushy]
- Distinguishing features: [beauty marks, dimples, freckles, scars, jaw definition]

Hair:
- Length: [specific — shoulder-length, mid-back, pixie, buzz cut]
- Texture: [straight, wavy, curly, coily, kinky]
- Color: [specific — jet black, dark brown with chestnut highlights, platinum blonde]
- Style: [how it's typically worn — side-parted left, center-parted, pulled back, loose]

Body:
- Build: [slim, athletic, medium, curvy, plus-size, muscular]
- Height impression: [petite, average, tall — gives proportional cues]

Default expression: [warm natural smile, neutral composed, confident slight smile]
Default gaze: [direct to camera, slightly off-camera, looking down]

Makeup baseline: [none / natural minimal / specific default look]
```

#### Step 2: Generate Character Reference Sheet

Use this prompt to create a multi-angle reference:
```
Character reference sheet of [paste full Character DNA].
Show 4 views in a 2x2 grid: front-facing (top-left), 3/4 left profile (top-right),
3/4 right profile (bottom-left), and back view (bottom-right).
Clean white background. Neutral expression. Wearing a simple [white/grey] t-shirt.
Even studio lighting from front. Consistent proportions and features across all views.
Professional character design reference sheet.
```

#### Step 3: Use in Every Subsequent Prompt

For every new image of this character:
1. Attach the reference sheet image
2. Include at beginning of prompt: `"[Name]" — [paste abbreviated Character DNA: 2-3 key lines]`
3. Add at end: `Maintain exact same facial features, skin tone, hair, and body proportions as the reference image.`
4. Only change: outfit, pose, environment, lighting

### Pillar 2: Brand Style Guide (Visual Consistency)

Create a reusable style block prefixed to every prompt in a campaign.

#### Template

Ask the user about their brand, then construct:

```
BRAND STYLE GUIDE: "[Brand Name]"

Photography style: [specific lighting preference — natural window light, studio controlled, golden hour only...]
Color palette: [3-5 specific colors with qualifiers — "warm cream (#F5F0E8)", "sage green (#B2BDA0)", "dusty rose (#D4A5A5)"]
Film reference: [specific stock — Kodak Portra 400 for warm editorial / Fujifilm Pro 400H for airy / none for clean digital]
Color grade: [warm with lifted shadows / cool and crisp / neutral true-to-life / moody desaturated]
Composition rules: [rule of thirds / centered / always leave X% negative space on (side) for text]
Model styling: [makeup level, hair vibe, clothing aesthetic]
Environment family: [types of locations that fit the brand — minimalist interiors, natural outdoor, urban architectural]
Mood: [3 specific words — "warm, intimate, aspirational" / "bold, confident, editorial"]
Texture preferences: [natural fabrics, organic materials / sleek modern surfaces / mixed vintage]

ALWAYS INCLUDE: [signature elements — natural textures, warm light, specific prop type]
NEVER INCLUDE: [brand anti-patterns — neon colors, cluttered backgrounds, heavy filters, specific things to avoid]
```

#### Usage

Prefix every prompt in the campaign with the full style guide block. This creates visual coherence even when scenes, outfits, and compositions change.

### Pillar 3: Product Reference Profile (Product Consistency)

For products that need to appear identically across different settings:

```
PRODUCT PROFILE: "[Product Name]"

Type: [category — serum bottle, handbag, sneaker, coffee mug]
Material: [glass, leather, ceramic, metal, fabric — with finish: matte, glossy, brushed, frosted]
Color: [exact colors with hex if possible — "matte black body (#1A1A1A) with brushed gold cap (#C9A96E)"]
Shape: [specific form description — "tall cylindrical bottle with rounded shoulders, flat disc cap"]
Size reference: [height relative to hand, or specific dimensions]
Key details: [embossed logo placement, stitching pattern, texture gradient, label design elements]
Distinguishing features: [what makes this product unique and must be preserved]
```

For every image featuring this product, attach the master reference image and include:
`Depict the exact same product as shown in the reference image — same shape, color, material, proportions, and details.`

## Consistency Workflow for a Full Campaign

```
1. CREATE Character DNA for each model (max 5 for Nano Banana 2)
2. CREATE Brand Style Guide for the campaign
3. CREATE Product Reference Profiles for featured products
4. GENERATE Character Reference Sheets (multi-angle)
5. GENERATE master Product Reference Photos (clean, on white)
6. GENERATE Hero Shot — this becomes the visual anchor
7. For each subsequent shot:
   a. Attach relevant reference images
   b. Prefix with Brand Style Guide
   c. Include Character DNA summary
   d. Include Product Profile
   e. Specify new: outfit, pose, environment
   f. End with: "Maintain consistency with reference images"
8. Use ITERATIVE CHAINING — each output becomes reference for next
```

## Troubleshooting Consistency Drift

If characters start looking different across generations:

- **Face changing**: Add more facial anchor points (mention specific bone structure, exact eye shape)
- **Skin tone shifting**: Use specific color codes (Fitzpatrick scale or MAC shade numbers)
- **Hair inconsistent**: Describe exact parting, length relative to body landmarks, texture
- **Body proportions off**: Mention shoulder width relative to head, limb proportions
- **Style drifting**: Re-attach the original hero shot as reference anchor
- **Color grade shifting**: Always name the exact film stock, don't rely on mood words alone

## Nano Banana 2 Consistency Limits

- **Characters**: Up to 5 unique characters maintained per workflow session
- **Objects**: Up to 14 distinct objects tracked for fidelity
- **Reference images**: Up to 14 images can be attached in a single prompt
- **Best practice**: Use 3-5 clear reference images at similar angles and lighting
- **Critical**: Always use image references, not just text descriptions, for consistency