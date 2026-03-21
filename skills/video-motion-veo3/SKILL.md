---
name: video-motion-veo3
description: >
  Create Google Veo 3 / Veo 3.1 video generation prompts to animate Nano Banana 2 images
  into cinematic videos with synchronized audio. Use when the user mentions "Veo", "Veo 3",
  "Google video", "video có âm thanh", "video có tiếng", "cinematic video", "video quảng cáo",
  "video with audio", "sound design", "dialogue video", or wants high-quality cinematic video
  generation with native audio/dialogue from still images or text descriptions.
metadata:
  version: "0.1.0"
---

# Veo 3 / 3.1 Video Motion Prompt Specialist

Generate Veo 3 prompts for cinematic video with synchronized audio — optimized for product ads, brand storytelling, and social media content.

## Why Veo 3 (vs Kling)

| Feature | Veo 3/3.1 | Kling 3.0 |
|---|---|---|
| **Audio generation** | Native — dialogue, SFX, ambient, music | No native audio |
| **Resolution** | Up to 4K | Up to 4K |
| **Character consistency** | Reference-to-video ("ingredients") | Image-to-video |
| **Best at** | Cinematic storytelling, dialogue scenes, atmospheric | Physics-driven motion, camera control, multi-shot |
| **Use for** | Brand films, dialogue ads, atmospheric content | Product reveal, fashion motion, UGC style |

**Rule of thumb:** Use Veo 3 when you need AUDIO (dialogue, sound effects, ambient sounds) or cinematic storytelling. Use Kling when you need precise CAMERA CONTROL or multi-shot sequences.

## Core Workflow: Nano Banana 2 → Veo 3

```
Step 1: Generate still image with Nano Banana 2
Step 2: Use as reference image in Veo 3 "Image-to-Video" or "Ingredients-to-Video"
Step 3: Write Veo 3 prompt with focus on: Action + Camera + Audio
Step 4: Generate cinematic video clip with synchronized sound
```

## Veo 3 Prompt Formula

```
[Camera/Cinematography] + [Subject] + [Action] + [Setting/Context] + [Style & Lighting] + [Audio Direction]
```

**Key difference from Kling:** Veo 3 prompts should be written like a **mini screenplay** — more narrative, more descriptive, with audio cues embedded.

## Prompt Templates by Video Type

### 1. Product Commercial (With Audio)

```
VEO 3 PROMPT:
Cinematic close-up, shallow depth of field. A sleek [product description] sits on
a [surface] in soft, warm studio lighting. The camera performs a slow, elegant
orbit around the product. Light glints catch the [material] surface as the angle
changes. A hand reaches in gracefully and picks up the product, turning it to
reveal the [detail].

Audio: Gentle ambient electronic music with warm synth pads. Soft "click" sound as
the product is picked up. Subtle reverb on all sounds suggesting a premium space.
(no dialogue) (no subtitles)
```

**Variations:**
- **With voiceover**: Add `A warm, confident female voice says: "Designed for those who notice the details."`
- **With sound design**: Add `Audio: Satisfying mechanical click when cap opens. Soft whoosh as product rotates. Low, warm bass tone throughout.`
- **ASMR style**: Add `Audio: ASMR-style close-mic sounds — soft crinkle of packaging, gentle tap on glass surface, whispered "mmm". No background music.`

### 2. Fashion Film / Brand Story

```
VEO 3 PROMPT:
Medium tracking shot, 35mm lens feel. A [model description] in [outfit] walks
through [location] at golden hour. The camera tracks alongside at walking pace.
Sunlight creates warm rim lighting on the subject. Fabric flows naturally with
each step. The model pauses, turns to camera with a confident expression, then
continues walking away. The camera holds as they recede into the warm light.

Style: Cinematic color grade with warm amber tones, slightly desaturated.
Film grain texture. Aspect ratio 9:16 vertical.

Audio: Ambient outdoor sounds — distant birds, soft wind. Footsteps on [surface]
in rhythm with walking. A mellow, understated lo-fi beat fades in subtly.
(no dialogue) (no subtitles)
```

### 3. Food / Restaurant Atmosphere

```
VEO 3 PROMPT:
Close-up, shallow depth of field, warm color temperature. A steaming bowl of
[dish] sits on a [surface] in a [restaurant setting]. Gentle steam curls rise
from the surface, lit by warm side lighting. A pair of chopsticks enters frame,
lifts noodles creating a satisfying stretch. Background is a soft bokeh of
warm restaurant lights and ambient movement.

Audio: Ambient restaurant atmosphere — soft chatter in background, gentle clink
of cutlery, sizzling from a distant kitchen. Close-mic sound of noodles being
lifted from broth. Warm, inviting ambiance. (no music) (no subtitles)
```

**Variation — Coffee shop:**
```
VEO 3 PROMPT:
Medium close-up, eye-level. A barista pours steamed milk into a latte art
pattern in a ceramic cup. The white milk swirls into the dark espresso creating
a leaf pattern. Steam rises gently. Warm café lighting with soft background bokeh
of a busy coffee shop.

Audio: Espresso machine hissing in background. Milk pouring — smooth, liquid sound.
Gentle café ambient noise. Soft indie acoustic guitar playing quietly from speakers.
(no dialogue) (no subtitles)
```

### 4. Skincare / Beauty Ritual

```
VEO 3 PROMPT:
Extreme close-up, macro lens feel, soft diffused lighting. A dropper releases
golden serum drops that fall in slow motion onto smooth skin. Each drop catches
the light, creating luminous highlights. The drops spread naturally across the
skin surface. Camera slowly dollies in, going even closer to the texture detail.
Dreamy, luxurious atmosphere.

Style: Soft, ethereal lighting. Clean, bright color palette with warm undertones.
Slight slow motion feel.

Audio: Delicate, minimal ambient music — soft piano notes with reverb. Quiet,
satisfying sound of liquid drops. Gentle breathing. ASMR-like intimate audio.
(no dialogue) (no subtitles)
```

### 5. Lifestyle / Brand Campaign Film

```
VEO 3 PROMPT:
Wide shot transitioning to medium. Early morning, a [person description] in
[outfit] opens floor-to-ceiling curtains in a modern minimalist apartment.
Warm golden sunlight floods the room. They pick up a [product] from the
nightstand, hold it up with a gentle smile, and walk toward the window.
Camera dollies forward, following them. The person pauses by the window,
silhouetted against the city skyline, turns and looks at camera with quiet
confidence.

Style: Cinematic, warm morning tones. Kodak Portra 400 color reference.
Gentle lens flare from morning sun. 9:16 vertical for TikTok.

Audio: Quiet morning ambiance — distant city sounds muffled through glass.
Soft footsteps on hardwood floor. Curtain fabric rustling. A warm female voice
says: "Every morning starts with a choice." Gentle, uplifting ambient music
swells softly. (no subtitles)
```

### 6. Mirror Selfie / UGC Style (With Audio)

```
VEO 3 PROMPT:
POV shot through a phone screen, handheld feel. A [person] stands in front of
a full-length mirror in a well-lit room. They hold up a phone, recording themselves.
They do a confident outfit check — smoothing the shirt, turning to show the
side profile, adjusting an accessory. Natural, candid movements. They smile at
their reflection and snap the photo. Authentic, not over-produced.

Style: Natural indoor lighting, slightly warm. iPhone/smartphone video aesthetic.
Vertical 9:16. Casual, authentic feel.

Audio: Room tone with natural reverb. Soft fabric rustling. A confident voice
says: "Okay this outfit goes hard." Phone camera shutter click at the end.
Trending audio snippet or lo-fi beat in background. (no subtitles)
```

## Audio Direction Guide for Veo 3

### Audio Prompt Structure
```
Audio: [Primary sound/music] + [Sound effects] + [Ambient/environmental] + [Dialogue if any]
```

### Dialogue Formatting
```
✅ CORRECT: A warm female voice says: "This changes everything."
✅ CORRECT: The person says: "Check this out" (casual, excited tone)
❌ WRONG: "This changes everything" (ambiguous — use Character says: format)
```

**Always add `(no subtitles)` to prevent unwanted text overlays.**

### Audio Moods by Content Type

| Content Type | Music | SFX | Ambient |
|---|---|---|---|
| Luxury product | Minimal electronic, warm synths | Soft clicks, glass, metal taps | Quiet, spacious reverb |
| Fashion | Lo-fi beat, indie, trending audio | Fabric rustle, heels clicking | Environmental (street, studio) |
| Food | None or soft acoustic | Sizzle, pour, crunch, utensil | Restaurant chatter, kitchen |
| Skincare/Beauty | Gentle piano, ambient pads | Liquid drops, spray, skin touch | ASMR-like quiet room |
| Lifestyle morning | Uplifting ambient, acoustic guitar | Footsteps, curtains, cup set down | Birds, city, morning quiet |
| UGC/TikTok | Trending audio / popular song reference | Phone shutter, fabric | Room tone, natural |
| Unboxing | None or light beat | Cardboard, tissue paper, unsnap | Quiet room, ASMR |

### Sound Effects Vocabulary
- **Package**: crinkle, tear, unsnap, slide open, tissue paper rustle
- **Product**: click, spray, pour, tap, glass clink, metal snap
- **Fabric**: rustle, swoosh, swish, flutter, soft thud
- **Environment**: footsteps (specify surface), door, wind, rain, traffic
- **Skin/Beauty**: soft application sound, liquid drop, gentle pat

## Veo 3 "Ingredients-to-Video" (Character Consistency)

Veo 3's reference system can maintain character consistency across clips:

```
Reference Image: [Nano Banana 2 character image]
Prompt: The same person from the reference image [new action/scene].
Maintain their exact appearance, clothing, and styling.
[Camera direction]. [Audio direction].
```

This is especially powerful for multi-clip campaigns where the same "model" appears in different scenarios.

## Veo 3 "First + Last Frame" (Transition Videos)

Generate a smooth transition between two Nano Banana 2 images:

```
First Frame: [Upload Nano Banana image A — e.g., product in box]
Last Frame: [Upload Nano Banana image B — e.g., product in hand, styled]

Prompt: Smooth cinematic transition from the starting scene to the ending scene.
Natural, physically plausible motion connecting the two frames. [Duration: 4 seconds].
Audio: [Satisfying transition sound — whoosh, subtle music swell].
```

**Use cases:**
- Before → After (skincare, styling)
- Boxed → Unboxed (product reveal)
- Day → Night (lifestyle mood change)
- Outfit 1 → Outfit 2 (fashion transition)

## Cinematography Terms for Veo 3

Veo 3 responds well to cinematic language:

- **Dolly shot**: Camera physically moves forward/backward
- **Tracking shot**: Camera follows alongside subject
- **Crane shot**: Camera rises or descends
- **Aerial view**: High overhead angle
- **Slow pan**: Camera rotates left/right in place
- **POV shot**: First-person perspective
- **Steadicam**: Smooth handheld following
- **Whip pan**: Fast pan creating motion blur (transition)
- **Rack focus**: Focus shifts between foreground and background
- **Pull focus**: Progressive focus change drawing attention

## Technical Specifications

- **Resolution**: 720p, 1080p, or 4K
- **Aspect ratios**: 16:9 (landscape), 9:16 (vertical/TikTok), 1:1 (square)
- **Duration**: 5-8 seconds per clip (optimal for social media)
- **Audio**: Native generation — dialogue, SFX, ambient, music all in one
- **Input**: Text-to-video, Image-to-video, Reference-to-video, First+Last frame