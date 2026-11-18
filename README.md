# The Floor Test: Indian parliamentary majority simulator

> The Floor Test: an interactive simulator that teaches Indian parliamentary majorities and floor tests through concept cards, a voting game and timed problems.

**[Live site](https://axomrank.github.io/floor-test-simulator/)** · [Part of AxomRank](https://github.com/axomrank)

## At a glance

- **Learn:** concept cards and a live chart. Adjust total strength, vacancies and absentees to see the threshold change
- **Play:** drag party blocs into Aye or Nay and check the result against the constitutional rule
- **Examine:** timed word problems (25 seconds each) with worked explanations
- **Progress** (XP, ranks from Backbencher to Prime Minister) is saved in `localStorage`. Single page, vanilla JS

## Quick start

```bash
python3 -m http.server 8000   # open http://localhost:8000
```

## Overview

An interactive, responsive, single-page educational web application designed to help candidates mastering high-stakes Indian competitive exams (e.g., UPSC CSE) understand the mathematical formulas and operational mechanics of parliamentary floor tests.

## Features

1. **Architecture & State Management**: 
   - SPA implementation in vanilla HTML5, CSS3, and JavaScript.
   - Persistent `localStorage` tracking of User XP, unlocked chapters, and dynamic ranks (ranging from **Backbencher** to **Prime Minister**).
   - Sidebar drawer containing chapter unlock controls and progress resets.

2. **Phase 1: Learn Interface**:
   - Tinder-style swipeable/clickable concept cards breaking down definitions.
   - Professional interactive visualization (rendered on HTML5 Canvas) mimicking Python Seaborn/R-Studio output formats.
   - Real-time sliders allowing adjustment of **Total Strength**, **Vacancies**, and **Absentees**, which dynamically recalculate and map passing thresholds.
   - Cinematic horizontal scrolling historical case timelines (e.g., the 1956 States Reorganisation Act, GST Act passage, etc.).

3. **Phase 2: Play Simulator**:
   - HTML5 Drag and Drop division lobby.
   - Drag political factions representing specific block voting strengths (e.g., Ruling Coalition, Opposition, Independents) into **Aye** or **Nay** zones.
   - Immediate mathematical validation against specific constitutional thresholds on submit.

4. **Phase 3: Examine Module**:
   - High-rigor, multi-variable constitutional word problems matching top-tier competitive level examinations.
   - Time-attack logic with a strict 25-second countdown timer.
   - Automatically provides detailed legal remedy formula analysis and deducts/adds XP dynamically based on results.

## Layout and Styling
- Modern, institutional aesthetics featuring Deep Navy (`#1a365d`), Gold (`#c59b27`), and Crisp White (`#ffffff`).
- Fully mobile-responsive flex and grid setups.
- Glassmorphism textures and fluid state transitions.

## How to Run locally on Ubuntu
You can host the application using any local web server. For convenience, a Python server is active:

1. Open your terminal in the workspace directory.
2. Run the server:
   ```bash
   python3 -m http.server 8000
   ```
3. Open your browser and navigate to:
   [http://localhost:8000](http://localhost:8000)

## Roadmap: future improvements

- [ ] Fold it into the AxomRank Indian Polity course as an interactive lesson
- [ ] Add Assamese text
- [ ] Add Assam Legislative Assembly scenarios (126 seats)
- [ ] Add an accessibility pass: keyboard drag-and-drop alternative, colour contrast
- [ ] Check each worked answer against the Constitution's articles

## For AI agents and contributors

Read [AGENTS.md](AGENTS.md) and [CONTEXT.md](CONTEXT.md) for the state model and coding rules.

Commit as the `axomrank` account. Keep changes small and reviewable, and run the repository's checks before pushing.

## Part of AxomRank

[AxomRank](https://axomrank.pages.dev) offers free, bilingual preparation for Assam government exams. Related repositories:

- **Learn:** [axomrank.github.io](https://github.com/axomrank/axomrank.github.io) (the AxomRank learning app)
- **Explore Assam history:** [ahom-kingdom-history](https://github.com/axomrank/ahom-kingdom-history) (illustrated Ahom kingdom website and 41 reign lessons), [assam-history-map](https://github.com/axomrank/assam-history-map) (year-by-year historical map), [assam-history-characters](https://github.com/axomrank/assam-history-characters) (character sheets for Assam's history), [assam-visual-archive](https://github.com/axomrank/assam-visual-archive) (gallery of Assam scenes and photographs), [assam-heritage-ai-art](https://github.com/axomrank/assam-heritage-ai-art) (AI art gallery of Assamese heritage)
- **Open data:** [assam-exam-pyq](https://github.com/axomrank/assam-exam-pyq) (2,398 previous-year questions with answers), [assam-exam-syllabus](https://github.com/axomrank/assam-exam-syllabus) (syllabi for 12 recruitment boards), [assam-maps](https://github.com/axomrank/assam-maps) (map portal and GIS layers), [assam-history-sources](https://github.com/axomrank/assam-history-sources) (Kamarupa inscriptions and primary sources)
- **Publishing and brand:** [axomrank-blog](https://github.com/axomrank/axomrank-blog) (exam guides built from real papers), [assam-history-books](https://github.com/axomrank/assam-history-books) (13-book history of Assam), [axomrank-brand-assets](https://github.com/axomrank/axomrank-brand-assets) (brand kit and social media library)

## License and contact

No license file yet, so all rights are reserved by default.

Corrections and questions: open an issue in this repository. AxomRank is run by Angsuman Das (sole proprietor).
