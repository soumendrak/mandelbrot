<div align="center">

# Mandelbrot

[![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-Live-brightgreen?style=flat-square)](https://soumendrak.github.io/mandelbrot/)
[![MIT License](https://img.shields.io/badge/License-MIT-blue?style=flat-square)](LICENSE)
[![HTML5](https://img.shields.io/badge/HTML5-%23E34F26?style=flat-square&logo=html5&logoColor=white)](https://html.spec.whatwg.org/)
[![Zero Dependencies](https://img.shields.io/badge/dependencies-0-success?style=flat-square)](https://www.w3.org/TR/html52/)

<!-- Inline SVG logo -->
<svg width="140" height="140" viewBox="0 0 140 140" xmlns="http://www.w3.org/2000/svg">
<rect width="140" height="140" rx="24" fill="#0a0a14"/>
  <circle cx="70" cy="70" r="50" fill="none" stroke="#ff6b35" stroke-width="0.5" opacity="0.3"/>
  <circle cx="70" cy="70" r="40" fill="none" stroke="#d94f1a" stroke-width="0.5" opacity="0.2"/>
  <circle cx="70" cy="70" r="30" fill="none" stroke="#ff6b35" stroke-width="0.5" opacity="0.15"/>
  <circle cx="70" cy="70" r="20" fill="none" stroke="#d94f1a" stroke-width="0.5" opacity="0.1"/>
  <path d="M 70 70 Q 85 50 95 65 Q 105 80 85 90 Q 65 100 60 85 Q 55 70 70 70" fill="#ff6b35" opacity="0.4"/>
  <text x="70" y="128" text-anchor="middle" font-family="sans-serif" font-size="8" fill="#8a8a9a">click to explore</text>
</svg>

**Zoomable, pannable Mandelbrot fractal explorer rendered on HTML canvas.**

**Live:** [https://soumendrak.github.io/mandelbrot/](https://soumendrak.github.io/mandelbrot/)

</div>

---

## Features

- Click to zoom in, Shift+click to zoom out
- Drag to pan around the fractal plane
- Scroll wheel to adjust iteration depth
- Smooth colour gradient (orange → deep blue → black)
- Display of current complex-plane coordinates
- Reset button to return to default view
- Dark theme with orange accent (#ff6b35)

## How It Works

The set is rendered by iterating `z = z² + c` for each pixel in the complex plane, up to a configurable iteration limit. The colour is determined by how many iterations it takes for `|z|` to exceed 2 (the escape radius). A smooth colouring algorithm maps iteration counts to HSL values, producing the gradient. Zoom changes the view boundaries; pan adjusts the centre point.

## Usage

1. Open `https://soumendrak.github.io/mandelbrot/` in any browser.
2. No build step, no installation, no server required.
3. Deploy anywhere — GitHub Pages, Netlify, or any static host.

```bash
git clone https://github.com/soumendrak/mandelbrot.git
# Open index.html directly
```

## License

Licensed under the [MIT License](LICENSE).

---

<p align="center"><sub>Built with ❤️ and zero dependencies</sub></p>
