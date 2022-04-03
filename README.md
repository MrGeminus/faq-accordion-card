# Frontend Mentor - FAQ accordion card solution

This is a solution to the [FAQ accordion card challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/faq-accordion-card-XlyjD0Oam). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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

## Overview

### The challenge

Users should be able to:

- View the optimal layout for the component depending on their device's screen size
- See hover states for all interactive elements on the page
- Hide/Show the answer to a question when the question is clicked
- **Bonus:** Complete the challenge without using JavaScript

### Screenshot

![](https://mrgeminus.github.io/faq-accordion-card/blob/main/preview.png?raw=true)

### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [https://mrgeminus.github.io/faq-accordion-card/](https://mrgeminus.github.io/faq-accordion-card/)

## My process

### Built with

- Semantic HTML5 markup
- Accessibility focus
- BEM naming convention
- CSS3
- Mobile-first workflow

### What I learned

While working on this project, I have discovered the experimental :has() CSS Selector.

It’s essentially a parent selector, although far more useful than just that.

In the below example, I utilize it to select and move the box illustration which is located inside an element with the class of card if the card contains a element without the open attribute that is directly followed by a hovered element with the class of faq__question.

``
`css`

.card:has(:not(.faq[open]) > .faq__question:hover) > .card__box-illustration {
        transform: translateX(-1.9rem);
    }

``

The browser support currently isn't the greatest, but that may change in the future.

### Continued development

I would definitely like to further improve in areas of accessibility and semantics.

### Useful resources

- [details and summary](https://css-tricks.com/two-issues-styling-the-details-element-and-how-to-solve-them/) - This helped me for XYZ reason. I really liked this pattern and will use it going forward.
- [:has() browser support](https://caniuse.com/?search=%3Ahas) - Here you can see the current browser support for this CSS Selector.

## Author

- Website - [MrGeminus](https://mrgeminus.com/)
- Frontend Mentor - [@MrGeminus](https://www.frontendmentor.io/profile/MrGeminus)