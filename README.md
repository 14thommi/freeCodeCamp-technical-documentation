# freeCodeCamp - Technical Documentation solution

This is a solution to the [Technical Documenation on freeCodeCamp]([https://www.frontendmentor.io/challenges/qr-code-component-iux_sIO_H](https://www.freecodecamp.org/learn/2022/responsive-web-design/#build-a-technical-documentation-page-project)).


## Table of contents

- [Overview](#overview)
  - [Screenshot](#screenshot)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Comparing to the source solution](#Comparing-to-the-source-solution)
  - [Continued development](#continued-development)


## Overview

Build a technical documentation application using Flexbox, pseudo-classes, fixed position elements, pseudo-elements, median queries and more. I attempted to recreate the original provided [solution](https://technical-documentation-page.freecodecamp.rocks/) provided by freeCodeCamp.


### Screenshot

![](./img/my-solution.png)


### Links

- Solution URL: [View Code in GitHub](https://github.com/14thommi/freeCodeCamp-technical-documentation)
- Live Site URL: [View Live Site](https://14thommi.github.io/frontend-mentor-qr-code-component/)


### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Media Query


### What I learned

I learned a few important lessons:

1. I tried to make the navbar dynamic to show on the left when wide screen and then go to the top of the screen when in a mobile view using Flexbox. The only issue was flexbox did not fix the link elements of the navbar to the same spot on the screen without scrolling. I thus pivoted to accomplish this by having the navbar `position: fixed` and use a media query to unfix the navbar so it sticks to the top of the screen.


### Comparing to the source solution

When comparing my code to the source code I want to point out a few techniques I should consider using in the future:

1. The `.main-section` element had two children `header` & `article` in the source code. By bucketing `p`, `code`, & `li` elements in an `article` they were able style the block instead of each individual element type. For example, I used `margin-left: 3rem;` for all elements where as I could have bucketing them into an `article` or `div` element and do that setting once.
2. To hide the horizontal scroll bar for the `navbar` when in mobile view considering using the following:

  ```css
  nav {
    overflow-x: hidden;
    overflow-y: auto;
  }
  ```


### Continued development

My primary goal right now is to get comfortable with using HTML and CSS basics so I will feel like my core skills in HTML and CSS will not be forgotten after a brief period devoted to studying JS. 
