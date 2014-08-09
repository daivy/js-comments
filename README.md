# js-comments [![NPM version](https://badge.fury.io/js/js-comments.png)](http://badge.fury.io/js/js-comments)

> Parse JavaScript code comments and generate API documentation.

Please [report any bugs or feature requests](https://github.com/jonschlinkert/js-comments/issues/new), thanks!

## Install
#### [npm](npmjs.org)

```bash
npm i js-comments --save
```
#### Install with [bower](https://github.com/bower/bower)
```bash
npm i js-comments --save
```

#### [bower](https://github.com/bower/bower)

```bash
bower install js-comments --save
```

js-comments

## API
## [index](index.js)



```js
var comments = require('js-comments');
var docs = comments('lib/*.js');
```
See [example output](./test/actual/comments.json).
See [example code comments](./index.js).

* ``src``: {String} The source file path

* ``dest``: {String} Optional destination file path for generating relative links.

* ``options``: {Object}

## Author

**Jon Schlinkert**

+ [github/jonschlinkert](https://github.com/jonschlinkert)
+ [twitter/jonschlinkert](http://twitter.com/jonschlinkert)

## License
Copyright (c) 2014 Jon Schlinkert, contributors.  
Originally modified from scrawl.js. Copyright (c) 2014 [Caolan McMahon](https://github.com/caolan), contributors.
Released under the MIT license

***

_This file was generated by [verb-cli](https://github.com/assemble/verb-cli) on August 02, 2014._