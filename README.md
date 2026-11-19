# Maël Hounkpatin — Personal Portfolio

A responsive one-page portfolio for **Maël Hounkpatin**, student at Epitech Bénin, interested in AI engineering, prompting and web development.

No build step: plain HTML, CSS and JavaScript.

---

## Features

- **3D hero scene** (Three.js): animated geometry, orbiting cubes and a particle field that react to the mouse and to scrolling
- **About section** with tabs: Skills, Experience, Education
- **Services section** with 3D tilt cards
- **Projects section** with Epitech and Lancaster projects, filters and 3D tilt + glare on hover
- **Scroll reveal** animations (3D flip-in)
- **Contact form** that posts to a Google Sheet
- **Responsive** layout with a slide-in hamburger menu on mobile
- Respects `prefers-reduced-motion`

---

## Project Structure

```
personal-portfolio/
├── index.html          # Single page (HTML + inline JS)
├── style.css           # All styles, animations and media queries
├── README.md
└── images/
    ├── background.jpeg # About section photo
    └── myCV.docx       # Downloadable CV
```

---

## Technologies

| Technology | Usage |
|---|---|
| HTML5 / CSS3 | Structure, styling, animations, responsive layout |
| Vanilla JavaScript | Tabs, project filters, 3D tilt, scroll reveal, mobile menu |
| Three.js r128 (cdnjs) | 3D hero scene |
| Font Awesome 6.5 | Icons |
| Google Fonts (Poppins) | Typography |
| Google Apps Script | Contact form backend |

---

## Run locally

Open `index.html` in a browser, or serve the folder with any static server.

## Deployment

Hosted on **Cloudflare Pages**, connected to this repository: every push to `main` redeploys the site.
Build settings: framework preset *None*, no build command, output directory `/`.

---

## Author

**Maël Hounkpatin** — [github.com/mael-alt-create](https://github.com/mael-alt-create)
