---
name: tiktok-ad-creator
description: >
  Create complete TikTok/Reels ad video prompt packages combining Nano Banana 2 image prompts
  with Kling/Veo 3 motion prompts. Use when the user mentions "TikTok", "Reels", "short video",
  "video quảng cáo", "ad video", "viral video", "video ngắn", "unboxing video", "review video",
  "ASMR", "UGC video", "video bán hàng", "content creator", or needs a complete image-to-video
  advertising workflow for social media platforms.
metadata:
  version: "0.2.0"
---

# TikTok / Reels Ad Creator

Generate complete prompt packages: Nano Banana 2 (first frame image) + Kling/Veo 3 (motion video) — ready for TikTok, Instagram Reels, YouTube Shorts advertising.

---

## Phase 1: Discovery & Campaign Planning (ALWAYS run this first)

Before generating any prompts, you MUST run the discovery phase. Never skip straight to templates.

### Step 1 — Gather the Brief

Use AskUserQuestion to collect (ask all at once, not one by one):

1. **Product / Subject** — What is being promoted? (product name, category, key feature)
2. **Target audience** — Who is this for? (age, gender, lifestyle, pain points)
3. **Platform & format** — TikTok / Reels / Shorts? Single clip or multi-clip series?
4. **Ad objective** — Awareness, desire, click-to-buy, review trust, or viral reach?
5. **Tone & aesthetic** — Aspirational? Authentic UGC? ASMR? Playful? Luxury?
6. **Audio needs** — Does the ad need voiceover, dialogue, or sound effects? (determines Kling vs Veo 3)
7. **Any references** — Competitor ads, mood boards, color palette, or visual style they like?

### Step 2 — Build the Campaign Brief

Synthesize the answers into a structured brief and **present it to the user for confirmation** before continuing:

```
CAMPAIGN BRIEF
--------------
Product:       [name + key visual differentiator]
Target:        [audience description]
Platform:      [platform(s) + aspect ratio]
Objective:     [awareness / desire / purchase / trust]
Tone:          [aesthetic + mood keywords]
Video engine:  [Kling / Veo 3 / Both — with reasoning]
Ad type(s):    [unboxing / review / lifestyle / etc.]
Duration:      [hook length + total ad length]
Audio:         [yes/no, type]
```

Ask: *"Đây có đúng hướng không? Hay bạn muốn điều chỉnh gì trước khi mình bắt đầu?"*

### Step 3 — Propose the Content Plan

Once the brief is confirmed, propose a concrete execution plan **before generating prompts**:

```
CONTENT PLAN
------------
Clip 1 — Hook (1-2s):   [describe the scroll-stopper moment + which template to use]
Clip 2 — Setup (2-3s):  [describe the scene + engine choice]
Clip 3 — Product (2s):  [describe how product is introduced]
Clip 4 — Demo (3s):     [describe product in action]
Clip 5 — Result (2s):   [describe the payoff moment]
Clip 6 — CTA (1s):      [hero shot + CTA text overlay area]

Engine recommendation:  Kling for clips [X, Y] / Veo 3 for clips [X, Y] — [reason]
Hook strategy:          [which hook type and why]
Estimated total:        ~[X] seconds
```

Ask: *"Mình có thể điều chỉnh số clip, thứ tự, hoặc thay đổi cách tiếp cận hook. Bạn muốn giữ nguyên hay chỉnh gì không?"*

### Step 4 — Generate Prompts

Only after the user approves the plan, generate the full prompt packages for each clip following the approved content plan. Use the templates in Phase 2 below.

If the user only needs **one specific clip** (not a full series), skip the multi-clip plan and generate that single package directly after brief confirmation.

---

## Phase 2: Prompt Package Templates

Each "prompt package" includes:
1. **Nano Banana 2 prompt** — generates the perfect first frame image
2. **Kling prompt** — animates that image into motion (camera control, physics)
3. **Veo 3 prompt** — alternative with native audio (dialogue, SFX, music)
4. **Negative prompts** — prevents common artifacts
5. **Editing notes** — post-production tips

## TikTok Ad Format Specs

- **Aspect ratio**: 9:16 (1080x1920)
- **Duration sweet spots**: 5-8 sec (hook clip), 15 sec (mini ad), 30 sec (full ad)
- **Safe zones**: Top 15% (UI elements), bottom 20% (caption/CTA area)
- **Hook**: First 1-2 seconds must be scroll-stopping
- **Audio**: Critical — 88% of TikTok is watched with sound on

## Complete Prompt Packages by Ad Type

---

### 1. PRODUCT UNBOXING VIDEO

**Goal**: Satisfying ASMR unboxing that builds desire.

**NANO BANANA 2 — First Frame:**
```
Top-down POV shot of two hands positioned at the sides of a [brand-style]
premium gift box on a clean [surface: white marble / light wood desk].
The box lid is slightly lifted, revealing a glimpse of [product] and tissue
paper inside. Soft overhead lighting creating gentle shadows. Shot on iPhone
15 Pro from directly above. Natural indoor daylight. Clean, minimal styling —
only the box and hands visible. 9:16 vertical format with product centered.
No clutter, no watermarks.
```

**KLING — Motion (No Audio):**
```
Hands slowly lift the box lid completely, revealing the product inside.
Tissue paper rustles as one hand carefully pulls it aside. The other hand
reaches in and gently lifts the product out, turning it 45 degrees to
catch the light. Smooth, deliberate ASMR-like movements. Static overhead
camera with very subtle slow push-in during the reveal moment.

Negative: no hand distortion, no extra fingers, no product deformation,
no sudden movements, no flickering, no box disappearing
```

**VEO 3 — Motion + Audio:**
```
POV top-down shot. Hands carefully open a premium box. Slow, deliberate
movements suggesting care and anticipation. The lid is lifted revealing
the product. Tissue paper is gently unwrapped. The product is lifted
out and held up to examine. Warm, soft lighting from above.

Audio: ASMR-style close-mic audio. Cardboard sliding sound as lid opens.
Soft tissue paper crinkle. Satisfying unsnap of magnetic closure. Quiet
room tone with subtle reverb. A whispered voice says: "Oh wow, the
packaging alone..." Gentle lo-fi beat fades in at the end. (no subtitles)
```

---

### 2. MIRROR SELFIE / OUTFIT CHECK

**Goal**: Authentic "getting ready" content showcasing fashion.

**NANO BANANA 2 — First Frame:**
```
Realistic mirror selfie photograph of a [model: age, gender, features,
hair] wearing [complete outfit description]. Standing in front of a
full-length mirror in a [room: well-lit bedroom / walk-in closet /
minimalist bathroom]. Holding a smartphone at chest height. Natural indoor
daylight from a window on the left. The mirror shows the full outfit
reflection. Shot aesthetic: authentic iPhone selfie, not overly styled.
Slightly warm color temperature. 9:16 vertical. Clean room background
visible in mirror reflection. No excessive filters, no watermarks.
```

**KLING — Motion:**
```
The person does a slow outfit check in the mirror. Slight turn to show
the side profile, hand smooths down the front of the [garment]. Turns back
to front, adjusts [accessory/collar/cuff]. Confident nod and slight
smile at reflection. Natural body sway and micro-movements. Phone stays
steady in hand. Handheld smartphone feel with natural micro-shake.

Negative: no facial warping, no mirror glitch, no phone distortion,
no changing outfit, no extra limbs, no unnatural movement
```

**VEO 3 — Motion + Audio:**
```
Mirror selfie video. A [person] stands before a full-length mirror,
phone in hand recording. They turn slowly showing the outfit from
multiple angles. Smooth fabric catches the light. They adjust [detail]
and smile confidently. Authentic, casual bedroom setting with good
natural light.

Audio: Soft indie trending track playing from a speaker. Fabric
rustling with movement. The person says: "This fit is giving everything"
(casual, confident tone). Phone shutter click. (no subtitles)
```

---

### 3. PRODUCT REVIEW / "HONEST OPINION"

**Goal**: Authentic-feeling UGC review that drives trust and purchase.

**NANO BANANA 2 — First Frame:**
```
Medium close-up of a [person: relatable, natural look, minimal makeup]
sitting at a desk/vanity, holding [product] at chest height, looking
directly at camera with an expressive face (mid-speech, slightly raised
eyebrows suggesting enthusiasm). Natural indoor lighting from window.
Behind them: blurred casual room setting (bookshelf, plants, neutral
decor). Product packaging visible on the desk. Shot on smartphone feel.
9:16 vertical. Authentic UGC aesthetic — not studio-perfect. No ring
light reflections, no heavy filter.
```

**KLING — Motion:**
```
The person gestures while talking, showing the product to camera.
They turn the product to show different angles. Natural head movements,
occasional nod, eyebrow raises. They open the product (if applicable)
and demonstrate use — applying on hand/face/showing texture. Genuine
enthusiasm in body language. Subtle forward lean when making a point.
Static camera with slight handheld micro-movement (UGC feel).

Negative: no facial warping, no changing expressions too rapidly,
no product deformation, no hand distortion, no robotic gestures
```

**VEO 3 — Motion + Audio:**
```
UGC-style medium shot. A [person] sits casually, holding [product].
They gesture naturally while speaking to camera. They show the product
close-up, demonstrate it, and give genuine reactions. Authentic bedroom
setting, natural lighting. Handheld smartphone camera feel.

Audio: Natural room acoustics. The person says: "Okay so I've been
using this for two weeks and honestly... game changer. Look at this
texture —" (enthusiastic, natural speech cadence). Subtle background
room tone. (no music) (no subtitles)
```

---

### 4. FOOD SHOWCASE / MUKBANG STYLE

**Goal**: Appetizing close-up that triggers cravings.

**NANO BANANA 2 — First Frame:**
```
Appetizing close-up food photograph of [dish with full visual description]
in [authentic serving vessel]. Chopsticks or fork positioned ready to take
first bite. Steam rising from the dish. Warm side-lighting from left
creating golden highlights on the food surface. Dark moody restaurant
background with warm bokeh lights. Shot on smartphone but high quality.
9:16 vertical, dish centered in upper-third of frame. Rich, warm color
palette. No text overlay, no watermark.
```

**KLING — Motion:**
```
Chopsticks lift a perfect bite from the dish — noodles stretch, sauce
drips back, steam curls. Slow motion 0.5x speed during the lift.
The bite hovers in frame. Background bokeh gently shifts. Very slow
push-in toward the food. Warm, appetizing lighting throughout.

Negative: no food disappearing, no unrealistic physics, no chopstick
distortion, no plate movement, no color shift, no flickering
```

**VEO 3 — Motion + Audio:**
```
Close-up food video. Chopsticks descend into a steaming [dish], lifting
a perfect bite. Noodles stretch satisfyingly. The camera slowly pushes
in. Warm, intimate restaurant lighting. Steam catches the backlight.

Audio: Close-mic ASMR: sizzling background, chopsticks clicking, noodle
slurp sound, satisfied "mmm". Ambient restaurant — soft chatter, distant
kitchen sounds. Gentle background jazz. (no dialogue) (no subtitles)
```

---

### 5. SKINCARE ROUTINE / "GET READY WITH ME"

**Goal**: Aspirational morning/night routine showcasing products.

**NANO BANANA 2 — First Frame:**
```
Lifestyle photograph of a [person: natural dewy skin, hair pulled back,
wearing white robe] in a bright minimalist bathroom. Holding [skincare
product] in one hand near face. Other hand touching clean, glowing skin.
Array of skincare products neatly arranged on the vanity counter.
Soft morning light streaming through a frosted window. Clean, bright,
airy aesthetic. Shot on smartphone. 9:16 vertical. Fresh, aspirational
wellness mood. No heavy makeup, no artificial skin smoothing.
```

**KLING — Motion:**
```
The person applies product in gentle upward strokes on their face.
Eyes close peacefully during application. They open eyes and smile softly
at their reflection (off-camera mirror implied). Hands move to pick up
the next product from the counter. Natural, unhurried morning routine
movements. Slight head tilts. Soft, peaceful body language.
Static camera with very subtle slow dolly-in.

Negative: no facial warping, no skin texture change, no product
distortion, no unnatural hand movements, no robotic expressions
```

**VEO 3 — Motion + Audio:**
```
Morning skincare routine. A [person] in a white robe applies [product]
to their face with gentle upward motions. Their expression is peaceful,
relaxed. Bright bathroom with morning light. They pick up the next
product from a neat lineup on the counter. Soft, mindful movements
throughout.

Audio: Quiet morning ambiance — birds faintly outside, soft breathing.
Product sounds: gentle pump dispenser, cream smoothing on skin. The
person says: "This has literally transformed my skin in two weeks."
(soft, genuine voice). Gentle piano melody fades in. (no subtitles)
```

---

### 6. PRODUCT-IN-LIFESTYLE (SUBTLE PLACEMENT)

**Goal**: The product naturally fits into an aspirational lifestyle scene.

**NANO BANANA 2 — First Frame:**
```
Lifestyle photograph of a [person] in [aspirational setting: modern café /
sunlit apartment / rooftop terrace / beach / co-working space]. [Product]
is visible but secondary — placed on the table / in their hand / in an
open bag nearby. The person is engaged in a natural activity: reading,
working on laptop, chatting with friend, enjoying a view. Product is
noticeable but not the forced center of attention. Natural golden hour
or soft indoor light. Shot on Fujifilm X-T5, lifestyle aesthetic.
9:16 vertical. Warm, aspirational color palette.
```

**KLING — Motion:**
```
The person naturally interacts with their environment — [typing / sipping
coffee / turning a page / laughing]. At some point, they casually pick up
or interact with the [product] in a completely natural way — a quick
glance at it, a sip from it, applying it. The product moment feels
organic, not staged. Gentle environmental motion: leaves in breeze,
coffee steam, background passersby. Slow pan or static with subtle drift.

Negative: no product teleporting, no unnatural attention to product,
no robotic gestures, no facial warping, no background glitch
```

---

## Hook Strategies (First 1-2 Seconds)

The first frame is critical for TikTok. Design the Nano Banana 2 image to be a "scroll stopper":

| Hook Type | First Frame Strategy | Why It Works |
|---|---|---|
| **Curiosity gap** | Hands about to open something, face showing surprise | Viewer needs to see what happens next |
| **Visual impact** | Extreme close-up of texture, vivid color, unusual angle | Visually arresting, breaks pattern |
| **Social proof** | Person mid-reaction, "OMG" expression | Emotional contagion, curiosity |
| **Transformation** | Before state clearly shown | Viewer wants to see the "after" |
| **ASMR trigger** | Close-up of satisfying texture, packaging detail | Sensory anticipation |
| **Relatable setup** | Mirror selfie, desk setup, "POV" angle | Viewer identifies with the scenario |

## Multi-Clip Campaign Notes

For campaigns with a recurring character across clips, remind the user to run the **character-consistency** skill first to generate a Character DNA before generating individual frames.

After all clips are generated, suggest editing sequence:
- Arrange: Hook → Setup → Product intro → Demo → Result → CTA
- Add text overlays in safe zones (top 15%, bottom 20%)
- Sync audio: trending sound for TikTok, voiceover for Reels

## Platform-Specific Tips

| Platform | Duration | Audio | Format | Key Difference |
|---|---|---|---|---|
| **TikTok** | 7-15 sec optimal | Trending sound critical | 9:16 | Fast hooks, authentic feel |
| **Instagram Reels** | 7-30 sec | Music/voiceover | 9:16 | Slightly more polished |
| **YouTube Shorts** | 15-60 sec | Less music-dependent | 9:16 | Can be more informational |
| **Instagram Stories** | 5-15 sec | Optional | 9:16 | Ephemeral, casual, polls/stickers |

## Choosing Kling vs Veo 3

| Scenario | Recommend | Why |
|---|---|---|
| Product spin/reveal, no audio | **Kling** | Superior camera control and physics |
| Fashion walking/motion | **Kling** | Better subject movement physics |
| Talking-head review | **Veo 3** | Native dialogue + lip sync |
| ASMR unboxing with sounds | **Veo 3** | Native SFX generation |
| Atmospheric brand film | **Veo 3** | Audio + cinematic quality |
| Multi-shot sequence | **Kling** | 6-shot native generation |
| UGC selfie style | **Either** | Kling for motion, Veo 3 for voice |
| Food with sizzle sounds | **Veo 3** | SFX critical for food content |