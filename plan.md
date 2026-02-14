# Divisible by Three — Web App Plan

## Overview
A single-page web app where the user enters a numeric range (start & end) and instantly sees all numbers divisible by 3 within that range.

## Tech Stack
- Plain HTML / CSS / JavaScript (no frameworks, no build step)

## File Structure
```
index.html   — markup, styles, and script (single self-contained file)
```

## UI Layout
1. **Header** — App title: "Divisible by Three"
2. **Input section** — Two number inputs ("Start" and "End") + a "Find" button
3. **Results section**
   - Summary line: "Found X numbers divisible by 3 in range [start, end]"
   - Grid/list of matching numbers, each styled as a pill/badge
4. **Edge-case handling** — Inline validation messages (e.g. start > end, non-numeric input)

## Logic
- On button click (and Enter key), read start/end values
- Validate inputs (both required, must be integers, start <= end, reasonable range cap to avoid browser freeze)
- Loop from start to end, collect numbers where `n % 3 === 0`
- Render results into the results container

## Styling
- Clean, minimal design with a centered card layout
- Responsive (works on mobile)
- Matching numbers displayed as colored badges in a flex-wrap grid

## Deliverables
1. Create `index.html` with all markup, styles, and JS inline
2. Commit and push to `claude/divisible-by-three-app-5edTY`
