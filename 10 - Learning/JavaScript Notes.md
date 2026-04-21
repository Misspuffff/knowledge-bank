---
tags:
  - type/reference
  - context/learning
  - topic/coding
  - topic/javascript
---
# JavaScript Notes

*Running notes as you learn. Concepts, patterns, things that clicked.*

---

## How you learn best
You built CodeQuest around this insight: **language-acquisition model** — immersion first, vocabulary as translation, pattern recognition before production. The same method applies to your own learning. Don't memorize syntax. Learn to read it.

Your goal isn't to become a developer. It's to be in the loop — understanding AI-generated code well enough to catch errors, push back, and direct it intentionally.

---

## Concepts that clicked

### `const` vs `let`
- `const` = this value won't change. Use it whenever you can — it signals intent.
- `let` = this value might change. Use it only when you need to reassign.
- `var` = old way. Ignore it.

```js
const toolName = "Figma"      // won't change
let xpCount = 0               // will update as user earns XP
```

> "AI used let for everything. When should you push back? When the value will never change — use const."

---

### Functions
A variable is a noun (stores something). A function is a verb (does something).

```js
function greet(name) {
  return "Hey, " + name
}

greet("Maddy") // → "Hey, Maddy"
```

- `return` hands the result back out. Without it, the function runs but gives nothing back.
- Parameters are inputs. The name inside `()` when you *define* it.
- Arguments are what you pass in when you *call* it.

---

### Reading AI code: the decode method
When AI writes something you don't recognize, trace it step by step:
1. What is each variable storing?
2. What does each function take in, and what does it return?
3. Follow the data — where does it start, where does it end up?

---

## Patterns I keep using
- `const` for anything that won't be reassigned
- Named functions over anonymous ones when readability matters
- Tracing data flow top-to-bottom when confused

---

## Things that confused me (and the answer)

| Confusion | Answer |
|---|---|
| Why does return matter? | Without return, the function runs but gives nothing back to the caller |
| When is let vs const? | const = fixed. let = might change. When in doubt, start with const |

---

## CodeQuest — the project
> [[../20 - Creative/Active Projects|→ See Active Projects for CodeQuest build status]]

**Stack:** React + Vite + Tailwind + Supabase
**What it teaches:** JavaScript fundamentals via language-acquisition model
**Module structure:** vocab → decode AI code → translate → produce → quiz → remediation
**10 modules total.** Pass 80% on module quiz to unlock next. Final 15-question course test at the end.

**Completed sessions:** 10 build sessions in Claude Code as of April 2026.
**Next:** Session 12 — content expansion for modules 4–9.

---

## Stack reference
> Full builder stack lives in [[../30 - Reference/My Stack|My Stack]] — single source of truth for every tool and technology.
