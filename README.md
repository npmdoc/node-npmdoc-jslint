# api documentation for  [jslint (v0.10.3)](https://github.com/reid/node-jslint)  [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-jslint.svg)](https://travis-ci.org/npmdoc/node-npmdoc-jslint)
#### The JavaScript Code Quality Tool

[![NPM](https://nodei.co/npm/jslint.png?downloads=true)](https://www.npmjs.com/package/jslint)

[![apidoc](https://npmdoc.github.io/node-npmdoc-jslint/build/screen-capture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-jslint_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-jslint/build..beta..travis-ci.org/apidoc.html)

![package-listing](https://npmdoc.github.io/node-npmdoc-jslint/build/screen-capture.npmPackageListing.svg)



# package.json

```json

{
    "author": {
        "name": "Reid Burke",
        "email": "me@reidburke.com"
    },
    "bin": {
        "jslint": "./bin/jslint.js"
    },
    "bugs": {
        "url": "https://github.com/reid/node-jslint/issues"
    },
    "contributors": [
        {
            "name": "Douglas Crockford",
            "email": "douglas@crockford.com"
        },
        {
            "name": "Mikeal Rogers",
            "email": "mikeal.rogers@gmail.com"
        },
        {
            "name": "Adam Moore"
        },
        {
            "name": "Luke Smith",
            "email": "lsmith@yahoo-inc.com"
        },
        {
            "name": "Anders Conbere",
            "email": "aconbere@gmail.com"
        },
        {
            "name": "Ryuichi OKUMURA",
            "email": "okuryu@okuryu.com"
        },
        {
            "name": "Sam Mikes",
            "email": "smikes@cubane.com"
        },
        {
            "name": "Dylan Lloyd"
        },
        {
            "name": "Andreas Hindborg"
        },
        {
            "name": "Andrew Pennebaker"
        },
        {
            "name": "Bnaya"
        },
        {
            "name": "Maximilian Antoni",
            "email": "mail@maxantoni.de"
        },
        {
            "name": "Vasil Velichkov"
        },
        {
            "name": "Rasmus Paetau"
        },
        {
            "name": "Bryan Horna"
        }
    ],
    "dependencies": {
        "exit": "~0.1.2",
        "glob": "^7.0.3",
        "nopt": "~3.0.1",
        "readable-stream": "~2.1.2"
    },
    "description": "The JavaScript Code Quality Tool",
    "devDependencies": {
        "fs.extra": "^1.3.2",
        "istanbul": "^0.4.3",
        "marked-man": "~0.1.5",
        "mocha": "^3.0.0"
    },
    "directories": {
        "lib": "./lib",
        "man": "./man",
        "doc": "./doc"
    },
    "dist": {
        "shasum": "890da3e79932edf06c5f4b52a7b5ba6436867436",
        "tarball": "https://registry.npmjs.org/jslint/-/jslint-0.10.3.tgz"
    },
    "engines": {
        "node": ">=0.8.0"
    },
    "files": [
        "man/jslint.1",
        "doc/jslint.md",
        "doc/jslint.html",
        "lib",
        "bin",
        "jslint.conf.example",
        "Makefile"
    ],
    "gitHead": "c2cdb60176983c5e4e93aebbcba1d8c2c93ac416",
    "homepage": "https://github.com/reid/node-jslint",
    "keywords": [
        "lint",
        "jslint",
        "code-quality",
        "static-analysis",
        "jshint",
        "eslint"
    ],
    "license": "BSD-3-Clause",
    "licenses": [
        {
            "type": "Modified MIT / BSD",
            "url": "https://github.com/reid/node-jslint/blob/master/LICENSE"
        }
    ],
    "main": "./lib/nodelint.js",
    "maintainers": [
        {
            "name": "reid",
            "email": "me@reidburke.com"
        },
        {
            "name": "okuryu",
            "email": "okuryu@okuryu.com"
        },
        {
            "name": "smikes",
            "email": "smikes@cubane.com"
        }
    ],
    "man": [
        "man/jslint.1"
    ],
    "name": "jslint",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/reid/node-jslint.git"
    },
    "scripts": {
        "mypublish": "make prepublish; npm publish",
        "test": "make test"
    },
    "version": "0.10.3"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module jslint](#apidoc.module.jslint)
1.  [function <span class="apidocSignatureSpan">jslint.</span>LintStream (options)](#apidoc.element.jslint.LintStream)
1.  [function <span class="apidocSignatureSpan">jslint.</span>LintStream.super_ (options)](#apidoc.element.jslint.LintStream.super_)
1.  [function <span class="apidocSignatureSpan">jslint.</span>collectorstream (options)](#apidoc.element.jslint.collectorstream)
1.  [function <span class="apidocSignatureSpan">jslint.</span>fileopener ()](#apidoc.element.jslint.fileopener)
1.  [function <span class="apidocSignatureSpan">jslint.</span>jsonreportstream (options)](#apidoc.element.jslint.jsonreportstream)
1.  [function <span class="apidocSignatureSpan">jslint.</span>load (edition)](#apidoc.element.jslint.load)
1.  [function <span class="apidocSignatureSpan">jslint.</span>looksLikeFileName (edition)](#apidoc.element.jslint.looksLikeFileName)
1.  [function <span class="apidocSignatureSpan">jslint.</span>reportstream (options)](#apidoc.element.jslint.reportstream)
1.  [function <span class="apidocSignatureSpan">jslint.</span>runMain (options, cb)](#apidoc.element.jslint.runMain)
1.  [function <span class="apidocSignatureSpan">jslint.</span>setConsole (c)](#apidoc.element.jslint.setConsole)
1.  [function <span class="apidocSignatureSpan">jslint.</span>stream (options)](#apidoc.element.jslint.stream)
1.  object <span class="apidocSignatureSpan">jslint.</span>LintStream.prototype
1.  object <span class="apidocSignatureSpan">jslint.</span>LintStream.super_.prototype
1.  object <span class="apidocSignatureSpan">jslint.</span>LintStream.super_.super_.prototype
1.  object <span class="apidocSignatureSpan">jslint.</span>collectorstream.prototype
1.  object <span class="apidocSignatureSpan">jslint.</span>color
1.  object <span class="apidocSignatureSpan">jslint.</span>fileopener.prototype
1.  object <span class="apidocSignatureSpan">jslint.</span>jsonreportstream.prototype
1.  object <span class="apidocSignatureSpan">jslint.</span>linter
1.  object <span class="apidocSignatureSpan">jslint.</span>main
1.  object <span class="apidocSignatureSpan">jslint.</span>options
1.  object <span class="apidocSignatureSpan">jslint.</span>reporter
1.  object <span class="apidocSignatureSpan">jslint.</span>reportstream.prototype
1.  object <span class="apidocSignatureSpan">jslint.</span>stream.prototype

#### [module jslint.LintStream](#apidoc.module.jslint.LintStream)
1.  [function <span class="apidocSignatureSpan">jslint.</span>LintStream (options)](#apidoc.element.jslint.LintStream.LintStream)
1.  [function <span class="apidocSignatureSpan">jslint.LintStream.</span>super_ (options)](#apidoc.element.jslint.LintStream.super_)

#### [module jslint.LintStream.prototype](#apidoc.module.jslint.LintStream.prototype)
1.  [function <span class="apidocSignatureSpan">jslint.LintStream.prototype.</span>_transform (chunk, ignore, callback)](#apidoc.element.jslint.LintStream.prototype._transform)

#### [module jslint.LintStream.super_](#apidoc.module.jslint.LintStream.super_)
1.  [function <span class="apidocSignatureSpan">jslint.LintStream.</span>super_ (options)](#apidoc.element.jslint.LintStream.super_.super_)

#### [module jslint.LintStream.super_.prototype](#apidoc.module.jslint.LintStream.super_.prototype)
1.  [function <span class="apidocSignatureSpan">jslint.LintStream.super_.prototype.</span>_read (n)](#apidoc.element.jslint.LintStream.super_.prototype._read)
1.  [function <span class="apidocSignatureSpan">jslint.LintStream.super_.prototype.</span>_transform (chunk, encoding, cb)](#apidoc.element.jslint.LintStream.super_.prototype._transform)
1.  [function <span class="apidocSignatureSpan">jslint.LintStream.super_.prototype.</span>_write (chunk, encoding, cb)](#apidoc.element.jslint.LintStream.super_.prototype._write)
1.  [function <span class="apidocSignatureSpan">jslint.LintStream.super_.prototype.</span>push (chunk, encoding)](#apidoc.element.jslint.LintStream.super_.prototype.push)

#### [module jslint.LintStream.super_.super_.prototype](#apidoc.module.jslint.LintStream.super_.super_.prototype)
1.  [function <span class="apidocSignatureSpan">jslint.LintStream.super_.super_.prototype.</span>_write (chunk, encoding, cb)](#apidoc.element.jslint.LintStream.super_.super_.prototype._write)
1.  [function <span class="apidocSignatureSpan">jslint.LintStream.super_.super_.prototype.</span>cork ()](#apidoc.element.jslint.LintStream.super_.super_.prototype.cork)
1.  [function <span class="apidocSignatureSpan">jslint.LintStream.super_.super_.prototype.</span>end (chunk, encoding, cb)](#apidoc.element.jslint.LintStream.super_.super_.prototype.end)
1.  [function <span class="apidocSignatureSpan">jslint.LintStream.super_.super_.prototype.</span>setDefaultEncoding (encoding)](#apidoc.element.jslint.LintStream.super_.super_.prototype.setDefaultEncoding)
1.  [function <span class="apidocSignatureSpan">jslint.LintStream.super_.super_.prototype.</span>uncork ()](#apidoc.element.jslint.LintStream.super_.super_.prototype.uncork)
1.  [function <span class="apidocSignatureSpan">jslint.LintStream.super_.super_.prototype.</span>write (chunk, encoding, cb)](#apidoc.element.jslint.LintStream.super_.super_.prototype.write)
1.  object <span class="apidocSignatureSpan">jslint.LintStream.super_.super_.prototype.</span>_writev

#### [module jslint.collectorstream](#apidoc.module.jslint.collectorstream)
1.  [function <span class="apidocSignatureSpan">jslint.</span>collectorstream (options)](#apidoc.element.jslint.collectorstream.collectorstream)
1.  [function <span class="apidocSignatureSpan">jslint.collectorstream.</span>super_ (options)](#apidoc.element.jslint.collectorstream.super_)

#### [module jslint.collectorstream.prototype](#apidoc.module.jslint.collectorstream.prototype)
1.  [function <span class="apidocSignatureSpan">jslint.collectorstream.prototype.</span>_transform (chunk, ignore, callback)](#apidoc.element.jslint.collectorstream.prototype._transform)

#### [module jslint.color](#apidoc.module.jslint.color)
1.  [function <span class="apidocSignatureSpan">jslint.color.</span>blue (string)](#apidoc.element.jslint.color.blue)
1.  [function <span class="apidocSignatureSpan">jslint.color.</span>bold (string)](#apidoc.element.jslint.color.bold)
1.  [function <span class="apidocSignatureSpan">jslint.color.</span>green (string)](#apidoc.element.jslint.color.green)
1.  [function <span class="apidocSignatureSpan">jslint.color.</span>grey (string)](#apidoc.element.jslint.color.grey)
1.  [function <span class="apidocSignatureSpan">jslint.color.</span>red (string)](#apidoc.element.jslint.color.red)
1.  [function <span class="apidocSignatureSpan">jslint.color.</span>yellow (string)](#apidoc.element.jslint.color.yellow)

#### [module jslint.fileopener](#apidoc.module.jslint.fileopener)
1.  [function <span class="apidocSignatureSpan">jslint.</span>fileopener ()](#apidoc.element.jslint.fileopener.fileopener)
1.  [function <span class="apidocSignatureSpan">jslint.fileopener.</span>super_ (options)](#apidoc.element.jslint.fileopener.super_)

#### [module jslint.fileopener.prototype](#apidoc.module.jslint.fileopener.prototype)
1.  [function <span class="apidocSignatureSpan">jslint.fileopener.prototype.</span>_transform (file, ignore, callback)](#apidoc.element.jslint.fileopener.prototype._transform)

#### [module jslint.jsonreportstream](#apidoc.module.jslint.jsonreportstream)
1.  [function <span class="apidocSignatureSpan">jslint.</span>jsonreportstream (options)](#apidoc.element.jslint.jsonreportstream.jsonreportstream)
1.  [function <span class="apidocSignatureSpan">jslint.jsonreportstream.</span>super_ (options)](#apidoc.element.jslint.jsonreportstream.super_)

#### [module jslint.jsonreportstream.prototype](#apidoc.module.jslint.jsonreportstream.prototype)
1.  [function <span class="apidocSignatureSpan">jslint.jsonreportstream.prototype.</span>_transform (chunk, ignore, callback)](#apidoc.element.jslint.jsonreportstream.prototype._transform)

#### [module jslint.linter](#apidoc.module.jslint.linter)
1.  [function <span class="apidocSignatureSpan">jslint.linter.</span>doLint (jslint, script, options)](#apidoc.element.jslint.linter.doLint)
1.  [function <span class="apidocSignatureSpan">jslint.linter.</span>merge (source, add)](#apidoc.element.jslint.linter.merge)
1.  [function <span class="apidocSignatureSpan">jslint.linter.</span>preprocessScript (script)](#apidoc.element.jslint.linter.preprocessScript)

#### [module jslint.main](#apidoc.module.jslint.main)
1.  [function <span class="apidocSignatureSpan">jslint.main.</span>commandOptions ()](#apidoc.element.jslint.main.commandOptions)
1.  [function <span class="apidocSignatureSpan">jslint.main.</span>expandGlob (glob)](#apidoc.element.jslint.main.expandGlob)
1.  [function <span class="apidocSignatureSpan">jslint.main.</span>globFiles (list, glob, filter)](#apidoc.element.jslint.main.globFiles)
1.  [function <span class="apidocSignatureSpan">jslint.main.</span>makeReporter (parsed)](#apidoc.element.jslint.main.makeReporter)
1.  [function <span class="apidocSignatureSpan">jslint.main.</span>noNodeModules (file)](#apidoc.element.jslint.main.noNodeModules)
1.  [function <span class="apidocSignatureSpan">jslint.main.</span>parseArgs (argv)](#apidoc.element.jslint.main.parseArgs)
1.  [function <span class="apidocSignatureSpan">jslint.main.</span>reportVersion (callback, options)](#apidoc.element.jslint.main.reportVersion)
1.  [function <span class="apidocSignatureSpan">jslint.main.</span>runMain (options, cb)](#apidoc.element.jslint.main.runMain)
1.  [function <span class="apidocSignatureSpan">jslint.main.</span>setConsole (c)](#apidoc.element.jslint.main.setConsole)
1.  [function <span class="apidocSignatureSpan">jslint.main.</span>setProcess (p)](#apidoc.element.jslint.main.setProcess)

#### [module jslint.options](#apidoc.module.jslint.options)
1.  [function <span class="apidocSignatureSpan">jslint.options.</span>addDefaults (options)](#apidoc.element.jslint.options.addDefaults)
1.  [function <span class="apidocSignatureSpan">jslint.options.</span>getOptions (homedir, options)](#apidoc.element.jslint.options.getOptions)
1.  [function <span class="apidocSignatureSpan">jslint.options.</span>loadAndParseConfig (filePath)](#apidoc.element.jslint.options.loadAndParseConfig)
1.  [function <span class="apidocSignatureSpan">jslint.options.</span>loadConfig (h, configFile)](#apidoc.element.jslint.options.loadConfig)
1.  [function <span class="apidocSignatureSpan">jslint.options.</span>merge (source, add)](#apidoc.element.jslint.options.merge)
1.  [function <span class="apidocSignatureSpan">jslint.options.</span>mergeConfigs (home, project)](#apidoc.element.jslint.options.mergeConfigs)
1.  [function <span class="apidocSignatureSpan">jslint.options.</span>preprocessOptions (options, config)](#apidoc.element.jslint.options.preprocessOptions)
1.  [function <span class="apidocSignatureSpan">jslint.options.</span>setConsole (c)](#apidoc.element.jslint.options.setConsole)
1.  [function <span class="apidocSignatureSpan">jslint.options.</span>splitPredefs (options)](#apidoc.element.jslint.options.splitPredefs)

#### [module jslint.reporter](#apidoc.module.jslint.reporter)
1.  [function <span class="apidocSignatureSpan">jslint.reporter.</span>makeReporter (logger, colorize, terse)](#apidoc.element.jslint.reporter.makeReporter)
1.  [function <span class="apidocSignatureSpan">jslint.reporter.</span>report (file, lint, colorize, terse)](#apidoc.element.jslint.reporter.report)
1.  [function <span class="apidocSignatureSpan">jslint.reporter.</span>setLogger (l)](#apidoc.element.jslint.reporter.setLogger)
1.  object <span class="apidocSignatureSpan">jslint.reporter.</span>logger

#### [module jslint.reportstream](#apidoc.module.jslint.reportstream)
1.  [function <span class="apidocSignatureSpan">jslint.</span>reportstream (options)](#apidoc.element.jslint.reportstream.reportstream)
1.  [function <span class="apidocSignatureSpan">jslint.reportstream.</span>super_ (options)](#apidoc.element.jslint.reportstream.super_)

#### [module jslint.reportstream.prototype](#apidoc.module.jslint.reportstream.prototype)
1.  [function <span class="apidocSignatureSpan">jslint.reportstream.prototype.</span>_transform (chunk, ignore, callback)](#apidoc.element.jslint.reportstream.prototype._transform)

#### [module jslint.stream](#apidoc.module.jslint.stream)
1.  [function <span class="apidocSignatureSpan">jslint.</span>stream (options)](#apidoc.element.jslint.stream.stream)
1.  [function <span class="apidocSignatureSpan">jslint.stream.</span>Duplex (options)](#apidoc.element.jslint.stream.Duplex)
1.  [function <span class="apidocSignatureSpan">jslint.stream.</span>PassThrough (options)](#apidoc.element.jslint.stream.PassThrough)
1.  [function <span class="apidocSignatureSpan">jslint.stream.</span>Readable (options)](#apidoc.element.jslint.stream.Readable)
1.  [function <span class="apidocSignatureSpan">jslint.stream.</span>ReadableState (options, stream)](#apidoc.element.jslint.stream.ReadableState)
1.  [function <span class="apidocSignatureSpan">jslint.stream.</span>Stream ()](#apidoc.element.jslint.stream.Stream)
1.  [function <span class="apidocSignatureSpan">jslint.stream.</span>Transform (options)](#apidoc.element.jslint.stream.Transform)
1.  [function <span class="apidocSignatureSpan">jslint.stream.</span>Writable (options)](#apidoc.element.jslint.stream.Writable)
1.  [function <span class="apidocSignatureSpan">jslint.stream.</span>_fromList (n, state)](#apidoc.element.jslint.stream._fromList)
1.  [function <span class="apidocSignatureSpan">jslint.stream.</span>super_ ()](#apidoc.element.jslint.stream.super_)

#### [module jslint.stream.prototype](#apidoc.module.jslint.stream.prototype)
1.  [function <span class="apidocSignatureSpan">jslint.stream.prototype.</span>_read (n)](#apidoc.element.jslint.stream.prototype._read)
1.  [function <span class="apidocSignatureSpan">jslint.stream.prototype.</span>addListener (ev, fn)](#apidoc.element.jslint.stream.prototype.addListener)
1.  [function <span class="apidocSignatureSpan">jslint.stream.prototype.</span>isPaused ()](#apidoc.element.jslint.stream.prototype.isPaused)
1.  [function <span class="apidocSignatureSpan">jslint.stream.prototype.</span>on (ev, fn)](#apidoc.element.jslint.stream.prototype.on)
1.  [function <span class="apidocSignatureSpan">jslint.stream.prototype.</span>pause ()](#apidoc.element.jslint.stream.prototype.pause)
1.  [function <span class="apidocSignatureSpan">jslint.stream.prototype.</span>pipe (dest, pipeOpts)](#apidoc.element.jslint.stream.prototype.pipe)
1.  [function <span class="apidocSignatureSpan">jslint.stream.prototype.</span>push (chunk, encoding)](#apidoc.element.jslint.stream.prototype.push)
1.  [function <span class="apidocSignatureSpan">jslint.stream.prototype.</span>read (n)](#apidoc.element.jslint.stream.prototype.read)
1.  [function <span class="apidocSignatureSpan">jslint.stream.prototype.</span>resume ()](#apidoc.element.jslint.stream.prototype.resume)
1.  [function <span class="apidocSignatureSpan">jslint.stream.prototype.</span>setEncoding (enc)](#apidoc.element.jslint.stream.prototype.setEncoding)
1.  [function <span class="apidocSignatureSpan">jslint.stream.prototype.</span>unpipe (dest)](#apidoc.element.jslint.stream.prototype.unpipe)
1.  [function <span class="apidocSignatureSpan">jslint.stream.prototype.</span>unshift (chunk)](#apidoc.element.jslint.stream.prototype.unshift)
1.  [function <span class="apidocSignatureSpan">jslint.stream.prototype.</span>wrap (stream)](#apidoc.element.jslint.stream.prototype.wrap)



# <a name="apidoc.module.jslint"></a>[module jslint](#apidoc.module.jslint)

#### <a name="apidoc.element.jslint.LintStream"></a>[function <span class="apidocSignatureSpan">jslint.</span>LintStream (options)](#apidoc.element.jslint.LintStream)
- description and source-code
```javascript
function LintStream_constructor(options) {
    if (!(this instanceof LintStream)) {
        return new LintStream(options);
    }
    Transform.call(this, {objectMode: true});

    // shallow copy options
    options = optModule.merge({}, options);
    this.JSlint = nodelint.load(options.edition);

    // initialize members
    this.options = options;
    this.linter = linter;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jslint.LintStream.super_"></a>[function <span class="apidocSignatureSpan">jslint.</span>LintStream.super_ (options)](#apidoc.element.jslint.LintStream.super_)
- description and source-code
```javascript
function Transform(options) {
  if (!(this instanceof Transform)) return new Transform(options);

  Duplex.call(this, options);

  this._transformState = new TransformState(this);

  // when the writable side finishes, then flush out anything remaining.
  var stream = this;

  // start out asking for a readable event once data is transformed.
  this._readableState.needReadable = true;

  // we have implemented the _read method, and done the other things
  // that Readable wants before the first _read call, so unset the
  // sync guard flag.
  this._readableState.sync = false;

  if (options) {
    if (typeof options.transform === 'function') this._transform = options.transform;

    if (typeof options.flush === 'function') this._flush = options.flush;
  }

  this.once('prefinish', function () {
    if (typeof this._flush === 'function') this._flush(function (er) {
      done(stream, er);
    });else done(stream);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jslint.collectorstream"></a>[function <span class="apidocSignatureSpan">jslint.</span>collectorstream (options)](#apidoc.element.jslint.collectorstream)
- description and source-code
```javascript
function CollectorStream_constructor(options) {
    if (!(this instanceof CollectorStream)) {
        return new CollectorStream(options);
    }

    Transform.call(this, {objectMode: true});

    this.lint = [];

    this.allOK = true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jslint.fileopener"></a>[function <span class="apidocSignatureSpan">jslint.</span>fileopener ()](#apidoc.element.jslint.fileopener)
- description and source-code
```javascript
function FileOpener() {
    Transform.call(this, {objectMode: true});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jslint.jsonreportstream"></a>[function <span class="apidocSignatureSpan">jslint.</span>jsonreportstream (options)](#apidoc.element.jslint.jsonreportstream)
- description and source-code
```javascript
function JSONReportStream_constructor(options) {
    if (!(this instanceof JSONReportStream)) {
        return new JSONReportStream(options);
    }

    Transform.call(this, {objectMode: true});

    this.allOK = true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jslint.load"></a>[function <span class="apidocSignatureSpan">jslint.</span>load (edition)](#apidoc.element.jslint.load)
- description and source-code
```javascript
load = function (edition) {
    'use strict';

    var ctx = vm.createContext(),
        fileName,
        jslintSource;

    function makePathFromName(name) {
        return path.join(__dirname, name) + ".js";
    }

    function makePathFromEdition(edition) {
        return makePathFromName("jslint-" + edition);
    }

    function read(name) {
        return fs.readFileSync(name);
    }


    if (edition) {
        if (looksLikeFileName(edition)) {
            fileName = edition;
        } else {
            fileName = makePathFromEdition(edition);
        }

        try {
            jslintSource = read(fileName);
        } catch (err) {
            con.warn("Unable to load edition " + edition + ", reverting to default. " + err);
        }
    }

    if (!jslintSource) {
        jslintSource = read(makePathFromName("jslint"));
    }

    vm.runInContext(jslintSource, ctx);

    if (!ctx.JSLINT) {
        ctx.JSLINT = function JSLINT(script, options) {
            var data = ctx.jslint(script, options, options.predef);
            ctx.JSLINT.data = function () {
                return data;
            };
        };
        ctx.JSLINT.edition = ctx.jslint('').edition;
    }

    return ctx.JSLINT;

}
```
- example usage
```shell
...
exports.parseArgs = parseArgs;

exports.reportVersion = function reportVersion(callback, options) {
    'use strict';
    process.nextTick(function () {
        var package_data = require('../package.json'),
            version = package_data.version,
            edition = nodelint.load(options.edition).edition;

        callback("node-jslint version: " + version + "  JSLint edition " + edition);
    });

};

function expandGlob(glob) {
...
```

#### <a name="apidoc.element.jslint.looksLikeFileName"></a>[function <span class="apidocSignatureSpan">jslint.</span>looksLikeFileName (edition)](#apidoc.element.jslint.looksLikeFileName)
- description and source-code
```javascript
function looksLikeFileName(edition) {
    'use strict';

    // contains .js or a path separator character '/' or '\'
    return (/\.js|\/|\\/).test(edition);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jslint.reportstream"></a>[function <span class="apidocSignatureSpan">jslint.</span>reportstream (options)](#apidoc.element.jslint.reportstream)
- description and source-code
```javascript
function ReportStream_constructor(options) {
    var stream = this;

    if (!(this instanceof ReportStream)) {
        return new ReportStream(options);
    }

    options = options || {};
    options.objectMode = true;
    Transform.call(this, options);

    this.reporter = reporter.makeReporter(
        {
            log: function (s) {
                stream.emit('data', s);
            },
            err: function (s) {
                stream.emit('data', s);
            }
        },
        options.color,
        options.terse
    );

    this.allOK = true;

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jslint.runMain"></a>[function <span class="apidocSignatureSpan">jslint.</span>runMain (options, cb)](#apidoc.element.jslint.runMain)
- description and source-code
```javascript
runMain = function (options, cb) {
    'use strict';

    if (options.version) {
        exports.reportVersion(con.log, options);
        return;
    }

    if (!options.argv.remain.length) {
        die("No files specified.");
    }

    var procOptions = optModule.getOptions(process.env.HOME, options),
        files = globFiles(options.argv.remain, glob, options.filter),
        opener = new FileOpener(),
        linter = new LintStream(procOptions),
        reporter = makeReporter(procOptions);

    opener.pipe(linter);
    linter.pipe(reporter);

    reporter.on('finish', function () {
        if (cb) {
            return cb(null, reporter.lint);
        }

        if (reporter.allOK) {
            return exit(0);
        }
        exit(1);
    });

    files.forEach(function (file) {
        opener.write(file);
    });
    opener.end();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jslint.setConsole"></a>[function <span class="apidocSignatureSpan">jslint.</span>setConsole (c)](#apidoc.element.jslint.setConsole)
- description and source-code
```javascript
setConsole = function (c) {
    'use strict';
    con = c;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jslint.stream"></a>[function <span class="apidocSignatureSpan">jslint.</span>stream (options)](#apidoc.element.jslint.stream)
- description and source-code
```javascript
function Readable(options) {
  Duplex = Duplex || require('./_stream_duplex');

  if (!(this instanceof Readable)) return new Readable(options);

  this._readableState = new ReadableState(options, this);

  // legacy
  this.readable = true;

  if (options && typeof options.read === 'function') this._read = options.read;

  Stream.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.jslint.LintStream"></a>[module jslint.LintStream](#apidoc.module.jslint.LintStream)

#### <a name="apidoc.element.jslint.LintStream.LintStream"></a>[function <span class="apidocSignatureSpan">jslint.</span>LintStream (options)](#apidoc.element.jslint.LintStream.LintStream)
- description and source-code
```javascript
function LintStream_constructor(options) {
    if (!(this instanceof LintStream)) {
        return new LintStream(options);
    }
    Transform.call(this, {objectMode: true});

    // shallow copy options
    options = optModule.merge({}, options);
    this.JSlint = nodelint.load(options.edition);

    // initialize members
    this.options = options;
    this.linter = linter;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jslint.LintStream.super_"></a>[function <span class="apidocSignatureSpan">jslint.LintStream.</span>super_ (options)](#apidoc.element.jslint.LintStream.super_)
- description and source-code
```javascript
function Transform(options) {
  if (!(this instanceof Transform)) return new Transform(options);

  Duplex.call(this, options);

  this._transformState = new TransformState(this);

  // when the writable side finishes, then flush out anything remaining.
  var stream = this;

  // start out asking for a readable event once data is transformed.
  this._readableState.needReadable = true;

  // we have implemented the _read method, and done the other things
  // that Readable wants before the first _read call, so unset the
  // sync guard flag.
  this._readableState.sync = false;

  if (options) {
    if (typeof options.transform === 'function') this._transform = options.transform;

    if (typeof options.flush === 'function') this._flush = options.flush;
  }

  this.once('prefinish', function () {
    if (typeof this._flush === 'function') this._flush(function (er) {
      done(stream, er);
    });else done(stream);
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.jslint.LintStream.prototype"></a>[module jslint.LintStream.prototype](#apidoc.module.jslint.LintStream.prototype)

#### <a name="apidoc.element.jslint.LintStream.prototype._transform"></a>[function <span class="apidocSignatureSpan">jslint.LintStream.prototype.</span>_transform (chunk, ignore, callback)](#apidoc.element.jslint.LintStream.prototype._transform)
- description and source-code
```javascript
function LintStream_transform(chunk, ignore, callback) {
    var fileName = chunk.file,
        body = chunk.body,
        linted = this.linter.doLint(this.JSlint, body, this.options);

    this.push({file: fileName, linted: linted});

    callback();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.jslint.LintStream.super_"></a>[module jslint.LintStream.super_](#apidoc.module.jslint.LintStream.super_)

#### <a name="apidoc.element.jslint.LintStream.super_.super_"></a>[function <span class="apidocSignatureSpan">jslint.LintStream.</span>super_ (options)](#apidoc.element.jslint.LintStream.super_.super_)
- description and source-code
```javascript
function Duplex(options) {
  if (!(this instanceof Duplex)) return new Duplex(options);

  Readable.call(this, options);
  Writable.call(this, options);

  if (options && options.readable === false) this.readable = false;

  if (options && options.writable === false) this.writable = false;

  this.allowHalfOpen = true;
  if (options && options.allowHalfOpen === false) this.allowHalfOpen = false;

  this.once('end', onend);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.jslint.LintStream.super_.prototype"></a>[module jslint.LintStream.super_.prototype](#apidoc.module.jslint.LintStream.super_.prototype)

#### <a name="apidoc.element.jslint.LintStream.super_.prototype._read"></a>[function <span class="apidocSignatureSpan">jslint.LintStream.super_.prototype.</span>_read (n)](#apidoc.element.jslint.LintStream.super_.prototype._read)
- description and source-code
```javascript
_read = function (n) {
  var ts = this._transformState;

  if (ts.writechunk !== null && ts.writecb && !ts.transforming) {
    ts.transforming = true;
    this._transform(ts.writechunk, ts.writeencoding, ts.afterTransform);
  } else {
    // mark that we need a transform, so that any data that comes in
    // will get processed, now that we've asked for it.
    ts.needTransform = true;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jslint.LintStream.super_.prototype._transform"></a>[function <span class="apidocSignatureSpan">jslint.LintStream.super_.prototype.</span>_transform (chunk, encoding, cb)](#apidoc.element.jslint.LintStream.super_.prototype._transform)
- description and source-code
```javascript
_transform = function (chunk, encoding, cb) {
  throw new Error('Not implemented');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jslint.LintStream.super_.prototype._write"></a>[function <span class="apidocSignatureSpan">jslint.LintStream.super_.prototype.</span>_write (chunk, encoding, cb)](#apidoc.element.jslint.LintStream.super_.prototype._write)
- description and source-code
```javascript
_write = function (chunk, encoding, cb) {
  var ts = this._transformState;
  ts.writecb = cb;
  ts.writechunk = chunk;
  ts.writeencoding = encoding;
  if (!ts.transforming) {
    var rs = this._readableState;
    if (ts.needTransform || rs.needReadable || rs.length < rs.highWaterMark) this._read(rs.highWaterMark);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jslint.LintStream.super_.prototype.push"></a>[function <span class="apidocSignatureSpan">jslint.LintStream.super_.prototype.</span>push (chunk, encoding)](#apidoc.element.jslint.LintStream.super_.prototype.push)
- description and source-code
```javascript
push = function (chunk, encoding) {
  this._transformState.needTransform = false;
  return Duplex.prototype.push.call(this, chunk, encoding);
}
```
- example usage
```shell
...

    this.allOK = true;
};
util.inherits(CollectorStream, Transform);

function CollectorStream_transform(chunk, ignore, callback) {
    // chunk: a package of lint data from JSLint
    this.lint.push([chunk.file, chunk.linted.errors]);

    this.allOK = this.allOK && chunk.linted.ok;

    callback();
}

CollectorStream.prototype._transform = CollectorStream_transform;
...
```



# <a name="apidoc.module.jslint.LintStream.super_.super_.prototype"></a>[module jslint.LintStream.super_.super_.prototype](#apidoc.module.jslint.LintStream.super_.super_.prototype)

#### <a name="apidoc.element.jslint.LintStream.super_.super_.prototype._write"></a>[function <span class="apidocSignatureSpan">jslint.LintStream.super_.super_.prototype.</span>_write (chunk, encoding, cb)](#apidoc.element.jslint.LintStream.super_.super_.prototype._write)
- description and source-code
```javascript
_write = function (chunk, encoding, cb) {
  cb(new Error('not implemented'));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jslint.LintStream.super_.super_.prototype.cork"></a>[function <span class="apidocSignatureSpan">jslint.LintStream.super_.super_.prototype.</span>cork ()](#apidoc.element.jslint.LintStream.super_.super_.prototype.cork)
- description and source-code
```javascript
cork = function () {
  var state = this._writableState;

  state.corked++;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jslint.LintStream.super_.super_.prototype.end"></a>[function <span class="apidocSignatureSpan">jslint.LintStream.super_.super_.prototype.</span>end (chunk, encoding, cb)](#apidoc.element.jslint.LintStream.super_.super_.prototype.end)
- description and source-code
```javascript
end = function (chunk, encoding, cb) {
  var state = this._writableState;

  if (typeof chunk === 'function') {
    cb = chunk;
    chunk = null;
    encoding = null;
  } else if (typeof encoding === 'function') {
    cb = encoding;
    encoding = null;
  }

  if (chunk !== null && chunk !== undefined) this.write(chunk, encoding);

  // .end() fully uncorks
  if (state.corked) {
    state.corked = 1;
    this.uncork();
  }

  // ignore unnecessary end() calls.
  if (!state.ending && !state.finished) endWritable(this, state, cb);
}
```
- example usage
```shell
...
        }
        exit(1);
    });

    files.forEach(function (file) {
        opener.write(file);
    });
    opener.end();
};
...
```

#### <a name="apidoc.element.jslint.LintStream.super_.super_.prototype.setDefaultEncoding"></a>[function <span class="apidocSignatureSpan">jslint.LintStream.super_.super_.prototype.</span>setDefaultEncoding (encoding)](#apidoc.element.jslint.LintStream.super_.super_.prototype.setDefaultEncoding)
- description and source-code
```javascript
function setDefaultEncoding(encoding) {
  // node::ParseEncoding() requires lower case.
  if (typeof encoding === 'string') encoding = encoding.toLowerCase();
  if (!(['hex', 'utf8', 'utf-8', 'ascii', 'binary', 'base64', 'ucs2', 'ucs-2', 'utf16le', 'utf-16le', 'raw'].indexOf((encoding + '').
toLowerCase()) > -1)) throw new TypeError('Unknown encoding: ' + encoding);
  this._writableState.defaultEncoding = encoding;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jslint.LintStream.super_.super_.prototype.uncork"></a>[function <span class="apidocSignatureSpan">jslint.LintStream.super_.super_.prototype.</span>uncork ()](#apidoc.element.jslint.LintStream.super_.super_.prototype.uncork)
- description and source-code
```javascript
uncork = function () {
  var state = this._writableState;

  if (state.corked) {
    state.corked--;

    if (!state.writing && !state.corked && !state.finished && !state.bufferProcessing && state.bufferedRequest) clearBuffer(this
, state);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jslint.LintStream.super_.super_.prototype.write"></a>[function <span class="apidocSignatureSpan">jslint.LintStream.super_.super_.prototype.</span>write (chunk, encoding, cb)](#apidoc.element.jslint.LintStream.super_.super_.prototype.write)
- description and source-code
```javascript
write = function (chunk, encoding, cb) {
  var state = this._writableState;
  var ret = false;

  if (typeof encoding === 'function') {
    cb = encoding;
    encoding = null;
  }

  if (Buffer.isBuffer(chunk)) encoding = 'buffer';else if (!encoding) encoding = state.defaultEncoding;

  if (typeof cb !== 'function') cb = nop;

  if (state.ended) writeAfterEnd(this, cb);else if (validChunk(this, state, chunk, cb)) {
    state.pendingcb++;
    ret = writeOrBuffer(this, state, chunk, encoding, cb);
  }

  return ret;
}
```
- example usage
```shell
...
        reporter = new CollectorStream(parsed);
    } else {
        reporter = new ReportStream(parsed);
    }

    reporter.on('data', function (chunk) {
        if (chunk === '.') {
            pro.stderr.write(chunk);
        } else {
            con.log(chunk);
        }
    });

    return reporter;
}
...
```



# <a name="apidoc.module.jslint.collectorstream"></a>[module jslint.collectorstream](#apidoc.module.jslint.collectorstream)

#### <a name="apidoc.element.jslint.collectorstream.collectorstream"></a>[function <span class="apidocSignatureSpan">jslint.</span>collectorstream (options)](#apidoc.element.jslint.collectorstream.collectorstream)
- description and source-code
```javascript
function CollectorStream_constructor(options) {
    if (!(this instanceof CollectorStream)) {
        return new CollectorStream(options);
    }

    Transform.call(this, {objectMode: true});

    this.lint = [];

    this.allOK = true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jslint.collectorstream.super_"></a>[function <span class="apidocSignatureSpan">jslint.collectorstream.</span>super_ (options)](#apidoc.element.jslint.collectorstream.super_)
- description and source-code
```javascript
function Transform(options) {
  if (!(this instanceof Transform)) return new Transform(options);

  Duplex.call(this, options);

  this._transformState = new TransformState(this);

  // when the writable side finishes, then flush out anything remaining.
  var stream = this;

  // start out asking for a readable event once data is transformed.
  this._readableState.needReadable = true;

  // we have implemented the _read method, and done the other things
  // that Readable wants before the first _read call, so unset the
  // sync guard flag.
  this._readableState.sync = false;

  if (options) {
    if (typeof options.transform === 'function') this._transform = options.transform;

    if (typeof options.flush === 'function') this._flush = options.flush;
  }

  this.once('prefinish', function () {
    if (typeof this._flush === 'function') this._flush(function (er) {
      done(stream, er);
    });else done(stream);
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.jslint.collectorstream.prototype"></a>[module jslint.collectorstream.prototype](#apidoc.module.jslint.collectorstream.prototype)

#### <a name="apidoc.element.jslint.collectorstream.prototype._transform"></a>[function <span class="apidocSignatureSpan">jslint.collectorstream.prototype.</span>_transform (chunk, ignore, callback)](#apidoc.element.jslint.collectorstream.prototype._transform)
- description and source-code
```javascript
function CollectorStream_transform(chunk, ignore, callback) {
    // chunk: a package of lint data from JSLint
    this.lint.push([chunk.file, chunk.linted.errors]);

    this.allOK = this.allOK && chunk.linted.ok;

    callback();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.jslint.color"></a>[module jslint.color](#apidoc.module.jslint.color)

#### <a name="apidoc.element.jslint.color.blue"></a>[function <span class="apidocSignatureSpan">jslint.color.</span>blue (string)](#apidoc.element.jslint.color.blue)
- description and source-code
```javascript
blue = function (string) {
    return color(code, string);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jslint.color.bold"></a>[function <span class="apidocSignatureSpan">jslint.color.</span>bold (string)](#apidoc.element.jslint.color.bold)
- description and source-code
```javascript
bold = function (string) {
    return color(code, string);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jslint.color.green"></a>[function <span class="apidocSignatureSpan">jslint.color.</span>green (string)](#apidoc.element.jslint.color.green)
- description and source-code
```javascript
green = function (string) {
    return color(code, string);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jslint.color.grey"></a>[function <span class="apidocSignatureSpan">jslint.color.</span>grey (string)](#apidoc.element.jslint.color.grey)
- description and source-code
```javascript
grey = function (string) {
    return color(code, string);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jslint.color.red"></a>[function <span class="apidocSignatureSpan">jslint.color.</span>red (string)](#apidoc.element.jslint.color.red)
- description and source-code
```javascript
red = function (string) {
    return color(code, string);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jslint.color.yellow"></a>[function <span class="apidocSignatureSpan">jslint.color.</span>yellow (string)](#apidoc.element.jslint.color.yellow)
- description and source-code
```javascript
yellow = function (string) {
    return color(code, string);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.jslint.fileopener"></a>[module jslint.fileopener](#apidoc.module.jslint.fileopener)

#### <a name="apidoc.element.jslint.fileopener.fileopener"></a>[function <span class="apidocSignatureSpan">jslint.</span>fileopener ()](#apidoc.element.jslint.fileopener.fileopener)
- description and source-code
```javascript
function FileOpener() {
    Transform.call(this, {objectMode: true});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jslint.fileopener.super_"></a>[function <span class="apidocSignatureSpan">jslint.fileopener.</span>super_ (options)](#apidoc.element.jslint.fileopener.super_)
- description and source-code
```javascript
function Transform(options) {
  if (!(this instanceof Transform)) return new Transform(options);

  Duplex.call(this, options);

  this._transformState = new TransformState(this);

  // when the writable side finishes, then flush out anything remaining.
  var stream = this;

  // start out asking for a readable event once data is transformed.
  this._readableState.needReadable = true;

  // we have implemented the _read method, and done the other things
  // that Readable wants before the first _read call, so unset the
  // sync guard flag.
  this._readableState.sync = false;

  if (options) {
    if (typeof options.transform === 'function') this._transform = options.transform;

    if (typeof options.flush === 'function') this._flush = options.flush;
  }

  this.once('prefinish', function () {
    if (typeof this._flush === 'function') this._flush(function (er) {
      done(stream, er);
    });else done(stream);
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.jslint.fileopener.prototype"></a>[module jslint.fileopener.prototype](#apidoc.module.jslint.fileopener.prototype)

#### <a name="apidoc.element.jslint.fileopener.prototype._transform"></a>[function <span class="apidocSignatureSpan">jslint.fileopener.prototype.</span>_transform (file, ignore, callback)](#apidoc.element.jslint.fileopener.prototype._transform)
- description and source-code
```javascript
function FileOpener_transform(file, ignore, callback) {
    var stream = this;
    fs.readFile(file, 'utf8', function (err, data) {
        if (err) {
            stream.emit('error', err);
            return;
        }

        stream.push({file: file, body: data});
        callback();
    });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.jslint.jsonreportstream"></a>[module jslint.jsonreportstream](#apidoc.module.jslint.jsonreportstream)

#### <a name="apidoc.element.jslint.jsonreportstream.jsonreportstream"></a>[function <span class="apidocSignatureSpan">jslint.</span>jsonreportstream (options)](#apidoc.element.jslint.jsonreportstream.jsonreportstream)
- description and source-code
```javascript
function JSONReportStream_constructor(options) {
    if (!(this instanceof JSONReportStream)) {
        return new JSONReportStream(options);
    }

    Transform.call(this, {objectMode: true});

    this.allOK = true;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jslint.jsonreportstream.super_"></a>[function <span class="apidocSignatureSpan">jslint.jsonreportstream.</span>super_ (options)](#apidoc.element.jslint.jsonreportstream.super_)
- description and source-code
```javascript
function Transform(options) {
  if (!(this instanceof Transform)) return new Transform(options);

  Duplex.call(this, options);

  this._transformState = new TransformState(this);

  // when the writable side finishes, then flush out anything remaining.
  var stream = this;

  // start out asking for a readable event once data is transformed.
  this._readableState.needReadable = true;

  // we have implemented the _read method, and done the other things
  // that Readable wants before the first _read call, so unset the
  // sync guard flag.
  this._readableState.sync = false;

  if (options) {
    if (typeof options.transform === 'function') this._transform = options.transform;

    if (typeof options.flush === 'function') this._flush = options.flush;
  }

  this.once('prefinish', function () {
    if (typeof this._flush === 'function') this._flush(function (er) {
      done(stream, er);
    });else done(stream);
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.jslint.jsonreportstream.prototype"></a>[module jslint.jsonreportstream.prototype](#apidoc.module.jslint.jsonreportstream.prototype)

#### <a name="apidoc.element.jslint.jsonreportstream.prototype._transform"></a>[function <span class="apidocSignatureSpan">jslint.jsonreportstream.prototype.</span>_transform (chunk, ignore, callback)](#apidoc.element.jslint.jsonreportstream.prototype._transform)
- description and source-code
```javascript
function JSONReportStream_transform(chunk, ignore, callback) {
    // chunk: a package of lint data from JSLint
    this.emit('data', JSON.stringify([chunk.file, chunk.linted.errors]));

    this.allOK = this.allOK && chunk.linted.ok;

    callback();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.jslint.linter"></a>[module jslint.linter](#apidoc.module.jslint.linter)

#### <a name="apidoc.element.jslint.linter.doLint"></a>[function <span class="apidocSignatureSpan">jslint.linter.</span>doLint (jslint, script, options)](#apidoc.element.jslint.linter.doLint)
- description and source-code
```javascript
doLint = function (jslint, script, options) {
    'use strict';
    var ok,
        result;

    script = preprocessScript(script);

    ok = jslint(script, options);

    result = jslint.data();
    if (result.ok === undefined) {
        result.ok = ok;
    }
    result.options = options;

    // es6
    result.errors = result.errors || result.warnings;

    return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jslint.linter.merge"></a>[function <span class="apidocSignatureSpan">jslint.linter.</span>merge (source, add)](#apidoc.element.jslint.linter.merge)
- description and source-code
```javascript
function merge(source, add) {
    'use strict';

    var result = source || {};

    if (!add) {
        return result;
    }

    Object.keys(add).forEach(function (prop) {
        if (!result.hasOwnProperty(prop)) {
            result[prop] = add[prop];
        }
    });

    return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jslint.linter.preprocessScript"></a>[function <span class="apidocSignatureSpan">jslint.linter.</span>preprocessScript (script)](#apidoc.element.jslint.linter.preprocessScript)
- description and source-code
```javascript
function preprocessScript(script) {
    'use strict';

    // Fix UTF8 with BOM
    if (script.charCodeAt(0) === 0xFEFF) {
        script = script.slice(1);
    }

    // remove shebang: replace it with empty line
    script = script.replace(/^#!.*/, "");

    return script;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.jslint.main"></a>[module jslint.main](#apidoc.module.jslint.main)

#### <a name="apidoc.element.jslint.main.commandOptions"></a>[function <span class="apidocSignatureSpan">jslint.main.</span>commandOptions ()](#apidoc.element.jslint.main.commandOptions)
- description and source-code
```javascript
function commandOptions() {
    'use strict';

    var commandOpts = {
            'indent': Number,
            'maxerr': Number,
            'maxlen': Number,
            'predef': [String, Array],
            'edition': String,
            'config': String
        },
<span class="apidocCodeCommentSpan">        /* flags defined in jslint-latest.js */
</span>        jslintFlags = [
            'ass', 'bitwise', 'browser', 'closure', 'continue',
            'debug', 'devel', 'eqeq', 'evil', 'forin', 'newcap',
            'node', 'nomen', 'passfail', 'plusplus', 'properties',
            'regexp', 'rhino', 'unparam', 'sloppy', 'stupid', 'sub',
            'todo', 'vars', 'white'
        ],
        /* flags used by node-jslint to control output */
        cliFlags = [
            'json', 'color', 'terse', 'version', 'filter'
        ],
        /* not used by jslint-latest.js */
        deprecatedFlags = [
            'anon', 'es5', 'on', 'undef', 'windows'
        ],
        allFlags = jslintFlags.concat(cliFlags).concat(deprecatedFlags);

    allFlags.forEach(function (option) {
        commandOpts[option] = Boolean;
    });

    return commandOpts;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jslint.main.expandGlob"></a>[function <span class="apidocSignatureSpan">jslint.main.</span>expandGlob (glob)](#apidoc.element.jslint.main.expandGlob)
- description and source-code
```javascript
function expandGlob(glob) {
    'use strict';

    return function (pattern) {
        return glob.sync(pattern);
    };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jslint.main.globFiles"></a>[function <span class="apidocSignatureSpan">jslint.main.</span>globFiles (list, glob, filter)](#apidoc.element.jslint.main.globFiles)
- description and source-code
```javascript
function globFiles(list, glob, filter) {
    'use strict';
    var remain = [];

    remain = list.map(expandGlob(glob))
        .reduce(flatten, []);

    if (filter) {
        remain = remain.filter(noNodeModules);
    }

    return remain;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jslint.main.makeReporter"></a>[function <span class="apidocSignatureSpan">jslint.main.</span>makeReporter (parsed)](#apidoc.element.jslint.main.makeReporter)
- description and source-code
```javascript
function makeReporter(parsed) {
    'use strict';
    var reporter;

    if (parsed.json) {
        reporter = new JSONReportStream(parsed);
    } else if (parsed.collector) {
        reporter = new CollectorStream(parsed);
    } else {
        reporter = new ReportStream(parsed);
    }

    reporter.on('data', function (chunk) {
        if (chunk === '.') {
            pro.stderr.write(chunk);
        } else {
            con.log(chunk);
        }
    });

    return reporter;
}
```
- example usage
```shell
...
    return new ReportStream(options);
}

options = options || {};
options.objectMode = true;
Transform.call(this, options);

this.reporter = reporter.makeReporter(
    {
        log: function (s) {
            stream.emit('data', s);
        },
        err: function (s) {
            stream.emit('data', s);
        }
...
```

#### <a name="apidoc.element.jslint.main.noNodeModules"></a>[function <span class="apidocSignatureSpan">jslint.main.</span>noNodeModules (file)](#apidoc.element.jslint.main.noNodeModules)
- description and source-code
```javascript
function noNodeModules(file) {
    'use strict';
    return file.indexOf('node_modules') === -1;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jslint.main.parseArgs"></a>[function <span class="apidocSignatureSpan">jslint.main.</span>parseArgs (argv)](#apidoc.element.jslint.main.parseArgs)
- description and source-code
```javascript
function parseArgs(argv) {
    'use strict';
    var args = nopt(commandOptions(), {}, argv);

    if (args.filter === undefined) {
        args.filter = true;
    }

    return args;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jslint.main.reportVersion"></a>[function <span class="apidocSignatureSpan">jslint.main.</span>reportVersion (callback, options)](#apidoc.element.jslint.main.reportVersion)
- description and source-code
```javascript
function reportVersion(callback, options) {
    'use strict';
    process.nextTick(function () {
        var package_data = require('../package.json'),
            version = package_data.version,
            edition = nodelint.load(options.edition).edition;

        callback("node-jslint version: " + version + "  JSLint edition " + edition);
    });

}
```
- example usage
```shell
...
}
exports.makeReporter = makeReporter;

exports.runMain = function (options, cb) {
'use strict';

if (options.version) {
    exports.reportVersion(con.log, options);
    return;
}

if (!options.argv.remain.length) {
    die("No files specified.");
}
...
```

#### <a name="apidoc.element.jslint.main.runMain"></a>[function <span class="apidocSignatureSpan">jslint.main.</span>runMain (options, cb)](#apidoc.element.jslint.main.runMain)
- description and source-code
```javascript
runMain = function (options, cb) {
    'use strict';

    if (options.version) {
        exports.reportVersion(con.log, options);
        return;
    }

    if (!options.argv.remain.length) {
        die("No files specified.");
    }

    var procOptions = optModule.getOptions(process.env.HOME, options),
        files = globFiles(options.argv.remain, glob, options.filter),
        opener = new FileOpener(),
        linter = new LintStream(procOptions),
        reporter = makeReporter(procOptions);

    opener.pipe(linter);
    linter.pipe(reporter);

    reporter.on('finish', function () {
        if (cb) {
            return cb(null, reporter.lint);
        }

        if (reporter.allOK) {
            return exit(0);
        }
        exit(1);
    });

    files.forEach(function (file) {
        opener.write(file);
    });
    opener.end();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jslint.main.setConsole"></a>[function <span class="apidocSignatureSpan">jslint.main.</span>setConsole (c)](#apidoc.element.jslint.main.setConsole)
- description and source-code
```javascript
setConsole = function (c) {
    'use strict';
    con = c;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jslint.main.setProcess"></a>[function <span class="apidocSignatureSpan">jslint.main.</span>setProcess (p)](#apidoc.element.jslint.main.setProcess)
- description and source-code
```javascript
setProcess = function (p) {
    'use strict';
    pro = p;
    exit = pro.exit.bind(pro);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.jslint.options"></a>[module jslint.options](#apidoc.module.jslint.options)

#### <a name="apidoc.element.jslint.options.addDefaults"></a>[function <span class="apidocSignatureSpan">jslint.options.</span>addDefaults (options)](#apidoc.element.jslint.options.addDefaults)
- description and source-code
```javascript
function addDefaults(options) {

    options = merge(options, {node: true, es5: true});

    return options;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jslint.options.getOptions"></a>[function <span class="apidocSignatureSpan">jslint.options.</span>getOptions (homedir, options)](#apidoc.element.jslint.options.getOptions)
- description and source-code
```javascript
function options_getOptions(homedir, options) {
    var config = loadConfig(homedir, options.config);

    return preprocessOptions(options, config);
}
```
- example usage
```shell
...
    return;
}

if (!options.argv.remain.length) {
    die("No files specified.");
}

var procOptions = optModule.getOptions(process.env.HOME, options),
    files = globFiles(options.argv.remain, glob, options.filter),
    opener = new FileOpener(),
    linter = new LintStream(procOptions),
    reporter = makeReporter(procOptions);

opener.pipe(linter);
linter.pipe(reporter);
...
```

#### <a name="apidoc.element.jslint.options.loadAndParseConfig"></a>[function <span class="apidocSignatureSpan">jslint.options.</span>loadAndParseConfig (filePath)](#apidoc.element.jslint.options.loadAndParseConfig)
- description and source-code
```javascript
function loadAndParseConfig(filePath) {
    try {
        return JSON.parse(fs.readFileSync(filePath, "utf-8"));
    } catch (err) {
        if (filePath && err.code !== "ENOENT") {
            con.warn('Error reading config file "' + filePath + '": ' + err);
        }
    }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jslint.options.loadConfig"></a>[function <span class="apidocSignatureSpan">jslint.options.</span>loadConfig (h, configFile)](#apidoc.element.jslint.options.loadConfig)
- description and source-code
```javascript
function loadConfig(h, configFile) {
    var home = h || '',
        homeConfigs = ['.jslint.conf', '.jslintrc'],
        projectConfigs = ['jslint.conf', '.jslint.conf', 'jslintrc', '.jslintrc'];

    if (configFile) {
        // explicitly specified config file overrides default config file name, path
        homeConfigs = [configFile];
    } else {
        homeConfigs = homeConfigs.map(function (file) {
            return path.join(home, file);
        });
    }

    projectConfigs = projectConfigs.map(function (file) {
        return path.join(process.cwd(), file);
    });

    return mergeConfigs(homeConfigs, projectConfigs);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jslint.options.merge"></a>[function <span class="apidocSignatureSpan">jslint.options.</span>merge (source, add)](#apidoc.element.jslint.options.merge)
- description and source-code
```javascript
function merge(source, add) {
    var result = source || {};

    if (!add) {
        return result;
    }

    Object.keys(add).forEach(function (prop) {
        if (!result.hasOwnProperty(prop)) {
            result[prop] = add[prop];
        }
    });

    return result;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jslint.options.mergeConfigs"></a>[function <span class="apidocSignatureSpan">jslint.options.</span>mergeConfigs (home, project)](#apidoc.element.jslint.options.mergeConfigs)
- description and source-code
```javascript
function mergeConfigs(home, project) {
    var homeConfig,
        cwdConfig,
        config;

    home.some(function (file) {
        homeConfig = loadAndParseConfig(file);
        return homeConfig;
    });

    project.some(function (file) {
        cwdConfig = loadAndParseConfig(file);
        return cwdConfig;
    });

    config = merge(cwdConfig, homeConfig);

    return config;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jslint.options.preprocessOptions"></a>[function <span class="apidocSignatureSpan">jslint.options.</span>preprocessOptions (options, config)](#apidoc.element.jslint.options.preprocessOptions)
- description and source-code
```javascript
function preprocessOptions(options, config) {
    options = merge({}, options);

    options = merge(options, config);

    options = addDefaults(options);

    options = splitPredefs(options);

    return options;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jslint.options.setConsole"></a>[function <span class="apidocSignatureSpan">jslint.options.</span>setConsole (c)](#apidoc.element.jslint.options.setConsole)
- description and source-code
```javascript
setConsole = function (c) {
    con = c;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jslint.options.splitPredefs"></a>[function <span class="apidocSignatureSpan">jslint.options.</span>splitPredefs (options)](#apidoc.element.jslint.options.splitPredefs)
- description and source-code
```javascript
function splitPredefs(options) {
    if (!options.predef) {
        return options;
    }
    if (Array.isArray(options.predef)) {
        return options;
    }

    options.predef = options.predef.split(',').filter(notFalsy);

    return options;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.jslint.reporter"></a>[module jslint.reporter](#apidoc.module.jslint.reporter)

#### <a name="apidoc.element.jslint.reporter.makeReporter"></a>[function <span class="apidocSignatureSpan">jslint.reporter.</span>makeReporter (logger, colorize, terse)](#apidoc.element.jslint.reporter.makeReporter)
- description and source-code
```javascript
makeReporter = function (logger, colorize, terse) {
    return {
        logger: logger,
        colorize: colorize,
        terse: terse,
        report: function (file, lint) {
            return exports.report.call(this, file, lint, this.colorize, this.terse);
        }
    };
}
```
- example usage
```shell
...
    return new ReportStream(options);
}

options = options || {};
options.objectMode = true;
Transform.call(this, options);

this.reporter = reporter.makeReporter(
    {
        log: function (s) {
            stream.emit('data', s);
        },
        err: function (s) {
            stream.emit('data', s);
        }
...
```

#### <a name="apidoc.element.jslint.reporter.report"></a>[function <span class="apidocSignatureSpan">jslint.reporter.</span>report (file, lint, colorize, terse)](#apidoc.element.jslint.reporter.report)
- description and source-code
```javascript
report = function (file, lint, colorize, terse) {
    var line,
        pad,
        errors,
        fudge = Number(lint.option && lint.option.fudge) || 0,
        logger = this.logger,
        fileMessage;

    function c(format, str) {
        if (colorize) {
            return color[format](str);
        }
        return str;
    }

    fileMessage = "\n" + c('bold', file);

    function row(e) {
        return e.line + fudge;
    }
    function col(e) {
        return (e.character || e.column) + fudge;
    }
    function evidence(e) {
        return e.evidence || (lint.lines && lint.lines[e.line]) || '';
    }
    function message(e) {
        return e.reason || e.message;
    }

    if (!lint.ok) {
        // remove nulls
        errors = lint.errors;// || lint.warnings;
        errors = errors.filter(function (e) {
            return e;
        });

        if (terse) {
            errors.forEach(function (e) {
                logger.log(file + ':' + row(e) + ':' + col(e) + ': ' + message(e));
            });
        } else {
            logger.log(fileMessage);
            errors.forEach(function (e, i) {
                pad = "#" + String(i + 1);
                while (pad.length < 3) {
                    pad = ' ' + pad;
                }
                line = ' // Line ' + row(e) + ', Pos ' + col(e);

                logger.log(pad + ' ' + c('yellow', message(e)));
                logger.log('    ' + evidence(e).trim() + c('grey', line));
            });
        }
    } else {
        if (terse) {
            logger.err(".");
        } else {
            logger.log(fileMessage + " is " + c('green', 'OK') + ".");
        }
    }

    return lint.ok;
}
```
- example usage
```shell
...

// You can request a Function Report, which shows all of the functions
// and the parameters and vars that they use. This can be used to find
// implied global variables and other problems. The report is in HTML and
// can be inserted in an HTML <body>. It should be given the result of the
// JSLINT.data function.

//     var myReport = JSLINT.report(data);

// You can request an HTML error report.

//     var myErrorReport = JSLINT.error_report(data);

// You can request a properties report, which produces a list of the program's
// properties in the form of a /*properties*/ declaration.
...
```

#### <a name="apidoc.element.jslint.reporter.setLogger"></a>[function <span class="apidocSignatureSpan">jslint.reporter.</span>setLogger (l)](#apidoc.element.jslint.reporter.setLogger)
- description and source-code
```javascript
setLogger = function (l) {
    this.logger = l;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.jslint.reportstream"></a>[module jslint.reportstream](#apidoc.module.jslint.reportstream)

#### <a name="apidoc.element.jslint.reportstream.reportstream"></a>[function <span class="apidocSignatureSpan">jslint.</span>reportstream (options)](#apidoc.element.jslint.reportstream.reportstream)
- description and source-code
```javascript
function ReportStream_constructor(options) {
    var stream = this;

    if (!(this instanceof ReportStream)) {
        return new ReportStream(options);
    }

    options = options || {};
    options.objectMode = true;
    Transform.call(this, options);

    this.reporter = reporter.makeReporter(
        {
            log: function (s) {
                stream.emit('data', s);
            },
            err: function (s) {
                stream.emit('data', s);
            }
        },
        options.color,
        options.terse
    );

    this.allOK = true;

}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jslint.reportstream.super_"></a>[function <span class="apidocSignatureSpan">jslint.reportstream.</span>super_ (options)](#apidoc.element.jslint.reportstream.super_)
- description and source-code
```javascript
function Transform(options) {
  if (!(this instanceof Transform)) return new Transform(options);

  Duplex.call(this, options);

  this._transformState = new TransformState(this);

  // when the writable side finishes, then flush out anything remaining.
  var stream = this;

  // start out asking for a readable event once data is transformed.
  this._readableState.needReadable = true;

  // we have implemented the _read method, and done the other things
  // that Readable wants before the first _read call, so unset the
  // sync guard flag.
  this._readableState.sync = false;

  if (options) {
    if (typeof options.transform === 'function') this._transform = options.transform;

    if (typeof options.flush === 'function') this._flush = options.flush;
  }

  this.once('prefinish', function () {
    if (typeof this._flush === 'function') this._flush(function (er) {
      done(stream, er);
    });else done(stream);
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.jslint.reportstream.prototype"></a>[module jslint.reportstream.prototype](#apidoc.module.jslint.reportstream.prototype)

#### <a name="apidoc.element.jslint.reportstream.prototype._transform"></a>[function <span class="apidocSignatureSpan">jslint.reportstream.prototype.</span>_transform (chunk, ignore, callback)](#apidoc.element.jslint.reportstream.prototype._transform)
- description and source-code
```javascript
function ReportStream_transform(chunk, ignore, callback) {
    // chunk: a package of lint data from JSLint

    this.reporter.report(chunk.file, chunk.linted);

    this.allOK = this.allOK && chunk.linted.ok;

    callback();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.jslint.stream"></a>[module jslint.stream](#apidoc.module.jslint.stream)

#### <a name="apidoc.element.jslint.stream.stream"></a>[function <span class="apidocSignatureSpan">jslint.</span>stream (options)](#apidoc.element.jslint.stream.stream)
- description and source-code
```javascript
function Readable(options) {
  Duplex = Duplex || require('./_stream_duplex');

  if (!(this instanceof Readable)) return new Readable(options);

  this._readableState = new ReadableState(options, this);

  // legacy
  this.readable = true;

  if (options && typeof options.read === 'function') this._read = options.read;

  Stream.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jslint.stream.Duplex"></a>[function <span class="apidocSignatureSpan">jslint.stream.</span>Duplex (options)](#apidoc.element.jslint.stream.Duplex)
- description and source-code
```javascript
function Duplex(options) {
  if (!(this instanceof Duplex)) return new Duplex(options);

  Readable.call(this, options);
  Writable.call(this, options);

  if (options && options.readable === false) this.readable = false;

  if (options && options.writable === false) this.writable = false;

  this.allowHalfOpen = true;
  if (options && options.allowHalfOpen === false) this.allowHalfOpen = false;

  this.once('end', onend);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jslint.stream.PassThrough"></a>[function <span class="apidocSignatureSpan">jslint.stream.</span>PassThrough (options)](#apidoc.element.jslint.stream.PassThrough)
- description and source-code
```javascript
function PassThrough(options) {
  if (!(this instanceof PassThrough)) return new PassThrough(options);

  Transform.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jslint.stream.Readable"></a>[function <span class="apidocSignatureSpan">jslint.stream.</span>Readable (options)](#apidoc.element.jslint.stream.Readable)
- description and source-code
```javascript
function Readable(options) {
  Duplex = Duplex || require('./_stream_duplex');

  if (!(this instanceof Readable)) return new Readable(options);

  this._readableState = new ReadableState(options, this);

  // legacy
  this.readable = true;

  if (options && typeof options.read === 'function') this._read = options.read;

  Stream.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jslint.stream.ReadableState"></a>[function <span class="apidocSignatureSpan">jslint.stream.</span>ReadableState (options, stream)](#apidoc.element.jslint.stream.ReadableState)
- description and source-code
```javascript
function ReadableState(options, stream) {
  Duplex = Duplex || require('./_stream_duplex');

  options = options || {};

  // object stream flag. Used to make read(n) ignore n and to
  // make all the buffer merging and length checks go away
  this.objectMode = !!options.objectMode;

  if (stream instanceof Duplex) this.objectMode = this.objectMode || !!options.readableObjectMode;

  // the point at which it stops calling _read() to fill the buffer
  // Note: 0 is a valid value, means "don't call _read preemptively ever"
  var hwm = options.highWaterMark;
  var defaultHwm = this.objectMode ? 16 : 16 * 1024;
  this.highWaterMark = hwm || hwm === 0 ? hwm : defaultHwm;

  // cast to ints.
  this.highWaterMark = ~ ~this.highWaterMark;

  // A linked list is used to store data chunks instead of an array because the
  // linked list can remove elements from the beginning faster than
  // array.shift()
  this.buffer = new BufferList();
  this.length = 0;
  this.pipes = null;
  this.pipesCount = 0;
  this.flowing = null;
  this.ended = false;
  this.endEmitted = false;
  this.reading = false;

  // a flag to be able to tell if the onwrite cb is called immediately,
  // or on a later tick.  We set this to true at first, because any
  // actions that shouldn't happen until "later" should generally also
  // not happen before the first write call.
  this.sync = true;

  // whenever we return null, then we set a flag to say
  // that we're awaiting a 'readable' event emission.
  this.needReadable = false;
  this.emittedReadable = false;
  this.readableListening = false;
  this.resumeScheduled = false;

  // Crypto is kind of old and crusty.  Historically, its default string
  // encoding is 'binary' so we have to make this configurable.
  // Everything else in the universe uses 'utf8', though.
  this.defaultEncoding = options.defaultEncoding || 'utf8';

  // when piping, we only care about 'readable' events that happen
  // after read()ing all the bytes and not getting any pushback.
  this.ranOut = false;

  // the number of writers that are awaiting a drain event in .pipe()s
  this.awaitDrain = 0;

  // if true, a maybeReadMore has been scheduled
  this.readingMore = false;

  this.decoder = null;
  this.encoding = null;
  if (options.encoding) {
    if (!StringDecoder) StringDecoder = require('string_decoder/').StringDecoder;
    this.decoder = new StringDecoder(options.encoding);
    this.encoding = options.encoding;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jslint.stream.Stream"></a>[function <span class="apidocSignatureSpan">jslint.stream.</span>Stream ()](#apidoc.element.jslint.stream.Stream)
- description and source-code
```javascript
function Stream() {
  EE.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jslint.stream.Transform"></a>[function <span class="apidocSignatureSpan">jslint.stream.</span>Transform (options)](#apidoc.element.jslint.stream.Transform)
- description and source-code
```javascript
function Transform(options) {
  if (!(this instanceof Transform)) return new Transform(options);

  Duplex.call(this, options);

  this._transformState = new TransformState(this);

  // when the writable side finishes, then flush out anything remaining.
  var stream = this;

  // start out asking for a readable event once data is transformed.
  this._readableState.needReadable = true;

  // we have implemented the _read method, and done the other things
  // that Readable wants before the first _read call, so unset the
  // sync guard flag.
  this._readableState.sync = false;

  if (options) {
    if (typeof options.transform === 'function') this._transform = options.transform;

    if (typeof options.flush === 'function') this._flush = options.flush;
  }

  this.once('prefinish', function () {
    if (typeof this._flush === 'function') this._flush(function (er) {
      done(stream, er);
    });else done(stream);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jslint.stream.Writable"></a>[function <span class="apidocSignatureSpan">jslint.stream.</span>Writable (options)](#apidoc.element.jslint.stream.Writable)
- description and source-code
```javascript
function Writable(options) {
  Duplex = Duplex || require('./_stream_duplex');

  // Writable ctor is applied to Duplexes, though they're not
  // instanceof Writable, they're instanceof Readable.
  if (!(this instanceof Writable) && !(this instanceof Duplex)) return new Writable(options);

  this._writableState = new WritableState(options, this);

  // legacy.
  this.writable = true;

  if (options) {
    if (typeof options.write === 'function') this._write = options.write;

    if (typeof options.writev === 'function') this._writev = options.writev;
  }

  Stream.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jslint.stream._fromList"></a>[function <span class="apidocSignatureSpan">jslint.stream.</span>_fromList (n, state)](#apidoc.element.jslint.stream._fromList)
- description and source-code
```javascript
function fromList(n, state) {
  // nothing buffered
  if (state.length === 0) return null;

  var ret;
  if (state.objectMode) ret = state.buffer.shift();else if (!n || n >= state.length) {
    // read it all, truncate the list
    if (state.decoder) ret = state.buffer.join('');else if (state.buffer.length === 1) ret = state.buffer.head.data;else ret = state
.buffer.concat(state.length);
    state.buffer.clear();
  } else {
    // read part of list
    ret = fromListPartial(n, state.buffer, state.decoder);
  }

  return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jslint.stream.super_"></a>[function <span class="apidocSignatureSpan">jslint.stream.</span>super_ ()](#apidoc.element.jslint.stream.super_)
- description and source-code
```javascript
function Stream() {
  EE.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.jslint.stream.prototype"></a>[module jslint.stream.prototype](#apidoc.module.jslint.stream.prototype)

#### <a name="apidoc.element.jslint.stream.prototype._read"></a>[function <span class="apidocSignatureSpan">jslint.stream.prototype.</span>_read (n)](#apidoc.element.jslint.stream.prototype._read)
- description and source-code
```javascript
_read = function (n) {
  this.emit('error', new Error('not implemented'));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jslint.stream.prototype.addListener"></a>[function <span class="apidocSignatureSpan">jslint.stream.prototype.</span>addListener (ev, fn)](#apidoc.element.jslint.stream.prototype.addListener)
- description and source-code
```javascript
addListener = function (ev, fn) {
  var res = Stream.prototype.on.call(this, ev, fn);

  if (ev === 'data') {
    // Start flowing on next tick if stream isn't explicitly paused
    if (this._readableState.flowing !== false) this.resume();
  } else if (ev === 'readable') {
    var state = this._readableState;
    if (!state.endEmitted && !state.readableListening) {
      state.readableListening = state.needReadable = true;
      state.emittedReadable = false;
      if (!state.reading) {
        processNextTick(nReadingNextTick, this);
      } else if (state.length) {
        emitReadable(this, state);
      }
    }
  }

  return res;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jslint.stream.prototype.isPaused"></a>[function <span class="apidocSignatureSpan">jslint.stream.prototype.</span>isPaused ()](#apidoc.element.jslint.stream.prototype.isPaused)
- description and source-code
```javascript
isPaused = function () {
  return this._readableState.flowing === false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jslint.stream.prototype.on"></a>[function <span class="apidocSignatureSpan">jslint.stream.prototype.</span>on (ev, fn)](#apidoc.element.jslint.stream.prototype.on)
- description and source-code
```javascript
on = function (ev, fn) {
  var res = Stream.prototype.on.call(this, ev, fn);

  if (ev === 'data') {
    // Start flowing on next tick if stream isn't explicitly paused
    if (this._readableState.flowing !== false) this.resume();
  } else if (ev === 'readable') {
    var state = this._readableState;
    if (!state.endEmitted && !state.readableListening) {
      state.readableListening = state.needReadable = true;
      state.emittedReadable = false;
      if (!state.reading) {
        processNextTick(nReadingNextTick, this);
      } else if (state.length) {
        emitReadable(this, state);
      }
    }
  }

  return res;
}
```
- example usage
```shell
...
    reporter = new JSONReportStream(parsed);
} else if (parsed.collector) {
    reporter = new CollectorStream(parsed);
} else {
    reporter = new ReportStream(parsed);
}

reporter.on('data', function (chunk) {
    if (chunk === '.') {
        pro.stderr.write(chunk);
    } else {
        con.log(chunk);
    }
});
...
```

#### <a name="apidoc.element.jslint.stream.prototype.pause"></a>[function <span class="apidocSignatureSpan">jslint.stream.prototype.</span>pause ()](#apidoc.element.jslint.stream.prototype.pause)
- description and source-code
```javascript
pause = function () {
  debug('call pause flowing=%j', this._readableState.flowing);
  if (false !== this._readableState.flowing) {
    debug('pause');
    this._readableState.flowing = false;
    this.emit('pause');
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jslint.stream.prototype.pipe"></a>[function <span class="apidocSignatureSpan">jslint.stream.prototype.</span>pipe (dest, pipeOpts)](#apidoc.element.jslint.stream.prototype.pipe)
- description and source-code
```javascript
pipe = function (dest, pipeOpts) {
  var src = this;
  var state = this._readableState;

  switch (state.pipesCount) {
    case 0:
      state.pipes = dest;
      break;
    case 1:
      state.pipes = [state.pipes, dest];
      break;
    default:
      state.pipes.push(dest);
      break;
  }
  state.pipesCount += 1;
  debug('pipe count=%d opts=%j', state.pipesCount, pipeOpts);

  var doEnd = (!pipeOpts || pipeOpts.end !== false) && dest !== process.stdout && dest !== process.stderr;

  var endFn = doEnd ? onend : cleanup;
  if (state.endEmitted) processNextTick(endFn);else src.once('end', endFn);

  dest.on('unpipe', onunpipe);
  function onunpipe(readable) {
    debug('onunpipe');
    if (readable === src) {
      cleanup();
    }
  }

  function onend() {
    debug('onend');
    dest.end();
  }

  // when the dest drains, it reduces the awaitDrain counter
  // on the source.  This would be more elegant with a .once()
  // handler in flow(), but adding and removing repeatedly is
  // too slow.
  var ondrain = pipeOnDrain(src);
  dest.on('drain', ondrain);

  var cleanedUp = false;
  function cleanup() {
    debug('cleanup');
    // cleanup event handlers once the pipe is broken
    dest.removeListener('close', onclose);
    dest.removeListener('finish', onfinish);
    dest.removeListener('drain', ondrain);
    dest.removeListener('error', onerror);
    dest.removeListener('unpipe', onunpipe);
    src.removeListener('end', onend);
    src.removeListener('end', cleanup);
    src.removeListener('data', ondata);

    cleanedUp = true;

    // if the reader is waiting for a drain event from this
    // specific writer, then it would cause it to never start
    // flowing again.
    // So, if this is awaiting a drain, then we just call it now.
    // If we don't know, then assume that we are waiting for one.
    if (state.awaitDrain && (!dest._writableState || dest._writableState.needDrain)) ondrain();
  }

  // If the user pushes more data while we're writing to dest then we'll end up
  // in ondata again. However, we only want to increase awaitDrain once because
  // dest will only emit one 'drain' event for the multiple writes.
  // => Introduce a guard on increasing awaitDrain.
  var increasedAwaitDrain = false;
  src.on('data', ondata);
  function ondata(chunk) {
    debug('ondata');
    increasedAwaitDrain = false;
    var ret = dest.write(chunk);
    if (false === ret && !increasedAwaitDrain) {
      // If the user unpiped during 'dest.write()', it is possible
      // to get stuck in a permanently paused state if that write
      // also returned false.
      // => Check whether 'dest' is still a piping destination.
      if ((state.pipesCount === 1 && state.pipes === dest || state.pipesCount > 1 && indexOf(state.pipes, dest) !== -1) && !cleanedUp
) {
        debug('false write response, pause', src._readableState.awaitDrain);
        src._readableState.awaitDrain++;
        increasedAwaitDrain = true;
      }
      src.pause();
    }
  }

  // if the dest has an error, then stop piping into it.
  // however, don't suppress the throwing behavior for this.
  function onerror(er) {
    debug('onerror', er);
    unpipe();
    dest.removeListener('error', onerror);
    if (EElistenerCount(dest, 'error') === 0) dest.emit('error', er);
  }

  // Make sure our error handler is attached before userland ones.
  prependListener(dest, 'error', onerror);

  // Both close and finish should trigger unpipe, but only once.
  function onclose() {
    dest.removeListener('finish', onfinish);
    unpipe();
  }
  dest.once('close', onclose);
  function onfinish() {
    debug('onfinish');
    dest.removeListener('close', onclose);
    unpipe();
  }
  dest.once('finish', onfinish);

  function unpipe() {
    debug('unpipe');
    src.unpipe(dest);
  }

  // tell the dest that it's being piped to
  dest.emit('pipe', src);

  // start the flow if it hasn't been started already.
  if (!state.flowing) {
    debug('pipe resume');
    src.resume();
  }

  return dest;
}
```
- example usage
```shell
...

var procOptions = optModule.getOptions(process.env.HOME, options),
    files = globFiles(options.argv.remain, glob, options.filter),
    opener = new FileOpener(),
    linter = new LintStream(procOptions),
    reporter = makeReporter(procOptions);

opener.pipe(linter);
linter.pipe(reporter);

reporter.on('finish', function () {
    if (cb) {
        return cb(null, reporter.lint);
    }
...
```

#### <a name="apidoc.element.jslint.stream.prototype.push"></a>[function <span class="apidocSignatureSpan">jslint.stream.prototype.</span>push (chunk, encoding)](#apidoc.element.jslint.stream.prototype.push)
- description and source-code
```javascript
push = function (chunk, encoding) {
  var state = this._readableState;

  if (!state.objectMode && typeof chunk === 'string') {
    encoding = encoding || state.defaultEncoding;
    if (encoding !== state.encoding) {
      chunk = bufferShim.from(chunk, encoding);
      encoding = '';
    }
  }

  return readableAddChunk(this, state, chunk, encoding, false);
}
```
- example usage
```shell
...

    this.allOK = true;
};
util.inherits(CollectorStream, Transform);

function CollectorStream_transform(chunk, ignore, callback) {
    // chunk: a package of lint data from JSLint
    this.lint.push([chunk.file, chunk.linted.errors]);

    this.allOK = this.allOK && chunk.linted.ok;

    callback();
}

CollectorStream.prototype._transform = CollectorStream_transform;
...
```

#### <a name="apidoc.element.jslint.stream.prototype.read"></a>[function <span class="apidocSignatureSpan">jslint.stream.prototype.</span>read (n)](#apidoc.element.jslint.stream.prototype.read)
- description and source-code
```javascript
read = function (n) {
  debug('read', n);
  n = parseInt(n, 10);
  var state = this._readableState;
  var nOrig = n;

  if (n !== 0) state.emittedReadable = false;

  // if we're doing read(0) to trigger a readable event, but we
  // already have a bunch of data in the buffer, then just trigger
  // the 'readable' event and move on.
  if (n === 0 && state.needReadable && (state.length >= state.highWaterMark || state.ended)) {
    debug('read: emitReadable', state.length, state.ended);
    if (state.length === 0 && state.ended) endReadable(this);else emitReadable(this);
    return null;
  }

  n = howMuchToRead(n, state);

  // if we've ended, and we're now clear, then finish it up.
  if (n === 0 && state.ended) {
    if (state.length === 0) endReadable(this);
    return null;
  }

  // All the actual chunk generation logic needs to be
  // *below* the call to _read.  The reason is that in certain
  // synthetic stream cases, such as passthrough streams, _read
  // may be a completely synchronous operation which may change
  // the state of the read buffer, providing enough data when
  // before there was *not* enough.
  //
  // So, the steps are:
  // 1. Figure out what the state of things will be after we do
  // a read from the buffer.
  //
  // 2. If that resulting state will trigger a _read, then call _read.
  // Note that this may be asynchronous, or synchronous.  Yes, it is
  // deeply ugly to write APIs this way, but that still doesn't mean
  // that the Readable class should behave improperly, as streams are
  // designed to be sync/async agnostic.
  // Take note if the _read call is sync or async (ie, if the read call
  // has returned yet), so that we know whether or not it's safe to emit
  // 'readable' etc.
  //
  // 3. Actually pull the requested chunks out of the buffer and return.

  // if we need a readable event, then we need to do some reading.
  var doRead = state.needReadable;
  debug('need readable', doRead);

  // if we currently have less than the highWaterMark, then also read some
  if (state.length === 0 || state.length - n < state.highWaterMark) {
    doRead = true;
    debug('length less than watermark', doRead);
  }

  // however, if we've ended, then there's no point, and if we're already
  // reading, then it's unnecessary.
  if (state.ended || state.reading) {
    doRead = false;
    debug('reading or ended', doRead);
  } else if (doRead) {
    debug('do read');
    state.reading = true;
    state.sync = true;
    // if the length is currently zero, then we *need* a readable event.
    if (state.length === 0) state.needReadable = true;
    // call internal read method
    this._read(state.highWaterMark);
    state.sync = false;
    // If _read pushed data synchronously, then 'reading' will be false,
    // and we need to re-evaluate how much data we can return to the user.
    if (!state.reading) n = howMuchToRead(nOrig, state);
  }

  var ret;
  if (n > 0) ret = fromList(n, state);else ret = null;

  if (ret === null) {
    state.needReadable = true;
    n = 0;
  } else {
    state.length -= n;
  }

  if (state.length === 0) {
    // If we have nothing in the buffer, then we want to know
    // as soon as we *do* get something into the buffer.
    if (!state.ended) state.needReadable = true;

    // If we tried to read() past the EOF, then emit end on the next tick.
    if (nOrig !== n && state.ended) endReadable(this);
  }

  if (ret !== null) this.emit('data', ret);

  return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jslint.stream.prototype.resume"></a>[function <span class="apidocSignatureSpan">jslint.stream.prototype.</span>resume ()](#apidoc.element.jslint.stream.prototype.resume)
- description and source-code
```javascript
resume = function () {
  var state = this._readableState;
  if (!state.flowing) {
    debug('resume');
    state.flowing = true;
    resume(this, state);
  }
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jslint.stream.prototype.setEncoding"></a>[function <span class="apidocSignatureSpan">jslint.stream.prototype.</span>setEncoding (enc)](#apidoc.element.jslint.stream.prototype.setEncoding)
- description and source-code
```javascript
setEncoding = function (enc) {
  if (!StringDecoder) StringDecoder = require('string_decoder/').StringDecoder;
  this._readableState.decoder = new StringDecoder(enc);
  this._readableState.encoding = enc;
  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jslint.stream.prototype.unpipe"></a>[function <span class="apidocSignatureSpan">jslint.stream.prototype.</span>unpipe (dest)](#apidoc.element.jslint.stream.prototype.unpipe)
- description and source-code
```javascript
unpipe = function (dest) {
  var state = this._readableState;

  // if we're not piping anywhere, then do nothing.
  if (state.pipesCount === 0) return this;

  // just one destination.  most common case.
  if (state.pipesCount === 1) {
    // passed in one, but it's not the right one.
    if (dest && dest !== state.pipes) return this;

    if (!dest) dest = state.pipes;

    // got a match.
    state.pipes = null;
    state.pipesCount = 0;
    state.flowing = false;
    if (dest) dest.emit('unpipe', this);
    return this;
  }

  // slow case. multiple pipe destinations.

  if (!dest) {
    // remove all.
    var dests = state.pipes;
    var len = state.pipesCount;
    state.pipes = null;
    state.pipesCount = 0;
    state.flowing = false;

    for (var _i = 0; _i < len; _i++) {
      dests[_i].emit('unpipe', this);
    }return this;
  }

  // try to find the right one.
  var i = indexOf(state.pipes, dest);
  if (i === -1) return this;

  state.pipes.splice(i, 1);
  state.pipesCount -= 1;
  if (state.pipesCount === 1) state.pipes = state.pipes[0];

  dest.emit('unpipe', this);

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jslint.stream.prototype.unshift"></a>[function <span class="apidocSignatureSpan">jslint.stream.prototype.</span>unshift (chunk)](#apidoc.element.jslint.stream.prototype.unshift)
- description and source-code
```javascript
unshift = function (chunk) {
  var state = this._readableState;
  return readableAddChunk(this, state, chunk, '', true);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.jslint.stream.prototype.wrap"></a>[function <span class="apidocSignatureSpan">jslint.stream.prototype.</span>wrap (stream)](#apidoc.element.jslint.stream.prototype.wrap)
- description and source-code
```javascript
wrap = function (stream) {
  var state = this._readableState;
  var paused = false;

  var self = this;
  stream.on('end', function () {
    debug('wrapped end');
    if (state.decoder && !state.ended) {
      var chunk = state.decoder.end();
      if (chunk && chunk.length) self.push(chunk);
    }

    self.push(null);
  });

  stream.on('data', function (chunk) {
    debug('wrapped data');
    if (state.decoder) chunk = state.decoder.write(chunk);

    // don't skip over falsy values in objectMode
    if (state.objectMode && (chunk === null || chunk === undefined)) return;else if (!state.objectMode && (!chunk || !chunk.length
)) return;

    var ret = self.push(chunk);
    if (!ret) {
      paused = true;
      stream.pause();
    }
  });

  // proxy all the other methods.
  // important when wrapping filters and duplexes.
  for (var i in stream) {
    if (this[i] === undefined && typeof stream[i] === 'function') {
      this[i] = function (method) {
        return function () {
          return stream[method].apply(stream, arguments);
        };
      }(i);
    }
  }

  // proxy certain important events.
  var events = ['error', 'close', 'destroy', 'pause', 'resume'];
  forEach(events, function (ev) {
    stream.on(ev, self.emit.bind(self, ev));
  });

  // when we try to consume some more bytes, simply unpause the
  // underlying stream.
  self._read = function (n) {
    debug('wrapped _read', n);
    if (paused) {
      paused = false;
      stream.resume();
    }
  };

  return self;
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
