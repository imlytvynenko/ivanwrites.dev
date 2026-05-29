---
title: Notes on Writing Code You Can Delete
description: Designing modules to be thrown away made my projects easier to change.
category: Software Development
date: 2026-04-22
tags: [Architecture, Simplicity]
readTime: 6 min read
image: https://images.unsplash.com/photo-1517694712202-14dd9538aa97?w=1400&q=85&auto=format&fit=crop
imageAlt: Code on a screen
---

The code I'm happiest with is the code I can delete without fear. Designing for deletion changed how I structure projects.

## Seams Over Cleverness

Clear boundaries between modules matter more than clever internals. If a piece is easy to cut out, it's easy to replace.

## Optimize for Change

Most software lives longer than we expect and changes more than we plan. Writing for the next person — usually future me — pays off quickly.

## Keep It Boring

Boring, obvious code is a feature. It's the code you can read at a glance and remove in an afternoon.
