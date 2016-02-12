# preload-img [![travis][travis-image]][travis-url] [![npm][npm-image]][npm-url] [![downloads][downloads-image]][downloads-url]

[travis-image]: https://img.shields.io/travis/feross/preload-img/master.svg
[travis-url]: https://travis-ci.org/feross/preload-img
[npm-image]: https://img.shields.io/npm/v/preload-img.svg
[npm-url]: https://npmjs.org/package/preload-img
[downloads-image]: https://img.shields.io/npm/dm/preload-img.svg
[downloads-url]: https://npmjs.org/package/preload-img

### Preload an image on a webpage

Works best with [browserify](http://browserify.org/)!

## install

```
npm install preload-img
```

## usage

If you know you'll need to load an image later, you can preload it upfront (when
your web app loads) to make sure that it loads instantly later.

```js
var preload = require('preload-img')

preload('/img/spinner.gif')
preload('/img/another-image.png')
```

Works best when the image has far-future HTTP cache headers set.

## real-world example

You can see this module in action on [Magic Keyboard](http://magickeyboard.io/).
Check the Network Tab in the Web Inspector to see that an image for each letter of
the alphabet is loaded before the user has actually typed any letters.

## license

MIT. Copyright (c) [Feross Aboukhadijeh](http://feross.org).
