# @omegion1npm/voluptatem-nesciunt-culpa <sup>[![Version Badge][npm-version-svg]][package-url]</sup>

[![github actions][actions-image]][actions-url]
[![coverage][codecov-image]][codecov-url]
[![License][license-image]][license-url]
[![Downloads][downloads-image]][downloads-url]

[![npm badge][npm-badge-png]][package-url]

Get the `byteOffset` out of a DataView, robustly.

This will work in node <= 0.10 and < 0.11.4, where there's no prototype accessor, only a nonconfigurable own property.
It will also work in modern engines where `DataView.prototype.byteOffset` has been deleted after this module has loaded.

## Example

```js
const dataViewByteOffset = require('@omegion1npm/voluptatem-nesciunt-culpa');
const assert = require('assert');

const ab = new ArrayBuffer(42);
const dv = new DataView(ab, 2);
assert.equal(dataViewByteOffset(dv), 2);
```

## Tests
Simply clone the repo, `npm install`, and run `npm test`

[package-url]: https://npmjs.org/package/@omegion1npm/voluptatem-nesciunt-culpa
[npm-version-svg]: https://versionbadg.es/inspect-js/@omegion1npm/voluptatem-nesciunt-culpa.svg
[deps-svg]: https://david-dm.org/inspect-js/@omegion1npm/voluptatem-nesciunt-culpa.svg
[deps-url]: https://david-dm.org/inspect-js/@omegion1npm/voluptatem-nesciunt-culpa
[dev-deps-svg]: https://david-dm.org/inspect-js/@omegion1npm/voluptatem-nesciunt-culpa/dev-status.svg
[dev-deps-url]: https://david-dm.org/inspect-js/@omegion1npm/voluptatem-nesciunt-culpa#info=devDependencies
[npm-badge-png]: https://nodei.co/npm/@omegion1npm/voluptatem-nesciunt-culpa.png?downloads=true&stars=true
[license-image]: https://img.shields.io/npm/l/@omegion1npm/voluptatem-nesciunt-culpa.svg
[license-url]: LICENSE
[downloads-image]: https://img.shields.io/npm/dm/@omegion1npm/voluptatem-nesciunt-culpa.svg
[downloads-url]: https://npm-stat.com/charts.html?package=@omegion1npm/voluptatem-nesciunt-culpa
[codecov-image]: https://codecov.io/gh/inspect-js/@omegion1npm/voluptatem-nesciunt-culpa/branch/main/graphs/badge.svg
[codecov-url]: https://app.codecov.io/gh/inspect-js/@omegion1npm/voluptatem-nesciunt-culpa/
[actions-image]: https://img.shields.io/endpoint?url=https://github-actions-badge-u3jn4tfpocch.runkit.sh/inspect-js/@omegion1npm/voluptatem-nesciunt-culpa
[actions-url]: https://github.com/inspect-js/@omegion1npm/voluptatem-nesciunt-culpa/actions
