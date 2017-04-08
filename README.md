# gulp-json5-to-json

A gulp plugin to convert JSON5 to strict JSON.

[![NPM Version][npm-image]][npm-url]

## Installation

```
$ npm install --save-dev gulp-json5-to-json
```

## Usage

```js
const gulp = require('gulp');
const json5 = require('gulp-json5-to-json');

gulp.task('default', () => {
  return gulp.src('src/**/*.json5')
    .pipe(json5({ beautify: true }))
    .pipe(gulp.dest('./build'));
});
```

### Options

- `beautify` - Causes the resulting file to be pretty-printed.

## License

[MIT](LICENSE)

[npm-image]: https://img.shields.io/npm/v/gulp-json5-to-json.svg?style=flat-square
[npm-url]: https://npmjs.org/package/gulp-json5-to-json
