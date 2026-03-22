---
name: video-motion
description: >
  Create video generation prompts for Kling 3.0 and Veo 3 to animate Nano Banana 2 images
  into motion videos. Use when the user mentions "Kling", "Veo", "Veo 3", "Google video",
  "video motion", "animate image", "image to video", "chuyển ảnh thành video", "tạo video",
  "motion", "Kling 3.0", "video từ ảnh", "animate", "video có âm thanh", "video có tiếng",
  "cinematic video", "video quảng cáo", "video with audio", "sound design", "dialogue video",
  "camera movement", or wants to turn a still image into a dynamic video clip for TikTok,
  Reels, or advertising.
metadata:
  version: "0.2.0"
---

# Video Motion Prompt Specialist

Generate Kling 3.0 and Veo 3 prompts to animate Nano Banana 2 images into professional motion videos — optimized for TikTok ads, product showcases, fashion lookbooks, and brand content.

## Choose Your Engine

| Feature | Kling 3.0 | Veo 3 |
|---|---|---|
| **Audio generation** | No native audio | Native — dialogue, SFX, ambient, music |
| **Camera control** | Precise, reliable | Good but less granular |
| **Multi-shot** | Up to 6 shots natively | Single clip |
| **Character consistency** | Image-to-video | Reference-to-video ("ingredients") |
| **Best at** | Physics-driven motion, product reveals, fashion walks | Cinematic storytelling, dialogue scenes, ASMR |
| **Use for** | Product spin, fashion motion, UGC (no audio) | Brand films, dialogue ads, atmospheric content |

**Rule of thumb:** Use **Kling** when you need precise camera control or multi-shot sequences. Use **Veo 3** when you need audio (dialogue, sound effects, ambient sounds).

---

## Core Workflow: Nano Banana 2 → Video

```
Step 1: Generate still image with Nano Banana 2
Step 2: Use image as first frame (Kling) or reference image (Veo 3)
Step 3: Write motion prompt focusing on movement + camera + (audio for Veo 3)
Step 4: Generate 5-10 second video clip
```

**Critical rule for Image-to-Video:** Describe only what MOVES and how the CAMERA behaves — do not re-describe the scene. The model already sees it in the image.

---

## Kling 3.0 Prompts

### Prompt Formula

**Text-to-Video:**
```
[Subject Description] + [Subject Movement] + [Scene/Environment] + [Camera Movement] + [Lighting/Atmosphere]
```

**Image-to-Video (primary use case):**
```
[Subject Movement] + [Camera Movement] + [Atmospheric Motion]
```

### Templates by Video Type

**Product Reveal:**
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

Variations: `360 Spin` — "The product rotates 360 degrees on its axis, smooth and continuous." | `Floating` — "Product gently levitates with subtle up-and-down motion (2cm oscillation). Particles of light drift around it."

---

**Fashion Model:**
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

Variations: `Hair flip` — "Model turns head right, hair sweeps dramatically. Slow motion 0.5x." | `Look-back-over-shoulder` — "Model turns 90 degrees away, looks back over shoulder. Static camera."

---

**Food Motion:**
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

---

**Skincare / Beauty:**
```
KLING PROMPT (Image-to-Video):
The dropper slowly releases a single golden serum drop in slow motion.
The drop lands creating delicate ripples. Light refracts through the serum
creating golden caustics. Extreme close-up, very slow dolly-in. Luxurious.

NEGATIVE PROMPT:
no unrealistic liquid physics, no product deformation, no flickering,
no sudden movements, no label distortion
```

---

**Mirror Selfie / UGC:**
```
KLING PROMPT (Image-to-Video):
The person holds up a phone taking a mirror selfie. Slight natural body sway.
Hand adjusts outfit — tugging at hem, smoothing fabric. Confident smile forms.
Subtle head tilt. Phone screen reflection catches the light.
Handheld smartphone camera feel with micro-movements.

NEGATIVE PROMPT:
no facial warping, no phone distortion, no mirror glitch, no unnatural
movements, no changing clothes, no extra fingers on phone
```

---

**Unboxing:**
```
KLING PROMPT (Image-to-Video):
Hands slowly lift the lid of the box, revealing the product nestled inside.
Tissue paper rustles as it's gently pulled aside. The product catches the light
as it's revealed. Overhead camera slowly dollies in during the reveal moment.
Soft ASMR-like careful movements.

NEGATIVE PROMPT:
no sudden movements, no product distortion during handling, no flickering
```

---

### Camera Movement Vocabulary

| Term | Effect | Best For |
|---|---|---|
| **Slow dolly-in** | Gradually moves closer | Product focus, intimacy |
| **Slow dolly-out** | Gradually pulls back | Context reveal |
| **Tracking shot (left/right)** | Follows subject laterally | Fashion walking |
| **Crane up / down** | Camera rises or descends | Grand reveal, detail |
| **Orbit (clockwise/counter)** | Circles around subject | Product 360, portrait |
| **Static shot** | No movement | Food macro, beauty, clean action |
| **Slow pan (left/right)** | Camera rotates in place | Scene scanning |
| **Tilt up/down** | Camera pivots vertically | Outfit reveal (shoes→head) |
| **Push-in** | Quick forward movement | Dramatic emphasis |
| **Handheld** | Micro-shake, organic | UGC feel, TikTok style |

Speed modifiers: `"Very slow"` (luxury) · `"Slow"` (cinematic) · `"Steady"` (product) · `"Smooth"` (lifestyle) · `"Gradual"` (reveal)

**Kling-specific tips:**
- One subject, one main action per prompt
- Always include negative prompt to prevent drift
- For Image-to-Video: 80% motion, 20% atmosphere
- Use `"over 5 seconds"` to pace motion
- Use `"(no camera shake)"` for clean product shots

### Multi-Shot Sequences (Kling 3.0)

Kling 3.0 supports up to 6 shots in one generation:

```
Shot 1: [Wide establishing] — Static wide shot of product. Soft ambient light.
Shot 2: [Medium approach] — Slow dolly-in from wide to medium.
Shot 3: [Detail close-up] — Extreme close-up on product texture. Shallow DOF. Static.
Shot 4: [In-use] — Hands enter frame, pick up product.
Shot 5: [Reaction] — Medium shot of person using product, subtle smile forming.
Shot 6: [Hero close-up] — Final tight shot of product with logo visible. Slow push-in.
```

Read `references/camera-motion-cheatsheet.md` for tested camera movements with reliability scores.

---

## Veo 3 Prompts

### Prompt Formula

```
[Camera/Cinematography] + [Subject] + [Action] + [Setting/Context] + [Style & Lighting] + [Audio Direction]
```

**Key difference from Kling:** Write Veo 3 prompts like a **mini screenplay** — more narrative, with audio cues embedded.

### Templates by Video Type

**Product Commercial (with audio):**
```
VEO 3 PROMPT:
Cinematic close-up, shallow depth of field. A sleek [product] sits on a [surface]
in soft, warm studio lighting. The camera performs a slow, elegant orbit around
the product. A hand reaches in gracefully and picks up the product, turning it
to reveal the [detail].

Audio: Gentle ambient electronic music with warm synth pads. Soft "click" sound
as the product is picked up. Subtle reverb suggesting a premium space.
(no dialogue) (no subtitles)
```

Variations: `With voiceover` — add `A warm, confident female voice says: "Designed for those who notice the details."` | `ASMR style` — add `Audio: ASMR-style close-mic sounds — soft crinkle of packaging, gentle tap on glass surface. No background music.`

---

**Fashion Film / Brand Story:**
```
VEO 3 PROMPT:
Medium tracking shot, 35mm lens feel. A [model] in [outfit] walks through [location]
at golden hour. The camera tracks alongside at walking pace. Fabric flows naturally.
The model pauses, turns to camera with a confident expression, then continues walking.

Style: Cinematic warm amber color grade, slight film grain. Aspect ratio 9:16.

Audio: Ambient outdoor sounds — distant birds, soft wind. Footsteps on [surface].
A mellow lo-fi beat fades in subtly. (no dialogue) (no subtitles)
```

---

**Food / Restaurant Atmosphere:**
```
VEO 3 PROMPT:
Close-up, shallow depth of field, warm color temperature. A steaming bowl of [dish]
sits in a [restaurant setting]. Steam curls rise, lit by warm side lighting.
Chopsticks enter frame, lift noodles creating a satisfying stretch.

Audio: Ambient restaurant — soft chatter, clink of cutlery, sizzling from a distant
kitchen. Close-mic sound of noodles being lifted from broth. (no music) (no subtitles)
```

---

**Skincare / Beauty Ritual:**
```
VEO 3 PROMPT:
Extreme close-up, macro lens feel, soft diffused lighting. A dropper releases golden
serum drops in slow motion onto smooth skin. Each drop catches the light. Camera
slowly dollies in. Dreamy, luxurious atmosphere.

Style: Soft ethereal lighting, clean bright palette with warm undertones.

Audio: Delicate minimal ambient music — soft piano with reverb. Quiet satisfying
sound of liquid drops. Gentle breathing. ASMR-like intimate audio. (no subtitles)
```

---

**Lifestyle / Brand Campaign:**
```
VEO 3 PROMPT:
Wide shot transitioning to medium. Early morning, a [person] in [outfit] opens
floor-to-ceiling curtains. Warm golden sunlight floods the room. They pick up a
[product], walk toward the window, silhouetted against the city skyline, and look
at camera with quiet confidence. Camera dollies forward following them.

Style: Cinematic warm morning tones. Kodak Portra 400 reference. 9:16 vertical.

Audio: Quiet morning ambiance — distant city sounds through glass, soft footsteps.
A warm female voice says: "Every morning starts with a choice."
Gentle uplifting ambient music swells. (no subtitles)
```

---

**Mirror Selfie / UGC (with audio):**
```
VEO 3 PROMPT:
POV shot through a phone screen, handheld feel. A [person] stands before a
full-length mirror. They do a confident outfit check — smoothing the shirt,
turning to show side profile, adjusting an accessory. Authentic, not over-produced.

Style: Natural indoor lighting, slightly warm. Vertical 9:16. iPhone aesthetic.

Audio: Soft indie trending track from a speaker. Fabric rustling. The person says:
"Okay this outfit goes hard." (confident, casual tone). Phone shutter click at end.
(no subtitles)
```

---

### Audio Direction Guide

**Audio prompt structure:**
```
Audio: [Primary sound/music] + [Sound effects] + [Ambient/environmental] + [Dialogue if any]
```

**Dialogue formatting:**
```
CORRECT: A warm female voice says: "This changes everything."
CORRECT: The person says: "Check this out" (casual, excited tone)
WRONG:   "This changes everything"  ← ambiguous, don't use
```
Always add `(no subtitles)` to prevent unwanted text overlays.

**Audio moods by content type:**

| Content Type | Music | SFX | Ambient |
|---|---|---|---|
| Luxury product | Minimal electronic, warm synths | Soft clicks, glass, metal taps | Quiet, spacious reverb |
| Fashion | Lo-fi beat, indie, trending audio | Fabric rustle, heels clicking | Street, studio |
| Food | None or soft acoustic | Sizzle, pour, crunch, utensil | Restaurant chatter, kitchen |
| Skincare/Beauty | Gentle piano, ambient pads | Liquid drops, spray, skin touch | ASMR-like quiet room |
| Lifestyle morning | Uplifting ambient, acoustic guitar | Footsteps, curtains, cup set down | Birds, city, morning quiet |
| UGC/TikTok | Trending audio / popular song | Phone shutter, fabric | Room tone, natural |
| Unboxing | None or light beat | Cardboard, tissue paper, unsnap | Quiet room, ASMR |

**Sound effects vocabulary:**
- Package: crinkle, tear, unsnap, slide open, tissue paper rustle
- Product: click, spray, pour, tap, glass clink, metal snap
- Fabric: rustle, swoosh, swish, flutter, soft thud
- Skin/Beauty: soft application sound, liquid drop, gentle pat

### Veo 3 Special Features

**Ingredients-to-Video (character consistency):**
```
Reference Image: [Nano Banana 2 character image]
Prompt: The same person from the reference image [new action/scene].
Maintain their exact appearance, clothing, and styling.
[Camera direction]. [Audio direction].
```

**First + Last Frame (transition videos):**
```
First Frame: [Nano Banana image A — e.g., product in box]
Last Frame:  [Nano Banana image B — e.g., product in hand, styled]

Prompt: Smooth cinematic transition from starting scene to ending scene.
Natural, physically plausible motion connecting the two frames. Duration: 4 seconds.
Audio: [Satisfying transition sound — whoosh, subtle music swell].
```

Use cases: Before/After (skincare, styling) · Boxed/Unboxed · Day/Night · Outfit 1/Outfit 2

---

## Negative Prompts

### Universal
```
no flickering, no morphing, no sudden cuts, no watermark, no text overlay
```

### For People
```
no facial warping, no changing facial features, no extra fingers, no limb distortion,
no teeth glitching, no eye color change, no skin tone shift, no hair color change,
no clothing change
```

### For Products
```
no product deformation, no label warping, no color shift, no shrinking, no growing,
no unrealistic reflections, no texture change, no logo distortion
```

### For Food
```
no melting objects, no food disappearing, no color change, no unrealistic liquid
physics, no plate movement
```

### For Camera
```
no camera drift, no sudden zooms, no shaky movement, no abrupt direction changes,
no rotation unless specified, no Dutch angle, no focus hunting
```
