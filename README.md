# npmtest-pjax

#### basic test coverage for  [pjax (v0.2.4)](https://github.com/MoOx/pjax#readme)  [![npm package](https://img.shields.io/npm/v/npmtest-pjax.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-pjax) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-pjax.svg)](https://travis-ci.org/npmtest/node-npmtest-pjax)

#### Easily enable fast Ajax navigation on any website (using pushState +  xhr)

[![NPM](https://nodei.co/npm/pjax.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/pjax)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-pjax/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-pjax/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-pjax/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-pjax/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-pjax/build/test-report.html)|
| test-server-github : | [![github.com test-server](https://npmtest.github.io/node-npmtest-pjax/GitHub-Mark-32px.png)](https://npmtest.github.io/node-npmtest-pjax/build/app/index.html) | | build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-pjax/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-pjax/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-pjax/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-pjax/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-pjax/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-pjax/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-pjax/build/test-report.html](https://npmtest.github.io/node-npmtest-pjax/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-pjax/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-pjax/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-pjax/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-pjax/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-pjax/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-pjax/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-pjax/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-pjax/build/screenCapture.npmPackageDependencyTree.svg)



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
