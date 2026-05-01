<div align="center">

# ArtiGuide

**Dark tech-style showcase framework | For project defense, product launch, tech demo**

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)
![License](https://img.shields.io/badge/License-MIT-blue.svg)

English | **[中文](./README.md)**

</div>

---

## Features

- Particle animation background (interactive)
- Cursor glow + 3D card tilt effects
- Tab switching + scroll-triggered animations
- PPT slideshow fullscreen display
- Responsive design, mobile-friendly

## Quick Start

```bash
git clone https://github.com/zgy123454zgy-afk/arti-guide-showcase.git
```

Open `perform.html` in your browser.

## Configure PPT

1. Export PPT as images (PNG/JPG), place in `./ppt/` folder
2. Update config in `perform.html`:

```javascript
const PPT_TOTAL = 10;           // Total image count
const PPT_PATH = './ppt/';      // Image path
const PPT_IMAGES = [];          // Optional: custom filename array
```

> See [`ppt/README.md`](./ppt/README.md) for details.

## Customize

**Theme colors** - modify CSS variables:
```css
:root {
    --accent-glow: #d4a843;   /* Primary accent */
    --accent-purple: #2e8b57; /* Secondary accent */
}
```

**Content** - modify `dataSources` and `features` arrays in JavaScript.

## Tech Stack

| Library | Purpose |
|---------|---------|
| [tsparticles](https://particles.js.org/) | Particle animation |
| [GSAP](https://greensock.com/gsap/) + ScrollTrigger | Animation engine |
| [VanillaTilt](https://micku7zu.github.io/vanilla-tilt.js/) | 3D tilt effect |

## Browser Support

Chrome 80+ · Firefox 75+ · Safari 13+ · Edge 80+

## Deploy

**GitHub Pages:** Settings → Pages → Branch: main → Save

**Local server:**
```bash
python -m http.server 8080
```

## License

[MIT License](./LICENSE)
