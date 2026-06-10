# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

Personal GitHub Pages site at `https://jib63.github.io`. Pure static HTML/CSS/JS — no build step, no framework, no dependencies beyond Google Fonts loaded at runtime.

## Structure

```
index.html   — single-page portfolio (hero, projects, photography, footer)
README.md
CLAUDE.md
```

## Deployment

Pushing to `main` triggers the GitHub Pages action automatically. The Pages source must be set to `/ (root)` in repo Settings → Pages (not `/docs`).

## Design tokens

All colors are CSS custom properties on `:root` in `index.html`:

| Variable      | Role                        |
|---------------|-----------------------------|
| `--bg`        | Page background             |
| `--surface`   | Card / section background   |
| `--accent`    | Blue highlight / links      |
| `--purple`    | Secondary accent            |
| `--amber`     | Photography / CTA color     |
| `--muted`     | Secondary text              |

## Key content areas

- **Hero** — GitHub avatar (`avatars.githubusercontent.com/u/29891501`), name, tagline, social buttons (GitHub / LinkedIn / Photography)
- **Projects grid** — 3 cards: CTS Departure (`jib63/CTS_destination`), Reliquum (`jib63.github.io/Reliquum-support/`), JibL (`jib63/JibL`)
- **iOS Apps belt** — 3 cards linking to each app's support landing: Reliquum (`jib63.github.io/Reliquum-support/`), MySoundLibrary (`jib63.github.io/MySoundLibrary-support/en/`), Rekko (`jib63.github.io/Rekko-support/`). Each card has a hand-rolled visual panel (`.card-icon-panel.{reliquum,sound,rekko}`) — keep them in sync if a new app lands.
- **Photography belt** — links to `https://www.jibstudios.com`; the mosaic currently uses Reliquum support screenshots as placeholders — replace `src` attributes with real photo URLs when available
- **Footer** — GitHub, LinkedIn (`linkedin.com/in/jbmeyer63`), JibStudios links
