# npmtest-deepstream.io

#### basic test coverage for  [deepstream.io (v2.2.0)](http://deepstream.io)  [![npm package](https://img.shields.io/npm/v/npmtest-deepstream.io.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-deepstream.io) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-deepstream.io.svg)](https://travis-ci.org/npmtest/node-npmtest-deepstream.io)

#### a scalable server for realtime webapps

[![NPM](https://nodei.co/npm/deepstream.io.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/deepstream.io)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-deepstream.io/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-deepstream.io/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-deepstream.io/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-deepstream.io/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-deepstream.io/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-deepstream.io/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-deepstream.io/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-deepstream.io/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-deepstream.io/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-deepstream.io/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-deepstream.io/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-deepstream.io/build/test-report.html](https://npmtest.github.io/node-npmtest-deepstream.io/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-deepstream.io/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-deepstream.io/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-deepstream.io/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-deepstream.io/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-deepstream.io/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-deepstream.io/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-deepstream.io/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-deepstream.io/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "name": "deepstream.io",
    "version": "2.2.0",
    "description": "a scalable server for realtime webapps",
    "main": "src/deepstream.io.js",
    "bin": {
        "deepstream": "./bin/deepstream"
    },
    "directories": {
        "test": "test"
    },
    "scripts": {
        "precommit": "npm run lint",
        "lint": "node_modules/.bin/eslint src/",
        "coverage": "istanbul cover node_modules/jasmine/bin/jasmine.js JASMINE_CONFIG_PATH=jasmine.json -x **/pid-helper.js",
        "watch": "node node_modules/watch/cli.js \"npm test\" ./src ./test",
        "reporter": "node jasmine-runner",
        "test": "jasmine JASMINE_CONFIG_PATH=jasmine.json",
        "test-http-server": "node test/test-helper/start-test-server.js",
        "license": "mkdir -p build && node scripts/license-aggregator > build/LICENSE && cat scripts/resources/missing-licenses.txt >> build/LICENSE"
    },
    "repository": {
        "type": "git",
        "url": "https://github.com/deepstreamIO/deepstream.io.git"
    },
    "dependencies": {
        "adm-zip": "^0.4.7",
        "colors": "^1.1.2",
        "commander": "^2.9.0",
        "glob": "^7.1.1",
        "js-yaml": "^3.8.1",
        "mkdirp": "^0.5.1",
        "needle": "^1.4.5",
        "uws": "https://github.com/deepstreamIO/uws-dependency.git#v0.12.0"
    },
    "devDependencies": {
        "async": "^2.1.4",
        "coveralls": "^2.11.16",
        "eslint-config-deepstream": "^2.2.0",
        "istanbul": "^0.4.5",
        "jasmine": "^2.5.3",
        "jasmine-spec-reporter": "^3.2.0",
        "n0p3": "^1.0.2",
        "nexe": "^1.1.2",
        "proxyquire": "1.7.11",
        "watch": "^1.0.1"
    },
    "author": "deepstreamHub GmbH",
    "license": "AGPL-3.0",
    "bugs": {
        "url": "https://github.com/deepstreamIO/deepstream.io/issues"
    },
    "homepage": "http://deepstream.io",
    "eslintConfig": {
        "extends": "deepstream"
    }
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
