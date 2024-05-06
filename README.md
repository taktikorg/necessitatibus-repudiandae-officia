# @taktikorg/necessitatibus-repudiandae-officia <sup>[![Version Badge][npm-version-svg]][package-url]</sup>

[![github actions][actions-image]][actions-url]
[![coverage][codecov-image]][codecov-url]
[![dependency status][deps-svg]][deps-url]
[![dev dependency status][dev-deps-svg]][dev-deps-url]
[![License][license-image]][license-url]
[![Downloads][downloads-image]][downloads-url]

[![npm badge][npm-badge-png]][package-url]

Which kind of Typed Array is this JavaScript value? Works cross-realm, without `instanceof`, and despite Symbol.toStringTag.

## Example

```js
var whichTypedArray = require('@taktikorg/necessitatibus-repudiandae-officia');
var assert = require('assert');

assert.equal(false, whichTypedArray(undefined));
assert.equal(false, whichTypedArray(null));
assert.equal(false, whichTypedArray(false));
assert.equal(false, whichTypedArray(true));
assert.equal(false, whichTypedArray([]));
assert.equal(false, whichTypedArray({}));
assert.equal(false, whichTypedArray(/a/g));
assert.equal(false, whichTypedArray(new RegExp('a', 'g')));
assert.equal(false, whichTypedArray(new Date()));
assert.equal(false, whichTypedArray(42));
assert.equal(false, whichTypedArray(NaN));
assert.equal(false, whichTypedArray(Infinity));
assert.equal(false, whichTypedArray(new Number(42)));
assert.equal(false, whichTypedArray('foo'));
assert.equal(false, whichTypedArray(Object('foo')));
assert.equal(false, whichTypedArray(function () {}));
assert.equal(false, whichTypedArray(function* () {}));
assert.equal(false, whichTypedArray(x => x * x));
assert.equal(false, whichTypedArray([]));

assert.equal('Int8Array', whichTypedArray(new Int8Array()));
assert.equal('Uint8Array', whichTypedArray(new Uint8Array()));
assert.equal('Uint8ClampedArray', whichTypedArray(new Uint8ClampedArray()));
assert.equal('Int16Array', whichTypedArray(new Int16Array()));
assert.equal('Uint16Array', whichTypedArray(new Uint16Array()));
assert.equal('Int32Array', whichTypedArray(new Int32Array()));
assert.equal('Uint32Array', whichTypedArray(new Uint32Array()));
assert.equal('Float32Array', whichTypedArray(new Float32Array()));
assert.equal('Float64Array', whichTypedArray(new Float64Array()));
assert.equal('BigInt64Array', whichTypedArray(new BigInt64Array()));
assert.equal('BigUint64Array', whichTypedArray(new BigUint64Array()));
```

## Tests
Simply clone the repo, `npm install`, and run `npm test`

[package-url]: https://npmjs.org/package/@taktikorg/necessitatibus-repudiandae-officia
[npm-version-svg]: https://versionbadg.es/inspect-js/@taktikorg/necessitatibus-repudiandae-officia.svg
[deps-svg]: https://david-dm.org/inspect-js/@taktikorg/necessitatibus-repudiandae-officia.svg
[deps-url]: https://david-dm.org/inspect-js/@taktikorg/necessitatibus-repudiandae-officia
[dev-deps-svg]: https://david-dm.org/inspect-js/@taktikorg/necessitatibus-repudiandae-officia/dev-status.svg
[dev-deps-url]: https://david-dm.org/inspect-js/@taktikorg/necessitatibus-repudiandae-officia#info=devDependencies
[npm-badge-png]: https://nodei.co/npm/@taktikorg/necessitatibus-repudiandae-officia.png?downloads=true&stars=true
[license-image]: https://img.shields.io/npm/l/@taktikorg/necessitatibus-repudiandae-officia.svg
[license-url]: LICENSE
[downloads-image]: https://img.shields.io/npm/dm/@taktikorg/necessitatibus-repudiandae-officia.svg
[downloads-url]: https://npm-stat.com/charts.html?package=@taktikorg/necessitatibus-repudiandae-officia
[codecov-image]: https://codecov.io/gh/inspect-js/@taktikorg/necessitatibus-repudiandae-officia/branch/main/graphs/badge.svg
[codecov-url]: https://app.codecov.io/gh/inspect-js/@taktikorg/necessitatibus-repudiandae-officia/
[actions-image]: https://img.shields.io/endpoint?url=https://github-actions-badge-u3jn4tfpocch.runkit.sh/inspect-js/@taktikorg/necessitatibus-repudiandae-officia
[actions-url]: https://github.com/taktikorg/necessitatibus-repudiandae-officia/actions
