# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This repo hosts static HTML pages for 烙馍网 (luomor.com), a content platform run since 2015. The pages serve as the default nginx index page.

## File Structure

| File | Description |
|------|-------------|
| `index.html` | Main intro page — "AI与生活" theme, dark tech aesthetic |
| `index1.html` | Alternate page — 烙馍 food culture theme, warm red/orange palette |
| `docs/log.txt` | Change log from AI sessions |
| `docs/README.md` | Original prompt that generated the pages |
| `centos/` | CentOS default HTML docs (reference material, not part of the site) |

## Development

- **No build step** — pages are plain HTML + inline CSS, no frameworks or dependencies
- **To preview**: open `index.html` directly in a browser, or serve with `python3 -m http.server`
- **To deploy**: commit and push; nginx serves `index.html` from this directory

## Conventions

- Single-file pages with inline `<style>` — no external CSS/JS files
- Pure HTML + CSS, no JavaScript framework or build tooling
- Responsive design with `@media (max-width: 768px)` breakpoints
- Chinese language content (`lang="zh-CN"`)
- Emoji/unicode entities used for decorative icons (e.g., `&#129652;`)
