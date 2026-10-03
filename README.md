# FTM / Compact Toroid Viewer (Mobile)

Mobile-friendly educational viewer for a spinning FTM/FRC-style compact toroid with a co-rotating “hammer” (orange-slice) brightness plane.

**Live:** https://ftm-toroid-viewer-mobile.vercel.app  
**Also:** https://ftm-toroid-viewer-mobile-tkflux.vercel.app  
**Repo:** https://github.com/TkFlux/ftm-toroid-viewer-mobile

Desktop sibling (unchanged): https://ftm-toroid-viewer.vercel.app

## Mobile UX
- Portrait (~390×844) and landscape layouts
- One-finger drag to orbit; pinch / two-finger / wheel zoom (no right-click)
- Collapsible bottom sheet + hamburger Controls FAB (side drawer in landscape)
- ~44px tap targets; large range thumbs; safe-area insets; no hover-only UI
- `touch-action` / overscroll guards so browser scroll does not steal canvas drags
- Same physics/sliders as desktop: spin, tilt, Bin/Bout, R, a, hammer intensity/width, opacity, pause/trails/reset
- Educational disclaimer (not a footage claim)
- Three.js via CDN (r128), single-file app (base64-encoded, gzip-compressed HTML in `viewer.b64`; `index.html` is the thin bootloader that fetches, decodes, and gunzips it)

## Local
From the repository directory, serve `index.html` and `viewer.b64` together over HTTP:

```bash
python3 -m http.server 8080
# then open http://localhost:8080/ in a browser
```
