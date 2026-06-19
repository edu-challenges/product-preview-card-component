# Frontend Mentor - Product preview card component solution

This is a solution to the [Product preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/product-preview-card-component-GO7UmttRfa). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
  - [AI Collaboration](#ai-collaboration)
- [Author](#author)

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover and focus states for interactive elements

### Links

- Solution URL: [https://github.com/edu-challenges/product-preview-card-component](https://github.com/edu-challenges/product-preview-card-component)
- Live Site URL: [https://edu-challenges.github.io/product-preview-card-component/](https://edu-challenges.github.io/product-preview-card-component/)

## My process

### Built with

- Semantic HTML5 markup (`<article>`, `<picture>`, `<s>`)
- CSS custom properties (tokens for colors, spacing, typography)
- Flexbox
- `<picture>` for responsive images
- Mobile-first workflow

### What I learned

**Responsive images with `<picture>`:**

Learned the difference between `srcset` and `<picture>`. `srcset` is for same image at different resolutions, while `<picture>` is for completely different images (mobile vs desktop). In this project, `<picture>` was the right choice because mobile and desktop versions have different crops.

```html
<picture>
  <source
    media="(min-width: 600px)"
    srcset="./images/image-product-desktop.jpg"
  />
  <img src="./images/image-product-mobile.jpg" alt="..." />
</picture>
```

**Semantic HTML for prices:**

Understanding the difference between `<del>` and `<s>` for strikethrough text. `<del>` means "deleted text" (screen readers announce "deleted"), while `<s>` means "no longer accurate/relevant" - perfect for showing an old price.

**CSS nesting organization:**

Finding the right balance between nested and flat CSS. For a small component, 3-4 levels of nesting works well. For larger projects, flattening improves maintainability.

**Flexbox 50/50 layout:**

Using `flex-shrink: 0` on image containers to prevent them from collapsing when content grows.

### Continued development

- Advanced accessibility (ARIA labels, focus management)
- CSS Grid for more complex layouts
- CSS container queries

### Useful resources

- [MDN Web Docs](https://developer.mozilla.org/) - Reference for HTML elements and CSS properties
- [CSS-Tricks Flexbox Guide](https://css-tricks.com/snippets/css/a-guide-to-flexbox/) - Visual guide for Flexbox concepts

### AI Collaboration

Used AI assistant (Open Code) to discuss best practices for:

- HTML semantics (`<picture>` vs `<srcset>`, `<s>` vs `<del>`)
- CSS organization (nesting levels, variable naming)
- Accessibility considerations

The AI provided explanations and alternatives rather than direct solutions, which helped deepen understanding of the concepts.

## Author

- Frontend Mentor - [@Yevestevez](https://www.frontendmentor.io/profile/Yevestevez)
- GitHub - [Yevestevez](https://github.com/Yevestevez/)
- LinkedIn - [Edu Yeves](https://www.linkedin.com/in/edu-yeves/)
