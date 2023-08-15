# Custom themes using CSS custom properties

This example was taken from the Odin Project's lesson on [CSS Custom properties](https://www.theodinproject.com/lessons/node-path-intermediate-html-and-css-custom-properties#creating-themes-with-custom-properties).

## Features

- Dark and light theme changes

```css
:root.dark {
  --border-btn: 1px solid rgb(220, 220, 220);
  --color-base-bg: rgb(18, 18, 18);
  --color-base-text: rgb(240, 240, 240);
  --color-btn-bg: rgb(36, 36, 36);
}

:root.light {
  --border-btn: 1px solid rgb(36, 36, 36);
  --color-base-bg: rgb(240, 240, 240);
  --color-base-text: rgb(18, 18, 18);
  --color-btn-bg: rgb(220, 220, 220);
}
```

## Watch out for

- When the page loads for the first time, no theme is applied! This is because the css has only `:root.dark` and `:root.light` without the `:root` itself.
- So no variables are be used for the first load. Only with the button interaction, a class of either `dark` or `light` gets added to root.
