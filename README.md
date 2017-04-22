# npmdoc-restle

#### api documentation for  [restle (v0.6.0)](http://restle.io)  [![npm package](https://img.shields.io/npm/v/npmdoc-restle.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-restle) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-restle.svg)](https://travis-ci.org/npmdoc/node-npmdoc-restle)

#### JSON API engine.

[![NPM](https://nodei.co/npm/restle.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/restle)

- [https://npmdoc.github.io/node-npmdoc-restle/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-restle/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-restle/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-restle/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-restle/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-restle/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Dylan Slack",
        "url": "http://dylanslack.com/"
    },
    "bin": {
        "restle": "./bin/restle"
    },
    "bugs": {
        "url": "https://github.com/dylnslck/restle/issues"
    },
    "dependencies": {
        "babel": "^5.6.14",
        "bluebird": "^2.9.34",
        "body-parser": "^1.10.1",
        "commander": "^2.8.1",
        "cors": "^2.7.1",
        "error-class": "^2.0.0",
        "express": "^4.7.2",
        "i": "^0.3.3",
        "lodash": "^3.10.1",
        "prompt": "^0.2.14",
        "restle-error": "0.0.5",
        "restle-memory": "^0.1.0",
        "string-template": "^0.2.1"
    },
    "description": "JSON API engine.",
    "devDependencies": {
        "babel-eslint": "^4.0.5",
        "coveralls": "^2.11.3",
        "documentation": "^3.0.4",
        "eslint": "^0.24.1",
        "faker": "^3.0.1",
        "mkdirp": "^0.5.1",
        "rimraf": "^2.4.0",
        "superagent-as-promised": "^3.2.1",
        "supertest": "^1.0.1",
        "tap-spec": "^4.0.2",
        "tape": "^4.2.1"
    },
    "directories": {},
    "dist": {
        "shasum": "eb775de05bce9c6107aeb73ba1b1b8ad5317968d",
        "tarball": "https://registry.npmjs.org/restle/-/restle-0.6.0.tgz"
    },
    "files": [
        "dist/lib",
        "dist/test",
        "lib/",
        "test/",
        "bin/",
        "LICENSE"
    ],
    "gitHead": "c311b13b21c2deec0d1b916fb76e85e165056c90",
    "homepage": "http://restle.io",
    "keywords": [
        "rest",
        "api",
        "express",
        "node",
        "ember-data"
    ],
    "license": "MIT",
    "main": "dist/lib/index.js",
    "maintainers": [
        {
            "name": "dcslack"
        }
    ],
    "name": "restle",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/dylnslck/restle.git"
    },
    "scripts": {
        "build": "npm run build:lib && npm run build:test",
        "build:lib": "mkdirp dist/lib && babel lib --out-dir dist/lib",
        "build:test": "mkdirp dist/test && babel test --out-dir dist/test",
        "clean": "rimraf dist coverage",
        "prepublish": "npm run clean && npm run build",
        "test": "npm run test:lint && npm run test:server",
        "test:coverage": "istanbul cover dist/test",
        "test:lint": "eslint lib test",
        "test:server": "npm run clean && npm run build && tape dist/test | tap-spec"
    },
    "version": "0.6.0"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
