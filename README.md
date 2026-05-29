# Ivan Writes

A minimal, black-and-white personal blog built with [Astro](https://astro.build) and [Tailwind CSS](https://tailwindcss.com). I write about software development, running, travel, productivity, and the small lessons that make life better.

🌐 [ivanwrites.dev](https://ivanwrites.dev)

## ✨ Features

- Content-collection–driven blog (Markdown posts with typed frontmatter)
- Posts split into **Software Development** and **Lifestyle** categories
- Homepage with the latest posts
- Category listing pages (`/software`, `/lifestyle`) and a full archive (`/blog`)
- Single post pages with an auto-generated "On this page" table of contents
- About, Projects, Now, and Uses pages
- Custom 404 page
- Reusable components and a clean, responsive, minimal design

## 🧱 Tech Stack

- **Framework:** Astro
- **Styling:** Tailwind CSS
- **Content:** Markdown via Astro content collections
- **Hosting:** AWS Amplify (static output)

## 🚀 Project Structure

```text
public/
├── icons/
│   └── lion-icon.png            # header logo + favicon
├── illustrations/
│   ├── lion-404.png             # 404 page illustration
│   └── workspace-line-art.svg   # homepage hero illustration
└── images/
    └── posts/                   # post images

src/
├── components/
│   ├── Header.astro
│   ├── Footer.astro
│   ├── Layout.astro
│   ├── PostCard.astro
│   └── CategoryBadge.astro
├── content/
│   └── blog/                    # Markdown posts (one collection)
├── pages/
│   ├── index.astro              # homepage (latest posts)
│   ├── blog/
│   │   ├── index.astro          # all posts
│   │   └── [slug].astro         # single post
│   ├── software/index.astro     # Software Development posts
│   ├── lifestyle/index.astro    # Lifestyle posts
│   ├── about.astro
│   ├── projects.astro
│   ├── now.astro
│   ├── uses.astro
│   └── 404.astro
├── styles/
│   └── global.css
└── content.config.ts            # blog collection schema
```

## ✍️ Adding a Post

Create a new Markdown file in `src/content/blog/`. The filename becomes the URL slug (e.g. `my-post.md` → `/blog/my-post`).

```md
---
title: My Post Title
description: A short summary used in listings and meta tags.
category: Software Development # or "Lifestyle"
date: 2026-05-28
tags: [Astro, Web]
readTime: 5 min read
image: https://example.com/cover.jpg # optional
imageAlt: Description of the image # optional
---

Your content here in **Markdown**.

## A heading

Headings become entries in the post's table of contents.
```

The post automatically appears on the homepage, `/blog`, and its category page.

## 🧞 Commands

All commands are run from the root of the project, from a terminal:

| Command                   | Action                                           |
| :------------------------ | :----------------------------------------------- |
| `npm install`             | Installs dependencies                            |
| `npm run dev`             | Starts local dev server at `localhost:4321`      |
| `npm run build`           | Build your production site to `./dist/`          |
| `npm run preview`         | Preview your build locally, before deploying     |
| `npm run astro ...`       | Run CLI commands like `astro add`, `astro check` |

> Requires Node.js `>=22.12.0`.
