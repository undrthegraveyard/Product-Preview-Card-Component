## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
- [Author](#author)


## Overview

Product preview card component 

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover and focus states for interactive elements

### Screenshot

![](./design/Final%20Design%20Desktop%20Preview.png)

![](./design/Final%20Design%20Mobile%20Preview.png)

### Links

- Solution URL:(https://github.com/undrthegraveyard/Product-Preview-Card-Component.git)
- Live Site URL: (https://undrthegraveyard.github.io/Product-Preview-Card-Component/)

## My process

- HTML and CSS(Grid)

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow

### What I learned

```html
<picture class="product__img">
         <source srcset="images/image-product-desktop.jpg" media="(min-width: 600px)">
          <img src="images/image-product-mobile.jpg" alt="Chanel Perfume">
        </picture>
```
```html
<p class="product__price">
              <span class="visually-hidden">Current Price:</span>
              $149.99
            </p>
```
```css
/* For screen reader */
.visually-hidden:not(:focus):not(:active){
    clip: rect(0 0 0 0);
    clip-path: inset(50%);
    height: 1px;
    overflow: hidden;
    position: absolute;
    white-space: nowrap;
    width: 1px;
}
```
```css

/* CSS Reset */
*, *::before, *::after {
    box-sizing: border-box;
  }
  * {
    margin: 0;
  }
  body {
    line-height: 1.7;
    -webkit-font-smoothing: antialiased;
  }
  img, picture, video, canvas, svg {
    display: block;
    max-width: 100%;
  }
  input, button, textarea, select {
    font: inherit;
  }
  p, h1, h2, h3, h4, h5, h6 {
    overflow-wrap: break-word;
  } 
  h1, h2, h3{
 line-height: 1;
  }
  /* end of reset */
```
```css
.button[data-icon="shopping-cart"]::before{
content: "";
width: 15px;
height: 16px;
background-color: var(--clr-primary-400);
color: var(--clr-neutral-100);
background-image: url(../images/icon-cart.svg);
}
```
### Continued development

- CSS Reset 
- CSS data and picture elements
- Ensuring acessibility 

## Author

- Website - [Shivam Agarwal](https://www.shivamagarwal.au)
- Frontend Mentor - [@undrthegraveyard](https://www.frontendmentor.io/profile undrthegraveyard)
- Twitter - [@shivam_agarwaal](https://twitter.com/shivam_agarwaal)
