# Excel VBA Shape Animator

**A checkbox-driven 3D animation demo for Excel — proving that Excel is capable of far more than spreadsheets.**

![VBA](https://img.shields.io/badge/Language-VBA-blue.svg)
![Excel](https://img.shields.io/badge/Platform-Excel-217346.svg)
![Animation](https://img.shields.io/badge/Feature-3D%20Rotation-brightgreen.svg)
![Dependencies](https://img.shields.io/badge/Dependencies-None-lightgrey.svg)

![Demo](docs/demo.gif)

## Description

Most people think of Excel as a grid for numbers. This project was built to challenge that assumption — showing that, backed entirely by VBA, Excel can render live 3D graphics, colorful shading, and animation using nothing but its own native shape engine.

Users generate shapes from dropdown selections, give them a randomized color blend, and set them spinning through seven rotation modes — controlled by a simple set of checkboxes. Shape creation lives inside a dedicated class module that listens for worksheet events, reacting live as the user changes a dropdown or types into a cell. A separate module handles the animation itself, adding depth and shadows to make shapes feel three-dimensional, shifting their colors frame by frame, with a simple stop button to interrupt a running animation at any time.

This was built as a passion project, meant to be a fun, visual reminder that Excel can be genuinely playful when you push past its default look and feel.

## Key Features

**Shape Creation**
- Pick a shape from a dropdown list — circles, stars, arrows, and more — no drawing required
- Every shape gets a randomized, multi-color blend fill, so no two shapes look exactly alike
- Choose how big the shape should be: a fixed size, a percentage you type in, or dimensions pulled straight from cells on the worksheet
- Type a percentage into a cell and the sheet checks it for you, correcting out-of-range or negative values automatically

**Animation**
- Seven spinning modes, toggled with checkboxes — spin on one axis, two at once, or all three together for a full tumbling effect
- Shading and shadow effects that make the spin look genuinely three-dimensional instead of flat
- Colors shift a little on every frame, so the animation never looks static or repetitive
- Start and stop the animation with a click, with no freezing or waiting
- Toggle between "video" and regular Excel view with a single button

**Under the Hood**
- Shape creation is built as a lightweight object-oriented model — a self-contained class module that responds directly to worksheet events
- Shape creation and animation are kept in separate pieces of code, keeping event-driven logic and animation logic cleanly apart

## Requirements
- Excel with macros enabled (developed and tested on Excel 365)
- No external references or add-ins required

## How to Use
1. Open the provided `.xlsm` file
2. Follow the on-screen instructions provided directly on the Excel sheet

---
*Built to prove that Excel still has surprises left in it.*
