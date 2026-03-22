---
description: End-to-end pipeline from idea to final TikTok/Reels video — image + video + ad
---

# Full Content Pipeline (Idea → Image → Video → Ad)

Use this workflow when the user wants the complete production pipeline: from a raw idea all the way to a finished ad-ready video. This orchestrates multiple skills in sequence.

## Pipeline Overview

```
Your Idea → Consistency Setup → NB2 Still Image → Kling/Veo 3 Video → TikTok/Reels
```

## Steps

### Stage 1: Define & Plan

1. **Understand the idea** — What does the user want to create? Clarify:
   - Subject / product / scene
   - Final destination (TikTok, Reels, brand film, lookbook, etc.)
   - Single image, single video, or multi-clip campaign?

2. **If multi-image or campaign** → run `/setup-consistency` workflow:
   - Character DNA for recurring people
   - Brand Style Guide for visual coherence
   - Product Reference Profile for featured products

### Stage 2: Generate Still Image

3. **Run `/generate-image-prompt`** — Route to the right category skill:
   - Fashion → `fashion-editorial`
   - Product → `product-commerce`
   - Food → `food-beverage`
   - Skincare → `skincare-beauty`
   - Lifestyle → `lifestyle-campaign`
   - General → `prompt-generator`

4. **Generate the NB2 prompt** and present to user.

5. **User generates the image** in Nano Banana 2 and confirms it looks good.

### Stage 3: Animate to Video

6. **Run `/animate-to-video`** — Choose engine:
   - Kling 3.0 for camera precision & physics
   - Veo 3 for audio (dialogue, SFX, music)

7. **Write motion prompt** — Image-to-Video rules (describe only movement + camera).

8. **User generates the video** and confirms quality.

### Stage 4: Ad Packaging (if TikTok/Reels)

9. **Run `/create-tiktok-ad`** — If the final output is for social ads:
   - Apply hook strategy
   - Build multi-clip content plan
   - Generate full prompt packages per clip
   - Post-production editing guidance

### Stage 5: Iterate & Refine

10. **Review results** — If anything needs adjustment:
    - Image not right? Refine NB2 prompt (tweak lighting, pose, environment)
    - Video has artifacts? Adjust negative prompts, simplify motion
    - Consistency drifting? Re-attach reference images, re-include Character DNA
    - Style off? Check Brand Style Guide is being prefixed to every prompt

11. **If user wants variants** → run `/analyze-and-clone` on the successful output.

## Skill Cross-References

| Need | Workflow | Skills Used |
|---|---|---|
| Just an image | `/generate-image-prompt` | prompt-generator, fashion-editorial, product-commerce, food-beverage, skincare-beauty, lifestyle-campaign |
| Just a video | `/animate-to-video` | video-motion |
| Full ad | `/create-tiktok-ad` | tiktok-ad-creator + video-motion + category skill |
| Consistency | `/setup-consistency` | character-consistency |
| Clone/variant | `/analyze-and-clone` | image-analysis |
| Everything | `/full-pipeline` | All skills orchestrated |
