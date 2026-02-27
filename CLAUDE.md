# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project

Personal academic website for Paul Michel, hosted on GitHub Pages at paulmichel0.github.io.

## Architecture

This is a pure static site with no build tools, no JavaScript, and no dependencies.

- `index.html` — The entire site. Single-page layout with a fixed sidebar (identity, contact, links) and a scrollable main content area (bio, current projects, publications).
- `cv/cv-michel.pdf` — Downloadable CV linked from the sidebar.
- All CSS is inline in `<style>` within `index.html`.

## Development

No build or test commands. Edit `index.html` directly and push to `main` to deploy via GitHub Pages.

## Conventions

- Keep everything in a single `index.html` file with inline CSS — do not extract CSS to separate files or add JavaScript unless explicitly requested.
- The sidebar is fixed at 250px width; main content is offset with `margin-left: 270px`.
- All external links use `target="_blank"` with `rel="noopener noreferrer"`.
- Google Search Console is verified via meta tag — do not remove the `google-site-verification` meta tag.
