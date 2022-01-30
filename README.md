# Colormath 🎨

Colormath is a color conversion and color manipulation library written in typescript for Node.js, Deno and Browser.

```js
const colors = require('colormath');

console.log(colors.rgb.toHex([255, 255, 255])); // '#ffffff'
console.log(colors.hex.toRgb('fff')); // [255, 255, 255]
```

## Installation

Using colormath through Node.js

```js
const colormath = require('colormath');
```

Using colormath through Browser

```html
<script src="https://cdn.skypack.dev/colormath@latest?min"></script>
```

Using colormath through Deno

```js
import * as colors from 'https://cdn.skypack.dev/colormath?dts';
```

## Supported Conversions

These are supported color conversions from A to B suported by the library.

> Only conversions which are used by people are added to the library and if you feel some of the unavailable color conversions are useful then you can create an issue or create a pr if you are able to add it yourself.

| ⬇ A \ B ➡  | rgb | hex | hsv | hsl | hwb | lab | lch | xyz | cmyk | ansi16 | ansi256 | gray |
|---------|-----|-----|-----|-----|-----|-----|-----|-----|------|--------|---------|------|
| rgb |  | ✔ | ✔ | ✔ | ✔ | ✔ | ❌ | ✔ | ✔ | ✔ | ✔ | ✔ |
| hex | ✔ |  | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ |
| hsv | ✔ | ✔ |  | ✔ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ |
| hsl | ✔ | ✔ | ✔ |  | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ |
| hwb | ✔ | ✔ | ❌ | ❌ |  | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ |
| lab | ✔ | ❌ | ❌ | ❌ | ❌ |  | ✔ | ✔ | ❌ | ❌ | ❌ | ❌ |
| lch | ❌ | ❌ | ❌ | ❌ | ❌ | ✔ |  | ❌ | ❌ | ❌ | ❌ | ❌ |
| xyz | ✔ | ❌ | ❌ | ❌ | ❌ | ✔ | ❌ |  | ❌ | ❌ | ❌ | ❌ |
| cmyk | ✔ | ✔ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ |  | ❌ | ❌ | ❌ |
| ansi16 | ✔ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ |  | ❌ | ❌ |
| ansi256 | ✔ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ |  | ❌ |
| gray | ✔ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ | ❌ |  |

- ✔ means the color conversion is supported.
- ❌ means the color conversion is not supported.

## Things to be added

- Support for `alpha` and string conversions.
- Find a better way to do `ColorResult`.
- Extracting colors from images.
- More color manipulation methods.

## Help

If any doubts, bugs or reports regarding the module or the documentation you can create an [issue](https://github.com/scientific-dev/colormath/issues) in github.