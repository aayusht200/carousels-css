# 🎠 Carousels Using CSS

A fully functional **carousel built entirely with CSS** — no JavaScript required.  
This project demonstrates the power of modern CSS scroll-linked features like `::scroll-button` and `::scroll-marker`.

---

## 🚀 Features

-   100% **CSS-powered** carousel (no JS)
-   Uses **new Chrome experimental selectors**
-   **Customizable design** through CSS variables
-   **Responsive layout** using CSS Grid
-   Smooth scrolling and scroll snapping
-   Easily switch between **text-based** or **image-based** slides

---

## 🧩 Project Structure

```
carousels-with-css/
│
├── index.html   # Carousel markup
├── style.css    # Main stylesheet (customizable)
└── README.md    # Project documentation
```

---

## 🎨 Customization

All visual aspects can be controlled via CSS variables in `style.css`. Look for the commented sections like:

```css
/* 🎨 COLOR SETTINGS — change these to restyle the carousel */
:root {
    --bg-card: hsl(208, 55%, 50%);
    --para-width: 50%;
    --aspect-ratio: 1 / 0.8;
    --border-radius: 1rem;
    --gap-main: 1rem;
    --scroll-btn-bg: color-mix(in srgb, var(--bg-card) 50%, transparent);
    --scroll-btn-font: 1rem;
}
```

Common customization options:

-   --bg-card — Main accent color (example: `hsl(208, 55%, 50%)`)
-   --para-width — Carousel width (example: `50%`)
-   --aspect-ratio — Controls height ratio (example: `1 / 0.8`)
-   --border-radius — Rounds corners (example: `1rem`)
-   --gap-main — Space between grid elements (example: `1rem`)
-   --scroll-btn-bg — Scroll arrow background
-   --scroll-btn-font — Arrow icon size (example: `1rem`)

Tip: Start by changing only color, border radius, and aspect ratio for visible impact.

---

## 🧱 HTML Structure

-   The `<div class="para-div">` acts as the main container.
-   Inside it, `<ul class="carousel-p">` contains all slides.
-   Each `<li>` is one carousel slide.

To add slides → duplicate a `<li>` block and edit its content.

To use images instead of text → uncomment the image-carousel section in `index.html` or replace slide content with an `<img>` tag and adjust CSS as needed.

---

## 🧭 Browser Support

This carousel uses experimental CSS features:

-   `::scroll-button`
-   `::scroll-marker`
-   `scroll-snap-type`
-   `scroll-marker-group`

Currently works best in Chrome Canary (with the experimental web platform features flag enabled):

1. Open Chrome Canary.
2. Go to `chrome://flags/#experimental-web-platform-features`
3. Set to **Enabled**.
4. Restart the browser.

Note: These selectors are experimental and may change or be unsupported in other browsers.

---

## ⚙️ Setup

Clone the repository and open the demo:

```bash
git clone https://github.com/aayusht200/carousels-css.git
cd carousels-css
# Open index.html in your browser (for best results use Chrome Canary)
```

To customize:

1. Open `style.css`.
2. Adjust the CSS variables in the `:root` section.
3. Save and refresh your browser.

---

## 🧪 Usage Notes

-   Use CSS variables for theming and responsive tweaks.
-   The layout uses CSS Grid for the carousel frame and `scroll-snap` for smooth snapping between slides.
-   If copying slides or switching to images, ensure images are sized and have `object-fit` set to maintain consistent aspect ratio.
-   Check Solution for images version in images.css, although its a large file it can easily be compressed into a smaller file due to repeating elements.
---

## References

-   Chrome Developers: Carousels with CSS — https://developer.chrome.com/blog/carousels-with-css
-   Video tutorial: Building a CSS-only Carousel — https://www.youtube.com/watch?v=g03Yldh9Nkw&t=279s

---

## 📜 License

This project is open-source and available under the MIT License.

---

## 👤 Author

Aayush Trivedi  
Front-End Developer (in training)  
Learning through The Odin Project and Meta Front-End Developer Certificate.
