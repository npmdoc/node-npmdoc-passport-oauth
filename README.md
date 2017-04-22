# npmdoc-passport-oauth

#### api documentation for  [passport-oauth (v1.0.0)](https://github.com/jaredhanson/passport-oauth#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-passport-oauth.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-passport-oauth) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-passport-oauth.svg)](https://travis-ci.org/npmdoc/node-npmdoc-passport-oauth)

#### OAuth 1.0 and 2.0 authentication strategies for Passport.

[![NPM](https://nodei.co/npm/passport-oauth.png?downloads=true&downloadRank=true&stars=true)](https://www.npmjs.com/package/passport-oauth)

- [https://npmdoc.github.io/node-npmdoc-passport-oauth/build/apidoc.html](https://npmdoc.github.io/node-npmdoc-passport-oauth/build/apidoc.html)

[![apidoc](https://npmdoc.github.io/node-npmdoc-passport-oauth/build/screenCapture.buildCi.browser.%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-passport-oauth/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-passport-oauth/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-passport-oauth/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Jared Hanson",
        "url": "http://www.jaredhanson.net/"
    },
    "bugs": {
        "url": "http://github.com/jaredhanson/passport-oauth/issues"
    },
    "dependencies": {
        "passport-oauth1": "1.x.x",
        "passport-oauth2": "1.x.x"
    },
    "description": "OAuth 1.0 and 2.0 authentication strategies for Passport.",
    "devDependencies": {
        "chai": "1.x.x",
        "chai-passport-strategy": "0.1.x",
        "mocha": "1.x.x"
    },
    "directories": {},
    "dist": {
        "shasum": "90aff63387540f02089af28cdad39ea7f80d77df",
        "tarball": "https://registry.npmjs.org/passport-oauth/-/passport-oauth-1.0.0.tgz"
    },
    "engines": {
        "node": ">= 0.4.0"
    },
    "homepage": "https://github.com/jaredhanson/passport-oauth#readme",
    "keywords": [
        "passport",
        "auth",
        "authn",
        "authentication",
        "authz",
        "authorization",
        "oauth",
        "oauth2"
    ],
    "licenses": [
        {
            "type": "MIT",
            "url": "http://www.opensource.org/licenses/MIT"
        }
    ],
    "main": "./lib",
    "maintainers": [
        {
            "name": "jaredhanson"
        }
    ],
    "name": "passport-oauth",
    "optionalDependencies": {},
    "readmeFilename": "README.md",
    "repository": {
        "type": "git",
        "url": "git://github.com/jaredhanson/passport-oauth.git"
    },
    "scripts": {
        "test": "node_modules/.bin/mocha --reporter spec --require test/bootstrap/node test/*.test.js"
    },
    "testling": {
        "browsers": [
            "chrome/latest"
        ],
        "harness": "mocha",
        "files": [
            "test/bootstrap/testling.js",
            "test/*.test.js",
            "test/**/*.test.js"
        ]
    },
    "version": "1.0.0",
    "bin": {}
}
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
