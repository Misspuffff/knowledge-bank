---
tags:
  - type/reference
  - project/air
  - topic/interaction
  - topic/design
created: 2026-04-15
type: reference
---

# AIR — Interaction Vocabulary

> How the body maps to sound and image. This is the design layer — the expressive range of the instrument.

---

## Face Channel — Continuous Modulation

| Blendshape | Audio Parameter | Notes |
|------------|-----------------|-------|
| `jawOpen` | Grain size | Open mouth = bigger grains = coarser texture |
| `browInnerUp` | Filter frequency | Raised brows = brighter, more open filter |
| `mouthSmileLeft` + `mouthSmileRight` | Reverb depth | Smiling = more spatial, diffuse sound |
| Head yaw/pitch/roll | Additional modulation | Directional head movement = parameter shift |
| `eyeBlinkLeft` / `eyeBlinkRight` | TBD | Asymmetric — needs separate handling |

**Visual response:** Ambient atmospheric shifts, color/intensity changes synced to blendshape values. All effects on the live camera feed (augmented mirror model).

---

## Hand Channel — Event Triggers

### Gesture Tiers (from CV scoring research)

| Tier | Gestures | CV Detectability |
|------|----------|-----------------|
| S | Strike, Clap, Point | Highest reliability |
| A | Wrist flick, Palm push, Finger spread | Strong |
| B | Two-hand gestures, Slow sweeps | Moderate |
| C | Subtle gestures, Micro-movements | Lower reliability |

### Visual Shockwave System
On gesture trigger: scan-line tears, pixel scatter, full-screen radiance burst.

---

## The Augmented Mirror Model

The performer sees themselves on screen. The screen is a reactive environment — not a control panel. Effects happen directly on the live camera feed. There is no separate UI overlay to navigate during performance.

---

## Nuance Goal

The instrument should feel **nuanced, not mechanical**. Temporal smoothing (EMA alpha 0.2) is critical — raw blendshape scores are too jittery for musical expression without it.
