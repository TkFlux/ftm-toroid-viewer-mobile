# FTM / Compact Toroid Viewer (Mobile)

Mobile-friendly educational geometry sketch of a fractal-toroidal / FRC-style envelope with a co-rotating “hammer” (orange-slice) brightness plane.

**Not a claim about any footage** — interactive plasma vocabulary toy for phones.

## Features

- Portrait (~390×844) and landscape layouts
- One-finger drag to orbit, pinch / two-finger / wheel to zoom
- Collapsible bottom-sheet controls (side drawer in landscape)
- Large tap targets (~44px+) and thumb-friendly sliders
- Safe-area padding for notched phones
- Same physics/geometry as the desktop viewer

## Run locally

Open `index.html` in a browser, or:

```bash
python3 -m http.server 8765
```

## Tech

Single-file HTML + Three.js (cdnjs r128).
