# Stats preview card component solution

This is a solution to the [Stats preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/stats-preview-card-component-8JqbgoU62).

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Useful resources](#useful-resources)
- [Author](#author)

## Overview

### The challenge

View the optimal layout depending on their device's screen size

### Screenshot

![](./screenshot.png)

### Links

- [Solution:](https://github.com/minhlong149/stats-preview-card-component/)
- [Live Site: ](https://minhlong149.github.io/stats-preview-card-component/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox

### What I learned

Centering element using grid:

```css
.centered {
  display: grid;
  place-items: center;
  min-height: 100vh; /* This is optional */
}
```

Rounding a div with elements like images inside:

```css
.rounded-border {
  overflow: hidden;
  border-radius: 10px;
}
```

Using `<picture>` for responsive images on diffent devices:

```html
<picture>
  <source media="(min-width: 1024px)" srcset="./images/image-header-desktop.jpg" width="540px" height="446">
  <source srcset="./images/image-header-mobile.jpg" width="654" height="480">
  <img src="./images/image-header-mobile.jpg" width="654" height="480">
</picture>
```

Some issues happended can be fixed like this:

```css
picture {
  font-size: 0;
}
```
```css
img {
  width: 100%;
  height: 100%;
}
```

### Useful resources

- [Flexbox Zombies](https://geddski.teachable.com/p/flexbox-zombies) - This game helped me to understand the concept of CSS Flexbox. Anyone want to understand more about Flexbox can check this out.

## Author

- Github - [Long Nguyen](https://github.com/minhlong149)
