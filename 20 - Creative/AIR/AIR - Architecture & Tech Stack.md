---
tags: [project/air, tech, architecture]
created: 2026-04-15
type: reference
---

# AIR — Architecture & Tech Stack

## Stack

| Layer | Tool |
|-------|------|
| Frontend framework | React + Vite |
| Audio engine | Tone.js (`GrainPlayer`) |
| Computer vision | `@mediapipe/tasks-vision` (Tasks Vision API) |
| State management | Zustand |
| Visuals | Canvas 2D API |
| Backend | Node.js / Express (local asset server) |
| Repo | [github.com/Misspuffff/purplemonkey](https://github.com/Misspuffff/purplemonkey) |

---

## Two-Channel Architecture

### Face Channel (Continuous)
- **Input:** MediaPipe FaceLandmarker blendshape scores
- **Key blendshapes:** `jawOpen`, `browInnerUp`, `eyeBlinkLeft`, `eyeBlinkRight`, `mouthSmileLeft`, `mouthSmileRight`, head pose
- **Output:** Modulates granular audio texture continuously
  - `jawOpen` → grain size
  - `browInnerUp` → filter frequency
  - Smile scores → reverb depth
  - Head pose → additional modulation axis
- **Audio source:** `ambientwub.wav` (AI-generated) via `Tone.GrainPlayer`
- **Visuals:** Ambient, atmospheric — reacts to expression in real time

### Hand Channel (Event-Driven)
- **Input:** Gesture detection — velocity-based strike detection
- **Output:** Percussive audio triggers + glitch shockwave visuals
- **Visual effects:** Scan-line tears, pixel scatter, full-screen radiance
- **Existing:** Functional hand gesture system already in codebase

---

## MediaPipe Notes

- Using `@mediapipe/tasks-vision` (Tasks API) — NOT the older `@mediapipe/face_mesh`
- Reason: Tasks API provides 52 pre-trained blendshape scores directly (no geometry derivation needed)
- Running mode: VIDEO (not LIVE_STREAM, not IMAGE)
- GPU delegate strategy is the right call for latency targets

---

## Known Issues / Technical Debt

- [ ] Head pose matrix validation — sign correctness unconfirmed
- [ ] Missing temporal smoothing — EMA with alpha 0.2 needed on blendshape scores
- [ ] Asymmetric blink handling — left/right need separate treatment
- [ ] Null/face-absent fallback logic — need lerp fallback, not hard cutoff
- [ ] `ambientwub.wav` not yet confirmed sourced — Phase 3 dependency

---

## Obsolete Code (to remove)

- InstrumentSelect UI
- PianoEngine
- Drum maps
- Keyboard note constants
