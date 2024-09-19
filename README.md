# reinarpg-square
[![NPM version](https://img.shields.io/npm/v/reinarpg-square.svg)](http://npmjs.com/package/reinarpg-square)
[![Build Status](https://github.com/PrismarineJS/reinarpg-square/workflows/CI/badge.svg)](https://github.com/PrismarineJS/reinarpg-square/actions?query=workflow%3A%22CI%22)

A diamond square minecraft generation

## Usage

```js
const World = require('reinarpg-world')('1.12')
const Vec3 = require('vec3').Vec3

const diamondSquare = require('reinarpg-square')({version: '1.12', seed: Math.floor(Math.random() * Math.pow(2, 31))})
const world = new World(diamondSquare)

world.getBlock(new Vec3(3, 50, 3)).then(block => console.log(JSON.stringify(block, null, 2)))
```

## Contributors

* @JWo1F did the initial code for reinarpg-square in reinarpg-server
* @demipixel
* @rom1504

## History

### 1.3.0

* Bump mcdata

### 1.2.0

* add 1.13 support (thanks @Deudly)

### 1.1.0

* convert to standard + make api compatible with multiple versions

### 1.0.0

* update dependencies

### 0.0.0

* first version, imported from reinarpg-server, works
