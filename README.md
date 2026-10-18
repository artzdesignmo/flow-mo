# Flow Mo — Interactive Fluid Playground

A real-time GPU fluid simulation in the browser. Drag to stir colourful fluid — vortices, mixing, dye advection, all computed live with a Navier-Stokes solver.

**Live demo:** https://artzdesignmo.github.io/flow-mo/

## Features

- **Real fluid dynamics** — GPU Navier-Stokes solver: advection, vorticity confinement, pressure projection (20 Jacobi iterations), gradient subtraction
- **Touch + mouse** — drag to inject velocity and dye; multi-touch supported
- **5 colour palettes** — Neon, Ocean, Sunset, Mono, Candy
- **Tunable** — splat force, swirl (vorticity), dye fade
- **Auto-demo mode** — attract mode that stirs itself
- **PNG capture** — one tap to save the current frame
- Single `index.html`, vanilla JS + WebGL, zero dependencies

## Tech

Classic stable-fluids on the GPU (Stam 2003 / GPU Gems): double-buffered velocity + dye framebuffers, ping-pong advection, curl → vorticity → divergence → pressure → gradient subtraction. Half-float textures where supported.

## Run

Open `index.html` in a browser (WebGL required).

## Part of OpenX

Flow Mo is Project 11 of the [OpenX series](https://openx-mo.vercel.app/) — an open-source lab by [artzdesignmo](https://github.com/artzdesignmo). MIT licensed.

☕ [Buy Me a Coffee](https://buymeacoffee.com/whynotartmoney)
