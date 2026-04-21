---
tags:
  - type/reference
  - context/learning
  - topic/ai
  - topic/tools
---
# AI Tools & Prompts

*A living log of tools, observations, and prompts worth keeping.*

---

## Mental model: what an agent actually is

From a Socratic conversation — the breakthrough framing:

> When you sit down to work, you receive a task, think about what steps it requires, take those steps one by one, and adjust when something unexpected happens. You *decided*, then *acted*, then *observed the result*, then *decided again*. That loop — decide, act, observe — is the heartbeat of an agent.

Think of it like a **sous chef**. You say: *"Prep the mise en place."* You don't explain every cut. They read the recipe, open the fridge, chop, taste, adjust. That's an agent — acting on your behalf, using judgment, using tools, working toward your goal.

**The real skill:** Think in *goals*, not steps. The agent handles the steps. You define what success looks like.

---

## Key observations (from the Improving Panel, April 2026)

- **"AI is just a tool, not the solution."** — Tal Phillips
- Critical thinking, curiosity, and problem-solving are now the main ticket — not supplementary skills
- Meta-prompting is underused: ask "why did you make this decision?" — it deepens output
- Skill files structure how you work with models — this is underutilized by most people
- Don't lose human thought — Claude is trained on general knowledge, not *your* knowledge
- If you can do it faster yourself, just do it
- "AI is like basic math — you need to know it like multiplication tables"
- **5 layers of AI:** chat → chips → cloud → models → applications (models = the OS layer)
- Sharing unreviewed AI output gives up trust and relationship agency
- Personal knowledge system beats scattered bookmarks/notes

---

## Prompts worth saving

### Meta-prompting
After any output you're not sure about:
> *"Why did you make this decision?"*

Surfaces the reasoning. Gives you something to push back on. Makes the next output better.

### Midjourney prompting trick
Use Claude to *write* the Midjourney prompts. Describe what you want as **narrative moments and emotional beats**, not visual descriptions.
> *"Frame it as if you're writing a scene direction, not an image description."*

This is what made the Adobe sprint work — layered AI: Claude writes prompts → Midjourney generates images → images inform video.

---

## AI + design work: what you've learned

From the Adobe sprint (Fall 2024) — future of storytelling for next-gen creatives, presented to Adobe's SVP:

Your dramatic writing background is an asset in prompting. You can frame requests as narrative moments — not just what you want visually but *why* it matters for the story. That's a skill most people building with AI tools don't have.

---

## The philosophy (from building Flow)

> *"AI shouldn't just do the work for you — it should amplify what you can do."*
> *"The journey matters. AI should surface directions and variations, not collapse the entire creative process into a single moment."*
> *"Good tools should amplify human creativity, not replace it — like how good story structure supports a narrative without dictating it."*

---

## Skill files
Custom Claude skills live in `/mnt/skills/user/` in the Claude environment.

Active: `kickr-email-polish`, `meeting-minutes-taker`, `hours-breakdown`, `coding-coach`, `kickr-kickoff-deck`, `portfolio-critique-agent`, `humanize`, `honest-agent`, `skill-creator`, and others.

Format: a `SKILL.md` that defines exactly how Claude should behave for a recurring task. Reusable, refineable, yours.

---

## Pipelines (repeatable workflows)

**Claude → Lovable** for editorial/visual web experiences:
1. Research + brief development in Claude (multiple iterations before touching Lovable)
2. Copy and visual direction established
3. Build in Lovable

**Claude → Claude Code** for functional apps:
1. Claude writes a detailed `PLAN.md`
2. Claude Code executes one discrete session at a time
3. Review → next session

---

## Builder stack
> Full tool list in [[../30 - Reference/My Stack|My Stack]] — single source of truth.

---

## Tools to explore

### Huxe App
- Came across this — want to understand if it can integrate with Obsidian
- Backup idea: build a custom daily brief tool instead

### OpenClaw
- Want to explore integrating **OpenClaw** (open-source local AI agent) with Obsidian for automation — check its GitHub for file system actions and any Obsidian connector. Look into the **Local REST API** community plugin as a bridge.

### Interactive codespace in Obsidian notes
- Is it possible to have a live/interactive coding environment embedded in notes?
- Worth researching Obsidian plugins (DataviewJS, Code Runner, or iframe approach)

### MCP config — Slack export
- Need to update MCP config for Slack export
- ==Open question: can I run more than one local MCP at the same time?

### Teams channel aggregator
- Explore best way to combine/monitor multiple Teams channels in one view
- Consider how changes would affect shortcuts on personal devices

### Gcal ↔ Outlook live sync
- Goal: bidirectional sync between Google Calendar and Outlook
- Use case: morning briefs on Pixel 10 pulling from both sources
- Research: Zapier / Make automations, or a Power Automate flow
