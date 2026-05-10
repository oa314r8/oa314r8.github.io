# Repository Maintenance Notes

## Purpose

This file provides instructions to AI agents working in this repository so site
updates stay consistent, reviewable, and easy to publish.

## Repository Shape

- `index.html` is the homepage.
- `archive/`, `recipes/`, and `woodworking/` contain public section pages.
- `content/recipes/` stores recipe source markdown used to create published
  recipe pages.
- `assets/` contains shared static media.

## Content Workflow

- Keep the public site as plain static HTML unless the user asks for a build
  system.
- Treat atomic markdown recipes as source material, not final presentation.
- When adding a recipe, create a dedicated page under `recipes/<slug>/index.html`
  and link it from `recipes/index.html`.
- Preserve the established site tone: dark fantasy with cyberpunk accents.

## Editing Rules

- Prefer surgical edits over broad rewrites.
- Keep navigation labels consistent across all pages.
- Maintain mobile-friendly layouts when adding new content blocks.
- Do not remove or overwrite user-authored content unless the request clearly
  calls for it.

## Publish Workflow

- Review `git diff` before committing.
- Commit related changes together with a clear message.
- Push only after the requested site updates are complete.

## Local Agent Notes

- Put any machine-specific or temporary agent notes in `AGENTS.local.md`.
- `AGENTS.local.md` is ignored by Git and should not be committed.
