# Frontend Mentor - Product preview card component solution

This is a solution to the [Product preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/product-preview-card-component-GO7UmttRfa). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)
- [Acknowledgments](#acknowledgments)


## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover and focus states for interactive elements

### Screenshot

![Screenshot large](./images/screenshot.png) 
![Screenshot mobile](./images/screenshot-mobile.png)

### Links

- Solution URL: [Review code](https://github.com/marefpceo/fem-product-preview-card)
- Live Site URL: [Live Test](https://marefpceo.github.io/fem-product-preview-card)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow

### What I learned

This project did not introduce and new concepts for me. However, since this is a smaller project to practice responsive designs, I took the opportunity to rely on CSS Grid for the component's overall layout. Doing so, allowed me to gain a better understanding on how useful CSS grid designs can be. I am overly confident with CSS Flexbox to the point that it has always been my go to. And for that reason, that is why I am focusing more attention to CSS Grid for major layouts. 

The code snippet below is a good example of how I can do more with CSS Grid using fewer lines of code. When the viewport width reaches 48rem (768px), the display shifts from a single column to a single row. The ```grid-auto-columns: 1fr``` attribute ensures that each grid item occupies the same amount of space.  

```css
.card {
  /* ... previous lines of css ... */

  @media (min-width: 48rem) {
    display: grid;
    grid-auto-columns: 1fr;
    grid-auto-flow: column;
    
    /* ... remaining lines of css ... */
  }
}
```

To achieve the same results using CSS Flexbox, only one line of code is needed for the display type. But additional code is needed to ensure that the image occupies the same space as the content. And in order to do that, we would have to apply changes to the ```<picture>``` div and ```.card-content``` class.
 
### Continued development

I plan on continuing to become more proficient in selecting and utilizing CSS Grid for major design layouts. With CSS Grid being a true two-dimensional control, it only makes since to learn how to properly use it and leverage it's true power.  

### Useful resources

- [MDN Web Docs](https://developer.mozilla.org/en-US/) - This serves as a general reference guide for HTML and CSS.
- [A Modern CSS Reset](https://www.joshwcomeau.com/css/custom-css-reset/) - I wanted a small and simple CSS reset and this did the job. Each section is explained very well with examples on why a reset was used.

## Author

- Website - [Lamar Stevens](https://www.lamar-stevens.com)
- Frontend Mentor - [@marefpceo](https://www.frontendmentor.io/profile/marefpceo)
- Twitter - [@stevens14704](https://www.twitter.com/stevens14704)

## Acknowledgments

[Josh W. Comeau](https://www.joshwcomeau.com/css/custom-css-reset/) - A Modern CSS Reset
