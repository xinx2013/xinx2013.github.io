# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

This is a static academic lab homepage hosted on GitHub Pages (repo: Stardust-lf/lab-homepage). The site is a Google Sites export — the main `index.html` is a ~2MB single file containing all HTML, CSS, and JavaScript inline (minified/obfuscated Google Sites runtime code).

## Architecture

- **`index.html`** — The entire site in one file, exported from Google Sites. Not hand-written; editing this directly is fragile due to the embedded minified JS/CSS.
- **`Home/`** — Image assets (JPGs) referenced by the site.
- **`CV-Xin.pdf`** — Downloadable CV linked from the site.
- **`PhDrecruit.jpg`** — PhD recruitment poster image.
- **`google84599d35c415955d.html`** — Google Search Console verification file.

## Development

There is no build system, package manager, or test suite. The site is purely static files served by GitHub Pages. Changes are deployed by pushing to the `main` branch.

To preview locally, serve the directory with any static file server (e.g., `python3 -m http.server`).

## Key Considerations

- The `index.html` is a Google Sites export and should not be manually edited for structural changes — re-export from Google Sites instead.
- Image filenames use hash-based names (e.g., `5173cb502327d18cfe5a58bac9a41aaf.jpg`); keep this convention when adding assets.
