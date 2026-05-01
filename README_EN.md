<div align="center">

# ArtiGuide · 文物智鉴

### Dark Tech-Style Showcase Page Framework

**For Project Defense · Product Launch · Technical Demo · Portfolio Display**

<br>

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-ES6+-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![GSAP](https://img.shields.io/badge/GSAP-3.12-88CE02?style=for-the-badge&logo=greensock&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-007ACC?style=for-the-badge)
![Stars](https://img.shields.io/github/stars/zgy123454zgy-afk/arti-guide-showcase?style=for-the-badge)
![Forks](https://img.shields.io/github/forks/zgy123454zgy-afk/arti-guide-showcase?style=for-the-badge)

<br>

English | **[中文](./README.md)**

<br>

![demo](https://img.shields.io/badge/🎬_Live_Demo-GitHub_Pages-238636?style=for-the-badge&logo=github)
![download](https://img.shields.io/badge/📦_Download-ZIP-007ACC?style=for-the-badge&logo=github)

</div>

---

## 📑 Table of Contents

- [Introduction](#-introduction)
- [Key Features](#-key-features)
- [Preview](#-preview)
- [Quick Start](#-quick-start)
- [Project Structure](#-project-structure)
- [Usage Guide](#-usage-guide)
  - [Modify Page Content](#1-modify-page-content)
  - [Configure PPT Slideshow](#2-configure-ppt-slideshow)
  - [Customize Theme](#3-customize-theme)
  - [Modify Particle Effects](#4-modify-particle-effects)
  - [Modify Navigation](#5-modify-navigation)
- [Tech Stack](#-tech-stack)
- [Browser Compatibility](#-browser-compatibility)
- [Deployment Guide](#-deployment-guide)
- [FAQ](#-faq)
- [Changelog](#-changelog)
- [Contributing](#-contributing)
- [License](#-license)
- [Acknowledgements](#-acknowledgements)
- [Contact](#-contact)

---

## 📖 Introduction

**ArtiGuide** is a meticulously designed dark-themed showcase page framework, built for scenarios that require high-quality visual presentation.

### Use Cases

| Scenario | Description |
|----------|-------------|
| 🎓 Project Defense | Graduation projects, course projects, research presentations |
| 🚀 Product Launch | New feature announcements, version updates |
| 💻 Tech Demo | Technical sharing, architecture design showcase |
| 🎨 Portfolio | Designer and developer portfolio display |
| 📊 Data Report | Data analysis visualization |
| 🏢 Corporate Site | Product landing page, company introduction |

### Why Choose This Framework?

- **Ready to Use** - Single file architecture, no dependencies to install
- **Highly Customizable** - All content, styles, and animations are easy to modify
- **Professional Visuals** - Particle animations, 3D cards, smooth transitions
- **Responsive Design** - Perfect adaptation from mobile to desktop
- **Zero Learning Curve** - Clean code structure with comprehensive comments

---

## ✨ Key Features

### Visual Effects

| Feature | Description | Technology |
|---------|-------------|------------|
| Particle Background | Dynamic particle network with mouse interaction | tsparticles 2.12 |
| Cursor Glow | Soft glow following mouse movement | JavaScript + CSS |
| 3D Card Tilt | Cards tilt in 3D on hover | VanillaTilt.js |
| Card Breathing | Slow pulsing glow on card borders | CSS Animation |
| Shine Sweep | Light sweep across card surface on hover | CSS Transform |
| Number Counter | Statistics animate from 0 to target value | GSAP |

### Interactive Features

| Feature | Description | Technology |
|---------|-------------|------------|
| Tab Switching | Smooth content switching with particle color change | GSAP |
| Spotlight Effect | Other cards dim when hovering one card | CSS + JavaScript |
| Scroll Animations | Elements animate in as they enter viewport | ScrollTrigger |
| PPT Slideshow | Fullscreen presentation mode | JavaScript |
| Back to Top | Auto-show on scroll, smooth scroll to top | JavaScript |
| Button Ripple | Expanding ripple effect on button click | CSS Animation |

### Layout Design

| Feature | Description |
|---------|-------------|
| Responsive Grid | Auto-adapting card grid layout |
| Sticky Navigation | Fixed top navigation on scroll |
| Scroll Indicator | Bouncing arrow at page bottom |
| Glassmorphism | Semi-transparent blurred backgrounds |

---

## 🎬 Preview

> 💡 **Tip:** Add project screenshots or GIF demos here

<!-- 
### Hero Section
![Hero Preview](./screenshots/hero.png)

### Card Effects
![Cards Preview](./screenshots/cards.png)

### PPT Slideshow
![PPT Preview](./screenshots/ppt.png)

### Mobile View
![Mobile Preview](./screenshots/mobile.png)
-->

**How to add preview screenshots:**

1. Create a `screenshots` folder in the project root
2. Place your screenshots in the folder
3. Uncomment the lines above and update image paths

---

## 🚀 Quick Start

### Option 1: Direct Download (Recommended for Beginners)

```
1. Click the green [Code] button at the top of the page
2. Select [Download ZIP]
3. Extract the downloaded file
4. Open perform.html in your browser
```

### Option 2: Git Clone

```bash
# Clone the repository
git clone https://github.com/zgy123454zgy-afk/arti-guide-showcase.git

# Enter project directory
cd arti-guide-showcase

# Open in browser (Windows)
start perform.html

# Open in browser (Mac)
open perform.html

# Open in browser (Linux)
xdg-open perform.html
```

### Option 3: GitHub Pages Deployment

```bash
# 1. Fork this repository to your account
# 2. Go to your forked repository
# 3. Settings → Pages
# 4. Source: Deploy from a branch
# 5. Branch: main, Folder: / (root)
# 6. Click Save
# 7. Wait 1-2 minutes, visit: https://<your-username>.github.io/arti-guide-showcase/
```

### Option 4: Local Server

```bash
# Using Python
python -m http.server 8080

# Using Node.js (requires http-server)
npx http-server -p 8080

# Using PHP
php -S localhost:8080

# Then visit http://localhost:8080
```

---

## 📁 Project Structure

```
arti-guide-showcase/
│
├── perform.html                # Main page file (HTML + CSS + JavaScript)
│   │
│   ├── <style>                 # All CSS styles
│   │   ├── Variables           # :root CSS Variables
│   │   ├── Layout              # Grid, Flexbox
│   │   ├── Components          # Cards, Buttons, Navigation
│   │   ├── Animations          # @keyframes
│   │   └── Responsive          # @media queries
│   │
│   ├── <body>                  # HTML structure
│   │   ├── Navigation          # Top navigation bar
│   │   ├── Hero                # Landing section
│   │   ├── Highlights Banner   # Scrolling highlight banner
│   │   ├── Tab Switcher        # Tab switcher
│   │   ├── Content Panels      # Content panels
│   │   ├── PPT Modal           # PPT modal dialog
│   │   └── Footer              # Page footer
│   │
│   └── <script>                # JavaScript logic
│       ├── Data Definition     # dataSources, features
│       ├── Animation Init      # GSAP, tsparticles
│       ├── Interaction Logic   # Tab, Filter, PPT
│       └── Utility Functions   # Helpers
│
├── ppt/                        # PPT images directory
│   ├── 1.png                   # Slide 1
│   ├── 2.png                   # Slide 2
│   ├── ...                     # More slides
│   └── README.md               # PPT configuration guide
│
├── screenshots/                # Project screenshots (optional)
│   ├── hero.png
│   ├── cards.png
│   └── mobile.png
│
├── .gitignore                  # Git ignore rules
├── LICENSE                     # MIT License
├── README.md                   # Chinese documentation
└── README_EN.md                # English documentation (this file)
```

### Design Philosophy

> **Single File Architecture**
> 
> This project integrates all code in a single HTML file. This is an intentional design choice:
> - ✅ Easy to share - Just one file needed
> - ✅ Easy to deploy - Upload to any static server
> - ✅ Easy to understand - All code in one place
> - ✅ No build tools - No npm, webpack, etc. needed
> 
> Feel free to refactor into multiple files if needed.

---

## 📘 Usage Guide

### 1. Modify Page Content

#### Change Website Title

```html
<!-- In <head> -->
<title>Your Project Name | Your Project Tagline</title>

<!-- In navigation bar -->
<div class="logo">Your Project Name</div>
```

#### Modify Hero Section

```html
<header class="hero" id="hero">
    <!-- Main title - supports two lines -->
    <h1 id="hero-title">
        <span>First Line Title</span>
        <span class="highlight">Second Line (Highlighted)</span>
    </h1>
    
    <!-- Description -->
    <p id="hero-desc">Your project description, recommended 100-200 words...</p>
    
    <!-- Statistics -->
    <div class="hero-stats" id="hero-stats">
        <div class="hero-stat">
            <div class="num" data-target="1000">0</div>
            <div class="label">Metric 1</div>
        </div>
        <div class="hero-stat">
            <div class="num" data-target="50">0</div>
            <div class="label">Metric 2</div>
        </div>
        <div class="hero-stat">
            <div class="num" data-target="100">0</div>
            <div class="label">Metric 3</div>
        </div>
        <div class="hero-stat">
            <div class="num" data-target="5000">0</div>
            <div class="label">Metric 4</div>
        </div>
    </div>
</header>
```

#### Modify Highlight Banner

```html
<div class="highlights-track" id="highlights-track">
    <span class="highlight-item">
        <span class="dot"></span>
        Your highlight text <strong>key point</strong>
    </span>
    <!-- Duplicate items for seamless scrolling -->
</div>
```

#### Modify Data Cards

```javascript
// Find and modify in the JavaScript section

const dataSources = [
    {
        name: "Card Title",           // Displayed at top-left
        field: "Category Tag",        // Displayed at top-right
        desc: "Card description...",  // Middle description
        tags: ["Tag1", "Tag2"],       // Bottom tags
        url: "https://..."            // Button link
    },
    // Add more cards...
];

const sourceCategories = ["All", "Category1", "Category2", "Category3"];

const features = [
    // Same structure...
];

const featureCategories = ["All", "CategoryA", "CategoryB", "CategoryC"];
```

#### Modify Navigation Links

```html
<nav>
    <div class="logo">ArtiGuide</div>
    <div class="nav-links">
        <a onclick="switchTab('sources')">Data Sources</a>
        <a onclick="switchTab('features')">Core Features</a>
        <a onclick="openPPT()">PPT Slides</a>
        <a href="https://github.com/..." target="_blank">GitHub</a>
    </div>
</nav>
```

#### Modify Footer

```html
<div class="footer">
    <p>&copy; 2026 <strong>Your Project Name</strong> — Your project description</p>
    <p style="margin-top: 8px; font-size: 12px;">
        Tech1 · Tech2 · Tech3
    </p>
</div>
```

---

### 2. Configure PPT Slideshow

#### Basic Configuration

```javascript
// Find in perform.html JavaScript section:

// ========== PPT Configuration ==========
const PPT_TOTAL = 17;              // ← Change to your total slide count
const PPT_PATH = './ppt/';         // ← Image path
const PPT_IMAGES = [];             // ← Optional: custom filename array
// ========== End Configuration ==========
```

#### Using Default Naming (Recommended)

Name images as `1.png`, `2.png`... and place in `ppt` folder:

```javascript
const PPT_TOTAL = 10;              // You have 10 images
const PPT_PATH = './ppt/';
const PPT_IMAGES = [];             // Leave empty, auto uses 1.png ~ 10.png
```

#### Using Custom Names

```javascript
const PPT_TOTAL = 5;
const PPT_PATH = './ppt/';
const PPT_IMAGES = [
    'title.png',
    'overview.png',
    'content1.png',
    'content2.png',
    'conclusion.png'
];
```

#### PPT Export Guide

| Software | Export Method |
|----------|---------------|
| Microsoft PowerPoint | File → Save As → PNG/JPG |
| Google Slides | File → Download → PNG image |
| Keynote | File → Export To → Image |
| LibreOffice Impress | File → Export → PNG |

**Recommended Settings:**

- Format: PNG (lossless, best quality)
- Resolution: 1920 × 1080 (16:9 widescreen)
- File size: < 2MB per image

---

### 3. Customize Theme

#### CSS Variables Overview

```css
:root {
    /* ===== Backgrounds ===== */
    --bg-dark: #030307;                        /* Page background */
    --bg-card: rgba(13, 13, 23, 0.6);          /* Card background */
    
    /* ===== Text Colors ===== */
    --text-primary: #ffffff;                    /* Primary text */
    --text-secondary: rgba(255, 255, 255, 0.6); /* Secondary text */
    
    /* ===== Accent Colors ===== */
    --accent-glow: #d4a843;                     /* Primary accent */
    --accent-purple: #2e8b57;                   /* Secondary accent */
    --accent-jade: #3aaf7c;                     /* Tertiary accent */
    
    /* ===== Glass Effect ===== */
    --glass-border: rgba(255, 255, 255, 0.06);  /* Border */
    --glass-bg: rgba(255, 255, 255, 0.03);      /* Background */
    
    /* ===== Typography ===== */
    --font-main: 'Inter', -apple-system, sans-serif;
    
    /* ===== Easing ===== */
    --ease-out-expo: cubic-bezier(0.19, 1, 0.22, 1);
}
```

#### Preset Color Schemes

**Scheme A: Golden Tech (Default)**
```css
--accent-glow: #d4a843;
--accent-purple: #2e8b57;
--accent-jade: #3aaf7c;
```

**Scheme B: Ocean Blue**
```css
--accent-glow: #4a9eff;
--accent-purple: #1a6bff;
--accent-jade: #00d4ff;
```

**Scheme C: Purple Galaxy**
```css
--accent-glow: #9b59b6;
--accent-purple: #8e44ad;
--accent-jade: #c39bd3;
```

**Scheme D: Chinese Red**
```css
--accent-glow: #e74c3c;
--accent-purple: #c0392b;
--accent-jade: #f39c12;
```

**Scheme E: Cyan Minimal**
```css
--accent-glow: #00bcd4;
--accent-purple: #0097a7;
--accent-jade: #4dd0e1;
```

---

### 4. Modify Particle Effects

```javascript
tsParticles.load("tsparticles", {
    fpsLimit: 120,
    particles: {
        number: { 
            value: 80,                    // Particle count (50-150 recommended)
            density: { enable: true, area: 800 }
        },
        color: { value: "#d4a843" },      // Particle color
        shape: { type: "circle" },        // Shape: circle / edge / triangle / polygon / star
        opacity: { 
            value: 0.5,                   // Opacity
            random: true,                 // Random opacity
            anim: { enable: true, speed: 1, opacity_min: 0.1 }
        },
        size: { value: 1, random: true }, // Size
        links: { 
            enable: true,                 // Show connections
            distance: 150,                // Connection distance
            color: "#d4a843",             // Connection color
            opacity: 0.2,                 // Connection opacity
            width: 1                      // Connection width
        },
        move: { 
            enable: true, 
            speed: 1,                     // Speed (0.5-3)
            direction: "none", 
            random: true, 
            straight: false, 
            outModes: "out" 
        }
    },
    interactivity: {
        events: { 
            onHover: { enable: true, mode: "grab" },    // Hover: grab / bubble / repulse
            onclick: { enable: true, mode: "push" }     // Click: push / remove / bubble
        },
        modes: { 
            grab: { distance: 200, links: { opacity: 0.5 } } 
        }
    },
    detectRetina: true
});
```

#### Particle Presets

**Dense Starfield** - For tech themes
```javascript
number: { value: 150 },
size: { value: 1.5, random: true },
links: { distance: 120, opacity: 0.15 },
move: { speed: 0.5 }
```

**Sparse Elegant** - For minimal themes
```javascript
number: { value: 40 },
size: { value: 2, random: true },
links: { distance: 200, opacity: 0.3 },
move: { speed: 0.8 }
```

**Fast Dynamic** - For energetic themes
```javascript
number: { value: 60 },
size: { value: 1 },
links: { distance: 180, opacity: 0.25 },
move: { speed: 3, random: false }
```

---

### 5. Modify Navigation

#### Add New Navigation Items

```html
<nav>
    <div class="logo">Your Project</div>
    <div class="nav-links">
        <!-- Internal tab switching -->
        <a onclick="switchTab('sources')">Data Sources</a>
        <a onclick="switchTab('features')">Features</a>
        
        <!-- Open PPT -->
        <a onclick="openPPT()">PPT Slides</a>
        
        <!-- External links -->
        <a href="https://github.com/you/repo" target="_blank">GitHub</a>
        <a href="https://your-blog.com" target="_blank">Blog</a>
        <a href="mailto:your@email.com">Contact</a>
        
        <!-- Anchor scroll -->
        <a href="#footer" onclick="document.getElementById('footer').scrollIntoView({behavior:'smooth'})">Contact Us</a>
    </div>
</nav>
```

#### Navigation Style Adjustments

```css
/* Change navigation height */
nav {
    height: 72px;  /* Change this value */
    padding: 0 5%; /* Left/right spacing */
}

/* Change link spacing */
.nav-links { 
    display: flex; 
    gap: 24px; /* Change this for spacing */
}

/* Change logo style */
.logo {
    font-size: 22px;    /* Font size */
    font-weight: 800;   /* Font weight */
}
```

---

## 🔧 Tech Stack

### Frontend Basics

| Technology | Version | Description | Documentation |
|------------|---------|-------------|---------------|
| HTML5 | - | Page structure, semantic tags | [MDN](https://developer.mozilla.org/en-US/docs/Web/HTML) |
| CSS3 | - | Styles, layouts, animations | [MDN](https://developer.mozilla.org/en-US/docs/Web/CSS) |
| JavaScript | ES6+ | Interactions, dynamic effects | [MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript) |

### Third-Party Libraries

| Library | Version | Size | Purpose | CDN |
|---------|---------|------|---------|-----|
| tsparticles | 2.12.0 | ~60KB | Particle animation background | [jsDelivr](https://cdn.jsdelivr.net/npm/tsparticles@2.12.0/) |
| VanillaTilt | 1.8.1 | ~8KB | 3D card tilt effect | [cdnjs](https://cdnjs.cloudflare.com/ajax/libs/vanilla-tilt/1.8.1/) |
| GSAP | 3.12.2 | ~30KB | Professional animation engine | [cdnjs](https://cdnjs.cloudflare.com/ajax/libs/gsap/3.12.2/) |
| ScrollTrigger | 3.12.2 | ~15KB | Scroll-triggered animations | [cdnjs](https://cdnjs.cloudflare.com/ajax/libs/gsap/3.12.2/) |
| Inter Font | - | ~30KB | UI font | [Google Fonts](https://fonts.googleapis.com/css2?family=Inter) |

### CSS Features

| Feature | Purpose | Compatibility |
|---------|---------|---------------|
| CSS Custom Properties | Theme color variables | Chrome 49+ |
| CSS Grid | Card grid layout | Chrome 57+ |
| Flexbox | Various layouts | Chrome 29+ |
| backdrop-filter | Glass blur effect | Chrome 76+ |
| @keyframes | Animation definitions | Chrome 43+ |
| perspective / transform-style | 3D effects | Chrome 36+ |

### JavaScript APIs

| API | Purpose |
|-----|---------|
| requestAnimationFrame | Smooth animation loops |
| IntersectionObserver | Element visibility detection |
| Web Audio API | Audio visualization (optional) |
| KeyboardEvent | Keyboard shortcuts |
| MouseEvent | Mouse interaction effects |

---

## 🌐 Browser Compatibility

| Browser | Min Version | Full Support | Notes |
|---------|-------------|--------------|-------|
| Google Chrome | 80+ | ✅ | Recommended |
| Microsoft Edge | 80+ | ✅ | Chromium-based |
| Mozilla Firefox | 75+ | ✅ | - |
| Apple Safari | 13+ | ✅ | macOS / iOS |
| Opera | 67+ | ✅ | Chromium-based |
| Samsung Internet | 13+ | ✅ | Mobile |
| IE | 11 | ⚠️ | Limited support |

> **Note:** This project uses modern features like `backdrop-filter`, `CSS Grid`, and CSS Variables. Some effects may not display correctly in older browsers.

---

## 🚀 Deployment Guide

### GitHub Pages (Recommended)

```bash
# Step 1: Fork this repository
# Step 2: Go to your forked repository
# Step 3: Settings → Pages
# Step 4: Source: "Deploy from a branch"
# Step 5: Branch: "main", Folder: "/ (root)"
# Step 6: Click Save
# Step 7: Wait 1-2 minutes
# Step 8: Visit https://<your-username>.github.io/arti-guide-showcase/
```

### Vercel

```bash
# 1. Sign up at Vercel: https://vercel.com
# 2. Import your GitHub repository
# 3. Keep default settings, click Deploy
# 4. Get free domain after completion
```

### Netlify

```bash
# 1. Sign up at Netlify: https://netlify.com
# 2. Drag and drop project folder to Netlify page
# 3. Or connect GitHub repository for auto-deploy
# 4. Get free domain after completion
```

### Traditional Server

```bash
# Upload perform.html and ppt folder to server
# Ensure server supports static file hosting

# Nginx configuration example
server {
    listen 80;
    server_name your-domain.com;
    root /path/to/arti-guide-showcase;
    index perform.html;
}
```

---

## ❓ FAQ

### Basic Issues

**Q: Page is blank/black after opening?**

A: Possible causes:
1. Network issue - This project relies on CDN for third-party libraries
2. Outdated browser - Please upgrade to recommended version
3. Console errors - Press F12 to check error messages

**Q: Particle animation not showing?**

A: Particle animation requires tsparticles from CDN. Check:
- Network can access `cdn.jsdelivr.net`
- No ad blocker is preventing loading

**Q: Cards don't have 3D tilt effect?**

A: VanillaTilt.js needs to load from CDN. Check:
- Network can access `cdnjs.cloudflare.com`
- Browser supports CSS 3D Transform

### PPT Related

**Q: PPT images not displaying?**

A: Check the following:
1. `ppt` folder exists and contains images
2. `PPT_TOTAL` is correctly set in `perform.html`
3. Image format is PNG or JPG
4. Image naming matches configuration
5. Some browsers may restrict local file access

**Q: PPT images loading slowly?**

A: Suggestions:
- Use image compression tools (like TinyPNG)
- Reduce resolution to 1920×1080
- Use JPG format instead of PNG
- Keep each image under 1MB

### Customization

**Q: How to add more Tab pages?**

A: 
1. Add new `.tab-panel` in HTML
2. Add corresponding data array in JavaScript
3. Modify `switchTab` function logic
4. Add corresponding Tab button

**Q: How to change fonts?**

A: 
1. Import new font in `<head>`
2. Modify `--font-main` variable in `:root`

**Q: How to disable certain animations?**

A: Find and comment out the corresponding initialization code:
- Disable particles: Comment `tsParticles.load(...)` 
- Disable tilt: Remove `VanillaTilt.init(...)` 
- Disable scroll animations: Remove `ScrollTrigger` related code

---

## 📝 Changelog

### v1.0.0 (2026-05-01)

- 🎉 Initial release
- ✨ Particle animation background
- ✨ 3D card tilt effects
- ✨ Tab page switching
- ✨ PPT slideshow display
- ✨ Responsive layout design
- ✨ Scroll-triggered animations

---

## 🤝 Contributing

All forms of contribution are welcome!

### How to Contribute

1. **Fork** this repository
2. Create your feature branch: `git checkout -b feature/AmazingFeature`
3. Commit your changes: `git commit -m 'Add some AmazingFeature'`
4. Push to the branch: `git push origin feature/AmazingFeature`
5. Open a **Pull Request**

### Contribution Types

- 🐛 Bug fixes
- ✨ New features
- 📝 Documentation improvements
- 🎨 Style optimizations
- ⚡ Performance improvements
- 🔧 Code refactoring

### Code Standards

- Keep code clean and clear
- Add necessary comments
- Follow existing code style
- Ensure compatibility

---

## 📄 License

This project is licensed under the [MIT License](./LICENSE).

```
MIT License

Copyright (c) 2026

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

---

## 🙏 Acknowledgements

Thanks to the following open source projects:

| Project | Author | License |
|---------|--------|---------|
| [tsparticles](https://particles.js.org/) | Matteo Bruni | MIT |
| [GSAP](https://greensock.com/) | GreenSock | Standard |
| [VanillaTilt.js](https://micku7zu.github.io/vanilla-tilt.js/) | Șandor Sergiu | MIT |
| [Inter Font](https://rsms.me/inter/) | Rasmus Andersson | OFL |

---

## 📮 Contact

For questions or suggestions, feel free to reach out:

- 📧 Email: [your-email@example.com]
- 🐙 GitHub: [Your GitHub Profile]
- 💬 Issues: [Submit an Issue](https://github.com/zgy123454zgy-afk/arti-guide-showcase/issues)

---

<div align="center">

### If this project helps you, please give a ⭐ Star!

<br>

![Star History](https://api.star-history.com/svg?repos=zgy123454zgy-afk/arti-guide-showcase&type=Date)

<br>

**Made with ❤️ by [Your Name](https://github.com/your-username)**

</div>
