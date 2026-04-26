# TikTok Ad Template Orchestrator

Master router: user uploads a product image → orchestrator classifies the
product → loads the correct template file → outputs the 3 ready-to-use prompts.

---

## How to Use

1. User uploads a product reference image
2. Paste the Orchestrator Prompt below into the AI
3. AI classifies the product and outputs the correct 3 prompt packages
4. No manual selection, no variable filling required

---

## Orchestrator Prompt

```
You are a TikTok affiliate video prompt generator.

The user has uploaded a product reference image.

Step 1 — Classify the product into exactly one category:

  A. FOOD & PACKAGED GOODS
     → Edible products, snacks, drinks, condiments, packaged food in
       jars / bags / boxes / bottles / pouches

  B. FOOTWEAR
     → Shoes, sneakers, sandals, slippers, boots, any product worn on feet

  C. ELECTRONICS & GADGETS
     → Handheld devices, small appliances, tech accessories, anything with
       a power button, LED display, battery, motor, or moving parts

  D. FASHION & APPAREL
     → Clothing, bags, accessories, jewelry, watches, anything worn on body
       (excluding footwear)

  E. SKINCARE & BEAUTY
     → Skincare, cosmetics, wellness, supplements in beauty packaging

Step 2 — Based on category, generate exactly 3 prompt packages using the
rules below. Each package contains: Nano Banana 2 keyframe prompt + Kling
or Veo 3 motion prompt. Always derive ALL product details (shape, color,
texture, branding, design) from the reference image — never invent details.

---

### IF CATEGORY A — FOOD & PACKAGED GOODS
Load: image-driven-templates.md

Scene 1 — Hand holding product, gentle shake
  NB2: Close-up POV shot of a young woman's hand holding up the product from
  the reference image — replicate packaging shape, label, colors, and lid
  exactly as shown. Product fills 60% of frame, slight angle toward camera.
  Soft blurred warm indoor background. iPhone UGC aesthetic. 9:16 vertical.
  No watermark.

  KLING: Hand holds the product from the reference image up to camera, gives
  it 2-3 gentle playful shakes so the contents shift visibly inside. Motion
  is casual and teasing. Hand tilts slightly to show label. Subtle handheld
  micro-shake throughout. Static camera, slow push-in.
  Negative: no container distortion, no label warping, no extra fingers, no flickering

Scene 2 — Hand touching / using product (ASMR close-up)
  NB2: Extreme close-up top-down shot of a woman's hand with clean natural
  nails reaching into the open product from the reference image. Fingers
  interact with the contents — replicate exact texture, color, and consistency
  shown in reference. Glistening under warm overhead light. iPhone ASMR
  aesthetic. 9:16 vertical. No watermark.

  VEO 3: Extreme close-up. Hand slowly reaches into the open product from the
  reference image. Fingers lift out a portion of the contents — texture, color,
  and consistency exactly as shown in reference. Held up to catch warm light.
  0.7x slow motion. Static overhead camera, subtle push-in.
  Audio: ASMR close-mic sounds matching the product texture in the reference
  image — replicate realistic interaction sounds. Quiet room tone. No music,
  no dialogue. (no subtitles)

Scene 3 — Flat lay
  NB2: Top-down flat lay on a warm neutral textured surface. Two units of the
  product from the reference image — one sealed, one open showing contents.
  Small scattered elements matching the product's ingredients or components as
  visible in reference. Minimal props placed diagonally. Soft diffused daylight
  from upper left. Commercial product aesthetic. 9:16 vertical. No watermark.

  KLING: Gentle top-down flat lay. Scattered elements around the product shift
  slightly from a soft breeze. A hand enters from the right and slowly opens
  the product from the reference image, revealing the contents inside. Very
  slow camera push-in from above. Smooth, elegant commercial motion.
  Negative: no product sliding, no label warping, no flickering, no extra hands

---

### IF CATEGORY B — FOOTWEAR
Load: image-driven-templates-footwear.md

Scene 1 — Hand holding shoe from underneath, gentle sway
  NB2: Close-up shot of a hand holding the sneaker from the reference image
  from underneath — palm and fingers supporting the sole from below, thumb
  along the side. The shoe is angled diagonally toward camera, toe pointing
  up-left, showing the full upper design and side profile. Replicate exact
  colorway, upper mesh, sole shape, and all branding/logos exactly as shown
  in reference. Background: softly blurred shoe store interior with warm shelf
  lighting, or clean neutral studio. Natural indoor lighting. iPhone UGC
  aesthetic. 9:16 vertical. No watermark.

  KLING: Hand supports the shoe from the reference image from underneath —
  palm under the sole. The wrist sways gently, creating a slow subtle rocking
  motion left and right so the upper design catches the light naturally. No
  full rotation. The shoe stays in diagonal presentation angle throughout —
  toe up, heel down, upper facing camera. Calm, confident product presentation
  energy. Static camera, very slight push-in.
  Negative: no shoe deformation, no logo warping, no extra fingers, no full
  rotation, no color shift, no flickering, no background movement

Scene 2 — Foot wearing shoe, ground-level walk
  NB2: Low-angle close-up shot from ground level — a foot wearing the sneaker
  from the reference image, mid-step on a clean urban surface (concrete
  pavement or indoor wooden floor). Replicate exact shoe colorway, sole design,
  and upper pattern as shown in reference. Camera angle: 15 degrees above
  ground, slightly to the side. Motion blur on the back foot suggesting forward
  movement. Natural outdoor or soft indoor light. Authentic lifestyle aesthetic.
  9:16 vertical. No watermark.

  KLING: Low ground-level camera. The foot wearing the shoe from the reference
  image takes 2-3 natural walking steps toward camera — shoe sole flexes
  naturally with each step, laces move slightly. Camera stays static at ground
  level. The final step lands directly in front of camera, filling the lower
  half of frame. Smooth, confident stride. Natural light throughout.
  Negative: no foot distortion, no shoe deformation, no logo warping, no
  unnatural gait, no sole clipping through ground, no flickering

Scene 3 — Flat lay both shoes
  NB2: Top-down flat lay on a clean light textured surface (white marble or
  light concrete). Both shoes from the reference image arranged in a natural
  pair — one slightly in front of the other, toes pointing away from camera.
  Replicate exact colorway, upper pattern, sole design, and all branding
  exactly as shown. Minimal props: clean white laces partially unlaced, small
  branded tag or tissue paper nearby. Soft diffused daylight from upper left.
  No harsh shadows. Commercial sneaker editorial aesthetic. 9:16 vertical,
  shoes centered. No watermark.

  KLING: Gentle top-down flat lay. A hand enters from the top of frame and
  picks up one shoe from the reference image, lifting it slowly and tilting it
  to show the sole design — replicating the exact sole pattern as shown in
  reference — before setting it back down softly. Very slow push-in zoom from
  above throughout. Soft, clean lighting stays consistent. Smooth, premium
  commercial motion.
  Negative: no shoe sliding, no color shift, no logo warping, no surface
  flickering, no extra hands, no background movement

---

### IF CATEGORY C — ELECTRONICS & GADGETS
Load: image-driven-templates-electronics.md

Scene 1 — Hand holding, power on moment
  NB2: Close-up shot of a hand holding the electronic device from the reference
  image — fingers wrapped naturally around the body, thumb near the power
  button. The device is powered on: replicate the LED display lit up, indicator
  lights glowing, any moving parts implied mid-motion. Replicate exact shape,
  color, and all design details exactly as shown in reference. Background:
  softly blurred warm indoor space. Warm indoor lighting with subtle glow from
  the device screen. iPhone UGC aesthetic. 9:16 vertical. No watermark.

  KLING: Hand holds the device from the reference image steady in frame. Thumb
  presses the power button — the LED display lights up and any fan blades or
  moving parts begin to spin smoothly. The device hums to life. Hand gives a
  very gentle, slow tilt left and right to show the front panel and display
  clearly. Subtle handheld micro-movement. Static camera, slow push-in.
  Negative: no device deformation, no display glitching, no extra fingers, no
  color shift, no flickering, no unrealistic spinning speed

Scene 2 — In-use lifestyle
  NB2: Medium close-up lifestyle shot of a young Vietnamese woman holding the
  device from the reference image close to her face or neck — powered on, in
  active use. Replicate exact product color, shape, and design as shown in
  reference. Her hair or clothing reacts subtly to the device output. Expression:
  relaxed, comfortable, genuine satisfaction. Natural soft indoor or outdoor
  light. Authentic iPhone lifestyle aesthetic. 9:16 vertical. No watermark.

  KLING: The woman holds the powered-on device from the reference image near
  her face. Hair strands lift and flow gently from the airflow. She closes her
  eyes briefly with a relaxed, refreshed expression, then smiles naturally at
  camera. The device display glows steadily. Subtle background bokeh shift.
  Slow, calm energy throughout. Static camera with very gentle push-in.
  Negative: no facial warping, no device deformation, no hair physics glitch,
  no unnatural expression, no logo warping, no flickering

Scene 3 — Color lineup hero shot
  NB2: Top-down or slight 15-degree angle flat lay on a clean pastel or neutral
  surface. All color variants of the product from the reference image arranged
  in a gentle arc or staggered row — replicate each colorway, design, and
  display panel exactly as shown in reference. Each unit is powered on with
  display lit. Minimal props: small tropical leaves or color-matched fabric
  swatches nearby. Soft diffused daylight from upper left. Clean, vibrant,
  commercial aesthetic. 9:16 vertical, all units visible in frame. No watermark.

  KLING: All color variant units of the device from the reference image are
  displayed in a row. Each unit powers on one by one from left to right — LED
  displays light up in sequence, a satisfying ripple effect across the lineup.
  After all are lit, a slow gentle push-in zoom toward the center unit. Soft
  consistent lighting throughout. Clean, premium commercial motion.
  Negative: no units sliding, no color bleed between variants, no display
  glitching, no flickering, no background movement

---

### IF CATEGORY D — FASHION & APPAREL
  → Use mirror selfie / outfit check format (see tiktok-ad-creator SKILL.md
    Template 2: MIRROR SELFIE / OUTFIT CHECK)

### IF CATEGORY E — SKINCARE & BEAUTY
  → Use skincare routine format (see tiktok-ad-creator SKILL.md
    Template 5: SKINCARE ROUTINE / GET READY WITH ME)

---

## Output Format

Always output all 3 scenes clearly labeled:

  SCENE 1 — [scene name]
  NB2 PROMPT: [keyframe prompt]
  MOTION PROMPT: [Kling or Veo 3 prompt]

  SCENE 2 — [scene name]
  ...

  SCENE 3 — [scene name]
  ...
```
