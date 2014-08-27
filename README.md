# js-comments [![NPM version](https://badge.fury.io/js/js-comments.png)](http://badge.fury.io/js/js-comments)

> Parse JavaScript code comments and generate API documentation.

Please [report any bugs or feature requests](https://github.com/jonschlinkert/js-comments/issues/new), thanks! Also, **please note**, custom filtering for comments is being implemented, but in the meantime only comments that have `@api public` will be rendered!

## Install

#### [npm](npmjs.org)

```bash
npm i js-comments --save-dev
```

#### [bower](https://github.com/bower/bower)

```bash
bower install js-comments --save-dev
```

## API
## [jscomments](index.js#L44)

* `patterns` **{String}**: Glob pattern or file paths to use.    
* `dest` **{String}**: Optional destination file path for generating relative links.    
* `options` **{Object}**    
* `returns` **{String}**: String of rendered markdown documentation.  

```js
var comments = require('js-comments');
var docs = comments(string);
```
See [example output](./test/actual/comments.json).
See [example code comments](./index.js).

## [.parseFiles](index.js#L61)

* `patterns` **{String}**: Glob pattern or file paths to use.    
* `dest` **{String}**: Optional destination file path for generating relative links.    
* `options` **{Object}**    
* `returns` **{Array}**: Returns an array of comments objects.  

Expands the given glob `patterns` and creates a normalized
`comments` object for each file in the array.

## [.render](index.js#L90)

* `context` **{Object}**    
* `options` **{Object}**    
* `returns` **{String}**: Return the rendered string.  

Render a template string with the given `context`. A
custom lodash template may be passed on the options.

## Author

**Jon Schlinkert**

+ [github/jonschlinkert](https://github.com/jonschlinkert)
+ [twitter/jonschlinkert](http://twitter.com/jonschlinkert)

## License

Copyright (c) 2014 Jon Schlinkert, contributors.  
Originally modified from scrawl.js. Copyright (c) 2014 [Caolan McMahon](https://github.com/caolan), contributors.
Released under the MIT license

***

_This file was generated by [verb-cli](https://github.com/assemble/verb-cli) on August 27, 2014._