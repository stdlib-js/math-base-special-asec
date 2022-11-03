<!--

@license Apache-2.0

Copyright (c) 2022 The Stdlib Authors.

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

   http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

-->

# asec

[![NPM version][npm-image]][npm-url] [![Build Status][test-image]][test-url] [![Coverage Status][coverage-image]][coverage-url] <!-- [![dependencies][dependencies-image]][dependencies-url] -->

> Compute the [inverse (arc) secant][arcsecant] of a number.



<section class="usage">

## Usage

```javascript
import asec from 'https://cdn.jsdelivr.net/gh/stdlib-js/math-base-special-asec@deno/mod.js';
```

#### asec( x )

Computes the [inverse (arc) secant][arcsecant] of `x`.

```javascript
var v = asec( 1.0 );
// returns 0.0

v = asec( 2.0 );
// returns ~1.0472

v = asec( NaN );
// returns NaN
```

The domain of `x` is restricted to the intervals `[-inf, -1]` and `[1, inf]`. For `x` outside of these intervals, the function returns `NaN`.

```javascript
var v = asec( -0.5 );
// returns NaN

v = asec( 0.5 );
// returns NaN
```

</section>

<!-- /.usage -->

<section class="examples">

## Examples

<!-- eslint no-undef: "error" -->

```javascript
import linspace from 'https://cdn.jsdelivr.net/gh/stdlib-js/array-base-linspace@deno/mod.js';
import asec from 'https://cdn.jsdelivr.net/gh/stdlib-js/math-base-special-asec@deno/mod.js';

var x = linspace( 1.0, 10.0, 100 );

var i;
for ( i = 0; i < x.length; i++ ) {
    console.log( asec( x[ i ] ) );
}
```

</section>

<!-- /.examples -->

<!-- Section for related `stdlib` packages. Do not manually edit this section, as it is automatically populated. -->

<section class="related">

</section>

<!-- /.related -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->


<section class="main-repo" >

* * *

## Notice

This package is part of [stdlib][stdlib], a standard library with an emphasis on numerical and scientific computing. The library provides a collection of robust, high performance libraries for mathematics, statistics, streams, utilities, and more.

For more information on the project, filing bug reports and feature requests, and guidance on how to develop [stdlib][stdlib], see the main project [repository][stdlib].

#### Community

[![Chat][chat-image]][chat-url]

---

## License

See [LICENSE][stdlib-license].


## Copyright

Copyright &copy; 2016-2022. The Stdlib [Authors][stdlib-authors].

</section>

<!-- /.stdlib -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->

<section class="links">

[npm-image]: http://img.shields.io/npm/v/@stdlib/math-base-special-asec.svg
[npm-url]: https://npmjs.org/package/@stdlib/math-base-special-asec

[test-image]: https://github.com/stdlib-js/math-base-special-asec/actions/workflows/test.yml/badge.svg?branch=v0.0.1
[test-url]: https://github.com/stdlib-js/math-base-special-asec/actions/workflows/test.yml?query=branch:v0.0.1

[coverage-image]: https://img.shields.io/codecov/c/github/stdlib-js/math-base-special-asec/main.svg
[coverage-url]: https://codecov.io/github/stdlib-js/math-base-special-asec?branch=main

<!--

[dependencies-image]: https://img.shields.io/david/stdlib-js/math-base-special-asec.svg
[dependencies-url]: https://david-dm.org/stdlib-js/math-base-special-asec/main

-->

[chat-image]: https://img.shields.io/gitter/room/stdlib-js/stdlib.svg
[chat-url]: https://gitter.im/stdlib-js/stdlib/

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[umd]: https://github.com/umdjs/umd
[es-module]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules

[deno-url]: https://github.com/stdlib-js/math-base-special-asec/tree/deno
[umd-url]: https://github.com/stdlib-js/math-base-special-asec/tree/umd
[esm-url]: https://github.com/stdlib-js/math-base-special-asec/tree/esm
[branches-url]: https://github.com/stdlib-js/math-base-special-asec/blob/main/branches.md

[stdlib-license]: https://raw.githubusercontent.com/stdlib-js/math-base-special-asec/main/LICENSE

[arcsecant]: https://en.wikipedia.org/wiki/Inverse_trigonometric_functions

</section>

<!-- /.links -->
