# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview
A browser-based game collection built as single-file HTML apps with embedded CSS and JS. No frameworks, no build tools, no dependencies.

## Development
- Open `.html` files directly in a browser to test (`open index.html` on macOS)
- No build step, package manager, or dev server required

## Pre-Commit Rule (MANDATORY)
**Always run `/code-review` before any `git commit`.** Do not commit if the review verdict is BLOCKED (any BLOCKER-severity issues remain). Resolve all BLOCKERs first, then re-run `/code-review` to confirm the verdict is APPROVED before committing.

## Games
- `index.html` — TicTacToe: two-player game with X/O neon styling
- `saibaba.html` — Sai Baba Oracle: yes/no oracle with golden glow, blessing quotes, and particle effects

## Design Conventions
- Dark gradient background (`#0f0c29` → `#302b63` → `#24243e`)
- Neon glow effects on interactive elements (red `#ff6b6b` for X, cyan `#48dbfb` for O)
- Fixed **800x600** `.game-container` wrapping all game content
- Single-file architecture: all HTML, CSS, and JS in one `.html` file per game
