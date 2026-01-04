# Frontend Mentor - Testimonials grid section solution

This is a solution to the [Testimonials grid section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/testimonials-grid-section-Nnw6J7Un7). 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the site depending on their device's screen size.
- Experience a professional UI with hover states and accessible design tokens.

### Screenshot

![](./desktop.png)

### Links

- Solution URL: [Add your GitHub repository URL here]
- Live Site URL: [Add your live site URL here, e.g., Vercel or GitHub Pages]

## My process

### Built with

- **Semantic HTML5 markup** – Using `article`, `blockquote`, and `header` for improved SEO and accessibility.
- **Sass (SCSS)** – Organized using a modular architecture for better maintainability.
- **BEM Methodology** – Block Element Modifier naming convention to manage CSS specificity.
- **CSS Grid** – Specifically using `grid-template-areas` for complex desktop layouts.
- **Mobile-first workflow** – Ensuring a seamless experience starting from small screens.
- **Fluid Typography** – Utilizing the `clamp()` function for responsive font sizes.

### What I learned

During this project, I strengthened my understanding of "Industrial Grade" CSS. I learned how to manage complex layouts using CSS Grid Areas, which makes the code much more readable than traditional grid column/row numbers.

I'm particularly proud of this Grid implementation:

```css
@media (min-width: 64rem) {
  .testimonial-grid {
    grid-template-areas: 
      "daniel daniel jonathan kira"
      "jeanette patrick patrick kira";
  }
}
```

I also implemented a global reset that respects accessibility by supporting users who prefer reduced motion:

```css
@media (prefers-reduced-motion: reduce) {
  *, *::before, *::after {
    animation-duration: 0.01ms !important;
    transition-duration: 0.01ms !important;
    scroll-behavior: auto !important;
  }
}
```

### Author

Baskoro Ramadhan
