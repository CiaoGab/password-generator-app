# Frontend Mentor - Password Generator App Solution

This is a solution to the [Password generator app challenge on Frontend Mentor](https://www.frontendmentor.io/challenges/password-generator-app-Mr8CLycqjh). Frontend Mentor challenges help you improve your coding skills by building realistic projects. 

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

- Generate a password based on selected inclusion options (uppercase, lowercase, numbers, symbols)
- Adjust password length with a slider
- Copy the generated password to the clipboard
- See a password strength rating based on length
- View hover and focus states for all interactive elements
- Use the app on various screen sizes with responsive design

### Screenshot

![Screenshot of the password generator app](./assets/images/Screenshot%202025-06-21%20213142.png)

### Links

- Solution URL: [Add solution URL here](https://your-solution-url.com)
- Live Site URL: [Add live site URL here](https://your-live-site-url.com)

## My process

### Built with

- Vanilla JavaScript
- Semantic HTML5
- CSS custom properties
- Flexbox
- Mobile-first responsive design

### What I learned

This project helped me practice dynamic DOM manipulation, clipboard API usage, and visual feedback implementation using JavaScript. I also improved my skills in:

- Handling user input and form validation
- Customizing sliders with dynamic backgrounds using JS
- Providing feedback through signal strength indicators

Example: updating the slider background dynamically:

```js
function updateSliderBackground() {
    const value = (slider.value - slider.min) / (slider.max - slider.min) * 100;
    slider.style.background = \`linear-gradient(
      to right,
      var(--Green200) 0%,
      var(--Green200) \${value}%,
      var(--Grey850) \${value}%,
      var(--Grey850) 100%
    )\`;
}
```

### Continued development

In the future, I want to:

- Add a toggle to show/hide the generated password
- Improve password strength calculation by factoring in character variety
- Implement dark/light theme switcher
- Add unit tests for the password generation logic

### Useful resources

- [MDN Web Docs - Clipboard API](https://developer.mozilla.org/en-US/docs/Web/API/Clipboard_API)
- [CSS Tricks - Range Slider Styling](https://css-tricks.com/styling-cross-browser-compatible-range-inputs-css/)
- [Frontend Mentor Community](https://www.frontendmentor.io/solutions) – for inspiration and solutions

## Author

- Website - https://juanvallejo.netlify.app/
- Frontend Mentor - https://www.frontendmentor.io/profile/CiaoGab
