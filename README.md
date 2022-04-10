# NFT preview card component solution

This is a solution to the [NFT preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/solutions/simple-card-with-interactions-Sk5sWU0Q9).

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size
- See hover states for interactive elements

### Screenshot

![result](./screenshot.png)

### Links

- Live Site URL: [https://mateus3009.github.io/NFT-preview-card-component/](https://mateus3009.github.io/NFT-preview-card-component/)

## My process

### Built with

- HTML
- CSS

### What I learned

- How to use css media feature `prefers-reduced-motion` to disable animations based on the user preferences

  ```css
    .nft_image_container::before {
      transition: none;
    }
  ```

- How to organize my code using css classes

  ```html
  <main class="card">
    <!-- other tags -->
  </main>
  ```
  ```css
  .card {
    /* some style */
  }
  ```

- How to set multiple backgrounds and box-shadows to my components:

  ```css
    div {
      box-shadow: 0 23px 10px 17px rgba(0, 0, 0, .1), 0 15px 20px 50px rgba(0, 0, 0, .03);
      /* just put a comma between the shadow parameters */
    }
  ```

  ```css
    div {
      background: url('images/bg.svg') no-repeat center center, (rgba(0, 0, 0, .4) 100%, rgba(0, 0, 0, .4) 100%);
      /* you can't mix background image and color so you can use a trick: linear-gradient */
    }
  ```

### Useful resources

- [CSS Multiple Backgrounds](https://www.w3schools.com/css/css3_backgrounds.asp)
- [Multiple Shadows in CSS](https://www.entheosweb.com/tutorials/css/multiple_shadows.asp)
- [prefers-reduced-motion](https://developer.mozilla.org/en-US/docs/Web/CSS/@media/prefers-reduced-motion)

## Author

- LinkedIn - [Mateus Sale albino](https://www.linkedin.com/in/mateusalbino/)
- Frontend Mentor - [@mateus3009](https://www.frontendmentor.io/profile/mateus3009)

## Acknowledgments

Thanks to [vanzasetia](https://github.com/vanzasetia) who gave me a [feedback](https://www.frontendmentor.io/solutions/simple-card-with-interactions-Sk5sWU0Q9#comment-625106e4f223eb5a99e889c4) about the importance of use css classes and how my interactive components should by wrapped in an anchor tag.

