# [gulp](https://github.com/wearefractal/gulp)-traceur [![Build Status](https://secure.travis-ci.org/sindresorhus/gulp-traceur.png?branch=master)](http://travis-ci.org/sindresorhus/gulp-traceur)

> [Traceur](https://github.com/google/traceur-compiler) is a JavaScript.next to JavaScript-of-today compiler

*Issues with the output should be reported on the Traceur [issue tracker](https://github.com/google/traceur-compiler/issues).*


## Install

Install with [npm](https://npmjs.org/package/gulp-traceur)

```
npm install --save-dev gulp-traceur
```


## Example

```js
var gulp = require('gulp');
var traceur = require('gulp-traceur');

gulp.task('default', function () {
	gulp.src('src/app.js')
		.pipe(traceur())
		.pipe(gulp.dest('dist'));
});
```


## API

### traceur(options)

[Options](https://github.com/google/traceur-compiler/issues/584) are passed through to Traceur, except for `options.filename` which is set for you.


## License

MIT © [Sindre Sorhus](http://sindresorhus.com)
