# Frontend Mentor - Stats preview card component solution

This is a solution to the [Stats preview card component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/stats-preview-card-component-8JqbgoU62). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [The challenge](#the-challenge)
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


### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

I started from the mobile first way, I used the div tags for the stats and then I changed my mind to finally use the UL tags (Totally regreted not to stay with the div tags). Flexbox was the main display used for the items in the card. I had some issues with the overlay of the card image but then I found the amazing resource from StevenStromick to solve it. During the development of the desktop version I had some troubles to get the gap between the list items, a great aproach from codegrepper was a big help. I feel I patched a frankenstein for the last details but I had to accept I'm noob and need to learn a lot more. 

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow


### What I learned

I learned a lot of stuff related with HMTL and CSS. 

How to overlay an image without a titanic struggle agains margins: 

```html
<div class="image-container">
      <div class="images">
        <img src="/images/image-header-mobile.jpg" alt="people talking" class="card-image" id="mobile-image">
        <img src="/images/image-header-desktop.jpg" alt="people talking" class="card-image" id="desktop-image">
        <div class="card-overlay"></div>
      </div>
    </div>
```

```css
.image-container{
    position: relative;
}

.card-image{
    display: block;
    width: 100%;
    height: auto;
}

.card-overlay{
    position: absolute;
    top: 0;
    bottom: 0;
    left: 0;
    right: 0;
    height: 100%;
    width: 100%;
    opacity: 0.4;
    background-color: var(--soft-violet);
}
}
```

How to get some space between list items if the flex tools are getting things hards for noobs like me.

```css
ul.stats {
        display: flex;
        align-items: stretch; 
        justify-content: space-between;
        width: 100%;
    }
```

The change between the mobile and desktop image gave some troubles. The best approach I found was this one. 

```html
<h1>Some HTML code I'm proud of</h1>
```
```css
    #mobile-image {
        display: none;
    }

    #desktop-image{
        display: block;
    }
    .image-container{
        width: 100%;
    }
```


### Continued development

I need to improve and develop my design skills. Was really hard to me figure out which fonts and colors were the right ones for the challenge. Also I want work more my flex grids skills, these are really hepful but quite confusing if you are not clear with relation between parents and child when you apply the display for these. 


### Useful resources

- [Example resource 1](https://www.codegrepper.com/code-examples/css/html+list+items+horizontally+with+flexbox) - This helped me with the space between list items. 

- [Example resource 2](https://stevenstromick.com/css/css-card-overlay/) - This got me out of hell when I was trying to do the overlay. 


## Author

- Website - [Alcides]
- Frontend Mentor - [@Alatmal](https://www.frontendmentor.io/profile/Alatmal)




