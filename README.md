# Andrei Nemeti — Architecture Portfolio

A single‑page, responsive portfolio website for **NEXT solutions**, built with semantic HTML, BEM‑styled CSS, and a touch of JS for smooth scrolling and a collapsible side navigation.

##  Features

* Responsive layout with modern CSS
* **BEM methodology** for scalable class naming
* Smooth in‑page anchor scrolling
* Accessible, keyboard‑friendly nav toggle
* Image hover captions for project cards
* Google Maps embed (customizable)

##  Tech Stack

* HTML5
* CSS3 (Normalize.css included)
* Vanilla JS (+ jQuery only for scroll animation)
* Font Awesome (icons)
* Google Fonts (Lato, Open Sans, Monoton)

##  Project Structure

```
project-root/
├─ index.html
├─ css/
│  ├─ normalize.css
│  └─ style.css
├─ img/
│  ├─ hero.jpg
│  ├─ logo.png
│  ├─ house1.jpg
│  ├─ house2.jpg
│  ├─ house3.jpg
│  └─ house4.jpg
└─ README.md
```

##  BEM Conventions

* **Blocks:** `.side-nav`, `.landing`, `.about`, `.work`, `.contact`, `.btn`
* **Elements:** `__logo`, `__link`, `__slogan-text`, `__services-list`, etc.
* **Modifiers:** `--expanded`, `--sub`, `--hover` (stateful helpers)

Example:

```css
.side-nav {}
.side-nav__link {}
.side-nav--expanded {}
```

##  Setup & Usage

1. **Clone or download** this repository.
2. Ensure the directory layout matches the tree above.
3. Open `index.html` in your browser (double‑click or serve locally).

### Local Development (optional)

You can use any static server. For example, with Node.js installed:

```bash
npx serve .


Navigate to `http://localhost:8080`.

##  Google Maps API

The page loads Google Maps via a script tag with a callback:

```html
<script async defer src="https://maps.googleapis.com/maps/api/js?key=YOUR_KEY&callback=initMap"></script>
```

* Replace `YOUR_KEY` with your own API key.
* For production, store keys as environment variables in your hosting platform and inject them at build/deploy time if possible.

##  Customization

* **Branding:** Update `img/logo.png`, fonts, and color accents in `style.css`.
* **Hero:** Replace `img/hero.jpg`.
* **Projects:** Swap `img/house*.jpg` and edit captions in the `work` section.
* **Copy:** All placeholder text was replaced with concise, production copy. Adjust to your brand voice as needed.

##  Accessibility Notes

* Nav toggle buttons have clear icons; ensure keyboard focus is visible.
* Provide `alt` text for all images (already present in markup).
* Maintain sufficient color contrast when adjusting colors.

##  Credits

* Icons: Font Awesome
* Fonts: Google Fonts
* Normalize.css for sane defaults

---

**Author:** Andrei Nemeti 
