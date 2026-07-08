# Nehru Timeline

An elegant, interactive historical timeline chronicling 15 major milestones in the life of Jawaharlal Nehru. This project serves as a practical implementation of interactive UI design patterns built strictly with pure HTML5 and CSS3—requiring absolute zero JavaScript runtime overhead.

## Overview & Value Proposition

Most interactive accordion components rely heavily on JavaScript event listeners to toggle classes and animate heights. This introduces script parsing penalties, potential layout shifts, and execution delays. 

This repository demonstrates a lightweight, highly responsive design alternative. By repurposing native HTML radio inputs and exploiting the CSS adjacent sibling combinator (`~`), interactive accordion states are handled entirely by the browser’s native rendering engine. It's resilient, extremely fast to paint, and infinitely accessible.

## Key Features

* **Zero-JS State Engine:** Toggle sections smoothly without a single line of script running in the browser execution thread.
* **Pure CSS Transitions:** Fluid expand and collapse animations using managed max-height transitions.
* **Fluid Vertical Spine Layout:** Responsive UI design featuring smart visual blending between headers and content blocks.
* **Production-Ready Hosting:** Pre-configured for automatic delivery via GitHub Pages.

## Tech Stack Breakdown

* **Markup:** HTML5 utilizing semantic structural elements.
* **Styling:** CSS3 variables, transitions, Flexbox layout models, and state pseudoclasses (`:checked`).
* **Automation:** GitHub Actions for static validation linting.

## Quick Start (Web-Based Setup)

You don't need to clone this repo locally to run or modify it. You can spin it up directly in your browser.

1. At the top right of this repository page, click the **Code** dropdown button.
2. Select the **Codespaces** tab.
3. Click **Create codespace on main**.
4. Once the environment initializes, click **Go Live** on the status bar or run a quick static preview server to review modifications instantly.

### Local Alternative
If you prefer traditional local execution, simply download the source files and run:
```bash
# Open directly via terminal on macOS/Linux
open index.html
```

## Project Structure
```bash
├── .gitignore          # Excludes environment and OS artifacts
├── README.md           # Documentation
├── index.html          # Semantic structure and historical copy
└── style.css           # Grid architecture, spine rules, and state engine
```

## Roadmap
[ ] Accessibility (a11y) Enhancements: Improve keyboard navigation profiles for radio-driven state triggers.

[ ] Media Integration: Add lightweight, highly compressed historical images for each interactive item block.

[ ] Dark Mode Support: Implement an adaptive, query-based CSS color scheme palette switch.
