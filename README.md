# npmtest-simple-peer

#### basic test-coverage for  [simple-peer (v8.1.0)](https://github.com/feross/simple-peer#readme)  [![npm package](https://img.shields.io/npm/v/npmtest-simple-peer.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-simple-peer) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-simple-peer.svg)](https://travis-ci.org/npmtest/node-npmtest-simple-peer)

#### Simple one-to-one WebRTC video/voice and data channels

[![NPM](https://nodei.co/npm/simple-peer.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/simple-peer)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-simple-peer/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-simple-peer/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-simple-peer/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-simple-peer/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-simple-peer/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-simple-peer/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-simple-peer/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-simple-peer/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-simple-peer/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-simple-peer/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-simple-peer/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-simple-peer/build/test-report.html](https://npmtest.github.io/node-npmtest-simple-peer/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-simple-peer/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-simple-peer/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-simple-peer/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-simple-peer/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-simple-peer/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-simple-peer/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-simple-peer/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-simple-peer/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Feross Aboukhadijeh",
        "url": "http://feross.org/"
    },
    "bugs": {
        "url": "https://github.com/feross/simple-peer/issues"
    },
    "dependencies": {
        "debug": "^2.1.0",
        "get-browser-rtc": "^1.0.0",
        "inherits": "^2.0.1",
        "randombytes": "^2.0.3",
        "readable-stream": "^2.0.5"
    },
    "description": "Simple one-to-one WebRTC video/voice and data channels",
    "devDependencies": {
        "browserify": "^14.0.0",
        "concat-stream": "^1.4.6",
        "electron-webrtc": "^0.3.0",
        "prettier-bytes": "^1.0.3",
        "simple-get": "^2.0.0",
        "speedometer": "^1.0.0",
        "standard": "*",
        "string-to-stream": "^1.0.0",
        "tape": "^4.0.0",
        "thunky": "^1.0.1",
        "uglify-js": "^2.4.15",
        "wrtc": "0.0.61",
        "ws": "^2.0.2",
        "zuul": "^3.8.0"
    },
    "directories": {},
    "dist": {
        "shasum": "0e3214e78b34c45cadbb284a3aee334dbcb4aff8",
        "tarball": "https://registry.npmjs.org/simple-peer/-/simple-peer-8.1.0.tgz"
    },
    "gitHead": "9eee5d289d198caca83d5a98f05c186df9bad21f",
    "homepage": "https://github.com/feross/simple-peer#readme",
    "keywords": [
        "data",
        "data channel",
        "data channel stream",
        "data channels",
        "p2p",
        "peer",
        "peer",
        "peer-to-peer",
        "stream",
        "video",
        "voice",
        "webrtc",
        "webrtc stream"
    ],
    "license": "MIT",
    "main": "index.js",
    "maintainers": [
        {
            "name": "contra"
        },
        {
            "name": "feross"
        },
        {
            "name": "mafintosh"
        },
        {
            "name": "maxogden"
        },
        {
            "name": "substack"
        }
    ],
    "name": "simple-peer",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git://github.com/feross/simple-peer.git"
    },
    "scripts": {
        "build": "browserify -s SimplePeer -r ./ | uglifyjs -m > simplepeer.min.js",
        "test": "standard && npm run test-node && npm run test-browser",
        "test-browser": "zuul -- test/*.js",
        "test-browser-local": "zuul --local -- test/*.js",
        "test-node": "npm run test-node-electron-webrtc && npm run test-node-wrtc",
        "test-node-electron-webrtc": "WRTC=electron-webrtc tape test/*.js",
        "test-node-wrtc": "WRTC=wrtc tape test/*.js"
    },
    "testling": {
        "files": "test/*.js"
    },
    "version": "8.1.0",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
