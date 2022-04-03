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

![Project preview image](preview.png?raw=true)

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

While working on this project, I have learned about the experimental :has() CSS Selector.

It’s essentially a parent selector, although far more useful than just that.

In the below example, I utilize it to select and move the box illustration which is located inside an element with the class of card if that card contains an element without an open attribute that is directly followed by a hovered element with the class of faq__question.

```css

.card:has(:not(.faq[open]) > .faq__question:hover) > .card__box-illustration {
        transform: translateX(-1.9rem);
    }

```

If the browser doesn't support the selector this rule will be ignored and the box won't move on the page.

The browser support currently isn't the greatest, but that may change in the future.

### Continued development

I would definitely like to further improve in areas of accessibility and semantics.

### Useful resources

- [Docs for details and summary element](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/details) - Everything about the details and summary element
- [Details element styling issues](https://css-tricks.com/two-issues-styling-the-details-element-and-how-to-solve-them/) - This article addresses two styling issues of the details element.
- [:has() browser support](https://caniuse.com/?search=%3Ahas) - A useful browser support checking tool for CSS properties.
- [Web Accessibility Evaluation Tools List](https://www.w3.org/WAI/ER/tools/) - List of tools that can be used for accessibility evaluation.

## Author

- Website - [MrGeminus](https://mrgeminus.com/)
- Frontend Mentor - [@MrGeminus](https://www.frontendmentor.io/profile/MrGeminus)