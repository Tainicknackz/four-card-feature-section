# Frontend Mentor - Four card feature section solution

This is a solution to the [Four card feature section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/four-card-feature-section-weK1eFYK). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

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

- View the optimal layout for the site depending on their device's screen size
  ![Desktop view](./screenshots/desktop-screenshot.png)
  ![Tablet view](./screenshots/tablet-screenshot.png)
  ![Mobile view](./screenshots/mobile-screenshot%20I.png)
  ![Mobile view cont.](./screenshots/mobile-screenshot%20II.png)

### Links

- Solution URL: [https://github.com/Tainicknackz/four-card-feature-section](https://github.com/Tainicknackz/four-card-feature-section)
- Live Site URL: [jade-cheesecake-e4bea4](https://jade-cheesecake-e4bea4.netlify.app/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- CSS FLEX-BOX
- CSS GRID
- Mobile-first workflow

### What I learned

_CSS Flex-box_, _grid-template-columns_, _grid-template-rows_, _grid-template-areas_, _align-self_ property in _CSS Grid_, and _Media Queries_ were clear to me. How to keep columns and rows responsive and scalable. **As shown below:-**

```HTML
<main class="box__wrapper">
  <div class="box__ctn">
    <div class="box__item box__cyan"></div>
    <div class="box__item box__red"></div>
    <div class="box__item box__orange"></div>
    <div class="box__item box__blue"></div>
  </div>
</main>
```

```CSS
/* Media Query for 1440px */
@media (min-width: 1200px) {

  .header__ctn {
    display: flex;
    flex-direction: column;
    align-items: center;
  }

  .box__ctn {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    grid-template-rows: 1fr 1fr;
    grid-template-areas:
      "cyan red blue"
      "cyan orange blue";
    gap: 2rem;
    width: 100%;
    max-width: 1000px;
  }

}
```

- Frontend Mentor - [@Tainicknackz](https://www.frontendmentor.io/profile/Tainicknackz)
- GitHub - [@Tainicknackz](https://www.github.com/Tainicknackz)
