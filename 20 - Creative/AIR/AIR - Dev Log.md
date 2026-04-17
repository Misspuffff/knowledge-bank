---
tags: [project/air, devlog]
created: 2026-04-15
type: log
---

# AIR — Dev Log

> Running log of sessions, decisions, blockers, and breakthroughs. Most recent at top.

---

## 2026-04-15 — Project knowledge migrated to Obsidian

Consolidated all AIR project context from Claude conversation memory into vault. Created full project folder structure mirroring Flow.

**Current state:**
- Hand gesture system functional — velocity-based strike detection, Tone.js samplers, canvas overlay drawing
- Tasks Vision API migration in progress (Phase 2)
- `phase-2-updated.md` prompt ready for Claude Code handoff

**Open blockers:**
- Head pose sign correctness unconfirmed
- EMA smoothing not yet implemented
- `ambientwub.wav` not yet sourced (Phase 3 dependency)

---

## Architecture Decision — Tasks Vision API Migration

**Decision:** Migrate from `@mediapipe/face_mesh` to `@mediapipe/tasks-vision` FaceLandmarker.

**Why:** The Tasks API provides 52 pre-trained blendshape scores directly. The blendshape score approach is the right level of abstraction for a musical instrument (you want `jawOpen: 0.73`, not "landmark 17 is 12px below landmark 14").

**Running mode:** VIDEO (not LIVE_STREAM). Stable choice for our use case.

---

## Concept Clarification — What AIR Is Not

- NOT a multi-instrument selector
- NO drums/piano/guitar modes
- NOT mode-switching of any kind
- The performer IS the instrument — one unified experience

---

## Visual System — Glitch Aesthetic Decision

The glitch visual effects are not decoration. They are culturally grounded in electronic music and dubstep. The augmented mirror model is core to the concept. All effects on the live camera feed. Not a separate overlay UI.

---

*Add new entries above. Date format: YYYY-MM-DD.*
