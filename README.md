# api documentation for  [streamqueue (v1.1.1)](https://github.com/nfroidure/StreamQueue)  [![npm package](https://img.shields.io/npm/v/npmdoc-streamqueue.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-streamqueue) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-streamqueue.svg)](https://travis-ci.org/npmdoc/node-npmdoc-streamqueue)
#### Pipe queued streams progressively, keeping datas order.

[![NPM](https://nodei.co/npm/streamqueue.png?downloads=true)](https://www.npmjs.com/package/streamqueue)

[![apidoc](https://npmdoc.github.io/node-npmdoc-streamqueue/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-streamqueue_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-streamqueue/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-streamqueue/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-streamqueue/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Nicolas Froidure",
        "url": "http://www.insertafter.com/blog.html"
    },
    "bugs": {
        "url": "https://github.com/nfroidure/StreamQueue/issues"
    },
    "dependencies": {
        "isstream": "^0.1.2",
        "readable-stream": "~1.0.33"
    },
    "description": "Pipe queued streams progressively, keeping datas order.",
    "devDependencies": {
        "coveralls": "~2.11.2",
        "istanbul": "~0.3.14",
        "mocha": "~2.2.5",
        "mocha-lcov-reporter": "~0.0.2",
        "streamtest": "~1.2.0"
    },
    "directories": {},
    "dist": {
        "shasum": "d3ad76686be924bbf9ca2c74a814a2182475d6d7",
        "tarball": "https://registry.npmjs.org/streamqueue/-/streamqueue-1.1.1.tgz"
    },
    "engines": {
        "node": ">= 0.10.0"
    },
    "gitHead": "a772c3925e60fd2f26b7a2f8e0aa500793df62bc",
    "homepage": "https://github.com/nfroidure/StreamQueue",
    "keywords": [
        "queue",
        "streaming",
        "stream",
        "async",
        "pipe"
    ],
    "licenses": [
        {
            "type": "MIT",
            "url": "https://github.com/nfroidure/StreamQueue/blob/master/LICENSE"
        }
    ],
    "main": "src/index.js",
    "maintainers": [
        {
            "name": "nfroidure",
            "email": "nfroidure@elitwork.com"
        }
    ],
    "name": "streamqueue",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/nfroidure/StreamQueue.git"
    },
    "scripts": {
        "cli": "env NPM_RUN_CLI=1",
        "cover": "./node_modules/istanbul/lib/cli.js cover --report html ./node_modules/mocha/bin/_mocha -- tests/*.mocha.js -R spec -t 5000",
        "coveralls": "./node_modules/istanbul/lib/cli.js cover ./node_modules/mocha/bin/_mocha --report lcovonly -- tests/*.mocha.js -R spec -t 5000 && cat ./coverage/lcov.info | ./node_modules/coveralls/bin/coveralls.js && rm -rf ./coverage",
        "lint": "eslint **/*.js *.js",
        "test": "./node_modules/mocha/bin/mocha tests/*.mocha.js"
    },
    "version": "1.1.1"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module streamqueue](#apidoc.module.streamqueue)
1.  [function <span class="apidocSignatureSpan">streamqueue.</span>obj (options)](#apidoc.element.streamqueue.obj)
1.  [function <span class="apidocSignatureSpan">streamqueue.</span>super_ (options)](#apidoc.element.streamqueue.super_)
1.  [function <span class="apidocSignatureSpan">streamqueue.</span>super_.Duplex (options)](#apidoc.element.streamqueue.super_.Duplex)
1.  [function <span class="apidocSignatureSpan">streamqueue.</span>super_.PassThrough (options)](#apidoc.element.streamqueue.super_.PassThrough)
1.  [function <span class="apidocSignatureSpan">streamqueue.</span>super_.Transform (options)](#apidoc.element.streamqueue.super_.Transform)
1.  [function <span class="apidocSignatureSpan">streamqueue.</span>super_.Writable (options)](#apidoc.element.streamqueue.super_.Writable)
1.  object <span class="apidocSignatureSpan">streamqueue.</span>super_.Duplex.prototype
1.  object <span class="apidocSignatureSpan">streamqueue.</span>super_.PassThrough.prototype
1.  object <span class="apidocSignatureSpan">streamqueue.</span>super_.Transform.prototype
1.  object <span class="apidocSignatureSpan">streamqueue.</span>super_.Writable.prototype
1.  object <span class="apidocSignatureSpan">streamqueue.</span>super_.prototype

#### [module streamqueue.super_](#apidoc.module.streamqueue.super_)
1.  [function <span class="apidocSignatureSpan">streamqueue.</span>super_ ()](#apidoc.element.streamqueue.super_.super_)
1.  [function <span class="apidocSignatureSpan">streamqueue.super_.</span>Duplex (options)](#apidoc.element.streamqueue.super_.Duplex)
1.  [function <span class="apidocSignatureSpan">streamqueue.super_.</span>PassThrough (options)](#apidoc.element.streamqueue.super_.PassThrough)
1.  [function <span class="apidocSignatureSpan">streamqueue.super_.</span>Readable (options)](#apidoc.element.streamqueue.super_.Readable)
1.  [function <span class="apidocSignatureSpan">streamqueue.super_.</span>ReadableState (options, stream)](#apidoc.element.streamqueue.super_.ReadableState)
1.  [function <span class="apidocSignatureSpan">streamqueue.super_.</span>Stream ()](#apidoc.element.streamqueue.super_.Stream)
1.  [function <span class="apidocSignatureSpan">streamqueue.super_.</span>Transform (options)](#apidoc.element.streamqueue.super_.Transform)
1.  [function <span class="apidocSignatureSpan">streamqueue.super_.</span>Writable (options)](#apidoc.element.streamqueue.super_.Writable)
1.  [function <span class="apidocSignatureSpan">streamqueue.super_.</span>_fromList (n, state)](#apidoc.element.streamqueue.super_._fromList)

#### [module streamqueue.super_.Duplex](#apidoc.module.streamqueue.super_.Duplex)
1.  [function <span class="apidocSignatureSpan">streamqueue.super_.</span>Duplex (options)](#apidoc.element.streamqueue.super_.Duplex.Duplex)
1.  [function <span class="apidocSignatureSpan">streamqueue.super_.Duplex.</span>super_ (options)](#apidoc.element.streamqueue.super_.Duplex.super_)

#### [module streamqueue.super_.Duplex.prototype](#apidoc.module.streamqueue.super_.Duplex.prototype)
1.  [function <span class="apidocSignatureSpan">streamqueue.super_.Duplex.prototype.</span>_write (chunk, encoding, cb)](#apidoc.element.streamqueue.super_.Duplex.prototype._write)
1.  [function <span class="apidocSignatureSpan">streamqueue.super_.Duplex.prototype.</span>end (chunk, encoding, cb)](#apidoc.element.streamqueue.super_.Duplex.prototype.end)
1.  [function <span class="apidocSignatureSpan">streamqueue.super_.Duplex.prototype.</span>write (chunk, encoding, cb)](#apidoc.element.streamqueue.super_.Duplex.prototype.write)

#### [module streamqueue.super_.PassThrough](#apidoc.module.streamqueue.super_.PassThrough)
1.  [function <span class="apidocSignatureSpan">streamqueue.super_.</span>PassThrough (options)](#apidoc.element.streamqueue.super_.PassThrough.PassThrough)
1.  [function <span class="apidocSignatureSpan">streamqueue.super_.PassThrough.</span>super_ (options)](#apidoc.element.streamqueue.super_.PassThrough.super_)

#### [module streamqueue.super_.PassThrough.prototype](#apidoc.module.streamqueue.super_.PassThrough.prototype)
1.  [function <span class="apidocSignatureSpan">streamqueue.super_.PassThrough.prototype.</span>_transform (chunk, encoding, cb)](#apidoc.element.streamqueue.super_.PassThrough.prototype._transform)

#### [module streamqueue.super_.Transform](#apidoc.module.streamqueue.super_.Transform)
1.  [function <span class="apidocSignatureSpan">streamqueue.super_.</span>Transform (options)](#apidoc.element.streamqueue.super_.Transform.Transform)
1.  [function <span class="apidocSignatureSpan">streamqueue.super_.Transform.</span>super_ (options)](#apidoc.element.streamqueue.super_.Transform.super_)

#### [module streamqueue.super_.Transform.prototype](#apidoc.module.streamqueue.super_.Transform.prototype)
1.  [function <span class="apidocSignatureSpan">streamqueue.super_.Transform.prototype.</span>_read (n)](#apidoc.element.streamqueue.super_.Transform.prototype._read)
1.  [function <span class="apidocSignatureSpan">streamqueue.super_.Transform.prototype.</span>_transform (chunk, encoding, cb)](#apidoc.element.streamqueue.super_.Transform.prototype._transform)
1.  [function <span class="apidocSignatureSpan">streamqueue.super_.Transform.prototype.</span>_write (chunk, encoding, cb)](#apidoc.element.streamqueue.super_.Transform.prototype._write)
1.  [function <span class="apidocSignatureSpan">streamqueue.super_.Transform.prototype.</span>push (chunk, encoding)](#apidoc.element.streamqueue.super_.Transform.prototype.push)

#### [module streamqueue.super_.Writable](#apidoc.module.streamqueue.super_.Writable)
1.  [function <span class="apidocSignatureSpan">streamqueue.super_.</span>Writable (options)](#apidoc.element.streamqueue.super_.Writable.Writable)
1.  [function <span class="apidocSignatureSpan">streamqueue.super_.Writable.</span>WritableState (options, stream)](#apidoc.element.streamqueue.super_.Writable.WritableState)
1.  [function <span class="apidocSignatureSpan">streamqueue.super_.Writable.</span>super_ ()](#apidoc.element.streamqueue.super_.Writable.super_)

#### [module streamqueue.super_.Writable.prototype](#apidoc.module.streamqueue.super_.Writable.prototype)
1.  [function <span class="apidocSignatureSpan">streamqueue.super_.Writable.prototype.</span>_write (chunk, encoding, cb)](#apidoc.element.streamqueue.super_.Writable.prototype._write)
1.  [function <span class="apidocSignatureSpan">streamqueue.super_.Writable.prototype.</span>end (chunk, encoding, cb)](#apidoc.element.streamqueue.super_.Writable.prototype.end)
1.  [function <span class="apidocSignatureSpan">streamqueue.super_.Writable.prototype.</span>pipe ()](#apidoc.element.streamqueue.super_.Writable.prototype.pipe)
1.  [function <span class="apidocSignatureSpan">streamqueue.super_.Writable.prototype.</span>write (chunk, encoding, cb)](#apidoc.element.streamqueue.super_.Writable.prototype.write)

#### [module streamqueue.super_.prototype](#apidoc.module.streamqueue.super_.prototype)
1.  [function <span class="apidocSignatureSpan">streamqueue.super_.prototype.</span>_read (n)](#apidoc.element.streamqueue.super_.prototype._read)
1.  [function <span class="apidocSignatureSpan">streamqueue.super_.prototype.</span>addListener (ev, fn)](#apidoc.element.streamqueue.super_.prototype.addListener)
1.  [function <span class="apidocSignatureSpan">streamqueue.super_.prototype.</span>on (ev, fn)](#apidoc.element.streamqueue.super_.prototype.on)
1.  [function <span class="apidocSignatureSpan">streamqueue.super_.prototype.</span>pause ()](#apidoc.element.streamqueue.super_.prototype.pause)
1.  [function <span class="apidocSignatureSpan">streamqueue.super_.prototype.</span>pipe (dest, pipeOpts)](#apidoc.element.streamqueue.super_.prototype.pipe)
1.  [function <span class="apidocSignatureSpan">streamqueue.super_.prototype.</span>push (chunk, encoding)](#apidoc.element.streamqueue.super_.prototype.push)
1.  [function <span class="apidocSignatureSpan">streamqueue.super_.prototype.</span>read (n)](#apidoc.element.streamqueue.super_.prototype.read)
1.  [function <span class="apidocSignatureSpan">streamqueue.super_.prototype.</span>resume ()](#apidoc.element.streamqueue.super_.prototype.resume)
1.  [function <span class="apidocSignatureSpan">streamqueue.super_.prototype.</span>setEncoding (enc)](#apidoc.element.streamqueue.super_.prototype.setEncoding)
1.  [function <span class="apidocSignatureSpan">streamqueue.super_.prototype.</span>unpipe (dest)](#apidoc.element.streamqueue.super_.prototype.unpipe)
1.  [function <span class="apidocSignatureSpan">streamqueue.super_.prototype.</span>unshift (chunk)](#apidoc.element.streamqueue.super_.prototype.unshift)
1.  [function <span class="apidocSignatureSpan">streamqueue.super_.prototype.</span>wrap (stream)](#apidoc.element.streamqueue.super_.prototype.wrap)



# <a name="apidoc.module.streamqueue"></a>[module streamqueue](#apidoc.module.streamqueue)

#### <a name="apidoc.element.streamqueue.obj"></a>[function <span class="apidocSignatureSpan">streamqueue.</span>obj (options)](#apidoc.element.streamqueue.obj)
- description and source-code
```javascript
function streamQueueObj(options) {
  var firstArgumentIsAStream = (!options) || isStream(options);
  var streams = [].slice.call(arguments, firstArgumentIsAStream ? 0 : 1);
  options = firstArgumentIsAStream ? {} : options;
  options.objectMode = true;
  return StreamQueue.apply({}.undef, [options].concat(streams));
}
```
- example usage
```shell
...
Append streams given in argument to the queue.

### StreamQueue.done([stream1, stream2, ... streamN])

Append streams given in argument to the queue and ends when the queue is empty.


### StreamQueue.obj([options], [stream1, stream2, ... streamN])

A shortcut for 'StreamQueue({objectMode: true})'.

## Stats

[![NPM](https://nodei.co/npm/streamqueue.png?downloads=true&stars=true)](https://nodei.co/npm/streamqueue/)
[![NPM](https://nodei.co/npm-dl/streamqueue.png)](https://nodei.co/npm/streamqueue/)
...
```

#### <a name="apidoc.element.streamqueue.super_"></a>[function <span class="apidocSignatureSpan">streamqueue.</span>super_ (options)](#apidoc.element.streamqueue.super_)
- description and source-code
```javascript
function Readable(options) {
  if (!(this instanceof Readable))
    return new Readable(options);

  this._readableState = new ReadableState(options, this);

  // legacy
  this.readable = true;

  Stream.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.streamqueue.super_.Duplex"></a>[function <span class="apidocSignatureSpan">streamqueue.</span>super_.Duplex (options)](#apidoc.element.streamqueue.super_.Duplex)
- description and source-code
```javascript
function Duplex(options) {
  if (!(this instanceof Duplex))
    return new Duplex(options);

  Readable.call(this, options);
  Writable.call(this, options);

  if (options && options.readable === false)
    this.readable = false;

  if (options && options.writable === false)
    this.writable = false;

  this.allowHalfOpen = true;
  if (options && options.allowHalfOpen === false)
    this.allowHalfOpen = false;

  this.once('end', onend);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.streamqueue.super_.PassThrough"></a>[function <span class="apidocSignatureSpan">streamqueue.</span>super_.PassThrough (options)](#apidoc.element.streamqueue.super_.PassThrough)
- description and source-code
```javascript
function PassThrough(options) {
  if (!(this instanceof PassThrough))
    return new PassThrough(options);

  Transform.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.streamqueue.super_.Transform"></a>[function <span class="apidocSignatureSpan">streamqueue.</span>super_.Transform (options)](#apidoc.element.streamqueue.super_.Transform)
- description and source-code
```javascript
function Transform(options) {
  if (!(this instanceof Transform))
    return new Transform(options);

  Duplex.call(this, options);

  var ts = this._transformState = new TransformState(options, this);

  // when the writable side finishes, then flush out anything remaining.
  var stream = this;

  // start out asking for a readable event once data is transformed.
  this._readableState.needReadable = true;

  // we have implemented the _read method, and done the other things
  // that Readable wants before the first _read call, so unset the
  // sync guard flag.
  this._readableState.sync = false;

  this.once('finish', function() {
    if ('function' === typeof this._flush)
      this._flush(function(er) {
        done(stream, er);
      });
    else
      done(stream);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.streamqueue.super_.Writable"></a>[function <span class="apidocSignatureSpan">streamqueue.</span>super_.Writable (options)](#apidoc.element.streamqueue.super_.Writable)
- description and source-code
```javascript
function Writable(options) {
  var Duplex = require('./_stream_duplex');

  // Writable ctor is applied to Duplexes, though they're not
  // instanceof Writable, they're instanceof Readable.
  if (!(this instanceof Writable) && !(this instanceof Duplex))
    return new Writable(options);

  this._writableState = new WritableState(options, this);

  // legacy.
  this.writable = true;

  Stream.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.streamqueue.super_"></a>[module streamqueue.super_](#apidoc.module.streamqueue.super_)

#### <a name="apidoc.element.streamqueue.super_.super_"></a>[function <span class="apidocSignatureSpan">streamqueue.</span>super_ ()](#apidoc.element.streamqueue.super_.super_)
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

#### <a name="apidoc.element.streamqueue.super_.Duplex"></a>[function <span class="apidocSignatureSpan">streamqueue.super_.</span>Duplex (options)](#apidoc.element.streamqueue.super_.Duplex)
- description and source-code
```javascript
function Duplex(options) {
  if (!(this instanceof Duplex))
    return new Duplex(options);

  Readable.call(this, options);
  Writable.call(this, options);

  if (options && options.readable === false)
    this.readable = false;

  if (options && options.writable === false)
    this.writable = false;

  this.allowHalfOpen = true;
  if (options && options.allowHalfOpen === false)
    this.allowHalfOpen = false;

  this.once('end', onend);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.streamqueue.super_.PassThrough"></a>[function <span class="apidocSignatureSpan">streamqueue.super_.</span>PassThrough (options)](#apidoc.element.streamqueue.super_.PassThrough)
- description and source-code
```javascript
function PassThrough(options) {
  if (!(this instanceof PassThrough))
    return new PassThrough(options);

  Transform.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.streamqueue.super_.Readable"></a>[function <span class="apidocSignatureSpan">streamqueue.super_.</span>Readable (options)](#apidoc.element.streamqueue.super_.Readable)
- description and source-code
```javascript
function Readable(options) {
  if (!(this instanceof Readable))
    return new Readable(options);

  this._readableState = new ReadableState(options, this);

  // legacy
  this.readable = true;

  Stream.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.streamqueue.super_.ReadableState"></a>[function <span class="apidocSignatureSpan">streamqueue.super_.</span>ReadableState (options, stream)](#apidoc.element.streamqueue.super_.ReadableState)
- description and source-code
```javascript
function ReadableState(options, stream) {
  options = options || {};

  // the point at which it stops calling _read() to fill the buffer
  // Note: 0 is a valid value, means "don't call _read preemptively ever"
  var hwm = options.highWaterMark;
  this.highWaterMark = (hwm || hwm === 0) ? hwm : 16 * 1024;

  // cast to ints.
  this.highWaterMark = ~~this.highWaterMark;

  this.buffer = [];
  this.length = 0;
  this.pipes = null;
  this.pipesCount = 0;
  this.flowing = false;
  this.ended = false;
  this.endEmitted = false;
  this.reading = false;

  // In streams that never have any data, and do push(null) right away,
  // the consumer can miss the 'end' event if they do some I/O before
  // consuming the stream.  So, we don't emit('end') until some reading
  // happens.
  this.calledRead = false;

  // a flag to be able to tell if the onwrite cb is called immediately,
  // or on a later tick.  We set this to true at first, becuase any
  // actions that shouldn't happen until "later" should generally also
  // not happen before the first write call.
  this.sync = true;

  // whenever we return null, then we set a flag to say
  // that we're awaiting a 'readable' event emission.
  this.needReadable = false;
  this.emittedReadable = false;
  this.readableListening = false;


  // object stream flag. Used to make read(n) ignore n and to
  // make all the buffer merging and length checks go away
  this.objectMode = !!options.objectMode;

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
    if (!StringDecoder)
      StringDecoder = require('string_decoder/').StringDecoder;
    this.decoder = new StringDecoder(options.encoding);
    this.encoding = options.encoding;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.streamqueue.super_.Stream"></a>[function <span class="apidocSignatureSpan">streamqueue.super_.</span>Stream ()](#apidoc.element.streamqueue.super_.Stream)
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

#### <a name="apidoc.element.streamqueue.super_.Transform"></a>[function <span class="apidocSignatureSpan">streamqueue.super_.</span>Transform (options)](#apidoc.element.streamqueue.super_.Transform)
- description and source-code
```javascript
function Transform(options) {
  if (!(this instanceof Transform))
    return new Transform(options);

  Duplex.call(this, options);

  var ts = this._transformState = new TransformState(options, this);

  // when the writable side finishes, then flush out anything remaining.
  var stream = this;

  // start out asking for a readable event once data is transformed.
  this._readableState.needReadable = true;

  // we have implemented the _read method, and done the other things
  // that Readable wants before the first _read call, so unset the
  // sync guard flag.
  this._readableState.sync = false;

  this.once('finish', function() {
    if ('function' === typeof this._flush)
      this._flush(function(er) {
        done(stream, er);
      });
    else
      done(stream);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.streamqueue.super_.Writable"></a>[function <span class="apidocSignatureSpan">streamqueue.super_.</span>Writable (options)](#apidoc.element.streamqueue.super_.Writable)
- description and source-code
```javascript
function Writable(options) {
  var Duplex = require('./_stream_duplex');

  // Writable ctor is applied to Duplexes, though they're not
  // instanceof Writable, they're instanceof Readable.
  if (!(this instanceof Writable) && !(this instanceof Duplex))
    return new Writable(options);

  this._writableState = new WritableState(options, this);

  // legacy.
  this.writable = true;

  Stream.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.streamqueue.super_._fromList"></a>[function <span class="apidocSignatureSpan">streamqueue.super_.</span>_fromList (n, state)](#apidoc.element.streamqueue.super_._fromList)
- description and source-code
```javascript
function fromList(n, state) {
  var list = state.buffer;
  var length = state.length;
  var stringMode = !!state.decoder;
  var objectMode = !!state.objectMode;
  var ret;

  // nothing in the list, definitely empty.
  if (list.length === 0)
    return null;

  if (length === 0)
    ret = null;
  else if (objectMode)
    ret = list.shift();
  else if (!n || n >= length) {
    // read it all, truncate the array.
    if (stringMode)
      ret = list.join('');
    else
      ret = Buffer.concat(list, length);
    list.length = 0;
  } else {
    // read just some of it.
    if (n < list[0].length) {
      // just take a part of the first list item.
      // slice is the same for buffers and strings.
      var buf = list[0];
      ret = buf.slice(0, n);
      list[0] = buf.slice(n);
    } else if (n === list[0].length) {
      // first list is a perfect match
      ret = list.shift();
    } else {
      // complex case.
      // we have enough to cover it, but it spans past the first buffer.
      if (stringMode)
        ret = '';
      else
        ret = new Buffer(n);

      var c = 0;
      for (var i = 0, l = list.length; i < l && c < n; i++) {
        var buf = list[0];
        var cpy = Math.min(n - c, buf.length);

        if (stringMode)
          ret += buf.slice(0, cpy);
        else
          buf.copy(ret, c, 0, cpy);

        if (cpy < buf.length)
          list[0] = buf.slice(cpy);
        else
          list.shift();

        c += cpy;
      }
    }
  }

  return ret;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.streamqueue.super_.Duplex"></a>[module streamqueue.super_.Duplex](#apidoc.module.streamqueue.super_.Duplex)

#### <a name="apidoc.element.streamqueue.super_.Duplex.Duplex"></a>[function <span class="apidocSignatureSpan">streamqueue.super_.</span>Duplex (options)](#apidoc.element.streamqueue.super_.Duplex.Duplex)
- description and source-code
```javascript
function Duplex(options) {
  if (!(this instanceof Duplex))
    return new Duplex(options);

  Readable.call(this, options);
  Writable.call(this, options);

  if (options && options.readable === false)
    this.readable = false;

  if (options && options.writable === false)
    this.writable = false;

  this.allowHalfOpen = true;
  if (options && options.allowHalfOpen === false)
    this.allowHalfOpen = false;

  this.once('end', onend);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.streamqueue.super_.Duplex.super_"></a>[function <span class="apidocSignatureSpan">streamqueue.super_.Duplex.</span>super_ (options)](#apidoc.element.streamqueue.super_.Duplex.super_)
- description and source-code
```javascript
function Readable(options) {
  if (!(this instanceof Readable))
    return new Readable(options);

  this._readableState = new ReadableState(options, this);

  // legacy
  this.readable = true;

  Stream.call(this);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.streamqueue.super_.Duplex.prototype"></a>[module streamqueue.super_.Duplex.prototype](#apidoc.module.streamqueue.super_.Duplex.prototype)

#### <a name="apidoc.element.streamqueue.super_.Duplex.prototype._write"></a>[function <span class="apidocSignatureSpan">streamqueue.super_.Duplex.prototype.</span>_write (chunk, encoding, cb)](#apidoc.element.streamqueue.super_.Duplex.prototype._write)
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

#### <a name="apidoc.element.streamqueue.super_.Duplex.prototype.end"></a>[function <span class="apidocSignatureSpan">streamqueue.super_.Duplex.prototype.</span>end (chunk, encoding, cb)](#apidoc.element.streamqueue.super_.Duplex.prototype.end)
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

  if (typeof chunk !== 'undefined' && chunk !== null)
    this.write(chunk, encoding);

  // ignore unnecessary end() calls.
  if (!state.ending && !state.finished)
    endWritable(this, state, cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.streamqueue.super_.Duplex.prototype.write"></a>[function <span class="apidocSignatureSpan">streamqueue.super_.Duplex.prototype.</span>write (chunk, encoding, cb)](#apidoc.element.streamqueue.super_.Duplex.prototype.write)
- description and source-code
```javascript
write = function (chunk, encoding, cb) {
  var state = this._writableState;
  var ret = false;

  if (typeof encoding === 'function') {
    cb = encoding;
    encoding = null;
  }

  if (Buffer.isBuffer(chunk))
    encoding = 'buffer';
  else if (!encoding)
    encoding = state.defaultEncoding;

  if (typeof cb !== 'function')
    cb = function() {};

  if (state.ended)
    writeAfterEnd(this, state, cb);
  else if (validChunk(this, state, chunk, cb))
    ret = writeOrBuffer(this, state, chunk, encoding, cb);

  return ret;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.streamqueue.super_.PassThrough"></a>[module streamqueue.super_.PassThrough](#apidoc.module.streamqueue.super_.PassThrough)

#### <a name="apidoc.element.streamqueue.super_.PassThrough.PassThrough"></a>[function <span class="apidocSignatureSpan">streamqueue.super_.</span>PassThrough (options)](#apidoc.element.streamqueue.super_.PassThrough.PassThrough)
- description and source-code
```javascript
function PassThrough(options) {
  if (!(this instanceof PassThrough))
    return new PassThrough(options);

  Transform.call(this, options);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.streamqueue.super_.PassThrough.super_"></a>[function <span class="apidocSignatureSpan">streamqueue.super_.PassThrough.</span>super_ (options)](#apidoc.element.streamqueue.super_.PassThrough.super_)
- description and source-code
```javascript
function Transform(options) {
  if (!(this instanceof Transform))
    return new Transform(options);

  Duplex.call(this, options);

  var ts = this._transformState = new TransformState(options, this);

  // when the writable side finishes, then flush out anything remaining.
  var stream = this;

  // start out asking for a readable event once data is transformed.
  this._readableState.needReadable = true;

  // we have implemented the _read method, and done the other things
  // that Readable wants before the first _read call, so unset the
  // sync guard flag.
  this._readableState.sync = false;

  this.once('finish', function() {
    if ('function' === typeof this._flush)
      this._flush(function(er) {
        done(stream, er);
      });
    else
      done(stream);
  });
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.streamqueue.super_.PassThrough.prototype"></a>[module streamqueue.super_.PassThrough.prototype](#apidoc.module.streamqueue.super_.PassThrough.prototype)

#### <a name="apidoc.element.streamqueue.super_.PassThrough.prototype._transform"></a>[function <span class="apidocSignatureSpan">streamqueue.super_.PassThrough.prototype.</span>_transform (chunk, encoding, cb)](#apidoc.element.streamqueue.super_.PassThrough.prototype._transform)
- description and source-code
```javascript
_transform = function (chunk, encoding, cb) {
  cb(null, chunk);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.streamqueue.super_.Transform"></a>[module streamqueue.super_.Transform](#apidoc.module.streamqueue.super_.Transform)

#### <a name="apidoc.element.streamqueue.super_.Transform.Transform"></a>[function <span class="apidocSignatureSpan">streamqueue.super_.</span>Transform (options)](#apidoc.element.streamqueue.super_.Transform.Transform)
- description and source-code
```javascript
function Transform(options) {
  if (!(this instanceof Transform))
    return new Transform(options);

  Duplex.call(this, options);

  var ts = this._transformState = new TransformState(options, this);

  // when the writable side finishes, then flush out anything remaining.
  var stream = this;

  // start out asking for a readable event once data is transformed.
  this._readableState.needReadable = true;

  // we have implemented the _read method, and done the other things
  // that Readable wants before the first _read call, so unset the
  // sync guard flag.
  this._readableState.sync = false;

  this.once('finish', function() {
    if ('function' === typeof this._flush)
      this._flush(function(er) {
        done(stream, er);
      });
    else
      done(stream);
  });
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.streamqueue.super_.Transform.super_"></a>[function <span class="apidocSignatureSpan">streamqueue.super_.Transform.</span>super_ (options)](#apidoc.element.streamqueue.super_.Transform.super_)
- description and source-code
```javascript
function Duplex(options) {
  if (!(this instanceof Duplex))
    return new Duplex(options);

  Readable.call(this, options);
  Writable.call(this, options);

  if (options && options.readable === false)
    this.readable = false;

  if (options && options.writable === false)
    this.writable = false;

  this.allowHalfOpen = true;
  if (options && options.allowHalfOpen === false)
    this.allowHalfOpen = false;

  this.once('end', onend);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.streamqueue.super_.Transform.prototype"></a>[module streamqueue.super_.Transform.prototype](#apidoc.module.streamqueue.super_.Transform.prototype)

#### <a name="apidoc.element.streamqueue.super_.Transform.prototype._read"></a>[function <span class="apidocSignatureSpan">streamqueue.super_.Transform.prototype.</span>_read (n)](#apidoc.element.streamqueue.super_.Transform.prototype._read)
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

#### <a name="apidoc.element.streamqueue.super_.Transform.prototype._transform"></a>[function <span class="apidocSignatureSpan">streamqueue.super_.Transform.prototype.</span>_transform (chunk, encoding, cb)](#apidoc.element.streamqueue.super_.Transform.prototype._transform)
- description and source-code
```javascript
_transform = function (chunk, encoding, cb) {
  throw new Error('not implemented');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.streamqueue.super_.Transform.prototype._write"></a>[function <span class="apidocSignatureSpan">streamqueue.super_.Transform.prototype.</span>_write (chunk, encoding, cb)](#apidoc.element.streamqueue.super_.Transform.prototype._write)
- description and source-code
```javascript
_write = function (chunk, encoding, cb) {
  var ts = this._transformState;
  ts.writecb = cb;
  ts.writechunk = chunk;
  ts.writeencoding = encoding;
  if (!ts.transforming) {
    var rs = this._readableState;
    if (ts.needTransform ||
        rs.needReadable ||
        rs.length < rs.highWaterMark)
      this._read(rs.highWaterMark);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.streamqueue.super_.Transform.prototype.push"></a>[function <span class="apidocSignatureSpan">streamqueue.super_.Transform.prototype.</span>push (chunk, encoding)](#apidoc.element.streamqueue.super_.Transform.prototype.push)
- description and source-code
```javascript
push = function (chunk, encoding) {
  this._transformState.needTransform = false;
  return Duplex.prototype.push.call(this, chunk, encoding);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.streamqueue.super_.Writable"></a>[module streamqueue.super_.Writable](#apidoc.module.streamqueue.super_.Writable)

#### <a name="apidoc.element.streamqueue.super_.Writable.Writable"></a>[function <span class="apidocSignatureSpan">streamqueue.super_.</span>Writable (options)](#apidoc.element.streamqueue.super_.Writable.Writable)
- description and source-code
```javascript
function Writable(options) {
  var Duplex = require('./_stream_duplex');

  // Writable ctor is applied to Duplexes, though they're not
  // instanceof Writable, they're instanceof Readable.
  if (!(this instanceof Writable) && !(this instanceof Duplex))
    return new Writable(options);

  this._writableState = new WritableState(options, this);

  // legacy.
  this.writable = true;

  Stream.call(this);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.streamqueue.super_.Writable.WritableState"></a>[function <span class="apidocSignatureSpan">streamqueue.super_.Writable.</span>WritableState (options, stream)](#apidoc.element.streamqueue.super_.Writable.WritableState)
- description and source-code
```javascript
function WritableState(options, stream) {
  options = options || {};

  // the point at which write() starts returning false
  // Note: 0 is a valid value, means that we always return false if
  // the entire buffer is not flushed immediately on write()
  var hwm = options.highWaterMark;
  this.highWaterMark = (hwm || hwm === 0) ? hwm : 16 * 1024;

  // object stream flag to indicate whether or not this stream
  // contains buffers or objects.
  this.objectMode = !!options.objectMode;

  // cast to ints.
  this.highWaterMark = ~~this.highWaterMark;

  this.needDrain = false;
  // at the start of calling end()
  this.ending = false;
  // when end() has been called, and returned
  this.ended = false;
  // when 'finish' is emitted
  this.finished = false;

  // should we decode strings into buffers before passing to _write?
  // this is here so that some node-core streams can optimize string
  // handling at a lower level.
  var noDecode = options.decodeStrings === false;
  this.decodeStrings = !noDecode;

  // Crypto is kind of old and crusty.  Historically, its default string
  // encoding is 'binary' so we have to make this configurable.
  // Everything else in the universe uses 'utf8', though.
  this.defaultEncoding = options.defaultEncoding || 'utf8';

  // not an actual buffer we keep track of, but a measurement
  // of how much we're waiting to get pushed to some underlying
  // socket or file.
  this.length = 0;

  // a flag to see when we're in the middle of a write.
  this.writing = false;

  // a flag to be able to tell if the onwrite cb is called immediately,
  // or on a later tick.  We set this to true at first, becuase any
  // actions that shouldn't happen until "later" should generally also
  // not happen before the first write call.
  this.sync = true;

  // a flag to know if we're processing previously buffered items, which
  // may call the _write() callback in the same tick, so that we don't
  // end up in an overlapped onwrite situation.
  this.bufferProcessing = false;

  // the callback that's passed to _write(chunk,cb)
  this.onwrite = function(er) {
    onwrite(stream, er);
  };

  // the callback that the user supplies to write(chunk,encoding,cb)
  this.writecb = null;

  // the amount that is being written when _write is called.
  this.writelen = 0;

  this.buffer = [];

  // True if the error was already emitted and should not be thrown again
  this.errorEmitted = false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.streamqueue.super_.Writable.super_"></a>[function <span class="apidocSignatureSpan">streamqueue.super_.Writable.</span>super_ ()](#apidoc.element.streamqueue.super_.Writable.super_)
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



# <a name="apidoc.module.streamqueue.super_.Writable.prototype"></a>[module streamqueue.super_.Writable.prototype](#apidoc.module.streamqueue.super_.Writable.prototype)

#### <a name="apidoc.element.streamqueue.super_.Writable.prototype._write"></a>[function <span class="apidocSignatureSpan">streamqueue.super_.Writable.prototype.</span>_write (chunk, encoding, cb)](#apidoc.element.streamqueue.super_.Writable.prototype._write)
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

#### <a name="apidoc.element.streamqueue.super_.Writable.prototype.end"></a>[function <span class="apidocSignatureSpan">streamqueue.super_.Writable.prototype.</span>end (chunk, encoding, cb)](#apidoc.element.streamqueue.super_.Writable.prototype.end)
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

  if (typeof chunk !== 'undefined' && chunk !== null)
    this.write(chunk, encoding);

  // ignore unnecessary end() calls.
  if (!state.ending && !state.finished)
    endWritable(this, state, cb);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.streamqueue.super_.Writable.prototype.pipe"></a>[function <span class="apidocSignatureSpan">streamqueue.super_.Writable.prototype.</span>pipe ()](#apidoc.element.streamqueue.super_.Writable.prototype.pipe)
- description and source-code
```javascript
pipe = function () {
  this.emit('error', new Error('Cannot pipe. Not readable.'));
}
```
- example usage
```shell
...
'''js
var streamqueue = require('streamqueue');

var queue = streamqueue(
  Fs.createReadStream('input.txt'),
  Fs.createReadStream('input2.txt'),
  Fs.createReadStream('input3.txt')
).pipe(process.stdout);
'''
StreamQueue also accept functions returning streams, the above can be written
 like this, doing system calls only when piping:
'''js
var streamqueue = require('streamqueue');

var queue = streamqueue(
...
```

#### <a name="apidoc.element.streamqueue.super_.Writable.prototype.write"></a>[function <span class="apidocSignatureSpan">streamqueue.super_.Writable.prototype.</span>write (chunk, encoding, cb)](#apidoc.element.streamqueue.super_.Writable.prototype.write)
- description and source-code
```javascript
write = function (chunk, encoding, cb) {
  var state = this._writableState;
  var ret = false;

  if (typeof encoding === 'function') {
    cb = encoding;
    encoding = null;
  }

  if (Buffer.isBuffer(chunk))
    encoding = 'buffer';
  else if (!encoding)
    encoding = state.defaultEncoding;

  if (typeof cb !== 'function')
    cb = function() {};

  if (state.ended)
    writeAfterEnd(this, state, cb);
  else if (validChunk(this, state, chunk, cb))
    ret = writeOrBuffer(this, state, chunk, encoding, cb);

  return ret;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.streamqueue.super_.prototype"></a>[module streamqueue.super_.prototype](#apidoc.module.streamqueue.super_.prototype)

#### <a name="apidoc.element.streamqueue.super_.prototype._read"></a>[function <span class="apidocSignatureSpan">streamqueue.super_.prototype.</span>_read (n)](#apidoc.element.streamqueue.super_.prototype._read)
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

#### <a name="apidoc.element.streamqueue.super_.prototype.addListener"></a>[function <span class="apidocSignatureSpan">streamqueue.super_.prototype.</span>addListener (ev, fn)](#apidoc.element.streamqueue.super_.prototype.addListener)
- description and source-code
```javascript
addListener = function (ev, fn) {
  var res = Stream.prototype.on.call(this, ev, fn);

  if (ev === 'data' && !this._readableState.flowing)
    emitDataEvents(this);

  if (ev === 'readable' && this.readable) {
    var state = this._readableState;
    if (!state.readableListening) {
      state.readableListening = true;
      state.emittedReadable = false;
      state.needReadable = true;
      if (!state.reading) {
        this.read(0);
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

#### <a name="apidoc.element.streamqueue.super_.prototype.on"></a>[function <span class="apidocSignatureSpan">streamqueue.super_.prototype.</span>on (ev, fn)](#apidoc.element.streamqueue.super_.prototype.on)
- description and source-code
```javascript
on = function (ev, fn) {
  var res = Stream.prototype.on.call(this, ev, fn);

  if (ev === 'data' && !this._readableState.flowing)
    emitDataEvents(this);

  if (ev === 'readable' && this.readable) {
    var state = this._readableState;
    if (!state.readableListening) {
      state.readableListening = true;
      state.emittedReadable = false;
      state.needReadable = true;
      if (!state.reading) {
        this.read(0);
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

#### <a name="apidoc.element.streamqueue.super_.prototype.pause"></a>[function <span class="apidocSignatureSpan">streamqueue.super_.prototype.</span>pause ()](#apidoc.element.streamqueue.super_.prototype.pause)
- description and source-code
```javascript
pause = function () {
  emitDataEvents(this, true);
  this.emit('pause');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.streamqueue.super_.prototype.pipe"></a>[function <span class="apidocSignatureSpan">streamqueue.super_.prototype.</span>pipe (dest, pipeOpts)](#apidoc.element.streamqueue.super_.prototype.pipe)
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

  var doEnd = (!pipeOpts || pipeOpts.end !== false) &&
              dest !== process.stdout &&
              dest !== process.stderr;

  var endFn = doEnd ? onend : cleanup;
  if (state.endEmitted)
    process.nextTick(endFn);
  else
    src.once('end', endFn);

  dest.on('unpipe', onunpipe);
  function onunpipe(readable) {
    if (readable !== src) return;
    cleanup();
  }

  function onend() {
    dest.end();
  }

  // when the dest drains, it reduces the awaitDrain counter
  // on the source.  This would be more elegant with a .once()
  // handler in flow(), but adding and removing repeatedly is
  // too slow.
  var ondrain = pipeOnDrain(src);
  dest.on('drain', ondrain);

  function cleanup() {
    // cleanup event handlers once the pipe is broken
    dest.removeListener('close', onclose);
    dest.removeListener('finish', onfinish);
    dest.removeListener('drain', ondrain);
    dest.removeListener('error', onerror);
    dest.removeListener('unpipe', onunpipe);
    src.removeListener('end', onend);
    src.removeListener('end', cleanup);

    // if the reader is waiting for a drain event from this
    // specific writer, then it would cause it to never start
    // flowing again.
    // So, if this is awaiting a drain, then we just call it now.
    // If we don't know, then assume that we are waiting for one.
    if (!dest._writableState || dest._writableState.needDrain)
      ondrain();
  }

  // if the dest has an error, then stop piping into it.
  // however, don't suppress the throwing behavior for this.
  function onerror(er) {
    unpipe();
    dest.removeListener('error', onerror);
    if (EE.listenerCount(dest, 'error') === 0)
      dest.emit('error', er);
  }
  // This is a brutally ugly hack to make sure that our error handler
  // is attached before any userland ones.  NEVER DO THIS.
  if (!dest._events || !dest._events.error)
    dest.on('error', onerror);
  else if (isArray(dest._events.error))
    dest._events.error.unshift(onerror);
  else
    dest._events.error = [onerror, dest._events.error];



  // Both close and finish should trigger unpipe, but only once.
  function onclose() {
    dest.removeListener('finish', onfinish);
    unpipe();
  }
  dest.once('close', onclose);
  function onfinish() {
    dest.removeListener('close', onclose);
    unpipe();
  }
  dest.once('finish', onfinish);

  function unpipe() {
    src.unpipe(dest);
  }

  // tell the dest that it's being piped to
  dest.emit('pipe', src);

  // start the flow if it hasn't been started already.
  if (!state.flowing) {
    // the handler that waits for readable events after all
    // the data gets sucked out in flow.
    // This would be easier to follow with a .once() handler
    // in flow(), but that is too slow.
    this.on('readable', pipeOnReadable);

    state.flowing = true;
    process.nextTick(function() {
      flow(src);
    });
  }

  return dest;
}
```
- example usage
```shell
...
'''js
var streamqueue = require('streamqueue');

var queue = streamqueue(
  Fs.createReadStream('input.txt'),
  Fs.createReadStream('input2.txt'),
  Fs.createReadStream('input3.txt')
).pipe(process.stdout);
'''
StreamQueue also accept functions returning streams, the above can be written
 like this, doing system calls only when piping:
'''js
var streamqueue = require('streamqueue');

var queue = streamqueue(
...
```

#### <a name="apidoc.element.streamqueue.super_.prototype.push"></a>[function <span class="apidocSignatureSpan">streamqueue.super_.prototype.</span>push (chunk, encoding)](#apidoc.element.streamqueue.super_.prototype.push)
- description and source-code
```javascript
push = function (chunk, encoding) {
  var state = this._readableState;

  if (typeof chunk === 'string' && !state.objectMode) {
    encoding = encoding || state.defaultEncoding;
    if (encoding !== state.encoding) {
      chunk = new Buffer(chunk, encoding);
      encoding = '';
    }
  }

  return readableAddChunk(this, state, chunk, encoding, false);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.streamqueue.super_.prototype.read"></a>[function <span class="apidocSignatureSpan">streamqueue.super_.prototype.</span>read (n)](#apidoc.element.streamqueue.super_.prototype.read)
- description and source-code
```javascript
read = function (n) {
  var state = this._readableState;
  state.calledRead = true;
  var nOrig = n;
  var ret;

  if (typeof n !== 'number' || n > 0)
    state.emittedReadable = false;

  // if we're doing read(0) to trigger a readable event, but we
  // already have a bunch of data in the buffer, then just trigger
  // the 'readable' event and move on.
  if (n === 0 &&
      state.needReadable &&
      (state.length >= state.highWaterMark || state.ended)) {
    emitReadable(this);
    return null;
  }

  n = howMuchToRead(n, state);

  // if we've ended, and we're now clear, then finish it up.
  if (n === 0 && state.ended) {
    ret = null;

    // In cases where the decoder did not receive enough data
    // to produce a full chunk, then immediately received an
    // EOF, state.buffer will contain [<Buffer >, <Buffer 00 ...>].
    // howMuchToRead will see this and coerce the amount to
    // read to zero (because it's looking at the length of the
    // first <Buffer > in state.buffer), and we'll end up here.
    //
    // This can only happen via state.decoder -- no other venue
    // exists for pushing a zero-length chunk into state.buffer
    // and triggering this behavior. In this case, we return our
    // remaining data and end the stream, if appropriate.
    if (state.length > 0 && state.decoder) {
      ret = fromList(n, state);
      state.length -= ret.length;
    }

    if (state.length === 0)
      endReadable(this);

    return ret;
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

  // if we currently have less than the highWaterMark, then also read some
  if (state.length - n <= state.highWaterMark)
    doRead = true;

  // however, if we've ended, then there's no point, and if we're already
  // reading, then it's unnecessary.
  if (state.ended || state.reading)
    doRead = false;

  if (doRead) {
    state.reading = true;
    state.sync = true;
    // if the length is currently zero, then we *need* a readable event.
    if (state.length === 0)
      state.needReadable = true;
    // call internal read method
    this._read(state.highWaterMark);
    state.sync = false;
  }

  // If _read called its callback synchronously, then 'reading'
  // will be false, and we need to re-evaluate how much data we
  // can return to the user.
  if (doRead && !state.reading)
    n = howMuchToRead(nOrig, state);

  if (n > 0)
    ret = fromList(n, state);
  else
    ret = null;

  if (ret === null) {
    state.needReadable = true;
    n = 0;
  }

  state.length -= n;

  // If we have nothing in the buffer, then we want to know
  // as soon as we *do* get something into the buffer.
  if (state.length === 0 && !state.ended)
    state.needReadable = true;

  // If we happened to read() exactly the remaining amount in the
  // buffer, and the EOF has been seen at this point, then make sure
  // that we emit 'end' on the very next tick.
  if (state.ended && !state.endEmitted && state.length === 0)
    endReadable(this);

  return ret;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.streamqueue.super_.prototype.resume"></a>[function <span class="apidocSignatureSpan">streamqueue.super_.prototype.</span>resume ()](#apidoc.element.streamqueue.super_.prototype.resume)
- description and source-code
```javascript
resume = function () {
  emitDataEvents(this);
  this.read(0);
  this.emit('resume');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.streamqueue.super_.prototype.setEncoding"></a>[function <span class="apidocSignatureSpan">streamqueue.super_.prototype.</span>setEncoding (enc)](#apidoc.element.streamqueue.super_.prototype.setEncoding)
- description and source-code
```javascript
setEncoding = function (enc) {
  if (!StringDecoder)
    StringDecoder = require('string_decoder/').StringDecoder;
  this._readableState.decoder = new StringDecoder(enc);
  this._readableState.encoding = enc;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.streamqueue.super_.prototype.unpipe"></a>[function <span class="apidocSignatureSpan">streamqueue.super_.prototype.</span>unpipe (dest)](#apidoc.element.streamqueue.super_.prototype.unpipe)
- description and source-code
```javascript
unpipe = function (dest) {
  var state = this._readableState;

  // if we're not piping anywhere, then do nothing.
  if (state.pipesCount === 0)
    return this;

  // just one destination.  most common case.
  if (state.pipesCount === 1) {
    // passed in one, but it's not the right one.
    if (dest && dest !== state.pipes)
      return this;

    if (!dest)
      dest = state.pipes;

    // got a match.
    state.pipes = null;
    state.pipesCount = 0;
    this.removeListener('readable', pipeOnReadable);
    state.flowing = false;
    if (dest)
      dest.emit('unpipe', this);
    return this;
  }

  // slow case. multiple pipe destinations.

  if (!dest) {
    // remove all.
    var dests = state.pipes;
    var len = state.pipesCount;
    state.pipes = null;
    state.pipesCount = 0;
    this.removeListener('readable', pipeOnReadable);
    state.flowing = false;

    for (var i = 0; i < len; i++)
      dests[i].emit('unpipe', this);
    return this;
  }

  // try to find the right one.
  var i = indexOf(state.pipes, dest);
  if (i === -1)
    return this;

  state.pipes.splice(i, 1);
  state.pipesCount -= 1;
  if (state.pipesCount === 1)
    state.pipes = state.pipes[0];

  dest.emit('unpipe', this);

  return this;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.streamqueue.super_.prototype.unshift"></a>[function <span class="apidocSignatureSpan">streamqueue.super_.prototype.</span>unshift (chunk)](#apidoc.element.streamqueue.super_.prototype.unshift)
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

#### <a name="apidoc.element.streamqueue.super_.prototype.wrap"></a>[function <span class="apidocSignatureSpan">streamqueue.super_.prototype.</span>wrap (stream)](#apidoc.element.streamqueue.super_.prototype.wrap)
- description and source-code
```javascript
wrap = function (stream) {
  var state = this._readableState;
  var paused = false;

  var self = this;
  stream.on('end', function() {
    if (state.decoder && !state.ended) {
      var chunk = state.decoder.end();
      if (chunk && chunk.length)
        self.push(chunk);
    }

    self.push(null);
  });

  stream.on('data', function(chunk) {
    if (state.decoder)
      chunk = state.decoder.write(chunk);

    // don't skip over falsy values in objectMode
    //if (state.objectMode && util.isNullOrUndefined(chunk))
    if (state.objectMode && (chunk === null || chunk === undefined))
      return;
    else if (!state.objectMode && (!chunk || !chunk.length))
      return;

    var ret = self.push(chunk);
    if (!ret) {
      paused = true;
      stream.pause();
    }
  });

  // proxy all the other methods.
  // important when wrapping filters and duplexes.
  for (var i in stream) {
    if (typeof stream[i] === 'function' &&
        typeof this[i] === 'undefined') {
      this[i] = function(method) { return function() {
        return stream[method].apply(stream, arguments);
      }}(i);
    }
  }

  // proxy certain important events.
  var events = ['error', 'close', 'destroy', 'pause', 'resume'];
  forEach(events, function(ev) {
    stream.on(ev, self.emit.bind(self, ev));
  });

  // when we try to consume some more bytes, simply unpause the
  // underlying stream.
  self._read = function(n) {
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
