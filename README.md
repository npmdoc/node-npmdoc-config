# api documentation for  [config (v1.25.1)](http://lorenwest.github.com/node-config)  [![npm package](https://img.shields.io/npm/v/npmdoc-config.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-config) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-config.svg)](https://travis-ci.org/npmdoc/node-npmdoc-config)
#### Configuration control for production node deployments

[![NPM](https://nodei.co/npm/config.png?downloads=true)](https://www.npmjs.com/package/config)

[![apidoc](https://npmdoc.github.io/node-npmdoc-config/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-config_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-config/build..beta..travis-ci.org/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-config/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-config/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Loren West",
        "email": "open_source@lorenwest.com"
    },
    "bugs": {
        "url": "https://github.com/lorenwest/node-config/issues"
    },
    "dependencies": {
        "json5": "0.4.0"
    },
    "description": "Configuration control for production node deployments",
    "devDependencies": {
        "coffee-script": ">=1.7.0",
        "cson": "^3.0.1",
        "hjson": "^1.2.0",
        "js-yaml": "^3.2.2",
        "properties": "~1.2.1",
        "toml": "^2.0.6",
        "underscore": "^1.8.3",
        "vows": ">=0.8.1",
        "x2js": "^2.0.1"
    },
    "directories": {
        "lib": "./lib"
    },
    "dist": {
        "shasum": "72ac51cde81e2c77c6b3b66d0130dae527a19c92",
        "tarball": "https://registry.npmjs.org/config/-/config-1.25.1.tgz"
    },
    "engines": {
        "node": ">0.4.x"
    },
    "gitHead": "c226283619b2f759ff236d5e1f65055a3c39ba54",
    "homepage": "http://lorenwest.github.com/node-config",
    "keywords": [
        "conf",
        "config",
        "configuration",
        "node-config",
        "config-node",
        "env",
        "environment"
    ],
    "license": "MIT",
    "main": "./lib/config.js",
    "maintainers": [
        {
            "name": "lorenwest",
            "email": "npm@lorenwest.com"
        },
        {
            "name": "markstos",
            "email": "mark@rideamigos.com"
        }
    ],
    "name": "config",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+ssh://git@github.com/lorenwest/node-config.git"
    },
    "scripts": {
        "test": "./node_modules/vows/bin/vows test/*.js --spec"
    },
    "version": "1.25.1"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module config](#apidoc.module.config)
1.  object <span class="apidocSignatureSpan">config.</span>defer
1.  object <span class="apidocSignatureSpan">config.</span>raw

#### [module config.defer](#apidoc.module.config.defer)
1.  [function <span class="apidocSignatureSpan">config.defer.</span>DeferredConfig ()](#apidoc.element.config.defer.DeferredConfig)
1.  [function <span class="apidocSignatureSpan">config.defer.</span>deferConfig (func)](#apidoc.element.config.defer.deferConfig)

#### [module config.raw](#apidoc.module.config.raw)
1.  [function <span class="apidocSignatureSpan">config.</span>raw (rawObj)](#apidoc.element.config.raw.raw)
1.  [function <span class="apidocSignatureSpan">config.raw.</span>RawConfig ()](#apidoc.element.config.raw.RawConfig)



# <a name="apidoc.module.config"></a>[module config](#apidoc.module.config)



# <a name="apidoc.module.config.defer"></a>[module config.defer](#apidoc.module.config.defer)

#### <a name="apidoc.element.config.defer.DeferredConfig"></a>[function <span class="apidocSignatureSpan">config.defer.</span>DeferredConfig ()](#apidoc.element.config.defer.DeferredConfig)
- description and source-code
```javascript
function DeferredConfig() {
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.config.defer.deferConfig"></a>[function <span class="apidocSignatureSpan">config.defer.</span>deferConfig (func)](#apidoc.element.config.defer.deferConfig)
- description and source-code
```javascript
function deferConfig(func) {
  var obj = Object.create(DeferredConfig.prototype);
  obj.resolve = func;
  return obj;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.config.raw"></a>[module config.raw](#apidoc.module.config.raw)

#### <a name="apidoc.element.config.raw.raw"></a>[function <span class="apidocSignatureSpan">config.</span>raw (rawObj)](#apidoc.element.config.raw.raw)
- description and source-code
```javascript
function raw(rawObj) {
  var obj = Object.create(RawConfig.prototype);
  obj.resolve = function () { return rawObj; }
  return obj;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.config.raw.RawConfig"></a>[function <span class="apidocSignatureSpan">config.raw.</span>RawConfig ()](#apidoc.element.config.raw.RawConfig)
- description and source-code
```javascript
function RawConfig() {
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
