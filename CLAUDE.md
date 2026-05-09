# CLAUDE.md
用中文沟通，能用中文的地方都用中文

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

A single-file Pomodoro timer built with pure HTML/CSS/JS. No build tools, no dependencies.

## How to Run

Open `index.html` directly in a browser — no server needed.

## Architecture

Everything lives in `index.html`:
- **CSS** (lines 7-162): Dark theme with SVG circular progress ring
- **HTML** (lines 164-208): Tabs, timer ring, control buttons, pomodoro count
- **JS** (lines 210-348): Timer logic — 25min work / 5min break, localStorage for daily count, browser notifications

Key constants: `WORK = 1500s`, `BREAK = 300s`. Timer uses `setInterval(1000)`. Progress ring driven by `stroke-dashoffset`.
