---
tags:
  - type/MOC
  - project/air
  - status/active
created: 2026-04-15
status: paused
type: MOC
aliases:
  - Audiovisual Instrument in Real-time
  - purplemonkey
---

# AIR — Map of Content

> *"The performer's face and body are the instrument. AIR inverts the web face."*

AIR (Audiovisual Instrument in Real-time) is a browser-based performance instrument that uses webcam input to translate facial expressions and hand gestures into unified real-time audio and visual output. Built with MediaPipe, Tone.js, React, and the Canvas API.

---

## Notes in this Project

| Note | Purpose |
|------|---------|
| [[AIR - Master Brief]] | Full concept, philosophy, and success criteria |
| [[AIR - Architecture & Tech Stack]] | Two-channel system, MediaPipe, Tone.js, Zustand |
| [[AIR - Interaction Vocabulary]] | Face blendshapes → audio; hand gestures → events |
| [[AIR - Phase Tracker]] | Six-phase dev plan, Claude Code prompt handoff |
| [[AIR - Dev Log]] | Running log of decisions, errors, and breakthroughs |

---

## Related Notes

- [[../../10 - Learning/AI Tools]]
- [[../../10 - Learning/JavaScript Notes]]
- [[../../40 - Career/Portfolio Status]]

---

## Current Focus

- [ ] Complete Tasks Vision API migration (Phase 2)
- [ ] Resolve EMA blendshape smoothing (alpha 0.2)
- [ ] Fix lerp fallback for null/face-absent states
- [ ] Confirm head pose sign correctness
- [ ] Source `ambientwub.wav` for GrainPlayer (Phase 3 dependency)
- [ ] Screen recording demo for LinkedIn/portfolio

---

## The Core Idea

AIR is not a multi-instrument selector. There are no modes. It is a single unified experience — the performer IS the instrument. Facial expressions modulate granular audio texture continuously. Hand gestures trigger percussive events. The performer sees themselves on screen; the screen is a reactive environment.

**Repo:** [github.com/Misspuffff/purplemonkey](https://github.com/Misspuffff/purplemonkey)
