# Working on floor-test-simulator

Single-page simulator for Indian parliamentary majorities. Part of AxomRank: see README.md for the overview and roadmap.

## Layout

- `index.html`: structure
- `style.css`: design system
- `app.js`: all data, state, rendering and game logic
- `CONTEXT.md`: full architecture and coding rules

## Commands

- `python3 -m http.server 8000`

## Rules

- State lives in one `state` object, persisted to `localStorage` under `floor_test_state`
- Check every constitutional rule against the article it cites before changing the problems
- Keep it dependency-free (vanilla HTML, CSS and JS)
- Commit as the `axomrank` account, in small reviewable commits.
