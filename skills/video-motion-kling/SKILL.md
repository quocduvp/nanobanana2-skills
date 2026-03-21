---
name: video-motion-kling
description: >
  Create Kling AI video generation prompts to animate Nano Banana 2 images into motion videos.
  Use when the user mentions "Kling", "video motion", "animate image", "image to video",
  "chuyển ảnh thành video", "tạo video", "motion", "Kling 3.0", "video từ ảnh", "animate",
  or wants to turn a still image into a dynamic video clip for TikTok, Reels, or advertising.
  Also triggers for camera movement, subject animation, product reveal, and multi-shot video.
metadata:
  version: "0.1.0"
---

# Kling AI Video Motion Prompt Specialist

Generate Kling 3.0 prompts to animate Nano Banana 2 images into professional motion videos — optimized for TikTok ads, product showcases, fashion lookbooks, and brand content.

## Core Workflow: Nano Banana 2 → Kling

```
Step 1: Generate still image with Nano Banana 2 (using other skills in this plugin)
Step 2: Use that image as "first frame" input in Kling Image-to-Video
Step 3: Write a Kling motion prompt focusing ONLY on movement + camera (scene already exists in image)
Step 4: Generate 5-10 second video clip
```

**Critical Rule for Image-to-Video:** When using a Nano Banana 2 image as first frame, the prompt should describe ONLY:
- What MOVES (subject action, environmental motion)
- How the CAMERA behaves (movement, speed, direction)
- Do NOT re-describe the scene — Kling already sees it in the image

## Kling 3.0 Prompt Formula

### Text-to-Video (Full Scene)
```
[Subject Description] + [Subject Movement] + [Scene/Environment] + [Camera Movement] + [Lighting/Atmosphere]
```

### Image-to-Video (Animate First Frame) — PRIMARY USE CASE
```
[Subject Movement] + [Camera Movement] + [Atmospheric Motion]
```

## Prompt Templates by Video Type

### 1. Product Reveal / Hero Shot Animation

**From still product image → dramatic reveal video:**

```
KLING PROMPT (Image-to-Video):
The product slowly rotates 30 degrees clockwise with a subtle floating motion.
Soft light rays shift gradually from left to right, catching new specular highlights
on the surface. Slow dolly-in from medium shot to close-up over 5 seconds.
Shallow depth of field background gently pulses with bokeh. (no camera shake)

NEGATIVE PROMPT:
no sudden movements, no camera drift, no flickering lights, no object deformation,
no changing product shape, no motion blur on product
```

**Variations:**
- **360 Spin**: "The product rotates 360 degrees on its axis, smooth and continuous, revealing all angles. Camera stays static at eye level."
- **Dramatic Zoom**: "Very slow push-in (dolly-in) focusing tighter and tighter on the product's key detail. Background bokeh intensifies."
- **Floating/Levitating**: "The product gently levitates with a subtle up-and-down floating motion (2cm oscillation). Particles of light drift around it."

### 2. Fashion Model Animation

**From still fashion image → natural movement:**

```
KLING PROMPT (Image-to-Video):
The model takes a confident step forward, coat swaying naturally with the movement.
Hair catches a gentle breeze from the right. Subtle weight shift from back foot to
front foot. Natural blink and slight smile forming. Slow tracking shot following
the model's forward movement. Fabric flows realistically with body physics.

NEGATIVE PROMPT:
no facial warping, no changing facial features, no extra fingers, no limb
distortion, no unnatural fabric physics, no robotic movement
```

**Variations by pose type:**
- **Hair flip**: "The model turns her head to the right, hair sweeping dramatically across. Wind catches the hair mid-motion. Slow motion 0.5x speed. Camera stays static."
- **Jacket adjustment**: "The model reaches up to adjust the collar of the jacket, pulling it slightly. Confident head tilt follows. Medium tracking shot."
- **Walking toward camera**: "The model walks confidently toward the camera with natural arm swing and hip movement. Slight smile. Camera slowly dollies backward maintaining framing."
- **Look-back-over-shoulder**: "The model turns 90 degrees away, then looks back over the shoulder at camera with a confident expression. Hair sways with the turn. Static camera, slight slow motion."

### 3. Food Motion

**From still food image → appetizing motion:**

```
KLING PROMPT (Image-to-Video):
Steam rises gently from the hot dish in soft, wispy curls. A hand enters frame
from the right, picks up chopsticks, and lifts noodles creating a satisfying
stretch. Sauce glistens as light shifts subtly. Very slow push-in toward the dish.
Warm atmospheric glow.

NEGATIVE PROMPT:
no unrealistic food physics, no melting objects, no changing dish appearance,
no sudden lighting changes, no camera shake
```

**Variations:**
- **Sauce pour**: "Thick golden sauce is slowly poured from above, draping over the dish. Each layer catches the light. Close-up static shot. Real-time speed."
- **Cheese pull**: "Hands pull apart the food revealing a long, stretchy cheese pull. Slow motion 0.5x. Static close-up. Steam rises from the hot interior."
- **Coffee pour**: "Hot coffee streams into the cup in a smooth pour. Crema forms on the surface. Steam curls upward. Close-up tracking the liquid."
- **Garnish drop**: "Fresh herbs drop from above onto the plated dish in slow motion. Each leaf lands softly. Slight bounce. Top-down static camera."

### 4. Skincare/Beauty Motion

**From still beauty/product image → luxurious motion:**

```
KLING PROMPT (Image-to-Video):
The dropper slowly releases a single golden serum drop. The drop falls in slow motion
and lands on a smooth surface, creating delicate ripples that expand outward.
Light refracts through the serum creating golden caustics. Extreme close-up,
very slow dolly-in. Luxurious and mesmerizing.

NEGATIVE PROMPT:
no unrealistic liquid physics, no product deformation, no flickering,
no sudden movements, no label distortion
```

**Variations:**
- **Cream texture spread**: "A finger slowly swirls into the cream, creating a satisfying spiral pattern. The texture is thick and smooth. Macro close-up, static."
- **Mist spray**: "A fine mist is sprayed from the bottle, catching the backlight in slow motion. Tiny droplets glitter in the air. Side-lit dramatic."
- **Product application on skin**: "Hands gently apply the product to the face in upward strokes. Skin appears to glow progressively as the product is absorbed. Medium close-up."

### 5. Mirror Selfie / UGC Style

**From still mirror selfie image → authentic motion:**

```
KLING PROMPT (Image-to-Video):
The person holds up a phone taking a mirror selfie. Slight natural body sway and
weight shift. Hand adjusts outfit — tugging at hem, smoothing fabric. Confident
smile forms. Subtle head tilt. Phone screen reflection catches the light.
Handheld smartphone camera feel with micro-movements. Natural indoor daylight.

NEGATIVE PROMPT:
no facial warping, no phone distortion, no mirror glitch, no unnatural
movements, no changing clothes, no extra fingers on phone
```

### 6. Unboxing Motion

**From still unboxing setup image → satisfying reveal:**

```
KLING PROMPT (Image-to-Video):
Hands slowly lift the lid of the box, revealing the product nestled inside.
Tissue paper rustles as it's gently pulled aside. The product catches the light
as it's revealed. Hands carefully lift the product out, turning it to show
different angles. Overhead camera slowly dollies in during the reveal moment.
Soft ASMR-like careful movements.

NEGATIVE PROMPT:
no sudden movements, no product distortion during handling, no changing hand
appearance, no unrealistic object physics, no flickering
```

## Camera Movement Vocabulary for Kling

### Movement Types (use these exact terms)

| Camera Term | Effect | Best For |
|---|---|---|
| **Slow dolly-in** | Gradually moves closer | Product focus, dramatic reveal, intimacy |
| **Slow dolly-out** | Gradually pulls back | Context reveal, environmental storytelling |
| **Tracking shot (left/right)** | Follows subject laterally | Fashion walking, lifestyle motion |
| **Crane up** | Camera rises upward | Grand reveal, establishing shot |
| **Crane down** | Camera descends | Approaching detail, food top-to-side |
| **Orbit (clockwise/counter)** | Circles around subject | Product 360, dramatic portrait |
| **Static shot** | No camera movement | Food, beauty macro, clean action |
| **Slow pan (left/right)** | Camera rotates in place | Scene scanning, lookbook |
| **Tilt up/down** | Camera pivots vertically | Outfit reveal (shoes→head), building |
| **Push-in** | Quick forward movement | Dramatic emphasis, surprise |
| **Pull-out** | Quick backward movement | Reveal, surprise context |
| **Handheld** | Micro-shake, organic | UGC feel, authentic, TikTok style |
| **POV shot** | First person perspective | Unboxing, hands-on product |

### Speed Modifiers
- **"Very slow"** — dreamy, luxurious, dramatic
- **"Slow"** — standard cinematic
- **"Steady"** — controlled, professional
- **"Smooth"** — no jitter, fluid
- **"Gradual"** — progressive change over clip duration

### Kling-Specific Tips
- One subject, one main action per prompt
- Camera movement should serve the narrative (not just move for the sake of moving)
- Always include negative prompt to prevent drift
- For Image-to-Video: focus 80% on motion, 20% on atmosphere
- Specify duration context: "over 5 seconds" helps pace the motion
- Use "(no camera shake)" or "(steady camera)" for clean product shots
- Use "handheld micro-movements" for UGC/TikTok authentic feel

## Negative Prompt Templates

### Universal Base
```
no flickering, no morphing, no sudden cuts, no watermark, no text overlay
```

### For People
```
no facial warping, no changing facial features, no extra fingers, no limb
distortion, no teeth glitching, no eye color change, no skin tone shift
```

### For Products
```
no product deformation, no label warping, no color shift, no shrinking/growing,
no unrealistic reflections, no texture change
```

### For Food
```
no melting objects, no food disappearing, no color change, no unrealistic
liquid physics, no plate movement
```

### For Camera
```
no camera drift, no sudden zooms, no shaky movement, no abrupt direction changes,
no rotation unless specified
```

## Multi-Shot Sequences (Kling 3.0)

Kling 3.0 supports up to 6 shots in one generation. Format:

```
Shot 1: [Wide establishing] — Static wide shot of the product on a table. Soft ambient light.
Shot 2: [Medium approach] — Slow dolly-in from wide to medium, approaching the product.
Shot 3: [Detail close-up] — Extreme close-up on product texture. Shallow DOF. Static.
Shot 4: [In-use] — Hands enter frame, pick up product. Slight overhead angle.
Shot 5: [Reaction] — Medium shot of person using product, subtle smile forming. Static.
Shot 6: [Hero close-up] — Final tight shot of product with logo visible. Slow push-in.
```

Read `references/camera-motion-cheatsheet.md` for the complete list of tested camera movements and their reliability scores on Kling 3.0.