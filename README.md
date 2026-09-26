# AI-Оператор

**A single-page course landing site that teaches the "80% prompt, 20% code" way of building with AI.**

![Static HTML5](https://img.shields.io/badge/Static-HTML5-E34F26?logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-Vanilla-F7DF1E?logo=javascript&logoColor=black)
![No dependencies](https://img.shields.io/badge/dependencies-none-8fe3c0)
![License MIT](https://img.shields.io/badge/License-MIT-c9a6ff)

[Features](#key-features) · [Tech Stack](#tech-stack) · [Quick Start](#getting-started) · [Project Structure](#project-structure)

---

<div align="center">
  <img src=".github/hero.png" alt="AI-Оператор landing page preview" width="800">
</div>

---

## Key Features

- 🎯 **80/20 Formula Visualizer** — an animated ratio bar that fills from 0 to 80%/20% the moment it scrolls into view, built with a CSS `scaleX` transition triggered by an `IntersectionObserver` (no animation libraries).
- 🐙 **Otto the Mascot** — a hand-coded interactive SVG octopus. Its pupils track the cursor in real time (`atan2`/`hypot` math on `mousemove`), and its tentacles/head shift into a faster "excited" animation on hover — all gracefully disabled for `prefers-reduced-motion`.
- 🔄 **5-Step Daily Pipeline** — a horizontal step diagram connected by a CSS gradient line, implemented with plain CSS Grid, which collapses into a vertical timeline on mobile via a single media query.
- ⚖️ **Good Prompt vs. Bad Prompt Comparison** — a side-by-side breakdown of a weak prompt versus a well-structured one, with hand-styled syntax highlighting (`role` / `string` / `comment` token classes) — no highlighting library involved.
- 💡 **Hover-Reveal Coding Basics** — four topic cards that slide up a hidden explanation panel on hover *or* keyboard focus (`:focus-within` + `tabindex`), keeping the effect accessible without a mouse.
- ✨ **Ambient Cursor Effects** — a soft radial "glow" that follows the cursor across the page, plus per-card spotlight highlights driven by mouse position via CSS custom properties, automatically skipped on touch devices and reduced-motion setups.

## Tech Stack

| Technology | Used for |
|---|---|
| HTML5 | Page structure and semantic markup (`index.html`) |
| CSS3 | All styling — custom properties, Grid/Flexbox layout, keyframe animations, responsive media queries |
| Vanilla JavaScript | Scroll reveals, cursor/spotlight effects, Otto's eye-tracking, and the demo signup form — no framework, no build step |
| Google Fonts | `Unbounded`, `Manrope`, `JetBrains Mono` loaded via `<link>` |

There is no backend: the signup form only shows a client-side confirmation message and does not send data anywhere.

## Getting Started

No build tools, no dependencies, no `npm install` — just open the file.

```bash
# 1. Clone the repository
git clone https://github.com/Tonxetyz/AI-Operator.git
cd AI-Operator

# 2. Open it directly in your browser
start index.html      # Windows
# open index.html      # macOS
# xdg-open index.html  # Linux

# ...or serve it locally (recommended for the fonts/animations to behave normally)
npx serve .
```

## Project Structure

```
AI-Оператор/
├── index.html   # The entire landing page — markup, CSS, and JS in one file
├── LICENSE      # MIT license
└── README.md    # This file
```

---

<div align="center">Made with prompt + a little bit of code.</div>
