# npmdoc-streamqueue

#### basic api documentation for  [streamqueue (v1.1.1)](https://github.com/nfroidure/StreamQueue)  [![npm package](https://img.shields.io/npm/v/npmdoc-streamqueue.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-streamqueue) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-streamqueue.svg)](https://travis-ci.org/npmdoc/node-npmdoc-streamqueue)

#### Pipe queued streams progressively, keeping datas order.

[![NPM](https://nodei.co/npm/streamqueue.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/streamqueue)

- [https://npmdoc.github.io/node-npmdoc-streamqueue/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-streamqueue/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-streamqueue/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-streamqueue/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-streamqueue/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-streamqueue/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Nicolas Froidure",
        "url": "http://www.insertafter.com/blog.html"
    },
    "bugs": {
        "url": "https://github.com/nfroidure/StreamQueue/issues"
    },
    "dependencies": {
        "isstream": "^0.1.2",
        "readable-stream": "~1.0.33"
    },
    "description": "Pipe queued streams progressively, keeping datas order.",
    "devDependencies": {
        "coveralls": "~2.11.2",
        "istanbul": "~0.3.14",
        "mocha": "~2.2.5",
        "mocha-lcov-reporter": "~0.0.2",
        "streamtest": "~1.2.0"
    },
    "directories": {},
    "dist": {
        "shasum": "d3ad76686be924bbf9ca2c74a814a2182475d6d7",
        "tarball": "https://registry.npmjs.org/streamqueue/-/streamqueue-1.1.1.tgz"
    },
    "engines": {
        "node": ">= 0.10.0"
    },
    "gitHead": "a772c3925e60fd2f26b7a2f8e0aa500793df62bc",
    "homepage": "https://github.com/nfroidure/StreamQueue",
    "keywords": [
        "queue",
        "streaming",
        "stream",
        "async",
        "pipe"
    ],
    "licenses": [
        {
            "type": "MIT",
            "url": "https://github.com/nfroidure/StreamQueue/blob/master/LICENSE"
        }
    ],
    "main": "src/index.js",
    "maintainers": [
        {
            "name": "nfroidure"
        }
    ],
    "name": "streamqueue",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git://github.com/nfroidure/StreamQueue.git"
    },
    "scripts": {
        "cli": "env NPM_RUN_CLI=1",
        "cover": "./node_modules/istanbul/lib/cli.js cover --report html ./node_modules/mocha/bin/_mocha -- tests/*.mocha.js -R spec -t 5000",
        "coveralls": "./node_modules/istanbul/lib/cli.js cover ./node_modules/mocha/bin/_mocha --report lcovonly -- tests/*.mocha.js -R spec -t 5000 && cat ./coverage/lcov.info | ./node_modules/coveralls/bin/coveralls.js && rm -rf ./coverage",
        "lint": "eslint **/*.js *.js",
        "test": "./node_modules/mocha/bin/mocha tests/*.mocha.js"
    },
    "version": "1.1.1",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
