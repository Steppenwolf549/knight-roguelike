# Repository Overview

This repository is a minimal, browser-based **knight movement prototype** implemented in a single file: `index.html`.

## What the game currently does

- Opens a 2D canvas (`960x540`) and places a circular knight placeholder in the center.
- Lets the player move that character in real time using:
  - **Keyboard**: `WASD` or arrow keys.
  - **Touch/Pointer**: an on-screen joystick (bottom-left) with a draggable knob.
- Combines keyboard and joystick input into one movement vector and normalizes it so diagonal movement is not faster.
- Updates movement each frame using delta time (`requestAnimationFrame` loop) for smooth, frame-rate-aware motion.
- Keeps the character inside the canvas bounds (no moving off-screen).
- Renders a small line from the character to indicate movement direction (a sword-like direction hint).

## What is included

- `index.html` — complete app (markup, styles, and JavaScript game logic).

## What is not included yet

- No enemies, combat, health system, score, or procedural rooms.
- No asset pipeline or build tooling.
- No package manifest (`package.json`) and no automated tests.
