## three-tdsloader

[THREE.TDSLoader](https://threejs.org/examples/js/loaders/TDSLoader.js) repackaged as a node module

## install

`npm i --save three-tdsloader`

## usage

```js

var THREE = require('three');
var TDSLoader = require('three-tdsloader');

var loader = new TDSLoader();

var scene = new THREE.Scene();

loader.load('./path/to/model.3ds', function (object3d) {
  scene.add(object3d);
});

```