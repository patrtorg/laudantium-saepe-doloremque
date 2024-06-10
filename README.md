# @patrtorg/laudantium-saepe-doloremque <sup>[![Version Badge][npm-version-svg]][package-url]</sup>

[![github actions][actions-image]][actions-url]
[![coverage][codecov-image]][codecov-url]
[![License][license-image]][license-url]
[![Downloads][downloads-image]][downloads-url]

[![npm badge][npm-badge-png]][package-url]

`Object.defineProperty`, but not IE 8's broken one.

## Example

```js
const assert = require('assert');

const $defineProperty = require('@patrtorg/laudantium-saepe-doloremque');

if ($defineProperty) {
    assert.equal($defineProperty, Object.defineProperty);
} else if (Object.defineProperty) {
    assert.equal($defineProperty, false, 'this is IE 8');
} else {
    assert.equal($defineProperty, false, 'this is an ES3 engine');
}
```

## Tests
Simply clone the repo, `npm install`, and run `npm test`

## Security

Please email [@ljharb](https://github.com/ljharb) or see https://tidelift.com/security if you have a potential security vulnerability to report.

[package-url]: https://npmjs.org/package/@patrtorg/laudantium-saepe-doloremque
[npm-version-svg]: https://versionbadg.es/ljharb/@patrtorg/laudantium-saepe-doloremque.svg
[deps-svg]: https://david-dm.org/ljharb/@patrtorg/laudantium-saepe-doloremque.svg
[deps-url]: https://david-dm.org/ljharb/@patrtorg/laudantium-saepe-doloremque
[dev-deps-svg]: https://david-dm.org/ljharb/@patrtorg/laudantium-saepe-doloremque/dev-status.svg
[dev-deps-url]: https://david-dm.org/ljharb/@patrtorg/laudantium-saepe-doloremque#info=devDependencies
[npm-badge-png]: https://nodei.co/npm/@patrtorg/laudantium-saepe-doloremque.png?downloads=true&stars=true
[license-image]: https://img.shields.io/npm/l/@patrtorg/laudantium-saepe-doloremque.svg
[license-url]: LICENSE
[downloads-image]: https://img.shields.io/npm/dm/@patrtorg/laudantium-saepe-doloremque.svg
[downloads-url]: https://npm-stat.com/charts.html?package=@patrtorg/laudantium-saepe-doloremque
[codecov-image]: https://codecov.io/gh/ljharb/@patrtorg/laudantium-saepe-doloremque/branch/main/graphs/badge.svg
[codecov-url]: https://app.codecov.io/gh/ljharb/@patrtorg/laudantium-saepe-doloremque/
[actions-image]: https://img.shields.io/endpoint?url=https://github-actions-badge-u3jn4tfpocch.runkit.sh/ljharb/@patrtorg/laudantium-saepe-doloremque
[actions-url]: https://github.com/patrtorg/laudantium-saepe-doloremque/actions
