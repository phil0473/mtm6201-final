# Plant Palette - Web Portfolio

**Course:** 26W_MTM6201_010 Advanced Web Design with HTML & CSS
**Author:** [Your Name]
**Live Site:** [Insert your GitHub Pages URL here]
**Figma Design:** [Insert your Figma Share Link here]

---

## 1. Development Process
I took a mobile-first approach, mapping the hi-fi Figma wireframes directly to Bootstrap's grid system rather than reinventing the wheel. The priority was stripping out the generic framework aesthetic. I established a global CSS file to override Bootstrap's native `:root` variables right away, locking in the custom "Forest Green" and "Golden Yellow" brand colors so the UI matched the intended creative strategy from day one. 

## 2. Challenges & Solutions

**Challenge 1: High-Res Asset Optimization**
* **The Issue:** The design relies heavily on large food photography, which threatened to tank mobile load times and break the layout.
* **The Solution:** I used the `<picture>` tag with `srcset` and media queries to force the browser to serve smaller, optimized image files specifically for screens under 768px. 

**Challenge 2: Complex UI Translation**
* **The Issue:** Structuring the segmented data points on the "Rooted In Responsibility" page without writing a massive, unmaintainable block of custom CSS.
* **The Solution:** I leveraged Bootstrap's native Card and Row components, nesting them to build out the exact visual chunks from the wireframes. I then used targeted CSS variables to override the default padding and border radii, matching the design perfectly without bloat.

## 3. Key Learnings
Good design is useless if it's not accessible. Building this forced me to rely strictly on semantic HTML (`<main>`, `<section>`) and clear visual hierarchy (like high-contrast "Sold Out" badges). I also learned that effectively using a framework like Bootstrap is 90% about knowing exactly which CSS variables to override, and 10% about actually writing new CSS.

---

## 4. Assets & Resources

### Frameworks & Libraries
* **Bootstrap v5.3:** Core grid layout and responsive UI components.

### Typography
* **Google Fonts:**
  * [Playfair Display](https://fonts.google.com/specimen/Playfair+Display) (Headings)
  * [Inter](https://fonts.google.com/specimen/Inter) (Body copy)

### Imagery & Media
*(Note: No AI-generated images were used in this project.)* * **Hero Background (`hero-bg.png`):** [Insert source, e.g., Unsplash by Photographer Name / Link] 
* **Farm Fresh Images (`farm-fresh-lg.jpg`, `farm-fresh-sm.jpg`):** [Insert source / Link] 
* **Menu Items (`salad.jpg`, `truffle-pasta.jpg`):** [Insert source / Link] 
* **About Hero (`about-hero-lg.jpg`, `about-hero-sm.jpg`):** [Insert source / Link] 
* **Impact Chart (`impact-chart.png`):** Custom graphic exported from my Figma file.
* **Icons (SVG):** Inline SVGs from [Bootstrap Icons](https://icons.getbootstrap.com/).