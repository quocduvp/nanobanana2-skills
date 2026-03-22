---
description: Animate a Nano Banana 2 still image into a motion video using Kling 3.0 or Veo 3
---

# Animate Image to Video

Use this workflow when the user has a Nano Banana 2 image (or description) and wants to turn it into a motion video.

## Steps

1. **Read the video motion skill** — Load `skills/video-motion/SKILL.md` for full instructions.

2. **Choose the engine** — Help the user pick based on their needs:
   - **Kling 3.0** → Precise camera control, physics, multi-shot (up to 6), product spins, fashion walks. **No native audio.**
   - **Veo 3** → Native audio (dialogue, SFX, ambient, music), cinematic storytelling, ASMR, brand films. **Single clip.**

   Quick decision:
   - Need audio? → **Veo 3**
   - Need camera precision or multi-shot? → **Kling 3.0**
   - Need both? → Generate **both** prompts (Kling for motion, Veo 3 for audio version)

3. **Determine the video type** — Match to template:
   - Product reveal / 360 spin
   - Fashion model motion (walk, hair flip, outfit check)
   - Food motion (steam, chopstick lift, pour)
   - Skincare / beauty ritual (dropper, application)
   - Mirror selfie / UGC
   - Unboxing
   - Lifestyle / brand film

4. **Write the motion prompt** — Follow the Image-to-Video rule:
   > Describe only what **MOVES** and how the **CAMERA** behaves — do NOT re-describe the scene (the model already sees it in the image).

   - **Kling formula:** `[Subject Movement] + [Camera Movement] + [Atmospheric Motion]`
   - **Veo 3 formula:** `[Camera/Cinematography] + [Subject] + [Action] + [Setting] + [Style & Lighting] + [Audio Direction]`

5. **Add negative prompts** — Use the appropriate set from the skill:
   - Universal negatives (always include)
   - People-specific, product-specific, food-specific as needed
   - Camera negatives (always include)

6. **If multi-shot** — For Kling 3.0, structure up to 6 shots:
   ```
   Shot 1: [Wide establishing] — ...
   Shot 2: [Medium approach] — ...
   Shot 3: [Detail close-up] — ...
   Shot 4: [In-use] — ...
   Shot 5: [Reaction] — ...
   Shot 6: [Hero close-up] — ...
   ```

7. **Output** — Present in clean code block(s) with engine label (KLING / VEO 3).

8. **If TikTok / Reels ad** → hand off to `/create-tiktok-ad` workflow instead.
