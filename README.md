# karma-chai-as-promised
chai-as-promised plugin for karma

[![NPM version](https://badge.fury.io/js/karma-chai-as-promised.svg)](http://badge.fury.io/js/validate-it) [![Dependency Status](https://david-dm.org/vlkosinov/karma-chai-as-promised.svg)](https://david-dm.org/vlkosinov/validate-it)

## Installation
```sh
$ npm install karma-chai-as-promised --save-dev
```
   
## Requirements

This Karma plugin requires Karma `>=0.10.9` and Chai `^2.1.2`
  
## Usage

Add `chai-as-promised` to the `frameworks` array in your Karma configuration:

```js
module.exports = function(config) {
  'use strict';
  config.set({
    frameworks: ['mocha', 'chai-as-promised', 'chai'],
    #...
  });
}
```

Keep in mind that, since Karma loads its frameworks in reverse and `chai-as-promised'` depends on `chai`, you should declare it accordingly as done above.

License
----

MIT
