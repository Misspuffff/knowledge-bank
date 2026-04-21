---
tags:
  - type/tracker
  - project/air
  - topic/development
created: 2026-04-15
type: tracker
---

# AIR — Phase Tracker

> Six-phase development plan. Each phase is handed off to a Claude Code session via an orientation prompt.

**Workflow split:**
- Claude Code → implementation execution
- This chat → decisions, debugging, architecture, prompt refinement

---

## Phase Overview

| Phase | Focus | Status |
|-------|-------|--------|
| 1 | Hand gesture system + percussive triggers | ✅ Complete |
| 2 | Tasks Vision API migration + FaceLandmarker integration | 🔄 In Progress |
| 3 | GrainPlayer + face → audio parameter mapping | ⏳ Blocked on `ambientwub.wav` |
| 4 | Glitch visual system (scan-line, pixel scatter, radiance) | ⏳ Pending |
| 5 | Temporal smoothing + polish pass | ⏳ Pending |
| 6 | Demo recording + obsolete code cleanup | ⏳ Pending |

---

## Phase 2 — Active

**Goal:** Replace `@mediapipe/face_mesh` with `@mediapipe/tasks-vision` FaceLandmarker. Access 52 blendshape scores.

### Phase 2 Technical Gaps to Resolve
- [ ] Head pose matrix validation — confirm sign correctness
- [ ] EMA smoothing (alpha 0.2) on blendshape outputs
- [ ] Lerp fallback for null/face-absent states (not hard cutoff)
- [ ] Asymmetric blink handling

---

## Phase 3 — Dependency

Requires `ambientwub.wav` to be available as GrainPlayer source. **Do not start Phase 3 without confirming this asset.**

---

## Key Decisions Log

| Decision | Rationale |
|----------|-----------|
| Tasks Vision API over `face_mesh` | Access to 52 pre-trained blendshape scores; no geometry derivation |
| VIDEO running mode | Better for continuous face tracking vs LIVE_STREAM |
| GPU delegate | Required for <33ms latency target |
| GrainPlayer (Tone.js) | Enables granular synthesis from audio buffer |
| Zustand for state | Lightweight, works well with React + Tone.js side effects |
