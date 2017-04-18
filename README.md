# npmtest-jade-lint

#### test coverage for  [jade-lint (v2.1.0)](https://github.com/pugjs/jade-lint#readme)  [![npm package](https://img.shields.io/npm/v/npmtest-jade-lint.svg?style=flat-square)](https://www.npmjs.org/package/npmtest-jade-lint) [![travis-ci.org build-status](https://api.travis-ci.org/npmtest/node-npmtest-jade-lint.svg)](https://travis-ci.org/npmtest/node-npmtest-jade-lint)

#### An unopinionated and configurable linter and style checker for Jade

[![NPM](https://nodei.co/npm/jade-lint.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/jade-lint)

| git-branch : | [alpha](https://github.com/npmtest/node-npmtest-jade-lint/tree/alpha)|
|--:|:--|
| coverage : | [![istanbul-coverage](https://npmtest.github.io/node-npmtest-jade-lint/build/coverage.badge.svg)](https://npmtest.github.io/node-npmtest-jade-lint/build/coverage.html/index.html)|
| test-report : | [![test-report](https://npmtest.github.io/node-npmtest-jade-lint/build/test-report.badge.svg)](https://npmtest.github.io/node-npmtest-jade-lint/build/test-report.html)|
| build-artifacts : | [![build-artifacts](https://npmtest.github.io/node-npmtest-jade-lint/glyphicons_144_folder_open.png)](https://github.com/npmtest/node-npmtest-jade-lint/tree/gh-pages/build)|

- [https://npmtest.github.io/node-npmtest-jade-lint/build/coverage.html/index.html](https://npmtest.github.io/node-npmtest-jade-lint/build/coverage.html/index.html)

[![istanbul-coverage](https://npmtest.github.io/node-npmtest-jade-lint/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fcoverage.lib.html.png)](https://npmtest.github.io/node-npmtest-jade-lint/build/coverage.html/index.html)

- [https://npmtest.github.io/node-npmtest-jade-lint/build/test-report.html](https://npmtest.github.io/node-npmtest-jade-lint/build/test-report.html)

[![test-report](https://npmtest.github.io/node-npmtest-jade-lint/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Ftest-report.html.png)](https://npmtest.github.io/node-npmtest-jade-lint/build/test-report.html)

- [https://npmdoc.github.io/node-npmdoc-jade-lint/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-jade-lint/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-jade-lint/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-jade-lint/build/apidoc.html)

![npmPackageListing](https://npmtest.github.io/node-npmtest-jade-lint/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmtest.github.io/node-npmtest-jade-lint/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Ben Edwards"
    },
    "bin": {
        "jade-lint": "./bin/jade-lint"
    },
    "bugs": {
        "url": "https://github.com/pugjs/jade-lint/issues"
    },
    "dependencies": {
        "commander": "^2.9.0",
        "css-selector-parser": "^1.1.0",
        "glob": "^6.0.1",
        "jade-attrs": "^2.0.0",
        "jade-error": "^1.1.1",
        "jade-lexer": "0.0.9",
        "minimatch": "^3.0.0",
        "void-elements": "^2.0.1"
    },
    "deprecated": "jade-lint will be unpublished soon, please use pug-lint",
    "description": "An unopinionated and configurable linter and style checker for Jade",
    "devDependencies": {
        "david": "^7.0.0",
        "docco": "^0.7.0",
        "eslint": "^1.8.0",
        "eslint-config-clock": "^1.0.0",
        "eslint-config-standard": "^4.3.2",
        "eslint-plugin-standard": "^1.3.0",
        "istanbul": "^0.4.0",
        "jsinspect": "^0.7.0",
        "mocha": "^2.3.3",
        "pliers": "^1.2.1",
        "pliers-clean-shrinkwrap": "^1.0.1",
        "sinon": "^1.17.2"
    },
    "directories": {},
    "dist": {
        "shasum": "8a71b7d589e28061226cee34b85946eca4b64928",
        "tarball": "https://registry.npmjs.org/jade-lint/-/jade-lint-2.1.0.tgz"
    },
    "gitHead": "b63689f7cf3cc7489db7d18e0e88934efcfab622",
    "homepage": "https://github.com/pugjs/jade-lint#readme",
    "keywords": [
        "jadelint",
        "jade-lint",
        "jade",
        "lint",
        "code style",
        "formatter",
        "style guide",
        "validate",
        "lint jade",
        "jade lint",
        "linter",
        "linter jade",
        "jade linter",
        "jade-linter",
        "linting",
        "linting jade",
        "jade linting",
        "jade-linting",
        "hint",
        "hint jade",
        "jade hint",
        "jade-hint",
        "hinter",
        "hinter jade",
        "jade hinter",
        "jade-hinter",
        "hinting",
        "hinting jade",
        "jade hinting",
        "jade-hinting"
    ],
    "license": "ISC",
    "main": "./lib/linter",
    "maintainers": [
        {
            "name": "benedfit"
        }
    ],
    "name": "jade-lint",
    "optionalDependencies": {},
    "publishConfig": {
        "registry": "http://registry.npmjs.org"
    },
    "repository": {
        "type": "git",
        "url": "git+ssh://git@github.com/pugjs/jade-lint.git"
    },
    "scripts": {
        "coverage": "istanbul cover ./node_modules/.bin/_mocha test",
        "depcheck": "david",
        "docs": "pliers buildRuleDocs",
        "inspect": "jsinspect",
        "lint": "eslint -f unix .",
        "posttest": "(istanbul check-coverage --statements 90 --branches 90 --functions 100 --lines 90 && rm -rf coverage) || echo Look at 'coverage/lcov-report/index.html' to find out more",
        "pretest": "npm run docs && npm run lint && npm run inspect && npm run depcheck",
        "test": "npm run coverage",
        "wrap": "npm prune && npm shrinkwrap && pliers cleanShrinkwrap"
    },
    "version": "2.1.0"
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
