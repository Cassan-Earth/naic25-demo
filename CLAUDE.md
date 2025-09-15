# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a simple static website project that displays PDF slides and video content. The project structure consists of:

- `index.html` - Main HTML file that displays a PDF document and video player
- `assets/` - Directory containing static assets:
  - `CassanLogo.png` - Logo image
  - `slides.pdf` - PDF document displayed on the page
  - `video.mp4` - Video file displayed on the page
- `CNAME` - Empty file for custom domain configuration

## Architecture

This is a static HTML website with no build process or dependencies. The site uses:

- Vanilla HTML with embedded CSS
- Native browser PDF viewer via `<object>` tag
- HTML5 video player for MP4 content
- Responsive design with system fonts

## Development

Since this is a static site with no build tools:

- No package.json, build scripts, or dependencies
- No linting, testing, or compilation steps required
- Changes can be made directly to HTML/CSS
- Static assets are served directly from the `assets/` directory

## Deployment

The presence of a `CNAME` file and `.gitignore` with Next.js/Vercel patterns suggests this may be deployed to GitHub Pages or a similar static hosting service, though the actual deployment configuration is not present in this repository.