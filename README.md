# Living Ink

A single-file, browser-based generative art toy. Draw ink strokes that seed a Physarum-style ("slime mold") particle simulation — three competing species chase and flee each other across the canvas, decaying and diffusing into evolving trails that never fully settle.

No build step, no dependencies beyond Three.js (loaded from CDN for the 3D view). Open `living-ink.html` in a browser.

## Features

- **Draw** — mouse/touch strokes seed the living particle simulation
- **Multi-species** — pick red/green/blue; each species chases one and flees another in a 3-way cycle
- **Live controls** — real-time sliders for speed, sensor distance, turn sensitivity, trail persistence, and chase/flee intensity
- **Mic-reactive** — optional microphone input speeds up and brightens the simulation with sound
- **Record & replay** — every stroke is timestamped and can be replayed back exactly
- **Lift to 3D** — snapshot the canvas into an orbit-controllable Three.js point cloud with an animated holographic shimmer shader
- **Export PNG** — save either the 2D canvas or the 3D view
- **Gallery** — save snapshots to a local (`localStorage`) gallery, and fork/continue evolving from any past save, tracking lineage between forks

## Tech

Vanilla JS, Canvas 2D for the simulation, Three.js (ES modules via CDN import map) for the 3D lift and shader. Everything lives in one HTML file.
