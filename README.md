# Frontend Mentor - Stats preview card component solution

This is a solution to the [Stats preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/stats-preview-card-component-8JqbgoU62). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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

- View the optimal layout depending on their device's screen size

### Screenshot


![Desktop Design](./desktop-design.jpg)
![Mobile Design](mobile-design.jpg)

### Links

- Solution URL: [Github Repo](https://github.com/akri-dev/front-end-mentor_stats-preview-card)
- Live Site URL: [Stats Preview Card Component](https://akri-dev.github.io/front-end-mentor_stats-preview-card/)

## My process


### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- CSS Grid

### What I learned

I learned how confusing (lol) it still is to have a responsive design, especially when using media queries.
Somehow my styling works, but personally, I don't think I fully understand how my css works 100%

I do understand this part:
```css
@media only screen and (max-width: 1109px) {
    .card {
        width: 90%;
    }

    main {
        font-size: 1rem;
    }

    .hook p {
        font-size: .74rem;
    }

    .stats {
        margin-top: 4rem;
    }
}
```

just not this one (ESPECIALLY THE CSS GRID):
```css
@media only screen and (max-width: 542px) {
    .card {
        display: grid;
        grid-template-columns: 1fr;
        grid-template-rows: 1fr 1fr;
        grid-column-gap: 0px;
        grid-row-gap: 0px;
        font-size: .8rem;
        height: 70%
    }

    .hook {
        grid-area: 2 / 1 / 3 / 2;
        text-align: center;
        margin: 3rem 2.5rem 0;
    }

    .hook p {
        padding: .1rem;
        font-size: .90rem;
        line-height: 1.7rem;
    }
    
    .card-image {
        grid-area: 1 / 1 / 2 / 2;
        background-position: top;
    }

    .stats {
        margin-top: 1rem;
        display: flex;
        justify-content: center;
        flex-direction: column;
        margin-bottom: 4rem;
    }
    .stats-items {
        display: block;
    }
    
    .stats-items:nth-child(1), 
    .stats-items:nth-child(2) {
        margin-bottom: 1.5rem;
        margin-right: 0;
    }

}
```

### Continued development

I'd like to focus more on understanding how CSS grid works.

### Useful resources

- [CSS Grid Generator](https://cssgrid-generator.netlify.app/) - This helped me for creating CSS code for grids.


## Author

- Github - [Akri](https://github.com/akri-dev)
- Frontend Mentor - [@akri-dev](https://www.frontendmentor.io/profile/akri-dev)