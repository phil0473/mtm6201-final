# Plant Palette - Web Portfolio

**Course 26W_MTM6201_010 Advanced Web Design with HTML & CSS
**Author:** Kiera Philippe
**Live Site:** https://phil0473.github.io/mtm6201-final/
**Figma Design:** https://www.figma.com/design/B7LRjw4IWMkvN4oBqATnwD/philippe-kiera-prototype?node-id=0-1&t=rUEC7k9NZRdnX8bi-1

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
*(Note: No AI-generated images were used in this project.)* * **Hero Background (`hero-bg.png`):** Pexels, Ella Olsson. Free to use. https://www.pexels.com/photo/fruit-salads-in-plate-1640774/

* **Farm Fresh Images (`farm-fresh-lg.jpg`):** Unsplash, Engin Akyurt. Free to use. https://unsplash.com/photos/red-green-and-yellow-chili-peppers-and-green-chili-peppers-Y5n8mCpvlZU

* **Menu Items (`salad.jpg`, `truffle-pasta.jpg`):** Pexels, Towfiqu Barbhuiya. https://www.pexels.com/photo/close-up-shot-of-a-salad-12474263/

Pexels, Nour Alhoda. https://www.pexels.com/photo/delicious-spaghetti-bolognese-on-wooden-board-32632540/


* **About Hero (`about-hero-lg.jpg`):** Unsplash, Sonny M. https://unsplash.com/photos/a-blue-bowl-filled-with-vegetables-and-a-wooden-spoon-yhc4pSbl01A

* **Impact Chart (`impact-chart.png`):** Custom graphic exported from my Figma file.
* **Icons (SVG):** Inline SVGs from [Bootstrap Icons](https://icons.getbootstrap.com/).