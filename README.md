# Frontend Mentor - QR code component solution

This is a solution to the [QR code component challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/qr-code-component-iux_sIO_H). Frontend Mentor challenges help you improve your coding skills by building realistic projects.

## Table of contents

- [Frontend Mentor - QR code component solution](#frontend-mentor---qr-code-component-solution)
  - [Table of contents](#table-of-contents)
  - [Overview](#overview)
    - [Screenshot](#screenshot)
    - [Links](#links)
  - [My process](#my-process)
    - [Built with](#built-with)
    - [What I learned](#what-i-learned)
    - [Continued development](#continued-development)
    - [Useful resources](#useful-resources)

## Overview

### Screenshot

![Screenshot of QR code component](/live%20webpage.png)

### Links

- Live Site URL: [GitHub Pages](https://rffkive.github.io/qr-code-component)

## My process

### Built with

- Semantic HTML5 markup
- CSS custom properties
- Flexbox
- Mobile-first workflow

### What I learned

This project helped me reinforce fundamental web development concepts. I focused on creating a responsive design that works well on all screen sizes while maintaining a clean, accessible structure.

Some key learning points:

- Centering elements both vertically and horizontally using Flexbox:

```css
body {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  min-height: 100vh;
}
```

- Using CSS custom properties for consistent styling:

```css
:root {
  --white: hsl(0, 0%, 100%);
  --light-gray: hsl(212, 45%, 89%);
  --grayish-blue: hsl(220, 15%, 55%);
  --dark-blue: hsl(218, 44%, 22%);
}
```

- I learned that font size and font weight should be reduced as we move down in the hierarchy of elements. This creates a visual hierarchy that guides the user's eye through the content:

```css
h2 {
  font-size: 22px;
  font-weight: 700;
  color: hsl(218, 44%, 22%); /* Darker color for headings */
}

p {
  font-size: 15px;
  font-weight: 400;
  color: hsl(220, 15%, 55%); /* Lighter color for paragraphs */
}
```

- Adding padding and box-shadow creates depth and separation, making the card stand out from the background:

```css
.container {
  padding: 16px;
  box-shadow: 0 10px 20px rgba(0, 0, 0, 0.05);
  border-radius: 20px;
}
```

- Setting images to width 100% ensures they properly fit within their containers while maintaining aspect ratio:

```css
.image img {
  width: 100%;
  display: block;
  border-radius: 10px; /* Adding curves to the image corners */
}
```

- Using border-radius effectively to create curved corners for both the container and the image:

```css
.container {
  border-radius: 20px;
}

.image img {
  border-radius: 10px;
}
```

### Continued development

In future projects, I want to focus on:

- Implementing more advanced CSS animations and transitions
- Exploring CSS Grid for more complex layouts
- Improving accessibility features
- Learning more about CSS best practices and optimization

### Useful resources

- [MDN Web Docs](https://developer.mozilla.org/en-US/) - Comprehensive documentation that helped me understand flexbox properties in depth.
- [CSS-Tricks Flexbox Guide](https://css-tricks.com/snippets/css/a-guide-to-flexbox/) - This visual guide to Flexbox was invaluable for centering elements.
- [Google Fonts](https://fonts.google.com/) - Used to import the Outfit font family.
- [Frontend Mentor](https://www.frontendmentor.io/) - The challenge platform that provided the design specifications.
