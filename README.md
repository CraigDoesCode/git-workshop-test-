# Frontend Mentor - Stats preview card component solution

This is my solution to the [Stats preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/stats-preview-card-component-8JqbgoU62). 

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
- [Acknowledgments](#acknowledgments)


## Overview

### The challenge

Users should be able to:

- View the optimal layout depending on their device's screen size

### Desktop view

![](resources/images/desktop-view.png)

### Mobile View
![](resources/images/mobile-view.png)

### Links
- Live Site URL: [craig1001.github.io/component-card-fm/](https://craig1001.github.io/component-card-fm/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox


### What I learned

Two different menthod of creating colour overlays, firstly setting the image and the background of a containger and adding and overlay element on top
, secondly making the background the desired color and reducing the opacity of the image to greate the appearance of an overlay.

See two versions below:

V1 (overlay):
```html
<div class="image desktop">
  <div class="overlay"></div>
</div>
```
```css
.image {
    width: 50%;
    background-image: url("../images/image-header-desktop.jpg");
}
.overlay{
    background-color: hsla(277, 64%, 61%, 60%);
    width: 100%;
    height: 100%;
}
```
V2 (underlay):
```html
<div class="mobile overlay">
          <img class="mobile" src="resources/images/image-header-mobile.jpg" alt="" />
        </div>
```
```css
  img {
        opacity: 40%;
  }
  .overlay {
      background-color: hsl(277, 64%, 61%);
  }
```

### Continued development

Moving forward I want to further my understanding of flex and responsive design so im able to organsie my css better.

## Author

- Website - [Craig Noford](https://www.linkedin.com/in/craig-norford-9a33838a/)
- Frontend Mentor - [@craig1001](https://www.frontendmentor.io/profile/craig1001)
- Twitter - [@craignorford](https://www.twitter.com/craignorford)

