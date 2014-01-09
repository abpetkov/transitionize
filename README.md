# Transitionize

## Description

Transitionize helps you to create CSS3 transitions dynamically to elements of your choice. This helps in cases where you need different transition properties or transition speed for the same element, but for different events, for example.

The idea came when I needed a simpler way to do that for another project of mine - [Switchery](https://github.com/abpetkov/switchery), where I had to change some of the properties speed when checking/unchecking the switchery.

## Installation

##### Standalone:

```html
<script src="dist/transitionize.js"></script>
```

##### NPM:

```shell
$ npm install transitionize
```

##### Component:

```shell
$ component install abpetkov/transitionize
```

##### Bower:

```shell
$ bower install transitionize
```

## Usage

```js
var elem = document.querySelector('.js-elem');
var prop = { 'key': 'value' };
var init = new Transitionize(elem, prop);
```

To run the example in this repository, with [Browserify](http://browserify.org/) already installed, execute the following command:

```shell
  browserify examples/browserify.js -o examples/bundle.js
```

## Examples

You can make as many keys as you want and they will work as long as they are CSS valid properties.

```js
var prop = {
    'border': '0.3s'
  , 'box-shadow': '0.3s'
  , 'text-shadow': '0.8s'
};
```

If you'd like to specify the `transition-timing-function` or the `transition-delay`, do it like so:

```js
var prop = {
  'background-color': '0.3s ease-in 1s'
};
```

## Development

If you've decided to go in development mode and tweak all of this a little bit, there are few things you should do.

After you clone the repository, do this in your terminal ([NPM](http://npmjs.org/) required):

```shell
$ npm install
```

Add the following code before the rest:

```js
var Transitionize = require('transitionize');
```

Make sure you're using the `build/build.js` file and you're ready.

There are some useful commands you can use.

`$ make install` - will install Node.js modules, components etc.

`$ make build` - will create a build file

`$ make standalone` - will create a standalone and minified files

## Contact

If you like this and want to see more of my work, share your appreciation by following me in [Twitter](https://twitter.com/abpetkov), [GitHub](https://github.com/abpetkov) or [Dribbble](http://dribbble.com/apetkov).

## License

The MIT License (MIT)

Copyright (c) 2013 Alexander Petkov

Permission is hereby granted, free of charge, to any person obtaining a copy of
this software and associated documentation files (the "Software"), to deal in
the Software without restriction, including without limitation the rights to
use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
the Software, and to permit persons to whom the Software is furnished to do so,
subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS
FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR
COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER
IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN
CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.