# Relief Maker

Turn a 2D photo into a 3D-printable relief or lithophane, entirely in your browser.

## Usage

1. Open `index.html` in a modern browser (internet connection needed to load Three.js from a CDN).
2. Drop, browse for, or paste (⌘V / Ctrl+V) an image.
3. Tune the settings — the 3D preview updates live.
4. Click **Download STL**.

No install, no build step, and your images never leave your machine.

## Features

- **Modes**: Relief (light areas raised) or Lithophane (dark areas thick, for backlit prints).
- **Size**: width in mm (height follows the image aspect ratio), base thickness, relief height.
- **Quality**: resolution (0.5–10 px/mm, capped at 1.5M grid points) and detail smoothing.
- **Image adjustments**: brightness, contrast, gamma, invert, mirror.
- **Light/dark transitions**: transition softening (blur in mm) and a max-slope limiter that turns hard steps into even ramps.
- **Frame**: raised border with width/height, plus bevels — chamfer, rounded, cove or ogee profiles, separate outer and inner bevel widths, and adjustable outer bevel depth.
- **Preview**: solid shaded or simulated backlit lithophane view, plus a 2D heightmap.
- **Output**: watertight, outward-facing binary STL in millimetres, ready for any slicer.

## Printing tips

- Relief: ~4 px/mm is plenty.
- Lithophane: white PLA, 100% infill, 0.1–0.12 mm layers, print standing upright.
- Use a max slope of 45–60° to reduce overhangs on high-contrast images.
