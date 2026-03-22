# Kling 3.0 Camera Motion Cheatsheet

## Tested Camera Movements — Reliability Guide

### High Reliability (Works consistently)

| Movement | Prompt Syntax | Duration | Best For |
|---|---|---|---|
| Slow dolly-in | "Slow dolly-in from medium to close-up" | 5-8 sec | Product reveal, intimacy |
| Static shot | "Static camera, no movement" | Any | Food macro, beauty, clean action |
| Slow pan left/right | "Camera slowly pans right revealing the scene" | 5-8 sec | Environmental reveal |
| Orbit (partial) | "Camera orbits clockwise 90 degrees around subject" | 5-8 sec | Product showcase |
| Tilt up | "Camera tilts upward from feet to head" | 5-8 sec | Outfit reveal, building |

### Medium Reliability (Usually works, may need regeneration)

| Movement | Prompt Syntax | Duration | Tips |
|---|---|---|---|
| Tracking shot | "Camera tracks alongside the walking subject" | 5-8 sec | Keep subject movement simple |
| Dolly-out | "Slow dolly-out revealing wider context" | 5-8 sec | Specify what's revealed |
| Crane up | "Camera cranes upward from ground level" | 5-8 sec | Start position matters |
| Handheld | "Handheld camera with natural micro-movements" | 3-5 sec | Don't overdo shakiness |
| Push-in (fast) | "Quick push-in toward subject's face" | 2-3 sec | Short duration works better |

### Lower Reliability (May need multiple attempts)

| Movement | Prompt Syntax | Tips |
|---|---|---|
| Full 360 orbit | "Camera orbits 360 degrees around product" | Break into 180° segments |
| Whip pan | "Fast whip pan left" | Often too aggressive |
| Complex combined | "Dolly-in while panning left" | Simplify to one movement |
| Crane + track | "Crane up while tracking forward" | Prioritize one direction |

## Movement Speed Modifiers

| Modifier | Use When | Example |
|---|---|---|
| "Very slow" | Luxury, beauty, dramatic reveal | "Very slow dolly-in over 8 seconds" |
| "Slow" | Standard cinematic | "Slow pan right" |
| "Steady" | Product, clean shots | "Steady orbit clockwise" |
| "Smooth" | Lifestyle, elegance | "Smooth tracking alongside" |
| "Gradual" | Progressive reveal | "Gradual crane upward" |
| "Quick" | Energy, impact, hook | "Quick push-in to face" |

## Image-to-Video Motion Commands

When using a Nano Banana 2 image as first frame, focus prompts on:

### Subject Motion Commands
```
"The person blinks naturally and turns head slightly to the right"
"The model takes one confident step forward"
"Hands reach into frame and interact with the product"
"Hair catches a gentle breeze, flowing to the left"
"Slight smile forms, eyes squint naturally"
"Fabric sways gently as if caught in a light wind"
"Steam rises in delicate wisps from the surface"
"Liquid pours smoothly from above into the container"
"The product rotates slowly on its axis"
"Leaves in the background shift gently in the wind"
```

### Environmental Motion Commands
```
"Light gradually shifts from cool to warm"
"Shadows lengthen as if time is passing"
"Background bokeh circles drift slightly"
"Dust particles float in the light beam"
"Water surface ripples gently"
"Candle flame flickers naturally"
"Curtain billows softly from an open window"
```

## Negative Prompt Library

### For People
```
no facial warping, no changing facial features, no morphing between expressions,
no extra fingers, no limb distortion, no teeth glitching, no eye color change,
no skin tone shift, no hair color change, no clothing change
```

### For Products
```
no product deformation, no label warping, no color shift, no shrinking,
no growing, no unrealistic reflections, no texture change, no logo distortion,
no material change
```

### For Camera
```
no camera drift, no sudden zooms, no shaky movement, no abrupt direction changes,
no rotation unless specified, no Dutch angle, no focus hunting
```

### For General Quality
```
no flickering, no morphing, no sudden cuts, no watermark, no text overlay,
no frame drops, no artifacts, no banding, no motion blur (unless requested)
```

## Multi-Shot Sequence Template

```
Shot 1: [WIDE/ESTABLISHING]
Static wide shot. [Environment description]. [Ambient motion only]. Duration: 2 sec.

Shot 2: [APPROACH/MEDIUM]
Slow dolly-in from wide to medium. [Subject comes into focus]. Duration: 3 sec.

Shot 3: [DETAIL/CLOSE-UP]
Static extreme close-up on [key detail]. Shallow DOF. Duration: 2 sec.

Shot 4: [ACTION/INTERACTION]
[Subject performs key action]. [Camera follows]. Duration: 3 sec.

Shot 5: [REACTION/EMOTION]
Medium close-up on [person's reaction]. Slight slow push-in. Duration: 2 sec.

Shot 6: [HERO/FINAL]
[Product/subject hero shot]. [Slow dolly-in or static]. Duration: 2 sec.
```