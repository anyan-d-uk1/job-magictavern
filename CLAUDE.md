# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a static single-page job posting website for a Narrative Designer position at Magic Tavern (麦吉太文). The entire site is contained in a single `index.html` file with no build system, no dependencies, and no package manager.

## Deployment

Hosted via GitHub Pages: https://anyan-d-uk1.github.io/job-magictavern/

## Development

No build step required. Open `index.html` directly in a browser or use any static file server:

```
python3 -m http.server 8000
```

## Architecture

- **Single file**: All HTML, CSS, and JavaScript live in `index.html` (~479 lines)
- **CSS**: Inline `<style>` block using CSS custom properties (`:root` variables) for a candy-themed color palette
- **Fonts**: Google Fonts (Baloo 2, Noto Sans SC, Quicksand) loaded via CDN
- **JavaScript**: Minimal inline script for scroll-based reveal animations using IntersectionObserver
- **Bilingual**: Content is in both English and Chinese (Simplified)
- **No external assets checked in**: Images referenced via external URLs
