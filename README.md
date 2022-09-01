<!--

@license Apache-2.0

Copyright (c) 2018 The Stdlib Authors.

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

# isAlphagram

[![NPM version][npm-image]][npm-url] [![Build Status][test-image]][test-url] [![Coverage Status][coverage-image]][coverage-url] <!-- [![dependencies][dependencies-image]][dependencies-url] -->

> Test if a value is an [alphagram][alphagram].

<section class="installation">

## Installation

```bash
npm install @stdlib/assert-is-alphagram
```

Alternatively,

-   To load the package in a website via a `script` tag without installation and bundlers, use the [ES Module][es-module] available on the [`esm` branch][esm-url].
-   If you are using Deno, visit the [`deno` branch][deno-url].
-   For use in Observable, or in browser/node environments, use the [Universal Module Definition (UMD)][umd] build available on the [`umd` branch][umd-url].

The [branches.md][branches-url] file summarizes the available branches and displays a diagram illustrating their relationships.

</section>

<section class="usage">

## Usage

```javascript
var isAlphagram = require( '@stdlib/assert-is-alphagram' );
```

#### isAlphagram( value )

Tests if a `value` is an [alphagram][alphagram] (i.e., a sequence of characters arranged in alphabetical order).

```javascript
var value = 'beep';

var bool = isAlphagram( value );
// returns true
```

</section>

<!-- /.usage -->

<section class="notes">

## Notes

-   The function first checks that an input `value` is a `string` before validating that the `value` is an [alphagram][alphagram]. For non-string values, the function returns `false`.

</section>

<!-- /.notes -->

<section class="examples">

## Examples

<!-- eslint-disable no-new-wrappers -->

<!-- eslint no-undef: "error" -->

```javascript
var isAlphagram = require( '@stdlib/assert-is-alphagram' );

var out = isAlphagram( 'beep' );
// returns true

out = isAlphagram( new String( 'beep' ) );
// returns true

out = isAlphagram( '' );
// returns false

out = isAlphagram( 'zba' );
// returns false

out = isAlphagram( 123 );
// returns false
```

</section>

<!-- /.examples -->

* * *

<section class="cli">

## CLI

<section class="installation">

## Installation

To use the module as a general utility, install the module globally

```bash
npm install -g @stdlib/assert-is-alphagram
```

</section>

<!-- CLI usage documentation. -->

<section class="usage">

### Usage

```text
Usage: is-alphagram [options] [<string>]

Options:

  -h,    --help                Print this message.
  -V,    --version             Print the package version.
```

</section>

<!-- /.usage -->

<section class="examples">

### Examples

```bash
$ is-alphagram beep
true
```

To use as a [standard stream][standard-streams],

```bash
$ echo -n 'hello' | is-alphagram
false
```

</section>

<!-- /.examples -->

</section>

<!-- /.cli -->

<!-- Section for related `stdlib` packages. Do not manually edit this section, as it is automatically populated. -->

<section class="related">

* * *

## See Also

-   <span class="package-name">[`@stdlib/assert/is-anagram`][@stdlib/assert/is-anagram]</span><span class="delimiter">: </span><span class="description">test if a value is an anagram.</span>

</section>

<!-- /.related -->

<!-- Section for all links. Make sure to keep an empty line after the `section` element and another before the `/section` close. -->


<section class="main-repo" >

* * *

## Notice

This package is part of [stdlib][stdlib], a standard library for JavaScript and Node.js, with an emphasis on numerical and scientific computing. The library provides a collection of robust, high performance libraries for mathematics, statistics, streams, utilities, and more.

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

[npm-image]: http://img.shields.io/npm/v/@stdlib/assert-is-alphagram.svg
[npm-url]: https://npmjs.org/package/@stdlib/assert-is-alphagram

[test-image]: https://github.com/stdlib-js/assert-is-alphagram/actions/workflows/test.yml/badge.svg?branch=main
[test-url]: https://github.com/stdlib-js/assert-is-alphagram/actions/workflows/test.yml?query=branch:main

[coverage-image]: https://img.shields.io/codecov/c/github/stdlib-js/assert-is-alphagram/main.svg
[coverage-url]: https://codecov.io/github/stdlib-js/assert-is-alphagram?branch=main

<!--

[dependencies-image]: https://img.shields.io/david/stdlib-js/assert-is-alphagram.svg
[dependencies-url]: https://david-dm.org/stdlib-js/assert-is-alphagram/main

-->

[chat-image]: https://img.shields.io/gitter/room/stdlib-js/stdlib.svg
[chat-url]: https://gitter.im/stdlib-js/stdlib/

[stdlib]: https://github.com/stdlib-js/stdlib

[stdlib-authors]: https://github.com/stdlib-js/stdlib/graphs/contributors

[umd]: https://github.com/umdjs/umd
[es-module]: https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules

[deno-url]: https://github.com/stdlib-js/assert-is-alphagram/tree/deno
[umd-url]: https://github.com/stdlib-js/assert-is-alphagram/tree/umd
[esm-url]: https://github.com/stdlib-js/assert-is-alphagram/tree/esm
[branches-url]: https://github.com/stdlib-js/assert-is-alphagram/blob/main/branches.md

[stdlib-license]: https://raw.githubusercontent.com/stdlib-js/assert-is-alphagram/main/LICENSE

[alphagram]: https://en.wiktionary.org/wiki/alphagram

[standard-streams]: https://en.wikipedia.org/wiki/Standard_streams

<!-- <related-links> -->

[@stdlib/assert/is-anagram]: https://github.com/stdlib-js/assert-is-anagram

<!-- </related-links> -->

</section>

<!-- /.links -->
