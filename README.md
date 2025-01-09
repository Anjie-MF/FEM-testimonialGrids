# Frontend Mentor - Testimonials grid section solution

This is a solution to the [Testimonials grid section challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/testimonials-grid-section-Nnw6J7Un7). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

## Table of contents

- [Overview](#overview)
  - [Screenshots](#screenshots)
  - [Links](#links)
- [My process](#my-process)
  - [Built with](#built-with)
  - [What I learned](#what-i-learned)
  - [Continued development](#continued-development)
  - [Useful resources](#useful-resources)
- [Author](#author)
- [Acknowledgments](#acknowledgments)

## Overview

### Screenshots

![](images/Screenshot%202025-desktop.png)
![](images/Screenshot%202025-mobile.png)

### Links

- Solution URL: [How I did it!!](https://github.com/Anjie-MF/FEM-testimonialGrids)
- Live Site URL: [What I did!](https://anjie-mf.github.io/FEM-testimonialGrids/)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- CSS Grid
- Mobile-first workflow

### What I learned

This was my first experience using the BEM (Block, Element, Modifier) methodology for coding. Initially, I found writing the modifiers somewhat cumbersome. However, this process ultimately helped me to focus and effectively group together recurring elements. Additionally, I no longer needed to expend mental energy on devising creative class names, a task that previously consumed more time than the actual coding itself. Another significant advantage became apparent during debugging. It became significantly easier to pinpoint the specific div causing the issue.
```html
<article class="testimonial testimonial--white testimonial--right">
```

Ah, CSS specificity—what a ride! Here's the story:

I ran into an issue where multiple classes applied to the same HTML element caused unintended behavior due to CSS specificity and cascade rules. Using the Computed and Elements tabs in the browser's Developer Tools, along with some strategic debugging (and yes, even !important at one point), I isolated the problem.

The solution? I increased specificity to resolve the conflict and tested incrementally to ensure everything worked as intended.

Big shoutout to @Bob on Discord, who suggested using grid rows and columns for more control—it was a game-changer. Also, thanks to @andiaz, whose code example helped me realize I needed four columns instead of three. Their insights were invaluable in solving this tricky grid layout issue! And lastly,thanks @Kapteyn Universe on Discord, for pointing out that Kira and Jeanette were both labeled as the fourth testimonial. This helped me understand the importance of properly labeling grid areas to avoid overlap and improve layout clarity.

```css
   .testimonial--white.testimonial--right {
        grid-column: 4;
        grid-row: 1/3;
    }
```

### Continued development

While I’m still in coding BootCamp, I’m eager to build more side projects using the BEM methodology. This was my first time using BEM, and while it took a long time to write, the process taught me a lot. My goal is to get faster and challenge myself to explore different coding styles and best practices along the way.


### Useful resources

- [Silktide Accessibility Checker](https://chromewebstore.google.com/detail/silktide-accessibility-ch/mpobacholfblmnpnfbiomjkecoojakah?hl=en)- Accessibility extenstion for Chrome browser
- [Piccalil CSS Reset](https://piccalil.li/blog/a-more-modern-css-reset/) - My go-to CSS reset
- [Dinson Kadudhus](https://responsivetesttool.com/) - Website Responsive Testing
- [LearntheWeb](https://learntheweb.courses/topics/html-semantics-cheat-sheet/) - My go-to HTML Semantic Cheatsheet


## Author

- LinkedIn - [Anjie M.F.](www.linkedin.com/in/anjiemay23)
- Frontend Mentor - [@Anjie-MF](https://www.frontendmentor.io/profile/Anjie-MF)
- GitHub - [@Anjie-MF](https://github.com/Anjie-MF)


## Acknowledgments

- Discord - @kapteynuniverse
- Discord - @bobstyle_23
- Frontend Mentor - [@andiaz](https://www.frontendmentor.io/profile/andiaz)

