---
tags:
  - type/reference
  - project/flow
  - topic/architecture
  - topic/tech-stack
created: 2026-04-15
status: active
type: technical
up:
  - - Flow MOC
---

# Flow — Architecture & Tech Stack

## Current Stack

| Layer | Technology | Notes |
|-------|-----------|-------|
| **Frontend** | React + TypeScript + Vite | Core application |
| **AI — Reasoning** | Gemini API (text-to-text + multimodal) | Via Google AI Studio |
| **AI — Image Gen** | Adobe Firefly | Image generation |
| **Data Persistence** | localStorage + IndexedDB | Client-side storage |
| **Canvas** | Infinite canvas (custom) | Drag-and-drop pin system |

## Current Implementation

What's already built in the prototype:
- ✅ Pin system for content organization
- ✅ Infinite canvas workspace
- ✅ Drag-and-drop functionality
- ✅ AI analysis capabilities
- ✅ Data persistence (localStorage + IndexedDB)
- ✅ Gemini integration

## Planned Architecture (Phase 3+)

```
[User Input]
     ↓
[Seed Column] → drag/drop, text, image upload
     ↓
[Gemini API] → multimodal reasoning, embeddings, semantic clustering
     ↓
[Canvas Engine] → node generation, branching, pulse animations
     ↓
[Output Panel] → concept cards, prompts, briefs
     ↓
[Export] → Adobe/Figma formats, creative brief docs
```

## Session Memory

Dynamic context window that carries previous ideation branches — each session builds on the last, behaving like a living sketchbook rather than a fresh chat.

## Export Targets

- Concept summary (markdown / PDF)
- Creative brief (slide-ready)
- AI prompt format (for Firefly or Midjourney)
- Adobe / Figma integration (Phase 4)

## Performance Notes

- Drag optimization needed for multiple pins
- Multi-select capabilities — in progress
- Mobile touch support — planned
