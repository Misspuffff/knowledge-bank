---
tags:
  - type/reference
  - context/reference
  - status/active
---

# Tag Taxonomy

> *Your vault's tag system at a glance. Every note has 2–4 nested tags in its frontmatter so you can filter the vault by type, project, client, status, or topic.*

---

## How tags work here

- Tags live in **YAML frontmatter** (`tags:` field), not inline in body text.
- They're **nested** with slashes (`type/MOC`, `client/anthropic`) so the Tags pane shows them as a collapsible tree.
- Each note has **2–4 tags** — lean on purpose. Add more only if a note really spans multiple categories.
- Open the **Tags pane** (right sidebar in Obsidian) to browse the tree, or use the search bar with `tag:#prefix/value`.

---

## Prefixes

### `type/` — what kind of note it is
| Tag | Use for |
|---|---|
| `type/MOC` | Map of Content (folder hub note) |
| `type/index` | Vault-wide index page |
| `type/note` | General knowledge note |
| `type/reference` | Reference material you look things up in |
| `type/log` | Running journal / dev log |
| `type/project` | A project file (usually in `20 - Creative`) |
| `type/brief` | Project brief / spec |
| `type/case-study` | Finished work writeup |
| `type/roadmap` | Phase plan or roadmap |
| `type/tracker` | Tracking sheet (applications, status, etc.) |
| `type/opportunity` | A specific job / role / pitch you're pursuing |
| `type/person` | A person note in `50 - People` |
| `type/template` | Reusable template |
| `type/prompt` | A Claude / AI prompt |
| `type/conversation` | A saved AI conversation |

### `context/` — which area of the vault it lives in
| Tag | Folder |
|---|---|
| `context/home` | Root |
| `context/inbox` | `00 - Inbox` |
| `context/learning` | `10 - Learning` |
| `context/creative` | `20 - Creative` |
| `context/reference` | `30 - Reference` |
| `context/career` | `40 - Career` |
| `context/people` | `50 - People` |
| `context/claude` | `claude/` |
| `context/scadpro` | `20 - Creative/SCADpro` |

### `project/` — your active builds
`project/air` · `project/flow` · `project/iwd-2026` · `project/lookline`

### `client/` — companies attached to work or applications
`client/adobe` · `client/google` · `client/mayo-clinic` · `client/skullcandy` · `client/great-dane` · `client/anthropic` · `client/microsoft` · `client/neuralink` · `client/proto` · `client/parliament` · `client/kickr`

### `status/` — where the note stands
| Tag | Meaning |
|---|---|
| `status/active` | Currently working on it |
| `status/archive` | Done, kept for reference |
| `status/complete` | Shipped / closed |
| `status/idea` | Capture only, not started |
| `status/cold` | Paused / on hold |

### `topic/` — subject matter
The most varied prefix. Common ones in use:

`topic/design` · `topic/ai` · `topic/tools` · `topic/coding` · `topic/javascript` · `topic/storytelling` · `topic/copywriting` · `topic/editing` · `topic/writing` · `topic/summarization` · `topic/clipping` · `topic/explanation` · `topic/social` · `topic/translation`

Add new `topic/` values freely — just keep them lowercase and singular.

---

## Useful searches

| Query | What you get |
|---|---|
| `tag:#status/active` | Everything you're working on right now |
| `tag:#client/anthropic` | All Anthropic-related notes |
| `tag:#project/air` | Every AIR file in one click |
| `tag:#type/opportunity AND tag:#status/active` | Live job applications |
| `tag:#type/prompt` | All your Claude custom prompts |
| `tag:#type/MOC` | Every folder hub note |
| `tag:#context/career AND tag:#status/active` | Active career work |

---

## Adding tags to new notes

When you create a note, add 2–4 tags in the frontmatter using this pattern:

```yaml
---
tags:
  - type/note
  - context/learning
  - topic/ai
---
```

**Rules of thumb:**
- Always include one `type/` and one `context/` tag.
- Add `project/` or `client/` if the note belongs to a specific build or company.
- Add `status/` if the note has a clear lifecycle (active, archive, complete, idea, cold).
- Add `topic/` only if it sharpens search — skip if it's redundant with the type or context.

---

## Related

- [[Home MOC]] — vault front door
- [[My Vault Map]] — full file index
- [[Reference MOC]] — this folder's hub
