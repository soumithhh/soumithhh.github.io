# Soumith's Jekyll Shelf & Blog Theme 📚✍️

A complete, lightweight Jekyll static site configured for a personal Bookshelf and Blog. Designed with a hand-drawn sketched visual style, custom collection support for books (`_books/`), client-side category filtering, sorting, and responsive layouts.

![Theme Preview](https://images.unsplash.com/photo-1507842217343-583bb7270b66?w=800&q=80)

---

## 🚀 Quick Start / Local Setup

### Prerequisites
- [Ruby](https://www.ruby-lang.org/en/downloads/) (v3.0+)
- [Bundler](https://bundler.io/) & [Jekyll](https://jekyllrb.com/)

### Running Locally
1. Clone this repository:
   ```bash
   git clone https://github.com/soumith/soumith-shelf.git
   cd soumith-shelf
   ```
2. Install dependencies:
   ```bash
   bundle install
   ```
3. Start local server:
   ```bash
   bundle exec jekyll serve
   ```
4. Open `http://localhost:4000` in your browser.

---

## 📂 Repository File Structure

```
.
├── _books/                   # 📚 Markdown files for your book shelf
│   ├── sample-book.md
│   ├── atomic-habits.md
│   └── clean-code.md
├── _posts/                   # ✍️ Blog posts directory
│   └── 2026-07-26-sample-post.md
├── _layouts/                 # 🎨 Jekyll HTML Page Templates
│   ├── default.html          # Base site frame & layout wrapper
│   ├── shelf.html            # Shelf grid with category filter & sort
│   ├── book.html             # Individual Book detail view
│   └── post.html             # Individual Blog post view
├── _includes/                # 🧩 Header & Footer partials
│   ├── header.html
│   └── footer.html
├── assets/
│   └── css/
│       └── main.css          # Base styles matching sketch layout design
├── _config.yml               # Jekyll configuration & collections definition
├── Gemfile                   # Ruby gem dependencies for GitHub Pages
├── index.html                # Home page
├── shelf.html                # Shelf listing page (/shelf/)
├── blog.html                 # Blog listing page (/blog/)
├── .gitignore
└── README.md
```

---

## 📖 Content Workflow: How to Add New Content

### 1. Adding a New Book to the Shelf
Simply create a new Markdown file inside the `_books/` directory (e.g. `_books/my-new-book.md`).

Include the following front-matter at the top of the file:

```markdown
---
layout: book
title: "The Design of Everyday Things"
author: "Don Norman"
category: "Design"
tags: ["design", "ux", "psychology"]
finished_date: "2026-07-20"
cover_image: "https://images.unsplash.com/photo-1544716278-ca5e3f4abd8c?w=400&q=80"
summary: "A powerful primer on human-centered design and usability."
---

### My Notes & Chapter Summaries

Write your review, key takeaways, and notes in standard Markdown here!
```

> **Note:** As soon as you add this file, Jekyll automatically displays it on the `/shelf` page, assigns its category to the filter dropdown, and generates a detail page at `/shelf/my-new-book/`!

### 2. Adding a Blog Post
Create a Markdown file inside `_posts/` with the required `YYYY-MM-DD-title.md` naming format:

```markdown
---
layout: post
title: "My First Blog Post"
date: 2026-07-26
author: "Soumith"
category: "General"
---

Write your blog post content here!
```

---

## 🌐 Deploying to GitHub Pages

1. Push this repository to GitHub.
2. In your GitHub repository, go to **Settings** > **Pages**.
3. Under **Build and deployment**:
   - **Source**: Select `Deploy from a branch`
   - **Branch**: Choose `main` (or `master`) and folder `/ (root)`.
4. Click **Save**. GitHub Pages will automatically compile Jekyll and publish your site!

---

## 🎨 Customizing Styles & Typography
- Main CSS is in `assets/css/main.css`.
- Google Fonts used: `Architects Daughter` & `Patrick Hand` for the hand-drawn sketch aesthetic.

Designed for **Soumith**.
