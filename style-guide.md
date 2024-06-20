# Front-end Style Guide

## Layout

The designs were created to the following widths:

- Mobile: 375px
- Desktop: 1440px

> 💡 These are just the design sizes. Ensure content is responsive and meets WCAG requirements by testing the full range of screen sizes from 320px to large screens.

## Colors

- Very Dark Grayish Blue: hsl(217, 19%, 35%)
- Desaturated Dark Blue: hsl(214, 17%, 51%)
- Grayish Blue: hsl(212, 23%, 69%)
- Light Grayish Blue: hsl(210, 46%, 95%)

## Typography

### Body Copy

- Font size: 13px

### Headings

- Family: [Manrope](https://fonts.google.com/specimen/Manrope)
- Weights: 500, 700

## Icons

We provide SVGs for the social icons. But please feel free to use a font icon library if you like. Some suggestions can be found below:

- [Font Awesome](https://fontawesome.com)
- [IcoMoon](https://icomoon.io)
- [Ionicons](https://ionicons.com)

> 💎 [Upgrade to Pro](https://www.frontendmentor.io/pro?ref=style-guide) for design file access to see all design details and get hands-on experience using a professional workflow with tools like Figma.

#button {
position: relative;
width: 40px;
height: 40px;
background-color: hsla(214, 17%, 51%, 0.123);
border: none;
border-radius: 50%;
color: white;
cursor: pointer;
display: inline-block;
}

#button img {
position: absolute;
top: 75%;
left: 70%;
transform: translate(-50%, -50%);
max-width: 100%;
max-height: 100%;
}

document.getElementById("button").addEventListener("click", function () {
document.querySelector(".share").style.display = "flex";
document.getElementById("buttonClose").style.display = "inline-block";
document.getElementById("button").style.display = "none";
});

function init() {
document.querySelector(".share").style.display = "none";
document.getElementById("buttonClose").style.display = "inline-block";
document.getElementById("button").style.display = "none";
}

document.getElementById("buttonClose").addEventListener("click", init);
document.getElementById("buttonCloseOne").addEventListener("click", init);
