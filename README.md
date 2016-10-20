[![npm version 0.0.4](https://badge.fury.io/js/truncated.js.svg)](https://www.npmjs.com/package/dollarshaveclub/shave)
[![Bower version 0.0.2](https://badge.fury.io/bo/truncated.js.svg)](https://github.com/yowainwright/dollarshaveclub/shave)

# Shave

> Shave text for smooth looking content within a specified space.

Shave is a javascript text truncation plugin that doesn't get in the way. It is an alternative to `text-overflow: ellipsis;` in that it will truncate *multi-line* text.

## Setup

```sh
npm i shave --save-dev
# or
bower i shave --save-dev
```

## Run

1. Add **dist/shave.js**.
3. `shave` text within the element you'd like to.

## Basic Examples
```javascript
shave('#foo'); // Shave a single element
shave('.bar'); // Shave multiple elements
shave('selector:not([not this selector])'); // Complex selectors
shave('selector', maxHeight); // Sets the max-height of the element
shave('selector', maxHeight, '🍻'); // Different character instead of an ellipsis
shave('selector', maxHeight, '🙌', 'your-css-class'); // Adds a custom class name
$('selector').shave(maxHeight); // Or with jQuery
```

## How?

**Shave.js** shaves an element's text string to the last full word that can fit within a specified max height.

## Why?

**Shave.js** is made for simplicity; it doesn't try to over solve truncation or provide tons of options. It truncates text to a specified max height.

## What about the original text?

**Shave.js** re-adds the _diff_ of the original selected element's text in a hidden `<span>`. It runs a check for that `<span>` to make sure text is shaved properly every time.

## What about size?

**Shave.js** is small - `~1.5kb` unminified and is meant to do 1 thing - _shave text to fit beautifully to a specified max height_.

## How can I use it?

You can use **Shave.js** in all modern formats and as a `jQuery` or `Zepto` plugin.

## Examples

[codepen example](http://codepen.io/yowainwright/pen/5f471214df90f43c7996c5914c88e858/) with plain javascript.

[Codepen example](http://codepen.io/yowainwright/pen/c35ad7a281bc58ce6f89d2adb94c5d14/) with jQuery.
