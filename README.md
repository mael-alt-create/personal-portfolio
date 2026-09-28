# Mael Hounkpatin — Personal Portfolio

A responsive one-page personal portfolio website for **Mael Hounkpatin**, UI/UX Designer & Web Developer based in Benin.

---

## Live Preview

> Open `index.html` in your browser — no build step required.

---

## Features

- **Hero section** with name, title, and background image
- **About section** with tabbed content: Skills, Experience, Education
- **Services section** with hover animation cards (Web Design, UI/UX, App Design)
- **Portfolio section** with hover overlay effect on project cards
- **Contact section** with a form that submits directly to a Google Sheet
- **Responsive design** — works on desktop, tablet (≤768px) and mobile (≤480px)
- **Mobile navigation** with slide-in hamburger menu

---

## Project Structure

```
personal-portfolio/
├── index.html          # Main HTML file (single page)
├── style.css           # All styles including responsive media queries
├── README.md           # Project documentation
└── images/
    ├── background.jpeg # Hero & about section image
    ├── logo.jpg        # Nav logo
    ├── work1.jpg       # Portfolio project 1
    ├── work2.jpg       # Portfolio project 2
    ├── work3.jpg       # Portfolio project 3
    └── myCV.docx       # Downloadable CV
```

---

## Technologies Used

| Technology | Usage |
|---|---|
| HTML5 | Page structure and semantics |
| CSS3 | Styling, animations, responsive layout |
| Vanilla JavaScript | Tab switching, mobile menu |
| Font Awesome 6.5 | Icons throughout the site |
| Google Apps Script | Contact form backend (Google Sheet) |

---

## Getting Started

No dependencies or build tools required.

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/personal-portfolio.git
   cd personal-portfolio
   ```

2. Open in your browser:
   ```bash
   # Any of these will work:
   open index.html          # macOS
   xdg-open index.html      # Linux
   start index.html         # Windows
   ```

3. Or use a local dev server for a better experience:
   ```bash
   # With VS Code Live Server extension — click "Go Live"
   # Or with Python:
   python3 -m http.server 8000
   ```

---

## Customization

### Personal information
Edit `index.html` and update:
- Your name, title, and bio in the **header** and **about** sections
- Your skills, experience, and education in the **tab contents**
- Your email, phone, and social links in the **contact** section

### Colors
The accent color is `#ff004f` (red). To change it globally, find and replace `#ff004f` in `style.css`.

### Contact form (Google Sheet)
The form uses a Google Apps Script webhook. To connect it to your own spreadsheet:

1. Create a Google Sheet
2. Go to **Extensions → Apps Script**
3. Paste your script and deploy it as a web app
4. Copy the deployment URL and replace the `scriptURL` value in `index.html`:
   ```js
   const scriptURL = 'YOUR_GOOGLE_APPS_SCRIPT_URL_HERE';
   ```

### CV download
Replace `images/myCV.docx` with your updated CV file. Consider using a `.pdf` for better browser compatibility:
```html
<a href="images/myCV.pdf" download class="btn btn2">Download CV</a>
```

---

## Bugs Fixed

| Bug | Fix applied |
|---|---|
| `meta http-eqiv` typo | Corrected to `http-equiv` |
| Double `placeholder` on email input | Removed duplicate attribute |
| `classlist` (lowercase) in JS | Fixed to `classList` |
| `opentab` iterating `tabcontents` but clearing `tablink` | Fixed loop variable (`tabcontent`) |
| `activetab` class name mismatch | Corrected to `active-tab` |
| `.work img` fixed at `width: 300px` | Changed to `width: 100%` |
| `.layer` had `transition: transform` | Fixed to `transition: height` |
| Identical service descriptions | Replaced with distinct copy per service |
| Missing Experience & Education tab content | Added full content for both tabs |

---

## Responsive Breakpoints

| Breakpoint | Target | Key changes |
|---|---|---|
| `≤ 768px` | Tablet | Hamburger menu, stacked About/Contact columns, smaller headings |
| `≤ 480px` | Mobile | Single-column grid for services & portfolio, smaller font sizes |

---

## License

This project is open source and available under the [MIT License](https://opensource.org/licenses/MIT).

---

## Author

**Mael Hounkpatin**
- Email: maelhounkpatin8@gmail.com
- GitHub: [github.com/your-username](https://github.com/your-username)
- Instagram: [@your-handle](https://instagram.com)
