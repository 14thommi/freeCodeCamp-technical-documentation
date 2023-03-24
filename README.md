# freeCodeCamp - Technical Documentation solution

This is a solution to the [Technical Documenation on freeCodeCamp]([https://www.frontendmentor.io/challenges/qr-code-component-iux_sIO_H](https://www.freecodecamp.org/learn/2022/responsive-web-design/#build-a-technical-documentation-page-project)).


## Table of contents

- [Overview](#overview)
  - [Screenshot](#screenshot)
  - [Links](#links)
  - [Requirements](#requirements)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Comparing to the source solution](#comparing-to-the-source-solution)
  - [Continued development](#continued-development)


## Overview

Build a technical documentation application using Flexbox, pseudo-classes, fixed position elements, pseudo-elements, median queries and more. I attempted to recreate the original provided [solution](https://technical-documentation-page.freecodecamp.rocks/) provided by freeCodeCamp.


### Screenshot

![](./img/my-solution.png)


### Links

- Solution URL: [View Code in GitHub](https://github.com/14thommi/freeCodeCamp-technical-documentation)
- Live Site URL: [View Live Site](https://14thommi.github.io/freeCodeCamp-technical-documentation/)
- Figma Wireframe: [Private Wireframe Link](https://www.figma.com/file/zyURXqsbIebDAWeqZXRCWV/freeCodeCamp---Technical-Documentation?t=APSl6KP3rQQPTw1d-6)


### Requirements

1. You can see a main element with a corresponding id="main-doc", which contains the page's main content (technical documentation)
2. Within the #main-doc element, you can see several section elements, each with a class of main-section. There should be a minimum of five
3. The first element within each .main-section should be a header element, which contains text that describes the topic of that section.
Each section element with the class of main-section should also have an id that corresponds with the text of each header contained within it. Any spaces should be replaced with underscores (e.g. The section that contains the header "JavaScript and Java" should have a corresponding id="JavaScript_and_Java")
4. The .main-section elements should contain at least ten p elements total (not each)
5. The .main-section elements should contain at least five code elements total (not each)
6. The .main-section elements should contain at least five li items total (not each)
7. You can see a nav element with a corresponding id="navbar"
8. The navbar element should contain one header element which contains text that describes the topic of the technical documentation
9. Additionally, the navbar should contain link (a) elements with the class of nav-link. There should be one for every element with the class main-section
10. The header element in the #navbar must come before any link (a) elements in the navbar
11. Each element with the class of nav-link should contain text that corresponds to the header text within each section (e.g. if you have a "Hello world" section/header, your navbar should have an element which contains the text "Hello world")
12. When you click on a navbar element, the page should navigate to the corresponding section of the #main-doc element (e.g. If you click on a .nav-link element that contains the text "Hello world", the page navigates to a section element with that id, and contains the corresponding header)
13. On regular sized devices (laptops, desktops), the element with id="navbar" should be shown on the left side of the screen and should always be visible to the user
14. Your technical documentation should use at least one media query

Fulfill the user stories and pass all the tests below to complete this project. Give it your own personal style. Happy Coding!

Note: Be sure to add <link rel="stylesheet" href="styles.css"> in your HTML to link your stylesheet and apply your CSS

## My Process

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
