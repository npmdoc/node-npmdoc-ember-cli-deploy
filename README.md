# api documentation for  [ember-cli-deploy (v1.0.0)](https://github.com/ember-cli-deploy/ember-cli-deploy#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-ember-cli-deploy.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-ember-cli-deploy) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-ember-cli-deploy.svg)](https://travis-ci.org/npmdoc/node-npmdoc-ember-cli-deploy)
#### A deployment pipeline for ember-cli apps

[![NPM](https://nodei.co/npm/ember-cli-deploy.png?downloads=true)](https://www.npmjs.com/package/ember-cli-deploy)

[![apidoc](https://npmdoc.github.io/node-npmdoc-ember-cli-deploy/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-ember-cli-deploy_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-ember-cli-deploy/build/apidoc.html)

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
            "name": "achambers",
            "email": "achambers@gmail.com"
        },
        {
            "name": "ghedamat",
            "email": "ghedamat@gmail.com"
        },
        {
            "name": "levelbossmike",
            "email": "michael@firstiwaslike.com"
        },
        {
            "name": "lukemelia",
            "email": "luke@lukemelia.com"
        },
        {
            "name": "ryanto",
            "email": "ryanto@gmail.com"
        },
        {
            "name": "samselikoff",
            "email": "sam.selikoff@gmail.com"
        }
    ],
    "name": "ember-cli-deploy",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/ember-cli-deploy/ember-cli-deploy.git"
    },
    "scripts": {
        "autotest": "node node_modules/mocha/bin/mocha --watch --reporter spec node-tests/**/*-test.js",
        "test": "node node_modules/mocha/bin/mocha node-tests/**/*-test.js"
    },
    "version": "1.0.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module ember-cli-deploy](#apidoc.module.ember-cli-deploy)
1.  [function <span class="apidocSignatureSpan">ember-cli-deploy.</span>blueprintsPath ()](#apidoc.element.ember-cli-deploy.blueprintsPath)
1.  [function <span class="apidocSignatureSpan">ember-cli-deploy.</span>includedCommands ()](#apidoc.element.ember-cli-deploy.includedCommands)
1.  [function <span class="apidocSignatureSpan">ember-cli-deploy.</span>postBuild (result)](#apidoc.element.ember-cli-deploy.postBuild)
1.  string <span class="apidocSignatureSpan">ember-cli-deploy.</span>name



# <a name="apidoc.module.ember-cli-deploy"></a>[module ember-cli-deploy](#apidoc.module.ember-cli-deploy)

#### <a name="apidoc.element.ember-cli-deploy.blueprintsPath"></a>[function <span class="apidocSignatureSpan">ember-cli-deploy.</span>blueprintsPath ()](#apidoc.element.ember-cli-deploy.blueprintsPath)
- description and source-code
```javascript
blueprintsPath = function () {
  return path.join(__dirname, 'blueprints');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ember-cli-deploy.includedCommands"></a>[function <span class="apidocSignatureSpan">ember-cli-deploy.</span>includedCommands ()](#apidoc.element.ember-cli-deploy.includedCommands)
- description and source-code
```javascript
includedCommands = function () {
  return commands;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.ember-cli-deploy.postBuild"></a>[function <span class="apidocSignatureSpan">ember-cli-deploy.</span>postBuild (result)](#apidoc.element.ember-cli-deploy.postBuild)
- description and source-code
```javascript
postBuild = function (result) {
  var _this = this;
  if (!this.app) {
    // You will need ember-cli >= 1.13 to use ember-cli-deploy's postBuild integration.
    // This is because prior to 1.13, 'this.app' is not available in the postBuild hook.
    return;
  }
  var options = this.app.options.emberCLIDeploy || {};

  var deployTarget = options.runOnPostBuild;
  if (deployTarget) {
    var ReadConfigTask = require('./lib/tasks/read-config');
    var readConfig = new ReadConfigTask({
      project: this.project,
      deployTarget: deployTarget,
      deployConfigFile: options.configFile
    });
    return readConfig.run().then(function(config){
      var DeployTask = require('./lib/tasks/deploy');
      var deploy = new DeployTask({
        project: _this.project,
        ui: _this.ui,
        deployTarget: deployTarget,
        config: config,
        shouldActivate: options.shouldActivate,
        commandOptions: {
          buildDir: result.directory
        }
      });
      return deploy.run();
    });
  }
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
