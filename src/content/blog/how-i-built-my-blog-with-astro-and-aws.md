---
title: How I Built My Blog with Astro and AWS
description: A step-by-step overview of my minimal blog setup using Astro, GitHub, and AWS Amplify.
category: Software Development
date: 2026-05-28
tags: [AWS, Astro, Web]
readTime: 8 min read
image: https://images.unsplash.com/photo-1506905925346-21bda4d32df4?w=1400&q=85&auto=format&fit=crop
imageAlt: Mountains reflected in a calm lake
---

I wanted a blog that's fast, minimal, and easy to maintain. After trying a few different setups, I ended up with this combination that I'm really happy with.

## Why Astro?

Astro ships less JavaScript by default. It generates static HTML and only loads what's necessary. The result? Blazing fast performance and a great authoring experience for content-heavy sites.

Coming from heavier frameworks, the islands architecture felt like a breath of fresh air — I add interactivity only where I actually need it.

## Tech Stack

Here's what I'm using:

- Astro
- Tailwind CSS
- Markdown / MDX
- GitHub
- AWS Amplify (hosting)

## Setting Up the Project

Spinning up a new Astro project takes a single command. From there, I added the Tailwind integration and a content collection for posts so everything stays type-safe and organized.

```bash
npm create astro@latest
npx astro add tailwind
```

Each post lives as a Markdown file with a small frontmatter block for the title, date, and tags. Astro turns that into fully static pages at build time.

## Deploying to AWS

I connected the GitHub repository to AWS Amplify. Every push to `main` triggers a build and deploys the static output to a global CDN, with HTTPS handled automatically.

The whole pipeline is effectively free for a personal site, and deploys finish in under a minute.

## Final Thoughts

This setup hits the sweet spot for me: fast, cheap, and pleasant to write in. If you want a low-maintenance blog you fully own, Astro on Amplify is hard to beat.
