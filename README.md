[![Netlify Status](https://api.netlify.com/api/v1/badges/2353da50-0f7e-4634-b443-32b6e0a557c3/deploy-status)](https://app.netlify.com/projects/makeqr/deploys)


# [QR Code Generator | Version 2.0.0](qr.junglestar.org)

A lightweight, single-file QR code generator that creates both SVG and PNG downloads. No backend, no dependencies (well we embed qrcode.js, hum... at build time!). Just pure, efficient client-side magic.

## Features

- Crazy annoying UltraGreen, so you get a dopamine boost.
- Generate QR codes from any text or URL
- Download as optimized SVG (tiny file size thanks to horizontal bar compression)
- Download as high-res PNG (1000x1000px)
- Clean, modern UI with that sweet green aesthetic
- Works completely offline (after first load)
- Press Enter to generate

## Why Another QR Generator?

Because sometimes you need a tool that just works, doesn't track you, doesn't require sign-up, and fits in a single HTML file. Also because we can't help ourselves.

## Technical Bits

- Uses QRCode.js for generation (embedded)
- Custom canvas-to-SVG converter that creates horizontal bars instead of individual pixels
- Result: ~20-50KB SVGs
- OKLCH color space for that UltraGreen `oklch(0.8353 0.3231 148.24)` that sickens your retina

## Usage

1. Open `index.html` in any modern browser
2. Type or paste your text/URL
3. Hit Generate (or press Enter)
4. Download as SVG or PNG
5. Use your QR code to confuse people at parties

---

Built by JUNGLESTAR | TOYBREAKER with 💚 and an unhealthy obsession for scratching own hitches and coding your own tools.

Not responsible for existential crises caused by discovering QR codes were not a passing fad.

You can help us make more useful WEBAPP TOYS like this one by either:

[Report a Bug](https://github.com/junglesta/qr.junglestar.org/issues) | [Buy Us Coffee](https://ko-fi.com/junglo)
