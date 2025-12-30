# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Overview

QR Code Generator - a lightweight, single-file web app that generates QR codes with SVG and PNG download options. Deployed on Netlify at qr.junglestar.org.

## Architecture

This is a zero-build, static site with everything in a single HTML file:

- **index.htm** - The entire application (HTML + CSS + JS inline)
- **qrcode.min.js** - QRCode.js library (git submodule from `qrcodejs/`)

Key technical details:
- Uses QRCode.js to generate QR codes on canvas
- Custom `canvasToSVG()` function converts canvas to optimized SVG using horizontal bar compression (not individual pixels)
- PNG export at 1000x1000px with disabled image smoothing for crisp scaling
- Brand color: `oklch(0.8353 0.3231 148.24)` (UltraGreen)

## Development

No build step required. Open `index.htm` directly in a browser or use any local server:

```bash
python -m http.server 8000
# or
npx serve
```

## Deployment

Automatic deployment via Netlify on push to `source` branch.

## Git Structure

- Main branch: `source`
- qrcodejs is a git submodule
