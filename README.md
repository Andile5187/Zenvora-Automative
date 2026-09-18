## Changelog

### [Date] – Part 2: CSS Styling and Responsive Design

**Added**
- Created external stylesheet `css/style.css` and linked it to all five HTML pages
  (Home, About Us, Services, Showroom, Contact Us).
- Added a base style / CSS reset (margin, box-sizing, font-family, background) applied
  site-wide from the external stylesheet.
- Added typography rules (font-family, font-size, font-weight, line-height,
  letter-spacing) for headings, paragraphs, labels and list items.
- Implemented Flexbox for the navigation bar (logo, links) so it lays out
  responsively across screen sizes.
- Implemented CSS Grid for the Contact Us details section (`.contact-grid`) and
  the Showroom image gallery (`.gallery`).
- Added decorative styling: background colours, borders, and box-shadows on
  paragraphs, form fields, and gallery images.
- Added interactive pseudo-classes (`:hover`, `:focus`, `:active`) to nav links,
  form inputs, and gallery images for better user feedback.
- Styled the contact form (inputs, textarea, submit button) for a consistent look.
- Added two responsive breakpoints via media queries (1024px for tablet, 600px
  for mobile) that switch the multi-column nav/grid/gallery layouts to
  single-column on smaller screens, using relative units (rem, %) throughout.

**Fixed (based on Part 1 feedback)**
- Removed invalid inline `<style>` blocks that were incorrectly placed inside
  `<header>` on each page.
- Fixed a broken `<img>` tag for the nav logo that was missing quotes and a
  `width` property.
- Added missing `<body>` tags on Home.html, About Us.html, Services.html and
  Showroom.html.
- Removed a duplicate, unclosed `<nav>` tag nested inside the main nav.
- Removed a stray `</details>` closing tag with no matching opening tag.
- Removed inline `style="color:..."` attributes throughout, replacing them with
  centralised styling in the external stylesheet for consistency and easier
  maintenance.

**Known limitation**
- Responsive images use fluid CSS (`max-width: 100%`) rather than `srcset`/`sizes`,
  since only a single resolution exists for each image asset. Multiple image
  sizes would need to be generated to implement true `srcset` responsive images.
