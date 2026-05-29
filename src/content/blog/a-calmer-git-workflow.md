---
title: A Calmer Git Workflow for Solo Projects
description: Fewer branches, smaller commits, and a habit of writing the changelog first.
category: Software Development
date: 2026-05-06
tags: [Git, Workflow, Habits]
readTime: 5 min read
image: https://images.unsplash.com/photo-1454165804606-c3d57bc86b40?w=1400&q=85&auto=format&fit=crop
imageAlt: Notebook and laptop on a desk
---

Working alone changed how I use Git. Without a team to coordinate with, most of the ceremony I used to follow just got in the way.

## Commit Small, Commit Often

Small commits are easier to review later and trivial to revert. I aim for one logical change per commit, with a message that explains the *why*.

## Write the Changelog First

Before starting a feature, I jot a line in the changelog describing what I want to ship. It keeps scope honest and doubles as a to-do list.

## Branches Are Optional

For solo work I mostly commit to `main`. When an idea is risky, a short-lived branch is enough — no long-running feature branches that drift for weeks.

This setup keeps me moving without the overhead.
