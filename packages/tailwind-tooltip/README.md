# Tailwind Tooltip

This plugin helps you to create a tooltip for your text.

> 📝 Currently, the positioning of the label can be done 
only for up and down.

## How to install

Add the package as dev dependency to the project with the
below command:

With `npm`

```bash
npm install -D @ceol/tailwind-tooltip
```

With `yarn`

```bash
yarn add -D @ceol/tailwind-tooltip
```

Now edit the tailwind.config.js file to load the plugin as
shown below:

```js
// tailwind.config.js
  module.exports = {
    content: [ ... ],
    theme: { ... },
    plugins: [
      require('@ceol/tailwind-tooltip'),
   ],
 };
```

## How To Use

Below is an example snippet to use tooltip in the markup.

```html
  <div class="tt">Hover Me.
    <span class="tt-text tt-pos-top">Tooltip Text</span>
  </div>
```

The main div is given the `tt` class and the span element 
inside this div is given `tt-text` and also direction to 
mention the tooltip location.

Possible values currently for tooltip position are 
`tt-pos-top` and `tt-pos-bottom`.
