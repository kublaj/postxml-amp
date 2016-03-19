# postxml-amp
[![npm version][npm-image]][npm-url]
[![Downloads Stats][npm-downloads]][npm-url]

> [PostXML] plugin to convert plain HTML to Google Accelerated Mobile Pages (AMP).

## Installation
`npm install postxml-amp --save-dev`

## Usage
[Postxml]

## Options
### cwd
**Assets (images/styles) file path**<br>
Type: `String`<br>
Default: `''`

### round
**Enable images dimensions rounding**<br>
Type: `String`<br>
Default: `true`

## Example

### Input
```html
<html><head><link rel="stylesheet" href="style.css"></head><img src="image.png"></html>
```

###### image.png
[image.png](/test/image.png)

###### style.css
```css
body {
  background-color: #FFF;
}
```

### Output
```html
<html amp=""><head><style amp-custom="">body{background-color:#FFF}</style></head><amp-img src="image.png" width="600" height="400"></amp-img></html>
```

## Licence
MIT

[PostXML]: https://github.com/postxml/postxml
[npm-url]: https://www.npmjs.org/package/postxml-amp
[npm-image]: https://img.shields.io/npm/v/postxml-amp.svg?style=flat-square
[npm-downloads]: https://img.shields.io/npm/dm/postxml-amp.svg?style=flat-square
