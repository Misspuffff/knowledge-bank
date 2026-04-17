# Obsidian + GitHub Learning Log

**Goal:** Get genuinely comfortable navigating Obsidian and GitHub — not just using them, but understanding *why* they work the way they do.

**Format:** Claude teaches directly in this file. Lessons build on each other. Exercises happen here.

---

## 🗺️ Curriculum Overview

### Module 1 — Obsidian Foundations
- [ ] What Obsidian actually is (and why it's weird at first)
- [ ] Vault structure: folders, files, and the MOC system
- [ ] How to navigate without getting lost
- [ ] Creating and linking notes
- [ ] Using this file as a live practice ground

### Module 2 — GitHub Foundations
- [ ] What GitHub actually is (repos, commits, branches — demystified)
- [ ] Reading a repo like a map
- [ ] The difference between GitHub (website) and Git (the tool)
- [ ] How to clone, edit, and push without terminal terror
- [ ] Connecting GitHub to real project work

### Module 3 — Using Them Together
- [ ] Why people use Obsidian + GitHub together
- [ ] Version-controlling your vault (optional but powerful)
- [ ] Practical workflows for a PM/strategist

---

## 📓 Lessons

*Lessons will appear below as we work through them.*

---

## ✅ Exercises Completed

*Logged here as you finish them.*

---

## 💬 Questions & Notes

*Jot anything confusing here mid-lesson.*

---

## Module 1 — Obsidian Foundations

### Lesson 1: What You're Actually Looking At

You opened Obsidian and saw a folder tree on the left. That folder tree is called the **File Explorer**, and it's showing you your **vault**.

A vault is just a regular folder on your computer that Obsidian is pointed at. Every note you create is a plain `.md` (Markdown) file sitting inside that folder. There's no database, no cloud lock-in — just files.

This matters because:
- You own everything. If you deleted Obsidian tomorrow, all your notes would still be there on your computer.
- The folder structure you see in Obsidian is the *real* folder structure on your hard drive.
- This file right now? It's stored at: `10 - Learning/Obsidian + GitHub Learning Log.md`

---

### The Three-Panel Layout

Obsidian typically has three areas:

| Area | What it is |
|---|---|
| **Left sidebar** | File Explorer (folder tree) + other panels |
| **Editor** | The open note you're reading/writing in |
| **Right sidebar** | Properties, backlinks, outline (can be hidden) |

You're currently in the **Editor** reading this file. The folder tree you mentioned is the **File Explorer** in the left sidebar.

---

### What a MOC Is

You may have noticed files called `Home MOC.md` and `Learning MOC.md` in your vault. MOC stands for **Map of Content** — it's just a note that links to other notes, acting like a table of contents or index. It's not a special Obsidian feature, just a convention smart people use to avoid getting lost.

---

### ✏️ Exercise 1.1 — Navigate Your Vault

Do these steps in Obsidian right now:

1. In the File Explorer, click on the `10 - Learning/` folder to expand it
2. Find and open `Learning MOC.md`
3. Read what's in it
4. Come back to this file (click it in the sidebar)

When you're done, come back to the Claude chat and tell me: **what did you see in Learning MOC.md?**

---

---

### Lesson 2: Internal Links — The Thing That Makes Obsidian Special

You saw `[[double bracket]]` links in your Learning MOC. These are called **internal links** (or wikilinks), and they're the core feature that separates Obsidian from a regular notes app.

When you write `[[filename]]`, Obsidian:
1. Creates a clickable link to that file
2. Tracks the connection — so you can later see *everything* that links *to* a note (called **backlinks**)
3. Even lets you link to notes that don't exist yet (they show up in a different color until you create them)

This is how people build a "second brain" — notes that reference each other like a web, not a hierarchy.

---

### ✏️ Exercise 1.2 — Click an Internal Link

1. Open `Learning MOC.md`
2. Click on `[[JavaScript/JavaScript Notes]]`
3. See where it takes you
4. Use the back arrow (top left, or `Ctrl/Cmd + Alt + ←`) to come back
5. Come back to this file

Then tell Claude: **what was in the JavaScript Notes file?**

---

### ✅ Exercise Log

| # | Exercise | Status |
|---|---|---|
| 1.1 | Navigate vault, open Learning MOC | ✅ Complete |
| 1.2 | Click an internal link | ⬜ In progress |

---

---

### Lesson 3: Creating and Editing Notes

You've been *reading* notes. Now let's *make* one.

There are three ways to create a new note in Obsidian:

| Method | How |
|---|---|
| **New note button** | Click the pencil/page icon at the top of the File Explorer |
| **Keyboard shortcut** | `Ctrl + N` (Windows) or `Cmd + N` (Mac) |
| **Click an empty link** | Write `[[Note That Doesn't Exist Yet]]` and click it |

When you create a note, it lands in your vault root (top level) by default. You can then drag it into the right folder in the File Explorer.

Editing is just... typing. Obsidian uses **Markdown** for formatting:

| What you type | What it looks like |
|---|---|
| `# Big Heading` | Big heading |
| `## Smaller Heading` | Smaller heading |
| `**bold**` | **bold** |
| `- item` | bullet point |
| `[[filename]]` | internal link |

You're already reading Markdown right now — this whole file is written in it.

---

### ✏️ Exercise 1.3 — Create Your Own Note

1. Press `Cmd/Ctrl + N` to create a new note
2. Name it `My Vault Map`
3. Write a heading: `# My Vault Map`
4. Add one line describing what each of your top-level folders is for (just guess if you're not sure)
5. Save it (Obsidian autosaves, but `Cmd/Ctrl + S` works too)
6. Drag it into `30 - Reference/` in the File Explorer

Then tell Claude: **did it land in the right folder?**

---

### ✅ Exercise Log

| # | Exercise | Status |
|---|---|---|
| 1.1 | Navigate vault, open Learning MOC | ✅ Complete |
| 1.2 | Click an internal link | ✅ Complete |
| 1.3 | Create and move a new note | ⬜ In progress |

---
