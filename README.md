## three-3dsloader

[THREE.TDSLoader](https://threejs.org/examples/js/loaders/TDSLoader.js) repackaged as a node module

另一个做了three-tds-loader，没法使用，顾自造轮子，但因名字冲突(太过相似)不得不取名three-3dsloader

## install

`npm i --save three-3dsloader`

## usage

```js

var THREE = require('three');
var TDSLoader = require('three-3dsloader');

var loader = new TDSLoader();

var scene = new THREE.Scene();

loader.load('./path/to/model.3ds', function (object3d) {
  scene.add(object3d);
});

```