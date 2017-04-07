# api documentation for  [passport-oauth (v1.0.0)](https://github.com/jaredhanson/passport-oauth#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-passport-oauth.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-passport-oauth) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-passport-oauth.svg)](https://travis-ci.org/npmdoc/node-npmdoc-passport-oauth)
#### OAuth 1.0 and 2.0 authentication strategies for Passport.

[![NPM](https://nodei.co/npm/passport-oauth.png?downloads=true)](https://www.npmjs.com/package/passport-oauth)

[![apidoc](https://npmdoc.github.io/node-npmdoc-passport-oauth/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-passport-oauth_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-passport-oauth/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-passport-oauth/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-passport-oauth/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Jared Hanson",
        "email": "jaredhanson@gmail.com",
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
            "name": "jaredhanson",
            "email": "jaredhanson@gmail.com"
        }
    ],
    "name": "passport-oauth",
    "optionalDependencies": {},
    "readme": "# passport-oauth\n\n[![Build](https://travis-ci.org/jaredhanson/passport-oauth.png)](http://travis-ci.org/jaredhanson/passport-oauth)\n[![Coverage](https://coveralls.io/repos/jaredhanson/passport-oauth/badge.png)](https://coveralls.io/r/jaredhanson/passport-oauth)\n[![Dependencies](https://david-dm.org/jaredhanson/passport-oauth.png)](http://david-dm.org/jaredhanson/passport-oauth)\n\n\nGeneral-purpose OAuth 1.0 and OAuth 2.0 authentication strategies for [Passport](https://github.com/jaredhanson/passport).\n\nThis is a meta-module that combines [passport-oauth1](https://github.com/jaredhanson/passport-oauth1)\nand [passport-oauth2](https://github.com/jaredhanson/passport-oauth2).  It\nexists for backwards-compatibility with the 0.1.x line of OAuth-based\nstrategies.  As of version 1.x.x, it is encouraged to declare dependencies\non the module that implements specific version of OAuth in use.\n\n## Install\n\n    $ npm install passport-oauth\n\n## Tests\n\n    $ npm install\n    $ npm test\n\n## Credits\n\n  - [Jared Hanson](http://github.com/jaredhanson)\n\n## License\n\n[The MIT License](http://opensource.org/licenses/MIT)\n\nCopyright (c) 2011-2013 Jared Hanson <[http://jaredhanson.net/](http://jaredhanson.net/)>\n",
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
    "version": "1.0.0"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module passport-oauth](#apidoc.module.passport-oauth)
1.  [function <span class="apidocSignatureSpan">passport-oauth.</span>InternalOAuthError (message, err)](#apidoc.element.passport-oauth.InternalOAuthError)
1.  [function <span class="apidocSignatureSpan">passport-oauth.</span>OAuth2Strategy (options, verify)](#apidoc.element.passport-oauth.OAuth2Strategy)
1.  [function <span class="apidocSignatureSpan">passport-oauth.</span>OAuth2Strategy.InternalOAuthError (message, err)](#apidoc.element.passport-oauth.OAuth2Strategy.InternalOAuthError)
1.  [function <span class="apidocSignatureSpan">passport-oauth.</span>OAuth2Strategy.super_ ()](#apidoc.element.passport-oauth.OAuth2Strategy.super_)
1.  [function <span class="apidocSignatureSpan">passport-oauth.</span>OAuthStrategy (options, verify)](#apidoc.element.passport-oauth.OAuthStrategy)
1.  object <span class="apidocSignatureSpan">passport-oauth.</span>InternalOAuthError.prototype
1.  object <span class="apidocSignatureSpan">passport-oauth.</span>OAuth2Strategy.InternalOAuthError.prototype
1.  object <span class="apidocSignatureSpan">passport-oauth.</span>OAuth2Strategy.prototype
1.  object <span class="apidocSignatureSpan">passport-oauth.</span>OAuth2Strategy.super_.prototype
1.  object <span class="apidocSignatureSpan">passport-oauth.</span>OAuthStrategy.prototype

#### [module passport-oauth.InternalOAuthError](#apidoc.module.passport-oauth.InternalOAuthError)
1.  [function <span class="apidocSignatureSpan">passport-oauth.</span>InternalOAuthError (message, err)](#apidoc.element.passport-oauth.InternalOAuthError.InternalOAuthError)

#### [module passport-oauth.InternalOAuthError.prototype](#apidoc.module.passport-oauth.InternalOAuthError.prototype)
1.  [function <span class="apidocSignatureSpan">passport-oauth.InternalOAuthError.prototype.</span>toString ()](#apidoc.element.passport-oauth.InternalOAuthError.prototype.toString)

#### [module passport-oauth.OAuth2Strategy](#apidoc.module.passport-oauth.OAuth2Strategy)
1.  [function <span class="apidocSignatureSpan">passport-oauth.</span>OAuth2Strategy (options, verify)](#apidoc.element.passport-oauth.OAuth2Strategy.OAuth2Strategy)
1.  [function <span class="apidocSignatureSpan">passport-oauth.OAuth2Strategy.</span>AuthorizationError (message, code, uri, status)](#apidoc.element.passport-oauth.OAuth2Strategy.AuthorizationError)
1.  [function <span class="apidocSignatureSpan">passport-oauth.OAuth2Strategy.</span>InternalOAuthError (message, err)](#apidoc.element.passport-oauth.OAuth2Strategy.InternalOAuthError)
1.  [function <span class="apidocSignatureSpan">passport-oauth.OAuth2Strategy.</span>Strategy (options, verify)](#apidoc.element.passport-oauth.OAuth2Strategy.Strategy)
1.  [function <span class="apidocSignatureSpan">passport-oauth.OAuth2Strategy.</span>TokenError (message, code, uri, status)](#apidoc.element.passport-oauth.OAuth2Strategy.TokenError)
1.  [function <span class="apidocSignatureSpan">passport-oauth.OAuth2Strategy.</span>super_ ()](#apidoc.element.passport-oauth.OAuth2Strategy.super_)

#### [module passport-oauth.OAuth2Strategy.InternalOAuthError](#apidoc.module.passport-oauth.OAuth2Strategy.InternalOAuthError)
1.  [function <span class="apidocSignatureSpan">passport-oauth.OAuth2Strategy.</span>InternalOAuthError (message, err)](#apidoc.element.passport-oauth.OAuth2Strategy.InternalOAuthError.InternalOAuthError)

#### [module passport-oauth.OAuth2Strategy.InternalOAuthError.prototype](#apidoc.module.passport-oauth.OAuth2Strategy.InternalOAuthError.prototype)
1.  [function <span class="apidocSignatureSpan">passport-oauth.OAuth2Strategy.InternalOAuthError.prototype.</span>toString ()](#apidoc.element.passport-oauth.OAuth2Strategy.InternalOAuthError.prototype.toString)

#### [module passport-oauth.OAuth2Strategy.prototype](#apidoc.module.passport-oauth.OAuth2Strategy.prototype)
1.  [function <span class="apidocSignatureSpan">passport-oauth.OAuth2Strategy.prototype.</span>_createOAuthError (message, err)](#apidoc.element.passport-oauth.OAuth2Strategy.prototype._createOAuthError)
1.  [function <span class="apidocSignatureSpan">passport-oauth.OAuth2Strategy.prototype.</span>_loadUserProfile (accessToken, done)](#apidoc.element.passport-oauth.OAuth2Strategy.prototype._loadUserProfile)
1.  [function <span class="apidocSignatureSpan">passport-oauth.OAuth2Strategy.prototype.</span>authenticate (req, options)](#apidoc.element.passport-oauth.OAuth2Strategy.prototype.authenticate)
1.  [function <span class="apidocSignatureSpan">passport-oauth.OAuth2Strategy.prototype.</span>authorizationParams (options)](#apidoc.element.passport-oauth.OAuth2Strategy.prototype.authorizationParams)
1.  [function <span class="apidocSignatureSpan">passport-oauth.OAuth2Strategy.prototype.</span>parseErrorResponse (body, status)](#apidoc.element.passport-oauth.OAuth2Strategy.prototype.parseErrorResponse)
1.  [function <span class="apidocSignatureSpan">passport-oauth.OAuth2Strategy.prototype.</span>tokenParams (options)](#apidoc.element.passport-oauth.OAuth2Strategy.prototype.tokenParams)
1.  [function <span class="apidocSignatureSpan">passport-oauth.OAuth2Strategy.prototype.</span>userProfile (accessToken, done)](#apidoc.element.passport-oauth.OAuth2Strategy.prototype.userProfile)

#### [module passport-oauth.OAuth2Strategy.super_](#apidoc.module.passport-oauth.OAuth2Strategy.super_)
1.  [function <span class="apidocSignatureSpan">passport-oauth.OAuth2Strategy.</span>super_ ()](#apidoc.element.passport-oauth.OAuth2Strategy.super_.super_)
1.  [function <span class="apidocSignatureSpan">passport-oauth.OAuth2Strategy.super_.</span>Strategy ()](#apidoc.element.passport-oauth.OAuth2Strategy.super_.Strategy)

#### [module passport-oauth.OAuth2Strategy.super_.prototype](#apidoc.module.passport-oauth.OAuth2Strategy.super_.prototype)
1.  [function <span class="apidocSignatureSpan">passport-oauth.OAuth2Strategy.super_.prototype.</span>authenticate (req, options)](#apidoc.element.passport-oauth.OAuth2Strategy.super_.prototype.authenticate)

#### [module passport-oauth.OAuthStrategy](#apidoc.module.passport-oauth.OAuthStrategy)
1.  [function <span class="apidocSignatureSpan">passport-oauth.</span>OAuthStrategy (options, verify)](#apidoc.element.passport-oauth.OAuthStrategy.OAuthStrategy)
1.  [function <span class="apidocSignatureSpan">passport-oauth.OAuthStrategy.</span>InternalOAuthError (message, err)](#apidoc.element.passport-oauth.OAuthStrategy.InternalOAuthError)
1.  [function <span class="apidocSignatureSpan">passport-oauth.OAuthStrategy.</span>Strategy (options, verify)](#apidoc.element.passport-oauth.OAuthStrategy.Strategy)
1.  [function <span class="apidocSignatureSpan">passport-oauth.OAuthStrategy.</span>super_ ()](#apidoc.element.passport-oauth.OAuthStrategy.super_)

#### [module passport-oauth.OAuthStrategy.prototype](#apidoc.module.passport-oauth.OAuthStrategy.prototype)
1.  [function <span class="apidocSignatureSpan">passport-oauth.OAuthStrategy.prototype.</span>_createOAuthError (message, err)](#apidoc.element.passport-oauth.OAuthStrategy.prototype._createOAuthError)
1.  [function <span class="apidocSignatureSpan">passport-oauth.OAuthStrategy.prototype.</span>_loadUserProfile (token, tokenSecret, params, done)](#apidoc.element.passport-oauth.OAuthStrategy.prototype._loadUserProfile)
1.  [function <span class="apidocSignatureSpan">passport-oauth.OAuthStrategy.prototype.</span>authenticate (req, options)](#apidoc.element.passport-oauth.OAuthStrategy.prototype.authenticate)
1.  [function <span class="apidocSignatureSpan">passport-oauth.OAuthStrategy.prototype.</span>parseErrorResponse (body, status)](#apidoc.element.passport-oauth.OAuthStrategy.prototype.parseErrorResponse)
1.  [function <span class="apidocSignatureSpan">passport-oauth.OAuthStrategy.prototype.</span>requestTokenParams (options)](#apidoc.element.passport-oauth.OAuthStrategy.prototype.requestTokenParams)
1.  [function <span class="apidocSignatureSpan">passport-oauth.OAuthStrategy.prototype.</span>userAuthorizationParams (options)](#apidoc.element.passport-oauth.OAuthStrategy.prototype.userAuthorizationParams)
1.  [function <span class="apidocSignatureSpan">passport-oauth.OAuthStrategy.prototype.</span>userProfile (token, tokenSecret, params, done)](#apidoc.element.passport-oauth.OAuthStrategy.prototype.userProfile)



# <a name="apidoc.module.passport-oauth"></a>[module passport-oauth](#apidoc.module.passport-oauth)

#### <a name="apidoc.element.passport-oauth.InternalOAuthError"></a>[function <span class="apidocSignatureSpan">passport-oauth.</span>InternalOAuthError (message, err)](#apidoc.element.passport-oauth.InternalOAuthError)
- description and source-code
```javascript
function InternalOAuthError(message, err) {
  Error.call(this);
  Error.captureStackTrace(this, this.constructor);
  this.name = this.constructor.name;
  this.message = message;
  this.oauthError = err;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.passport-oauth.OAuth2Strategy"></a>[function <span class="apidocSignatureSpan">passport-oauth.</span>OAuth2Strategy (options, verify)](#apidoc.element.passport-oauth.OAuth2Strategy)
- description and source-code
```javascript
function OAuth2Strategy(options, verify) {
  if (typeof options == 'function') {
    verify = options;
    options = undefined;
  }
  options = options || {};

  if (!verify) { throw new TypeError('OAuth2Strategy requires a verify callback'); }
  if (!options.authorizationURL) { throw new TypeError('OAuth2Strategy requires a authorizationURL option'); }
  if (!options.tokenURL) { throw new TypeError('OAuth2Strategy requires a tokenURL option'); }
  if (!options.clientID) { throw new TypeError('OAuth2Strategy requires a clientID option'); }

  passport.Strategy.call(this);
  this.name = 'oauth2';
  this._verify = verify;

  // NOTE: The _oauth2 property is considered "protected".  Subclasses are
  //       allowed to use it when making protected resource requests to retrieve
  //       the user profile.
  this._oauth2 = new OAuth2(options.clientID,  options.clientSecret,
      '', options.authorizationURL, options.tokenURL, options.customHeaders);

  this._callbackURL = options.callbackURL;
  this._scope = options.scope;
  this._scopeSeparator = options.scopeSeparator || ' ';
  this._key = options.sessionKey || ('oauth2:' + url.parse(options.authorizationURL).hostname);

  if (options.store) {
    this._stateStore = options.store;
  } else {
    if (options.state) {
      this._stateStore = new SessionStateStore({ key: this._key });
    } else {
      this._stateStore = new NullStateStore();
    }
  }
  this._trustProxy = options.proxy;
  this._passReqToCallback = options.passReqToCallback;
  this._skipUserProfile = (options.skipUserProfile === undefined) ? false : options.skipUserProfile;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.passport-oauth.OAuth2Strategy.InternalOAuthError"></a>[function <span class="apidocSignatureSpan">passport-oauth.</span>OAuth2Strategy.InternalOAuthError (message, err)](#apidoc.element.passport-oauth.OAuth2Strategy.InternalOAuthError)
- description and source-code
```javascript
function InternalOAuthError(message, err) {
  Error.call(this);
  Error.captureStackTrace(this, this.constructor);
  this.name = this.constructor.name;
  this.message = message;
  this.oauthError = err;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.passport-oauth.OAuth2Strategy.super_"></a>[function <span class="apidocSignatureSpan">passport-oauth.</span>OAuth2Strategy.super_ ()](#apidoc.element.passport-oauth.OAuth2Strategy.super_)
- description and source-code
```javascript
function Strategy() {
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.passport-oauth.OAuthStrategy"></a>[function <span class="apidocSignatureSpan">passport-oauth.</span>OAuthStrategy (options, verify)](#apidoc.element.passport-oauth.OAuthStrategy)
- description and source-code
```javascript
function OAuthStrategy(options, verify) {
  if (typeof options == 'function') {
    verify = options;
    options = undefined;
  }
  options = options || {};

  if (!verify) { throw new TypeError('OAuthStrategy requires a verify callback'); }
  if (!options.requestTokenURL) { throw new TypeError('OAuthStrategy requires a requestTokenURL option'); }
  if (!options.accessTokenURL) { throw new TypeError('OAuthStrategy requires a accessTokenURL option'); }
  if (!options.userAuthorizationURL) { throw new TypeError('OAuthStrategy requires a userAuthorizationURL option'); }
  if (!options.consumerKey) { throw new TypeError('OAuthStrategy requires a consumerKey option'); }
  if (options.consumerSecret === undefined) { throw new TypeError('OAuthStrategy requires a consumerSecret option'); }

  passport.Strategy.call(this);
  this.name = 'oauth';
  this._verify = verify;

  // NOTE: The _oauth property is considered "protected".  Subclasses are
  //       allowed to use it when making protected resource requests to retrieve
  //       the user profile.
  this._oauth = new OAuth(options.requestTokenURL, options.accessTokenURL,
                          options.consumerKey,  options.consumerSecret,
                          '1.0', null, options.signatureMethod || 'HMAC-SHA1',
                          null, options.customHeaders);

  this._userAuthorizationURL = options.userAuthorizationURL;
  this._callbackURL = options.callbackURL;
  this._key = options.sessionKey || 'oauth';
  this._requestTokenStore = options.requestTokenStore || new SessionRequestTokenStore({ key: this._key });
  this._trustProxy = options.proxy;
  this._passReqToCallback = options.passReqToCallback;
  this._skipUserProfile = (options.skipUserProfile === undefined) ? false : options.skipUserProfile;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.passport-oauth.InternalOAuthError"></a>[module passport-oauth.InternalOAuthError](#apidoc.module.passport-oauth.InternalOAuthError)

#### <a name="apidoc.element.passport-oauth.InternalOAuthError.InternalOAuthError"></a>[function <span class="apidocSignatureSpan">passport-oauth.</span>InternalOAuthError (message, err)](#apidoc.element.passport-oauth.InternalOAuthError.InternalOAuthError)
- description and source-code
```javascript
function InternalOAuthError(message, err) {
  Error.call(this);
  Error.captureStackTrace(this, this.constructor);
  this.name = this.constructor.name;
  this.message = message;
  this.oauthError = err;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.passport-oauth.InternalOAuthError.prototype"></a>[module passport-oauth.InternalOAuthError.prototype](#apidoc.module.passport-oauth.InternalOAuthError.prototype)

#### <a name="apidoc.element.passport-oauth.InternalOAuthError.prototype.toString"></a>[function <span class="apidocSignatureSpan">passport-oauth.InternalOAuthError.prototype.</span>toString ()](#apidoc.element.passport-oauth.InternalOAuthError.prototype.toString)
- description and source-code
```javascript
toString = function () {
  var m = this.name;
  if (this.message) { m += ': ' + this.message; }
  if (this.oauthError) {
    if (this.oauthError instanceof Error) {
      m = this.oauthError.toString();
    } else if (this.oauthError.statusCode && this.oauthError.data) {
      m += ' (status: ' + this.oauthError.statusCode + ' data: ' + this.oauthError.data + ')';
    }
  }
  return m;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.passport-oauth.OAuth2Strategy"></a>[module passport-oauth.OAuth2Strategy](#apidoc.module.passport-oauth.OAuth2Strategy)

#### <a name="apidoc.element.passport-oauth.OAuth2Strategy.OAuth2Strategy"></a>[function <span class="apidocSignatureSpan">passport-oauth.</span>OAuth2Strategy (options, verify)](#apidoc.element.passport-oauth.OAuth2Strategy.OAuth2Strategy)
- description and source-code
```javascript
function OAuth2Strategy(options, verify) {
  if (typeof options == 'function') {
    verify = options;
    options = undefined;
  }
  options = options || {};

  if (!verify) { throw new TypeError('OAuth2Strategy requires a verify callback'); }
  if (!options.authorizationURL) { throw new TypeError('OAuth2Strategy requires a authorizationURL option'); }
  if (!options.tokenURL) { throw new TypeError('OAuth2Strategy requires a tokenURL option'); }
  if (!options.clientID) { throw new TypeError('OAuth2Strategy requires a clientID option'); }

  passport.Strategy.call(this);
  this.name = 'oauth2';
  this._verify = verify;

  // NOTE: The _oauth2 property is considered "protected".  Subclasses are
  //       allowed to use it when making protected resource requests to retrieve
  //       the user profile.
  this._oauth2 = new OAuth2(options.clientID,  options.clientSecret,
      '', options.authorizationURL, options.tokenURL, options.customHeaders);

  this._callbackURL = options.callbackURL;
  this._scope = options.scope;
  this._scopeSeparator = options.scopeSeparator || ' ';
  this._key = options.sessionKey || ('oauth2:' + url.parse(options.authorizationURL).hostname);

  if (options.store) {
    this._stateStore = options.store;
  } else {
    if (options.state) {
      this._stateStore = new SessionStateStore({ key: this._key });
    } else {
      this._stateStore = new NullStateStore();
    }
  }
  this._trustProxy = options.proxy;
  this._passReqToCallback = options.passReqToCallback;
  this._skipUserProfile = (options.skipUserProfile === undefined) ? false : options.skipUserProfile;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.passport-oauth.OAuth2Strategy.AuthorizationError"></a>[function <span class="apidocSignatureSpan">passport-oauth.OAuth2Strategy.</span>AuthorizationError (message, code, uri, status)](#apidoc.element.passport-oauth.OAuth2Strategy.AuthorizationError)
- description and source-code
```javascript
function AuthorizationError(message, code, uri, status) {
  if (!status) {
    switch (code) {
      case 'access_denied': status = 403; break;
      case 'server_error': status = 502; break;
      case 'temporarily_unavailable': status = 503; break;
    }
  }

  Error.call(this);
  Error.captureStackTrace(this, this.constructor);
  this.name = this.constructor.name;
  this.message = message;
  this.code = code || 'server_error';
  this.uri = uri;
  this.status = status || 500;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.passport-oauth.OAuth2Strategy.InternalOAuthError"></a>[function <span class="apidocSignatureSpan">passport-oauth.OAuth2Strategy.</span>InternalOAuthError (message, err)](#apidoc.element.passport-oauth.OAuth2Strategy.InternalOAuthError)
- description and source-code
```javascript
function InternalOAuthError(message, err) {
  Error.call(this);
  Error.captureStackTrace(this, this.constructor);
  this.name = this.constructor.name;
  this.message = message;
  this.oauthError = err;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.passport-oauth.OAuth2Strategy.Strategy"></a>[function <span class="apidocSignatureSpan">passport-oauth.OAuth2Strategy.</span>Strategy (options, verify)](#apidoc.element.passport-oauth.OAuth2Strategy.Strategy)
- description and source-code
```javascript
function OAuth2Strategy(options, verify) {
  if (typeof options == 'function') {
    verify = options;
    options = undefined;
  }
  options = options || {};

  if (!verify) { throw new TypeError('OAuth2Strategy requires a verify callback'); }
  if (!options.authorizationURL) { throw new TypeError('OAuth2Strategy requires a authorizationURL option'); }
  if (!options.tokenURL) { throw new TypeError('OAuth2Strategy requires a tokenURL option'); }
  if (!options.clientID) { throw new TypeError('OAuth2Strategy requires a clientID option'); }

  passport.Strategy.call(this);
  this.name = 'oauth2';
  this._verify = verify;

  // NOTE: The _oauth2 property is considered "protected".  Subclasses are
  //       allowed to use it when making protected resource requests to retrieve
  //       the user profile.
  this._oauth2 = new OAuth2(options.clientID,  options.clientSecret,
      '', options.authorizationURL, options.tokenURL, options.customHeaders);

  this._callbackURL = options.callbackURL;
  this._scope = options.scope;
  this._scopeSeparator = options.scopeSeparator || ' ';
  this._key = options.sessionKey || ('oauth2:' + url.parse(options.authorizationURL).hostname);

  if (options.store) {
    this._stateStore = options.store;
  } else {
    if (options.state) {
      this._stateStore = new SessionStateStore({ key: this._key });
    } else {
      this._stateStore = new NullStateStore();
    }
  }
  this._trustProxy = options.proxy;
  this._passReqToCallback = options.passReqToCallback;
  this._skipUserProfile = (options.skipUserProfile === undefined) ? false : options.skipUserProfile;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.passport-oauth.OAuth2Strategy.TokenError"></a>[function <span class="apidocSignatureSpan">passport-oauth.OAuth2Strategy.</span>TokenError (message, code, uri, status)](#apidoc.element.passport-oauth.OAuth2Strategy.TokenError)
- description and source-code
```javascript
function TokenError(message, code, uri, status) {
  Error.call(this);
  Error.captureStackTrace(this, this.constructor);
  this.name = this.constructor.name;
  this.message = message;
  this.code = code || 'invalid_request';
  this.uri = uri;
  this.status = status || 500;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.passport-oauth.OAuth2Strategy.super_"></a>[function <span class="apidocSignatureSpan">passport-oauth.OAuth2Strategy.</span>super_ ()](#apidoc.element.passport-oauth.OAuth2Strategy.super_)
- description and source-code
```javascript
function Strategy() {
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.passport-oauth.OAuth2Strategy.InternalOAuthError"></a>[module passport-oauth.OAuth2Strategy.InternalOAuthError](#apidoc.module.passport-oauth.OAuth2Strategy.InternalOAuthError)

#### <a name="apidoc.element.passport-oauth.OAuth2Strategy.InternalOAuthError.InternalOAuthError"></a>[function <span class="apidocSignatureSpan">passport-oauth.OAuth2Strategy.</span>InternalOAuthError (message, err)](#apidoc.element.passport-oauth.OAuth2Strategy.InternalOAuthError.InternalOAuthError)
- description and source-code
```javascript
function InternalOAuthError(message, err) {
  Error.call(this);
  Error.captureStackTrace(this, this.constructor);
  this.name = this.constructor.name;
  this.message = message;
  this.oauthError = err;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.passport-oauth.OAuth2Strategy.InternalOAuthError.prototype"></a>[module passport-oauth.OAuth2Strategy.InternalOAuthError.prototype](#apidoc.module.passport-oauth.OAuth2Strategy.InternalOAuthError.prototype)

#### <a name="apidoc.element.passport-oauth.OAuth2Strategy.InternalOAuthError.prototype.toString"></a>[function <span class="apidocSignatureSpan">passport-oauth.OAuth2Strategy.InternalOAuthError.prototype.</span>toString ()](#apidoc.element.passport-oauth.OAuth2Strategy.InternalOAuthError.prototype.toString)
- description and source-code
```javascript
toString = function () {
  var m = this.name;
  if (this.message) { m += ': ' + this.message; }
  if (this.oauthError) {
    if (this.oauthError instanceof Error) {
      m = this.oauthError.toString();
    } else if (this.oauthError.statusCode && this.oauthError.data) {
      m += ' (status: ' + this.oauthError.statusCode + ' data: ' + this.oauthError.data + ')';
    }
  }
  return m;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.passport-oauth.OAuth2Strategy.prototype"></a>[module passport-oauth.OAuth2Strategy.prototype](#apidoc.module.passport-oauth.OAuth2Strategy.prototype)

#### <a name="apidoc.element.passport-oauth.OAuth2Strategy.prototype._createOAuthError"></a>[function <span class="apidocSignatureSpan">passport-oauth.OAuth2Strategy.prototype.</span>_createOAuthError (message, err)](#apidoc.element.passport-oauth.OAuth2Strategy.prototype._createOAuthError)
- description and source-code
```javascript
_createOAuthError = function (message, err) {
  var e;
  if (err.statusCode && err.data) {
    try {
      e = this.parseErrorResponse(err.data, err.statusCode);
    } catch (_) {}
  }
  if (!e) { e = new InternalOAuthError(message, err); }
  return e;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.passport-oauth.OAuth2Strategy.prototype._loadUserProfile"></a>[function <span class="apidocSignatureSpan">passport-oauth.OAuth2Strategy.prototype.</span>_loadUserProfile (accessToken, done)](#apidoc.element.passport-oauth.OAuth2Strategy.prototype._loadUserProfile)
- description and source-code
```javascript
_loadUserProfile = function (accessToken, done) {
  var self = this;

  function loadIt() {
    return self.userProfile(accessToken, done);
  }
  function skipIt() {
    return done(null);
  }

  if (typeof this._skipUserProfile == 'function' && this._skipUserProfile.length > 1) {
    // async
    this._skipUserProfile(accessToken, function(err, skip) {
      if (err) { return done(err); }
      if (!skip) { return loadIt(); }
      return skipIt();
    });
  } else {
    var skip = (typeof this._skipUserProfile == 'function') ? this._skipUserProfile() : this._skipUserProfile;
    if (!skip) { return loadIt(); }
    return skipIt();
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.passport-oauth.OAuth2Strategy.prototype.authenticate"></a>[function <span class="apidocSignatureSpan">passport-oauth.OAuth2Strategy.prototype.</span>authenticate (req, options)](#apidoc.element.passport-oauth.OAuth2Strategy.prototype.authenticate)
- description and source-code
```javascript
authenticate = function (req, options) {
  options = options || {};
  var self = this;

  if (req.query && req.query.error) {
    if (req.query.error == 'access_denied') {
      return this.fail({ message: req.query.error_description });
    } else {
      return this.error(new AuthorizationError(req.query.error_description, req.query.error, req.query.error_uri));
    }
  }

  var callbackURL = options.callbackURL || this._callbackURL;
  if (callbackURL) {
    var parsed = url.parse(callbackURL);
    if (!parsed.protocol) {
      // The callback URL is relative, resolve a fully qualified URL from the
      // URL of the originating request.
      callbackURL = url.resolve(utils.originalURL(req, { proxy: this._trustProxy }), callbackURL);
    }
  }

  var meta = {
    authorizationURL: this._oauth2._authorizeUrl,
    tokenURL: this._oauth2._accessTokenUrl,
    clientID: this._oauth2._clientId
  }

  if (req.query && req.query.code) {
    function loaded(err, ok, state) {
      if (err) { return self.error(err); }
      if (!ok) {
        return self.fail(state, 403);
      }

      var code = req.query.code;

      var params = self.tokenParams(options);
      params.grant_type = 'authorization_code';
      if (callbackURL) { params.redirect_uri = callbackURL; }

      self._oauth2.getOAuthAccessToken(code, params,
        function(err, accessToken, refreshToken, params) {
          if (err) { return self.error(self._createOAuthError('Failed to obtain access token', err)); }

          self._loadUserProfile(accessToken, function(err, profile) {
            if (err) { return self.error(err); }

            function verified(err, user, info) {
              if (err) { return self.error(err); }
              if (!user) { return self.fail(info); }

              info = info || {};
              if (state) { info.state = state; }
              self.success(user, info);
            }

            try {
              if (self._passReqToCallback) {
                var arity = self._verify.length;
                if (arity == 6) {
                  self._verify(req, accessToken, refreshToken, params, profile, verified);
                } else { // arity == 5
                  self._verify(req, accessToken, refreshToken, profile, verified);
                }
              } else {
                var arity = self._verify.length;
                if (arity == 5) {
                  self._verify(accessToken, refreshToken, params, profile, verified);
                } else { // arity == 4
                  self._verify(accessToken, refreshToken, profile, verified);
                }
              }
            } catch (ex) {
              return self.error(ex);
            }
          });
        }
      );
    }

    var state = req.query.state;
    try {
      var arity = this._stateStore.verify.length;
      if (arity == 4) {
        this._stateStore.verify(req, state, meta, loaded);
      } else { // arity == 3
        this._stateStore.verify(req, state, loaded);
      }
    } catch (ex) {
      return this.error(ex);
    }
  } else {
    var params = this.authorizationParams(options);
    params.response_type = 'code';
    if (callbackURL) { params.redirect_uri = callbackURL; }
    var scope = options.scope || this._scope;
    if (scope) {
      if (Array.isArray(scope)) { scope = scope.join(this._scopeSeparator); }
      params.scope = scope;
    }

    var state = options.state;
    if (state) {
      params.state = state;

      var parsed = url.parse(this._oauth2._authorizeUrl, true);
      utils.merge(parsed.query, params);
      parsed.query['client_id'] = this._oauth2._clientId;
      delete parsed.search;
      var location = url.format(parsed);
      this.redirect(location);
    } else {
      function stored(err, state) {
        if (err) { return self.error(err); }

        if (state) { params.state = state; }
        var parsed = url.parse(self._oauth2._authorizeUrl, true);
        utils.merge(parsed.query, params);
        parsed.query['client_id'] = self._oauth2._clientId;
        delete parsed.search; ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.passport-oauth.OAuth2Strategy.prototype.authorizationParams"></a>[function <span class="apidocSignatureSpan">passport-oauth.OAuth2Strategy.prototype.</span>authorizationParams (options)](#apidoc.element.passport-oauth.OAuth2Strategy.prototype.authorizationParams)
- description and source-code
```javascript
authorizationParams = function (options) {
  return {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.passport-oauth.OAuth2Strategy.prototype.parseErrorResponse"></a>[function <span class="apidocSignatureSpan">passport-oauth.OAuth2Strategy.prototype.</span>parseErrorResponse (body, status)](#apidoc.element.passport-oauth.OAuth2Strategy.prototype.parseErrorResponse)
- description and source-code
```javascript
parseErrorResponse = function (body, status) {
  var json = JSON.parse(body);
  if (json.error) {
    return new TokenError(json.error_description, json.error, json.error_uri);
  }
  return null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.passport-oauth.OAuth2Strategy.prototype.tokenParams"></a>[function <span class="apidocSignatureSpan">passport-oauth.OAuth2Strategy.prototype.</span>tokenParams (options)](#apidoc.element.passport-oauth.OAuth2Strategy.prototype.tokenParams)
- description and source-code
```javascript
tokenParams = function (options) {
  return {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.passport-oauth.OAuth2Strategy.prototype.userProfile"></a>[function <span class="apidocSignatureSpan">passport-oauth.OAuth2Strategy.prototype.</span>userProfile (accessToken, done)](#apidoc.element.passport-oauth.OAuth2Strategy.prototype.userProfile)
- description and source-code
```javascript
userProfile = function (accessToken, done) {
  return done(null, {});
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.passport-oauth.OAuth2Strategy.super_"></a>[module passport-oauth.OAuth2Strategy.super_](#apidoc.module.passport-oauth.OAuth2Strategy.super_)

#### <a name="apidoc.element.passport-oauth.OAuth2Strategy.super_.super_"></a>[function <span class="apidocSignatureSpan">passport-oauth.OAuth2Strategy.</span>super_ ()](#apidoc.element.passport-oauth.OAuth2Strategy.super_.super_)
- description and source-code
```javascript
function Strategy() {
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.passport-oauth.OAuth2Strategy.super_.Strategy"></a>[function <span class="apidocSignatureSpan">passport-oauth.OAuth2Strategy.super_.</span>Strategy ()](#apidoc.element.passport-oauth.OAuth2Strategy.super_.Strategy)
- description and source-code
```javascript
function Strategy() {
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.passport-oauth.OAuth2Strategy.super_.prototype"></a>[module passport-oauth.OAuth2Strategy.super_.prototype](#apidoc.module.passport-oauth.OAuth2Strategy.super_.prototype)

#### <a name="apidoc.element.passport-oauth.OAuth2Strategy.super_.prototype.authenticate"></a>[function <span class="apidocSignatureSpan">passport-oauth.OAuth2Strategy.super_.prototype.</span>authenticate (req, options)](#apidoc.element.passport-oauth.OAuth2Strategy.super_.prototype.authenticate)
- description and source-code
```javascript
authenticate = function (req, options) {
  throw new Error('Strategy#authenticate must be overridden by subclass');
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.passport-oauth.OAuthStrategy"></a>[module passport-oauth.OAuthStrategy](#apidoc.module.passport-oauth.OAuthStrategy)

#### <a name="apidoc.element.passport-oauth.OAuthStrategy.OAuthStrategy"></a>[function <span class="apidocSignatureSpan">passport-oauth.</span>OAuthStrategy (options, verify)](#apidoc.element.passport-oauth.OAuthStrategy.OAuthStrategy)
- description and source-code
```javascript
function OAuthStrategy(options, verify) {
  if (typeof options == 'function') {
    verify = options;
    options = undefined;
  }
  options = options || {};

  if (!verify) { throw new TypeError('OAuthStrategy requires a verify callback'); }
  if (!options.requestTokenURL) { throw new TypeError('OAuthStrategy requires a requestTokenURL option'); }
  if (!options.accessTokenURL) { throw new TypeError('OAuthStrategy requires a accessTokenURL option'); }
  if (!options.userAuthorizationURL) { throw new TypeError('OAuthStrategy requires a userAuthorizationURL option'); }
  if (!options.consumerKey) { throw new TypeError('OAuthStrategy requires a consumerKey option'); }
  if (options.consumerSecret === undefined) { throw new TypeError('OAuthStrategy requires a consumerSecret option'); }

  passport.Strategy.call(this);
  this.name = 'oauth';
  this._verify = verify;

  // NOTE: The _oauth property is considered "protected".  Subclasses are
  //       allowed to use it when making protected resource requests to retrieve
  //       the user profile.
  this._oauth = new OAuth(options.requestTokenURL, options.accessTokenURL,
                          options.consumerKey,  options.consumerSecret,
                          '1.0', null, options.signatureMethod || 'HMAC-SHA1',
                          null, options.customHeaders);

  this._userAuthorizationURL = options.userAuthorizationURL;
  this._callbackURL = options.callbackURL;
  this._key = options.sessionKey || 'oauth';
  this._requestTokenStore = options.requestTokenStore || new SessionRequestTokenStore({ key: this._key });
  this._trustProxy = options.proxy;
  this._passReqToCallback = options.passReqToCallback;
  this._skipUserProfile = (options.skipUserProfile === undefined) ? false : options.skipUserProfile;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.passport-oauth.OAuthStrategy.InternalOAuthError"></a>[function <span class="apidocSignatureSpan">passport-oauth.OAuthStrategy.</span>InternalOAuthError (message, err)](#apidoc.element.passport-oauth.OAuthStrategy.InternalOAuthError)
- description and source-code
```javascript
function InternalOAuthError(message, err) {
  Error.call(this);
  Error.captureStackTrace(this, this.constructor);
  this.name = this.constructor.name;
  this.message = message;
  this.oauthError = err;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.passport-oauth.OAuthStrategy.Strategy"></a>[function <span class="apidocSignatureSpan">passport-oauth.OAuthStrategy.</span>Strategy (options, verify)](#apidoc.element.passport-oauth.OAuthStrategy.Strategy)
- description and source-code
```javascript
function OAuthStrategy(options, verify) {
  if (typeof options == 'function') {
    verify = options;
    options = undefined;
  }
  options = options || {};

  if (!verify) { throw new TypeError('OAuthStrategy requires a verify callback'); }
  if (!options.requestTokenURL) { throw new TypeError('OAuthStrategy requires a requestTokenURL option'); }
  if (!options.accessTokenURL) { throw new TypeError('OAuthStrategy requires a accessTokenURL option'); }
  if (!options.userAuthorizationURL) { throw new TypeError('OAuthStrategy requires a userAuthorizationURL option'); }
  if (!options.consumerKey) { throw new TypeError('OAuthStrategy requires a consumerKey option'); }
  if (options.consumerSecret === undefined) { throw new TypeError('OAuthStrategy requires a consumerSecret option'); }

  passport.Strategy.call(this);
  this.name = 'oauth';
  this._verify = verify;

  // NOTE: The _oauth property is considered "protected".  Subclasses are
  //       allowed to use it when making protected resource requests to retrieve
  //       the user profile.
  this._oauth = new OAuth(options.requestTokenURL, options.accessTokenURL,
                          options.consumerKey,  options.consumerSecret,
                          '1.0', null, options.signatureMethod || 'HMAC-SHA1',
                          null, options.customHeaders);

  this._userAuthorizationURL = options.userAuthorizationURL;
  this._callbackURL = options.callbackURL;
  this._key = options.sessionKey || 'oauth';
  this._requestTokenStore = options.requestTokenStore || new SessionRequestTokenStore({ key: this._key });
  this._trustProxy = options.proxy;
  this._passReqToCallback = options.passReqToCallback;
  this._skipUserProfile = (options.skipUserProfile === undefined) ? false : options.skipUserProfile;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.passport-oauth.OAuthStrategy.super_"></a>[function <span class="apidocSignatureSpan">passport-oauth.OAuthStrategy.</span>super_ ()](#apidoc.element.passport-oauth.OAuthStrategy.super_)
- description and source-code
```javascript
function Strategy() {
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.passport-oauth.OAuthStrategy.prototype"></a>[module passport-oauth.OAuthStrategy.prototype](#apidoc.module.passport-oauth.OAuthStrategy.prototype)

#### <a name="apidoc.element.passport-oauth.OAuthStrategy.prototype._createOAuthError"></a>[function <span class="apidocSignatureSpan">passport-oauth.OAuthStrategy.prototype.</span>_createOAuthError (message, err)](#apidoc.element.passport-oauth.OAuthStrategy.prototype._createOAuthError)
- description and source-code
```javascript
_createOAuthError = function (message, err) {
  var e;
  if (err.statusCode && err.data) {
    try {
      e = this.parseErrorResponse(err.data, err.statusCode);
    } catch (_) {}
  }
  if (!e) { e = new InternalOAuthError(message, err); }
  return e;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.passport-oauth.OAuthStrategy.prototype._loadUserProfile"></a>[function <span class="apidocSignatureSpan">passport-oauth.OAuthStrategy.prototype.</span>_loadUserProfile (token, tokenSecret, params, done)](#apidoc.element.passport-oauth.OAuthStrategy.prototype._loadUserProfile)
- description and source-code
```javascript
_loadUserProfile = function (token, tokenSecret, params, done) {
  var self = this;

  function loadIt() {
    return self.userProfile(token, tokenSecret, params, done);
  }
  function skipIt() {
    return done(null);
  }

  if (typeof this._skipUserProfile == 'function' && this._skipUserProfile.length > 1) {
    // async
    this._skipUserProfile(token, tokenSecret, function(err, skip) {
      if (err) { return done(err); }
      if (!skip) { return loadIt(); }
      return skipIt();
    });
  } else {
    var skip = (typeof this._skipUserProfile == 'function') ? this._skipUserProfile() : this._skipUserProfile;
    if (!skip) { return loadIt(); }
    return skipIt();
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.passport-oauth.OAuthStrategy.prototype.authenticate"></a>[function <span class="apidocSignatureSpan">passport-oauth.OAuthStrategy.prototype.</span>authenticate (req, options)](#apidoc.element.passport-oauth.OAuthStrategy.prototype.authenticate)
- description and source-code
```javascript
authenticate = function (req, options) {
  options = options || {};

  var self = this;
  var meta = {
    requestTokenURL: this._oauth._requestUrl,
    accessTokenURL: this._oauth._accessUrl,
    userAuthorizationURL:  this._userAuthorizationURL,
    consumerKey: this._oauth._consumerKey
  }

  if (req.query && req.query.oauth_token) {
    // The request being authenticated contains an oauth_token parameter in the
    // query portion of the URL.  This indicates that the service provider has
    // redirected the user back to the application, after authenticating the
    // user and obtaining their authorization.
    //
    // The value of the oauth_token parameter is the request token.  Together
    // with knowledge of the token secret (stored in the session), the request
    // token can be exchanged for an access token and token secret.
    //
    // This access token and token secret, along with the optional ability to
    // fetch profile information from the service provider, is sufficient to
    // establish the identity of the user.
    var oauthToken = req.query.oauth_token;

    function loaded(err, oauthTokenSecret, state) {
      if (err) { return self.error(err); }
      if (!oauthTokenSecret) {
        return self.fail(state, 403);
      }

      // NOTE: The oauth_verifier parameter will be supplied in the query portion
      //       of the redirect URL, if the server supports OAuth 1.0a.
      var oauthVerifier = req.query.oauth_verifier || null;

      self._oauth.getOAuthAccessToken(oauthToken, oauthTokenSecret, oauthVerifier, function(err, token, tokenSecret, params) {
        if (err) { return self.error(self._createOAuthError('Failed to obtain access token', err)); }

        function destroyed(err) {
          if (err) { return self.error(err); }

          self._loadUserProfile(token, tokenSecret, params, function(err, profile) {
            if (err) { return self.error(err); }

            function verified(err, user, info) {
              if (err) { return self.error(err); }
              if (!user) { return self.fail(info); }

              info = info || {};
              if (state) { info.state = state; }
              self.success(user, info);
            }

            try {
              if (self._passReqToCallback) {
                var arity = self._verify.length;
                if (arity == 6) {
                  self._verify(req, token, tokenSecret, params, profile, verified);
                } else { // arity == 5
                  self._verify(req, token, tokenSecret, profile, verified);
                }
              } else {
                var arity = self._verify.length;
                if (arity == 5) {
                  self._verify(token, tokenSecret, params, profile, verified);
                } else { // arity == 4
                  self._verify(token, tokenSecret, profile, verified);
                }
              }
            } catch (ex) {
              return self.error(ex);
            }
          });
        }

        // The request token has been exchanged for an access token.  Since the
        // request token is a single-use token, that data can be removed from the
        // store.
        try {
          var arity = self._requestTokenStore.destroy.length;
          if (arity == 4) {
            self._requestTokenStore.destroy(req, oauthToken, meta, destroyed);
          } else { // arity == 3
            self._requestTokenStore.destroy(req, oauthToken, destroyed);
          }
        } catch (ex) {
          return self.error(ex);
        }
      });
    }

    try {
      var arity = self._requestTokenStore.get.length;
      if (arity == 4) {
        this._requestTokenStore.get(req, oauthToken, meta, loaded);
      } else { // arity == 3
        this._requestTokenStore.get(req, oauthToken, loaded);
      }
    } catch (ex) {
      return this.error(ex);
    }
  } else {
    // In order to authenticate via OAuth, the application must obtain a request
    // token from the service provider and redirect th ...
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.passport-oauth.OAuthStrategy.prototype.parseErrorResponse"></a>[function <span class="apidocSignatureSpan">passport-oauth.OAuthStrategy.prototype.</span>parseErrorResponse (body, status)](#apidoc.element.passport-oauth.OAuthStrategy.prototype.parseErrorResponse)
- description and source-code
```javascript
parseErrorResponse = function (body, status) {
  return null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.passport-oauth.OAuthStrategy.prototype.requestTokenParams"></a>[function <span class="apidocSignatureSpan">passport-oauth.OAuthStrategy.prototype.</span>requestTokenParams (options)](#apidoc.element.passport-oauth.OAuthStrategy.prototype.requestTokenParams)
- description and source-code
```javascript
requestTokenParams = function (options) {
  return {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.passport-oauth.OAuthStrategy.prototype.userAuthorizationParams"></a>[function <span class="apidocSignatureSpan">passport-oauth.OAuthStrategy.prototype.</span>userAuthorizationParams (options)](#apidoc.element.passport-oauth.OAuthStrategy.prototype.userAuthorizationParams)
- description and source-code
```javascript
userAuthorizationParams = function (options) {
  return {};
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.passport-oauth.OAuthStrategy.prototype.userProfile"></a>[function <span class="apidocSignatureSpan">passport-oauth.OAuthStrategy.prototype.</span>userProfile (token, tokenSecret, params, done)](#apidoc.element.passport-oauth.OAuthStrategy.prototype.userProfile)
- description and source-code
```javascript
userProfile = function (token, tokenSecret, params, done) {
  return done(null, {});
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
