# npmdoc-jslint

api documentation for  [jslint (v0.10.3)](https://github.com/reid/node-jslint)  [![npm package](https://img.shields.io/npm/v/npmdoc-jslint.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-jslint) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-jslint.svg)](https://travis-ci.org/npmdoc/node-npmdoc-jslint)

The JavaScript Code Quality Tool

[![NPM](https://nodei.co/npm/jslint.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/jslint)

- [https://npmdoc.github.io/node-npmdoc-jslint/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-jslint/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-jslint/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-jslint/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-jslint/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-jslint/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Reid Burke"
    },
    "bin": {
        "jslint": "./bin/jslint.js"
    },
    "bugs": {
        "url": "https://github.com/reid/node-jslint/issues"
    },
    "contributors": [
        {
            "name": "Douglas Crockford"
        },
        {
            "name": "Mikeal Rogers"
        },
        {
            "name": "Adam Moore"
        },
        {
            "name": "Luke Smith"
        },
        {
            "name": "Anders Conbere"
        },
        {
            "name": "Ryuichi OKUMURA"
        },
        {
            "name": "Sam Mikes"
        },
        {
            "name": "Dylan Lloyd"
        },
        {
            "name": "Andreas Hindborg"
        },
        {
            "name": "Andrew Pennebaker"
        },
        {
            "name": "Bnaya"
        },
        {
            "name": "Maximilian Antoni"
        },
        {
            "name": "Vasil Velichkov"
        },
        {
            "name": "Rasmus Paetau"
        },
        {
            "name": "Bryan Horna"
        }
    ],
    "dependencies": {
        "exit": "~0.1.2",
        "glob": "^7.0.3",
        "nopt": "~3.0.1",
        "readable-stream": "~2.1.2"
    },
    "description": "The JavaScript Code Quality Tool",
    "devDependencies": {
        "fs.extra": "^1.3.2",
        "istanbul": "^0.4.3",
        "marked-man": "~0.1.5",
        "mocha": "^3.0.0"
    },
    "directories": {
        "lib": "./lib",
        "man": "./man",
        "doc": "./doc"
    },
    "dist": {
        "shasum": "890da3e79932edf06c5f4b52a7b5ba6436867436",
        "tarball": "https://registry.npmjs.org/jslint/-/jslint-0.10.3.tgz"
    },
    "engines": {
        "node": ">=0.8.0"
    },
    "files": [
        "man/jslint.1",
        "doc/jslint.md",
        "doc/jslint.html",
        "lib",
        "bin",
        "jslint.conf.example",
        "Makefile"
    ],
    "gitHead": "c2cdb60176983c5e4e93aebbcba1d8c2c93ac416",
    "homepage": "https://github.com/reid/node-jslint",
    "keywords": [
        "lint",
        "jslint",
        "code-quality",
        "static-analysis",
        "jshint",
        "eslint"
    ],
    "license": "BSD-3-Clause",
    "licenses": [
        {
            "type": "Modified MIT / BSD",
            "url": "https://github.com/reid/node-jslint/blob/master/LICENSE"
        }
    ],
    "main": "./lib/nodelint.js",
    "maintainers": [
        {
            "name": "reid"
        },
        {
            "name": "okuryu"
        },
        {
            "name": "smikes"
        }
    ],
    "man": [
        "man/jslint.1"
    ],
    "name": "jslint",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git://github.com/reid/node-jslint.git"
    },
    "scripts": {
        "mypublish": "make prepublish; npm publish",
        "test": "make test"
    },
    "version": "0.10.3"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
