# JS - SVG icons

## Synopsis

Package provide an unified library of [SVG](https://en.wikipedia.org/wiki/Scalable_Vector_Graphics) icons.
Initially based on [Google Material Icons](https://github.com/google/material-design-icons/)

### Motivation for creating this library

Font-based icons like **font-awesome** have a lot of **limitations**:

* *font-based icons* is a **global dependency**
* *font-based icons* are **not extendable**. You have no chance to easilly add a new icon
* Different browser have **different font render engines** *font-based-icons*

**Related articles on this topic**

* **[Chris Coyier](http://chriscoyier.net/about/)** ([CSS-Tricks](https://css-tricks.com/) and [codepen.io](http://codepen.io/) co-founder):

  [Inline SVG vs Icon Fonts](https://css-tricks.com/icon-fonts-vs-svg/)

* **[Lars Kappert](https://github.com/webpro)** :

  [Why and how I’m using SVG sprites over fonts for icons](https://medium.com/@webprolific/why-and-how-i-m-using-svg-over-fonts-for-icons-7241dab890f0#.5bc934hd5)

### Difference from base [Google Material Icons](https://github.com/google/material-design-icons/) library
* Much reduced resulting package size (~60MB vs ~500KB)
* Icon files paths normalized to `[package-name]/lib/[icon-name]`
* Removed hardcoded color values in a few icons

## Usage

### Installation
`npm install --save -E @opuscapita/svg-icons`

### Import an icon using webpack

```js
let buildIcon = require('!!raw-loader!@opuscapita/svg-icons/lib/build.svg');
```

In this way you get a raw *.svg* file content.

If `require` not working, ensure [raw-loader](https://www.npmjs.com/package/raw-loader) installed.

## License

OpusCapita 2016
