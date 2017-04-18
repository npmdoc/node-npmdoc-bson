# npmdoc-bson

#### api documentation for  [bson (v1.0.4)](https://github.com/mongodb/js-bson#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-bson.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-bson) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-bson.svg)](https://travis-ci.org/npmdoc/node-npmdoc-bson)

#### A bson parser for node.js and the browser

[![NPM](https://nodei.co/npm/bson.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/bson)

- [https://npmdoc.github.io/node-npmdoc-bson/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-bson/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-bson/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-bson/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-bson/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-bson/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Christian Amor Kvalheim"
    },
    "browser": "lib/bson/bson.js",
    "bugs": {
        "url": "https://github.com/mongodb/js-bson/issues"
    },
    "config": {
        "native": false
    },
    "contributors": [],
    "dependencies": {},
    "description": "A bson parser for node.js and the browser",
    "devDependencies": {
        "babel-core": "^6.14.0",
        "babel-loader": "^6.2.5",
        "babel-polyfill": "^6.13.0",
        "babel-preset-es2015": "^6.14.0",
        "babel-preset-stage-0": "^6.5.0",
        "babel-register": "^6.14.0",
        "benchmark": "1.0.0",
        "colors": "1.1.0",
        "nodeunit": "0.9.0",
        "webpack": "^1.13.2",
        "webpack-polyfills-plugin": "0.0.9"
    },
    "directories": {
        "lib": "./lib/bson"
    },
    "dist": {
        "shasum": "93c10d39eaa5b58415cbc4052f3e53e562b0b72c",
        "tarball": "https://registry.npmjs.org/bson/-/bson-1.0.4.tgz"
    },
    "engines": {
        "node": ">=0.6.19"
    },
    "files": [
        "lib",
        "index.js",
        "browser_build",
        "bower.json"
    ],
    "gitHead": "8dd35ca73c30a2bcab61615ccc5edd053aeb868b",
    "homepage": "https://github.com/mongodb/js-bson#readme",
    "keywords": [
        "mongodb",
        "bson",
        "parser"
    ],
    "license": "Apache-2.0",
    "main": "./index",
    "maintainers": [
        {
            "name": "octave"
        },
        {
            "name": "christkv"
        }
    ],
    "name": "bson",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/mongodb/js-bson.git"
    },
    "scripts": {
        "build": "webpack --config ./webpack.dist.config.js",
        "test": "nodeunit ./test/node"
    },
    "version": "1.0.4"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
