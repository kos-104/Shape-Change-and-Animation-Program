# Excel VBA Shape Animator

**A checkbox-driven 3D animation demo for Excel — proving that Excel is capable of far more than spreadsheets.**

![VBA](https://img.shields.io/badge/Language-VBA-blue.svg)
![Excel](https://img.shields.io/badge/Platform-Excel-217346.svg)
![Animation](https://img.shields.io/badge/Feature-3D%20Rotation-brightgreen.svg)

## Description

Most people think of Excel as a grid for numbers. This project was built to challenge that assumption — showing that, backed entirely by VBA, Excel can render live 3D graphics, gradient fills, and animation using nothing but its own native shape engine. No add-ins, no external libraries — just Excel pushed a bit further than most people realize it can go.

Users generate shapes from dropdown selections, style them with randomized gradient fills, and animate them through seven rotation modes — X, Y, Z, and combinations of all three — controlled by a simple set of checkboxes.

A dedicated class handles shape creation: picking shape type and gradient style from dropdowns, sizing shapes by preset, percentage, or worksheet-derived dimensions, and validating percentage input as it's typed in — auto-correcting out-of-range or negative values along the way. A separate module handles the animation itself, applying 3D depth, shadow effects, and randomized color shifts frame by frame, with a simple stop button to interrupt a running animation at any time.

This was built as a passion project, meant to be a fun, visual reminder that Excel can be genuinely playful when you push past its default look and feel.

## Key Features

- Dropdown-driven shape and gradient-fill generation, with live input validation and auto-correction
- Randomized 3-stop gradient fills and a consistent rotate-and-flip style applied to every shape
- Seven checkbox-selectable 3D rotation modes (single, dual, and full triple-axis)
- Dynamic shadow and extrusion effects that shift with
