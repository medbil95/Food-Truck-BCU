# Food-Truck-BCU
Food Truck website.
# Mo's Burgers – Food Truck Website

**Live site:** `https://<medbil95>.github.io/<Food Truck BCU>/`
**Repository:** `https://github.com/<your-medbil95>/<Food Truck BCU>`

## Project overview
A lightweight, responsive marketing site for a halal food truck. It shows the menu with prices, weekly opening times, a location map and a contact form. Built with plain HTML5, CSS and JavaScript (no frameworks or build step).

```
index.html      page structure
css/styles.css  mobile-first styles
js/main.js      interactivity
assets/         burger.svg, map.svg
screenshots/    mobile.png, desktop.png
```

## Sitemap
Single page with anchor sections: **Home (hero)** → **Menu** (`#menu`) → **Opening times** (`#hours`) → **Find us** (`#find-us`) → **Contact** (`#contact`).

## Responsiveness notes
- Mobile-first: base styles target ≤480px; enhancements are added with `min-width` media queries.
- **Mobile (≤480px):** single-column layout, hamburger menu, stacked hero.
- **Tablet (≥768px):** two-column menu grid, hours and map side by side, inline nav.
- **Desktop (≥1024px):** three-column menu grid, hero image beside the text.
- Layout uses CSS Grid (menu, hours/map) and Flexbox (header, hero, menu rows). Spacing and colours come from CSS variables.

## JavaScript features
1. Hamburger menu toggle (closes on link click, Escape or resize).
2. Today's opening hours highlighted automatically.
3. Contact form validation using HTML attributes (`required`, `minlength`, `type="email"`, `pattern`) plus JS error messages. Front-end only; nothing is sent.

## Accessibility
- Semantic landmarks: `header`, `nav`, `main`, `section`, `article`, `figure`, `footer`; one `h1` then `h2`/`h3` in order.
- Skip link, visible focus styles, `aria-expanded`/`aria-controls` on the menu button.
- Every form field has a label; errors are linked with `aria-describedby`, `aria-invalid` and `aria-live`.
- Alt text on all images; descriptive link text; table with caption and header cells.
- Colour contrast checked for text and buttons; `prefers-reduced-motion` respected.

## Screenshots
| Mobile  | Desktop |
|---|---|
| ![Mobile](screenshots/mobile.png) | | ![Desktop](screenshots/desktop.png) |

## Credits
- `assets/burger.svg` and `assets/map.svg`: original artwork created for this project (free to reuse).
- 🍔 and 📍 are Unicode emoji drawn by the viewer's system font.
- Map link opens Google Maps; no Google assets are embedded.
- Address, email and social handle are placeholders.
