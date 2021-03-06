# npmdoc-pjax

#### basic api documentation for  [pjax (v0.2.4)](https://github.com/MoOx/pjax#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-pjax.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-pjax) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-pjax.svg)](https://travis-ci.org/npmdoc/node-npmdoc-pjax)

#### Easily enable fast Ajax navigation on any website (using pushState +  xhr)

[![NPM](https://nodei.co/npm/pjax.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/pjax)

- [https://npmdoc.github.io/node-npmdoc-pjax/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-pjax/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-pjax/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-pjax/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-pjax/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-pjax/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Maxime Thirouin"
    },
    "bugs": {
        "url": "https://github.com/MoOx/pjax/issues"
    },
    "dependencies": {},
    "description": "Easily enable fast Ajax navigation on any website (using pushState +  xhr)",
    "devDependencies": {
        "browserify": "^3.46.0",
        "coverify": "^1.0.6",
        "jscs": "^1.6.2",
        "jshint": "^2.5.6",
        "npmpub": "^3.1.0",
        "opn-cli": "^3.1.0",
        "serve": "1.4.0",
        "tape": "^3.0.0",
        "testling": "^1.6.1"
    },
    "directories": {},
    "dist": {
        "shasum": "0ae5885cfe663eb6a786156ed9c3de5bcb627513",
        "tarball": "https://registry.npmjs.org/pjax/-/pjax-0.2.4.tgz"
    },
    "files": [
        "index.js",
        "lib",
        "pjax.js"
    ],
    "gitHead": "917c6f6bcb5d84309d646bad94fa6540151a0f4d",
    "homepage": "https://github.com/MoOx/pjax#readme",
    "keywords": [
        "pjax",
        "push",
        "state",
        "ajax",
        "navigation",
        "transition",
        "animation"
    ],
    "license": "MIT",
    "main": "src/pjax.js",
    "maintainers": [
        {
            "name": "moox"
        }
    ],
    "name": "pjax",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/MoOx/pjax.git"
    },
    "scripts": {
        "#release": "testling does not work in a process launch by npm... :facepalm:",
        "coverage": "browserify -t coverify tests/**/*.js | testling | coverify",
        "example": "opn http://localhost:3000/example/; serve .",
        "lint": "jscs **/*.js && jshint . --exclude-path .gitignore",
        "prepublish": "npm run standalone",
        "release": "echo \"npmpub --skip-test --dry && npm test && npmpub --skip-test --skip-cleanup\"",
        "standalone": "browserify index.js --standalone Pjax > pjax.js",
        "test": "npm run lint && npm run standalone && npm run tests",
        "test--html": "testling --html > tests/scripts/index.html",
        "tests": "testling"
    },
    "testling": {
        "files": "tests/**/*.js",
        "browsers": [
            "ie/10..latest",
            "firefox/4.0",
            "firefox/latest",
            "firefox/nightly",
            "chrome/10",
            "chrome/latest",
            "chrome/canary",
            "opera/12..latest",
            "opera/next",
            "safari/5.1..latest",
            "ipad/6.0..latest",
            "iphone/6.0..latest",
            "android-browser/4.2..latest"
        ]
    },
    "version": "0.2.4",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
