# Excel VBA Shape Animator

**A checkbox-driven 3D animation demo for Excel — proving that Excel is capable of far more than spreadsheets.**

![VBA](https://img.shields.io/badge/Language-VBA-blue.svg)
![Excel](https://img.shields.io/badge/Platform-Excel-217346.svg)
![Animation](https://img.shields.io/badge/Feature-3D%20Rotation-brightgreen.svg)

## Description

Most people think of Excel as a grid for numbers. This project was built to challenge that assumption — showing that, backed entirely by VBA, Excel can render live 3D graphics, colorful shading, and animation using nothing but its own native shape engine. No add-ins, no external libraries — just Excel pushed a bit further than most people realize it can go.

Users generate shapes from dropdown selections, give them a randomized color blend, and set them spinning through seven different rotation modes — controlled by a simple set of checkboxes.

A dedicated class handles shape creation: picking shape type and color-blend style from dropdowns, sizing shapes by preset, percentage, or worksheet-derived dimensions, and validating percentage input as it's typed in — auto-correcting out-of-range or negative values along the way. A separate module handles the animation itself, adding depth and shadows to make shapes feel three-dimensional, shifting their colors frame by frame, with a simple stop button to interrupt a running animation at any time.

This was built as a passion project, meant to be a fun, visual reminder that Excel can be genuinely playful when you push past its default look and feel.

## Key Features

**Shape Creation**
- Pick a shape from a dropdown list — circles, stars, arrows, and more — no drawing required
- Every shape gets a randomized, multi-color blend fill, so no two shapes look exactly alike
- Choose how big the shape should be: a fixed size, a percentage you type in, or dimensions pulled straight from cells on the worksheet
- Type a percentage into a cell and the sheet checks it for you — numbers over 100% get capped, and negative numbers get automatically corrected with a note explaining why

**Animation**
- Seven different spinning modes, turned on and off with checkboxes — spin on one axis, two at once, or all three together for a full tumbling effect
- Shapes get shading and shadow effects that make the spin look genuinely three-dimensional instead of flat
- Colors shift and blend a little on every frame, so the animation never looks static or repetitive
- Click a button to start the animation, and click again to stop it cleanly at any moment — no freezing, no waiting

**Under the Hood**
- Shape creation and animation are handled by separate, self-contained pieces of code, keeping the logic organized and easy to follow
- All the animation timing, colors, and sizing rules are defined in one place, making the whole thing easy to adjust or extend
