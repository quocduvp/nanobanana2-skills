---
description: Create a complete TikTok/Reels/Shorts ad prompt package (image + video + audio)
---

# Create TikTok / Reels Ad

Use this workflow when the user wants a complete social media advertisement package. This is the most comprehensive workflow — it combines image generation, video motion, and ad strategy.

## Steps

### Phase 1: Discovery & Campaign Planning

1. **Read the TikTok ad skill** — Load `skills/tiktok-ad-creator/SKILL.md` for full instructions.

2. **Gather the brief** — Ask the user all at once (not one by one):
   - Product / subject being promoted?
   - Target audience (age, gender, lifestyle, pain points)?
   - Platform & format (TikTok / Reels / Shorts; single clip or multi-clip)?
   - Ad objective (awareness, desire, click-to-buy, review trust, viral)?
   - Tone & aesthetic (aspirational, UGC, ASMR, playful, luxury)?
   - Audio needs? (voiceover, dialogue, SFX → determines Kling vs Veo 3)
   - Any references or visual style preferences?

3. **Build the Campaign Brief** — Synthesize into structured brief and present for confirmation:
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

4. **Propose the Content Plan** — Lay out each clip before generating prompts:
   ```
   CONTENT PLAN
   ------------
   Clip 1 — Hook (1-2s):   [scroll-stopper moment]
   Clip 2 — Setup (2-3s):  [scene description]
   Clip 3 — Product (2s):  [product introduction]
   Clip 4 — Demo (3s):     [product in action]
   Clip 5 — Result (2s):   [payoff moment]
   Clip 6 — CTA (1s):      [hero shot + CTA area]
   ```

5. **Get user approval** on both brief and content plan before proceeding.

### Phase 2: Generate Prompt Packages

6. **For each clip, generate a full prompt package:**
   - **Nano Banana 2 prompt** — the still image (first frame)
   - **Kling 3.0 prompt** — motion without audio
   - **Veo 3 prompt** — motion WITH audio (dialogue, SFX, music)
   - **Negative prompts** — anti-artifact directives
   - **Editing notes** — post-production tips

7. **Apply hook strategy** for Clip 1 — Design the NB2 first frame as a "scroll stopper":
   - Curiosity gap (hands about to open something)
   - Visual impact (extreme close-up, vivid color)
   - Social proof (person mid-reaction)
   - Transformation (before state shown)
   - ASMR trigger (satisfying texture close-up)
   - Relatable setup (mirror selfie, "POV" angle)

8. **If multi-clip with recurring character** → run `/setup-consistency` workflow first.

### Phase 3: Post-Production Guidance

9. **Suggest editing sequence:**
   - Arrange: Hook → Setup → Product intro → Demo → Result → CTA
   - Text overlays: safe zones (top 15%, bottom 20%)
   - Audio sync: trending sound for TikTok, voiceover for Reels

10. **Platform-specific tips:**
    - TikTok: 7-15 sec, trending sound critical, authentic feel
    - Reels: 7-30 sec, slightly more polished, music/voiceover
    - Shorts: 15-60 sec, more informational OK
