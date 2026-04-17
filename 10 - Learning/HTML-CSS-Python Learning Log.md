# 🧠 HTML / CSS / Python Learning Log
*Taught by Claude · Updated live in Obsidian*

---

## 📍 How This Works
- Claude teaches you directly in this file
- Each session gets its own dated section
- Code examples, exercises, and your notes all live here
- Tag questions with `❓` and we'll address them next session

---

## 🗺️ Curriculum Roadmap

### Phase 1 — HTML Foundations
- [ ] What is HTML? Structure of a webpage
- [ ] Tags, elements, and attributes
- [ ] Headings, paragraphs, links, images
- [ ] Lists (ordered & unordered)
- [ ] Divs and semantic HTML

### Phase 2 — CSS Basics
- [ ] What is CSS? How it connects to HTML
- [ ] Selectors, properties, values
- [ ] Colors, fonts, spacing (margin/padding)
- [ ] The box model
- [ ] Flexbox intro

### Phase 3 — Python Foundations
- [ ] What is Python? How it's different from HTML/CSS
- [ ] Variables and data types
- [ ] Functions
- [ ] Lists and loops
- [ ] Reading and writing files

---

## 📚 Sessions

---

### 📅 Session 1 — April 15, 2026
**Topic: What is HTML? Your first webpage.**

---

#### 🌐 What is HTML?

HTML stands for **HyperText Markup Language**. It's not really a programming language — it's a **structure language**. Think of it like the skeleton of a webpage.

Every webpage you've ever visited is made of HTML. It tells the browser:
- "Here's a heading"
- "Here's a paragraph"
- "Here's an image"
- "Here's a link"

CSS is what makes it *look good*. JavaScript makes it *do things*. But HTML is always the foundation.

---

#### 🏷️ Tags — The Building Blocks

HTML is made of **tags**. Tags wrap around content and tell the browser what that content *is*.

A tag looks like this:

```html
<p>This is a paragraph.</p>
```

- `<p>` is the **opening tag**
- `</p>` is the **closing tag** (note the `/`)
- Everything between them is the **content**

Together, the opening tag + content + closing tag = an **element**.

---

#### 🧱 A Complete HTML Page

Every HTML file has the same basic skeleton:

```html
<!DOCTYPE html>
<html>
  <head>
    <title>My First Page</title>
  </head>
  <body>
    <h1>Hello, world!</h1>
    <p>This is my first webpage.</p>
  </body>
</html>
```

Here's what each part does:

| Tag | What it does |
|---|---|
| `<!DOCTYPE html>` | Tells the browser this is HTML5 |
| `<html>` | Wraps the entire page |
| `<head>` | Invisible info (title, metadata) |
| `<title>` | The name shown in the browser tab |
| `<body>` | Everything *visible* on the page |
| `<h1>` | A big heading |
| `<p>` | A paragraph |

---

#### ✏️ Your First Exercise

Try this: In your code editor (or even a plain `.txt` file renamed to `.html`), type out the skeleton above. Change the `<title>` and `<h1>` to something personal. Save it, then drag the file into a browser window.

You just built a webpage. 🎉

> 📝 **Your notes here:**


---

#### ❓ Questions from this session
*(Add any questions here and Claude will answer them at the start of the next session)*


---
*Next session → HTML: Headings, paragraphs, links & images*


---

## April 2026 — Language Switch Note

> Thinking about switching from JavaScript to Python as primary focus.
> Bring this up with Claude next session — ask for a proper ramp-up plan given what's already been built in JS.
> CodeQuest can stay in JS; Python might be a parallel track for data/scripting work.
