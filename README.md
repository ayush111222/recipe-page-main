# Frontend Mentor - Recipe page solution

This is a solution to the [Recipe page challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/recipe-page-KiTsR8QQKm). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
- [Author](#author)

**Note: Delete this note and update the table of contents based on what sections you keep.**

## Overview

## The challenge 

Your challenge is to build out this recipe page and get it looking as close to the design as possible.

You can use any tools you like to help you complete the challenge. So if you've got something you'd like to practice, feel free to give it a go.

### Screenshot

![](./screenshot.jpg)

### Links

- Solution URL: [Add solution URL here](https://www.frontendmentor.io/solutions/semantic-html5-markup-mobile-first-grid-flexbox-css-variables-qdF2w9TTHP)
- Live Site URL: [Add live site URL here](https://ayush111222.github.io/recipe-page-main/)

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid
- Mobile-first workflow

### What I learned

- Learned about the scope attribute, if we have a vertical header cells table (like in this project) with the scope attribute we can define the scope of the header cells (where the header cell is pointing to) to make the table more accessible. 

```html
<th
  scope="row"
  class="nutrition-table-head font-normal neutral-color-wenge-brown"
>
  Calories
</th>
```

- How can we create custom bullet points, we can select them saparately and style them as we like.

```css
.prep-time-list-item::before,
.ingredients-list-item::before {
  content: "•";
  position: absolute;
  left: 0;
  top: 50%;
  transform: translateY(-50%);
  font-size: 1.3rem;
  color: var(--primary-dark-raspberry);
  line-height: 1;
}
```

- learned about counter-reset and counter-increment properties, with this properties we can create custom
number list (example:- for ol) and we can style them as we like.

```css
.instructions-list {
  display: grid;
  gap: 0.5rem;
  counter-reset: my-counter;
  margin-block-end: 1.9rem;
}

.instructions-list-item::before {
  counter-increment: my-counter;
  content: counter(my-counter) ". ";
  position: absolute;
  left: 0.5rem;
  top: 0;
  font-family: var(--font-family-outfit);
  font-weight: 700;
  color: var(--primary-nutmeg);
}
```

### Continued development

I will continue focusing on how can i use semantic tags in meaningfull way and about accessiblility how can i make my website more accessible there is so much to learn about semantic markup and accessiblility.

## Author

- Frontend Mentor - [@yourusername](https://www.frontendmentor.io/profile/ayush111222)

