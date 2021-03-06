# ng-input-currency

[![Build Status](https://travis-ci.org/aspcanada/ng-input-currency.svg?branch=master)](https://travis-ci.org/aspcanada/ng-input-currency)

[build]: https://img.shields.io/travis/project/aspcanada/ng-input-currency.svg?branch=master&style=flat-square
[coverage]: http://img.shields.io/coveralls/aspcanada/ng-input-currency.svg?branch=master&style=flat-square
[bower]: https://img.shields.io/bower/v/ng-input-currency.svg?style=flat-square
[npm]: https://img.shields.io/npm/v/ng-input-currency.svg?style=flat-square

Angular directive for formatting inputs as currency fields. This repo is inspired by [format-as-currency](https://github.com/bcherny/format-as-currency).

## Demo

http://aspcanada.github.io/ng-input-currency/demo

## Installation

Install via bower:

- Bower: `bower install git://github.com/aspcanada/ng-input-currency`

## Usage

```html
<div ng-controller="myController">
  <input ng-input-currency ng-model="value" type="text">
</div>

<script src="bower_components/angular/angular.js"></script>
<script src="bower_components/ng-input-currency/dist/ng-input-currency.js"></script>
<script>
  angular
  .module('myModule', ['ngInputCurrency'])
  .controller('myController', function ($scope) {
    $scope.value = '' // currency input value
  });
</script>
```

### With a module loader

#### Browserify

```js
var formatAsCurrency = require('ng-input-currency')
angular.module('myModule', [ngInputCurrency])
```

#### Rollup

```js
import * as ngInputCurrency from 'ng-input-currency'
angular.module('myModule', [ngInputCurrency])
```

#### Webpack

```js
var ngInputCurrency = require('ng-input-currency')
angular.module('myModule', [ngInputCurrency])
```

## Running the tests

```sh
npm test
```

## Contributing

Contributions are welcome!
