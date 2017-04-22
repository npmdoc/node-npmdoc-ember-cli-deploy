# npmdoc-ember-cli-deploy

#### api documentation for  [ember-cli-deploy (v1.0.0)](https://github.com/ember-cli-deploy/ember-cli-deploy#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-ember-cli-deploy.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-ember-cli-deploy) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-ember-cli-deploy.svg)](https://travis-ci.org/npmdoc/node-npmdoc-ember-cli-deploy)

#### A deployment pipeline for ember-cli apps

[![NPM](https://nodei.co/npm/ember-cli-deploy.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/ember-cli-deploy)

- [https://npmdoc.github.io/node-npmdoc-ember-cli-deploy/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-ember-cli-deploy/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-ember-cli-deploy/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-ember-cli-deploy/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-ember-cli-deploy/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-ember-cli-deploy/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "The ember-cli-deploy core team and contributors"
    },
    "bugs": {
        "url": "https://github.com/ember-cli-deploy/ember-cli-deploy/issues"
    },
    "dependencies": {
        "chalk": "^1.1.3",
        "core-object": "^2.0.0",
        "dag-map": "^2.0.1",
        "dotenv": "^1.2.0",
        "ember-cli-deploy-progress": "^1.3.0",
        "lodash": "^4.0.0",
        "rsvp": "^3.3.3",
        "silent-error": "^1.0.0"
    },
    "description": "A deployment pipeline for ember-cli apps",
    "devDependencies": {
        "chai": "^1.9.2",
        "chai-as-promised": "^4.1.1",
        "ember-cli": "^2.10.0",
        "ember-cli-release": "0.2.9",
        "github": "0.2.3",
        "mocha": "^2.0.1",
        "mocha-jshint": "^2.2.6"
    },
    "directories": {
        "doc": "doc",
        "test": "tests"
    },
    "dist": {
        "shasum": "34a9608d71f8168911f4b2f45135ad4b23220358",
        "tarball": "https://registry.npmjs.org/ember-cli-deploy/-/ember-cli-deploy-1.0.0.tgz"
    },
    "ember-addon": {
        "configPath": "tests/dummy/config"
    },
    "engines": {
        "node": ">= 0.10.0"
    },
    "gitHead": "8286b9ea2c3624b0015aaaf1dd50d24b6df67cf6",
    "homepage": "https://github.com/ember-cli-deploy/ember-cli-deploy#readme",
    "keywords": [
        "ember-addon",
        "ember-cli-deploy"
    ],
    "license": "MIT",
    "maintainers": [
        {
            "name": "achambers"
        },
        {
            "name": "ghedamat"
        },
        {
            "name": "levelbossmike"
        },
        {
            "name": "lukemelia"
        },
        {
            "name": "ryanto"
        },
        {
            "name": "samselikoff"
        }
    ],
    "name": "ember-cli-deploy",
    "optionalDependencies": {},
    "repository": {
        "type": "git",
        "url": "git+https://github.com/ember-cli-deploy/ember-cli-deploy.git"
    },
    "scripts": {
        "autotest": "node node_modules/mocha/bin/mocha --watch --reporter spec node-tests/**/*-test.js",
        "test": "node node_modules/mocha/bin/mocha node-tests/**/*-test.js"
    },
    "version": "1.0.0",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
