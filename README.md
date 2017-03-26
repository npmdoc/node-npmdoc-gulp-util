# api documentation for  [gulp-util (v3.0.8)](https://github.com/gulpjs/gulp-util#readme)  [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-gulp-util.svg)](https://travis-ci.org/npmdoc/node-npmdoc-gulp-util)
#### Utility functions for gulp plugins

[![NPM](https://nodei.co/npm/gulp-util.png?downloads=true)](https://www.npmjs.com/package/gulp-util)

[![apidoc](https://npmdoc.github.io/node-npmdoc-gulp-util/build/screen-capture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-gulp-util_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-gulp-util/build..beta..travis-ci.org/apidoc.html)

![package-listing](https://npmdoc.github.io/node-npmdoc-gulp-util/build/screen-capture.npmPackageListing.svg)



# package.json

```json

{
    "author": {
        "name": "Fractal",
        "email": "contact@wearefractal.com",
        "url": "http://wearefractal.com/"
    },
    "bugs": {
        "url": "https://github.com/gulpjs/gulp-util/issues"
    },
    "dependencies": {
        "array-differ": "^1.0.0",
        "array-uniq": "^1.0.2",
        "beeper": "^1.0.0",
        "chalk": "^1.0.0",
        "dateformat": "^2.0.0",
        "fancy-log": "^1.1.0",
        "gulplog": "^1.0.0",
        "has-gulplog": "^0.1.0",
        "lodash._reescape": "^3.0.0",
        "lodash._reevaluate": "^3.0.0",
        "lodash._reinterpolate": "^3.0.0",
        "lodash.template": "^3.0.0",
        "minimist": "^1.1.0",
        "multipipe": "^0.1.2",
        "object-assign": "^3.0.0",
        "replace-ext": "0.0.1",
        "through2": "^2.0.0",
        "vinyl": "^0.5.0"
    },
    "description": "Utility functions for gulp plugins",
    "devDependencies": {
        "buffer-equal": "^0.0.1",
        "coveralls": "^2.11.2",
        "event-stream": "^3.1.7",
        "istanbul": "^0.3.5",
        "istanbul-coveralls": "^1.0.1",
        "jshint": "^2.5.11",
        "lodash.templatesettings": "^3.0.0",
        "mocha": "^2.0.1",
        "rimraf": "^2.2.8",
        "should": "^7.0.1"
    },
    "directories": {},
    "dist": {
        "shasum": "0054e1e744502e27c04c187c3ecc505dd54bbb4f",
        "tarball": "https://registry.npmjs.org/gulp-util/-/gulp-util-3.0.8.tgz"
    },
    "engines": {
        "node": ">=0.10"
    },
    "files": [
        "index.js",
        "lib"
    ],
    "gitHead": "28c2aa2a3f8782a995b47ed051ab52885c705024",
    "homepage": "https://github.com/gulpjs/gulp-util#readme",
    "license": "MIT",
    "maintainers": [
        {
            "name": "contra",
            "email": "contra@wearefractal.com"
        },
        {
            "name": "fractal",
            "email": "contact@wearefractal.com"
        },
        {
            "name": "phated",
            "email": "blaine.bublitz@gmail.com"
        }
    ],
    "name": "gulp-util",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/gulpjs/gulp-util.git"
    },
    "scripts": {
        "coveralls": "istanbul cover _mocha --report lcovonly && istanbul-coveralls",
        "test": "jshint *.js lib/*.js test/*.js && mocha"
    },
    "version": "3.0.8"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module gulp-util](#apidoc.module.gulp-util)
1.  [function <span class="apidocSignatureSpan">gulp-util.</span>File (file)](#apidoc.element.gulp-util.File)
1.  [function <span class="apidocSignatureSpan">gulp-util.</span>PluginError (plugin, message, opt)](#apidoc.element.gulp-util.PluginError)
1.  [function <span class="apidocSignatureSpan">gulp-util.</span>beep (val, cb)](#apidoc.element.gulp-util.beep)
1.  [function <span class="apidocSignatureSpan">gulp-util.</span>buffer (fn)](#apidoc.element.gulp-util.buffer)
1.  [function <span class="apidocSignatureSpan">gulp-util.</span>combine ()](#apidoc.element.gulp-util.combine)
1.  [function <span class="apidocSignatureSpan">gulp-util.</span>date (date, mask, utc, gmt)](#apidoc.element.gulp-util.date)
1.  [function <span class="apidocSignatureSpan">gulp-util.</span>isBuffer (o)](#apidoc.element.gulp-util.isBuffer)
1.  [function <span class="apidocSignatureSpan">gulp-util.</span>isNull (v)](#apidoc.element.gulp-util.isNull)
1.  [function <span class="apidocSignatureSpan">gulp-util.</span>isStream (o)](#apidoc.element.gulp-util.isStream)
1.  [function <span class="apidocSignatureSpan">gulp-util.</span>log ()](#apidoc.element.gulp-util.log)
1.  [function <span class="apidocSignatureSpan">gulp-util.</span>noop ()](#apidoc.element.gulp-util.noop)
1.  [function <span class="apidocSignatureSpan">gulp-util.</span>replaceExtension (npath, ext)](#apidoc.element.gulp-util.replaceExtension)
1.  [function <span class="apidocSignatureSpan">gulp-util.</span>template (tmpl, data)](#apidoc.element.gulp-util.template)
1.  object <span class="apidocSignatureSpan">gulp-util.</span>File.prototype
1.  object <span class="apidocSignatureSpan">gulp-util.</span>PluginError.prototype
1.  object <span class="apidocSignatureSpan">gulp-util.</span>colors
1.  object <span class="apidocSignatureSpan">gulp-util.</span>env
1.  string <span class="apidocSignatureSpan">gulp-util.</span>linefeed

#### [module gulp-util.File](#apidoc.module.gulp-util.File)
1.  [function <span class="apidocSignatureSpan">gulp-util.</span>File (file)](#apidoc.element.gulp-util.File.File)
1.  [function <span class="apidocSignatureSpan">gulp-util.File.</span>isVinyl (file)](#apidoc.element.gulp-util.File.isVinyl)

#### [module gulp-util.File.prototype](#apidoc.module.gulp-util.File.prototype)
1.  [function <span class="apidocSignatureSpan">gulp-util.File.prototype.</span>clone (opt)](#apidoc.element.gulp-util.File.prototype.clone)
1.  [function <span class="apidocSignatureSpan">gulp-util.File.prototype.</span>inspect ()](#apidoc.element.gulp-util.File.prototype.inspect)
1.  [function <span class="apidocSignatureSpan">gulp-util.File.prototype.</span>isBuffer ()](#apidoc.element.gulp-util.File.prototype.isBuffer)
1.  [function <span class="apidocSignatureSpan">gulp-util.File.prototype.</span>isDirectory ()](#apidoc.element.gulp-util.File.prototype.isDirectory)
1.  [function <span class="apidocSignatureSpan">gulp-util.File.prototype.</span>isNull ()](#apidoc.element.gulp-util.File.prototype.isNull)
1.  [function <span class="apidocSignatureSpan">gulp-util.File.prototype.</span>isStream ()](#apidoc.element.gulp-util.File.prototype.isStream)
1.  [function <span class="apidocSignatureSpan">gulp-util.File.prototype.</span>pipe (stream, opt)](#apidoc.element.gulp-util.File.prototype.pipe)

#### [module gulp-util.PluginError](#apidoc.module.gulp-util.PluginError)
1.  [function <span class="apidocSignatureSpan">gulp-util.</span>PluginError (plugin, message, opt)](#apidoc.element.gulp-util.PluginError.PluginError)
1.  [function <span class="apidocSignatureSpan">gulp-util.PluginError.</span>super_ ()](#apidoc.element.gulp-util.PluginError.super_)

#### [module gulp-util.PluginError.prototype](#apidoc.module.gulp-util.PluginError.prototype)
1.  [function <span class="apidocSignatureSpan">gulp-util.PluginError.prototype.</span>_messageDetails ()](#apidoc.element.gulp-util.PluginError.prototype._messageDetails)
1.  [function <span class="apidocSignatureSpan">gulp-util.PluginError.prototype.</span>_messageWithDetails ()](#apidoc.element.gulp-util.PluginError.prototype._messageWithDetails)
1.  [function <span class="apidocSignatureSpan">gulp-util.PluginError.prototype.</span>toString ()](#apidoc.element.gulp-util.PluginError.prototype.toString)

#### [module gulp-util.colors](#apidoc.module.gulp-util.colors)
1.  boolean <span class="apidocSignatureSpan">gulp-util.colors.</span>enabled
1.  boolean <span class="apidocSignatureSpan">gulp-util.colors.</span>supportsColor
1.  [function <span class="apidocSignatureSpan">gulp-util.colors.</span>hasColor ()](#apidoc.element.gulp-util.colors.hasColor)
1.  [function <span class="apidocSignatureSpan">gulp-util.colors.</span>stripColor (str)](#apidoc.element.gulp-util.colors.stripColor)
1.  object <span class="apidocSignatureSpan">gulp-util.colors.</span>styles



# <a name="apidoc.module.gulp-util"></a>[module gulp-util](#apidoc.module.gulp-util)

#### <a name="apidoc.element.gulp-util.File"></a>[function <span class="apidocSignatureSpan">gulp-util.</span>File (file)](#apidoc.element.gulp-util.File)
- description and source-code
```javascript
function File(file) {
  if (!file) file = {};

  // record path change
  var history = file.path ? [file.path] : file.history;
  this.history = history || [];

  this.cwd = file.cwd || process.cwd();
  this.base = file.base || this.cwd;

  // stat = files stats object
  this.stat = file.stat || null;

  // contents = stream, buffer, or null if not read
  this.contents = file.contents || null;

  this._isVinyl = true;
}
```
- example usage
```shell
...
This is a lodash.template function wrapper. You must pass in a valid gulp file object so it is available to the user or it will
error. You can not configure any of the delimiters. Look at the [lodash docs](http://lodash.com/docs#template) for more info.

## new File(obj)

This is just [vinyl](https://github.com/wearefractal/vinyl)

'''javascript
var file = new gutil.File({
  base: path.join(__dirname, './fixtures/'),
  cwd: __dirname,
  path: path.join(__dirname, './fixtures/test.coffee')
});
'''

## noop()
...
```

#### <a name="apidoc.element.gulp-util.PluginError"></a>[function <span class="apidocSignatureSpan">gulp-util.</span>PluginError (plugin, message, opt)](#apidoc.element.gulp-util.PluginError)
- description and source-code
```javascript
function PluginError(plugin, message, opt) {
  if (!(this instanceof PluginError)) throw new Error('Call PluginError using new');

  Error.call(this);

  var options = parseOptions(plugin, message, opt);
  var self = this;

  // if options has an error, grab details from it
  if (options.error) {
    // These properties are not enumerable, so we have to add them explicitly.
    arrayUniq(Object.keys(options.error).concat(nonEnumberableProperties))
      .forEach(function(prop) {
        self[prop] = options.error[prop];
      });
  }

  var properties = ['name', 'message', 'fileName', 'lineNumber', 'stack', 'showStack', 'showProperties', 'plugin'];

  // options object can override
  properties.forEach(function(prop) {
    if (prop in options) this[prop] = options[prop];
  }, this);

  // defaults
  if (!this.name) this.name = 'Error';

  if (!this.stack) {
    // Error.captureStackTrace appends a stack property which relies on the toString method of the object it is applied to.
    // Since we are using our own toString method which controls when to display the stack trace if we don't go through this
    // safety object, then we'll get stack overflow problems.
    var safety = {
      toString: function() {
        return this._messageWithDetails() + '\nStack:';
      }.bind(this)
    };
    Error.captureStackTrace(safety, arguments.callee || this.constructor);
    this.__safety = safety;
  }

  if (!this.plugin) throw new Error('Missing plugin name');
  if (!this.message) throw new Error('Missing error message');
}
```
- example usage
```shell
...
- If you pass an error in as the message the stack will be pulled from that, otherwise one will be created.
- Note that if you pass in a custom stack string you need to include the message along with that.
- Error properties will be included in 'err.toString()'. Can be omitted by including '{showProperties: false}' in the options.

These are all acceptable forms of instantiation:

'''javascript
var err = new gutil.PluginError('test', {
  message: 'something broke'
});

var err = new gutil.PluginError({
  plugin: 'test',
  message: 'something broke'
});
...
```

#### <a name="apidoc.element.gulp-util.beep"></a>[function <span class="apidocSignatureSpan">gulp-util.</span>beep (val, cb)](#apidoc.element.gulp-util.beep)
- description and source-code
```javascript
beep = function (val, cb) {
	if (!process.stdout.isTTY ||
		process.argv.indexOf('--no-beep') !== -1 ||
		process.argv.indexOf('--beep=false') !== -1) {
		return;
	}

	cb = cb || function () {};

	if (val === parseInt(val)) {
		if (val < 0) {
			throw new TypeError('Negative numbers are not accepted');
		}

		if (val === 0) {
			cb();
			return;
		}

		for (var i = 0; i < val; i++) {
			setTimeout(function (i) {
				beep();

				if (i === val - 1) {
					cb();
				}
			}, BEEP_DELAY * i, i);
		}
	} else if (!val) {
		beep();
		cb();
	} else if (typeof val === 'string') {
		melodicalBeep(val.split(''), cb);
	} else {
		throw new TypeError('Not an accepted type');
	}
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-util.buffer"></a>[function <span class="apidocSignatureSpan">gulp-util.</span>buffer (fn)](#apidoc.element.gulp-util.buffer)
- description and source-code
```javascript
buffer = function (fn) {
  var buf = [];
  var end = function(cb) {
    this.push(buf);
    cb();
    if(fn) fn(null, buf);
  };
  var push = function(data, enc, cb) {
    buf.push(data);
    cb();
  };
  return through.obj(push, end);
}
```
- example usage
```shell
...

The stream will emit one data event after the stream piped to it has ended. The data will be the same array passed to the callback
.

Callback is optional and receives two arguments: error and data

'''javascript
gulp.src('stuff/*.js')
  .pipe(gutil.buffer(function(err, files) {

  }));
'''

## new PluginError(pluginName, message[, options])

- pluginName should be the module name of your plugin
...
```

#### <a name="apidoc.element.gulp-util.combine"></a>[function <span class="apidocSignatureSpan">gulp-util.</span>combine ()](#apidoc.element.gulp-util.combine)
- description and source-code
```javascript
combine = function (){
  var args = arguments;
  if (args.length === 1 && Array.isArray(args[0])) {
    args = args[0];
  }
  return function(){
    return pipeline.apply(pipeline, args);
  };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-util.date"></a>[function <span class="apidocSignatureSpan">gulp-util.</span>date (date, mask, utc, gmt)](#apidoc.element.gulp-util.date)
- description and source-code
```javascript
date = function (date, mask, utc, gmt) {

      // You can't provide utc if you skip other args (use the 'UTC:' mask prefix)
      if (arguments.length === 1 && kindOf(date) === 'string' && !/\d/.test(date)) {
        mask = date;
        date = undefined;
      }

      date = date || new Date;

      if(!(date instanceof Date)) {
        date = new Date(date);
      }

      if (isNaN(date)) {
        throw TypeError('Invalid date');
      }

      mask = String(dateFormat.masks[mask] || mask || dateFormat.masks['default']);

      // Allow setting the utc/gmt argument via the mask
      var maskSlice = mask.slice(0, 4);
      if (maskSlice === 'UTC:' || maskSlice === 'GMT:') {
        mask = mask.slice(4);
        utc = true;
        if (maskSlice === 'GMT:') {
          gmt = true;
        }
      }

      var _ = utc ? 'getUTC' : 'get';
      var d = date[_ + 'Date']();
      var D = date[_ + 'Day']();
      var m = date[_ + 'Month']();
      var y = date[_ + 'FullYear']();
      var H = date[_ + 'Hours']();
      var M = date[_ + 'Minutes']();
      var s = date[_ + 'Seconds']();
      var L = date[_ + 'Milliseconds']();
      var o = utc ? 0 : date.getTimezoneOffset();
      var W = getWeek(date);
      var N = getDayOfWeek(date);
      var flags = {
        d:    d,
        dd:   pad(d),
        ddd:  dateFormat.i18n.dayNames[D],
        dddd: dateFormat.i18n.dayNames[D + 7],
        m:    m + 1,
        mm:   pad(m + 1),
        mmm:  dateFormat.i18n.monthNames[m],
        mmmm: dateFormat.i18n.monthNames[m + 12],
        yy:   String(y).slice(2),
        yyyy: y,
        h:    H % 12 || 12,
        hh:   pad(H % 12 || 12),
        H:    H,
        HH:   pad(H),
        M:    M,
        MM:   pad(M),
        s:    s,
        ss:   pad(s),
        l:    pad(L, 3),
        L:    pad(Math.round(L / 10)),
        t:    H < 12 ? 'a'  : 'p',
        tt:   H < 12 ? 'am' : 'pm',
        T:    H < 12 ? 'A'  : 'P',
        TT:   H < 12 ? 'AM' : 'PM',
        Z:    gmt ? 'GMT' : utc ? 'UTC' : (String(date).match(timezone) || ['']).pop().replace(timezoneClip, ''),
        o:    (o > 0 ? '-' : '+') + pad(Math.floor(Math.abs(o) / 60) * 100 + Math.abs(o) % 60, 4),
        S:    ['th', 'st', 'nd', 'rd'][d % 10 > 3 ? 0 : (d % 100 - d % 10 != 10) * d % 10],
        W:    W,
        N:    N
      };

      return mask.replace(token, function (match) {
        if (match in flags) {
          return flags[match];
        }
        return match.slice(1, match.length - 1);
      });
    }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-util.isBuffer"></a>[function <span class="apidocSignatureSpan">gulp-util.</span>isBuffer (o)](#apidoc.element.gulp-util.isBuffer)
- description and source-code
```javascript
isBuffer = function (o) {
  return typeof o === 'object' && o instanceof Buffer;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-util.isNull"></a>[function <span class="apidocSignatureSpan">gulp-util.</span>isNull (v)](#apidoc.element.gulp-util.isNull)
- description and source-code
```javascript
isNull = function (v) {
  return v === null;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-util.isStream"></a>[function <span class="apidocSignatureSpan">gulp-util.</span>isStream (o)](#apidoc.element.gulp-util.isStream)
- description and source-code
```javascript
isStream = function (o) {
  return !!o && o instanceof Stream;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-util.log"></a>[function <span class="apidocSignatureSpan">gulp-util.</span>log ()](#apidoc.element.gulp-util.log)
- description and source-code
```javascript
log = function (){
  if(hasGulplog()){
    // specifically deferring loading here to keep from registering it globally
    var gulplog = require('gulplog');
    gulplog.info.apply(gulplog, arguments);
  } else {
    // specifically defering loading because it might not be used
    var fancylog = require('fancy-log');
    fancylog.apply(null, arguments);
  }
  return this;
}
```
- example usage
```shell
...
</table>

## Usage

'''javascript
var gutil = require('gulp-util');

gutil.log('stuff happened', 'Really it did', gutil.colors.magenta('123'));

gutil.replaceExtension('file.coffee', '.js'); // file.js

var opt = {
  name: 'todd',
  file: someGulpFile
};
...
```

#### <a name="apidoc.element.gulp-util.noop"></a>[function <span class="apidocSignatureSpan">gulp-util.</span>noop ()](#apidoc.element.gulp-util.noop)
- description and source-code
```javascript
noop = function () {
  return through.obj();
}
```
- example usage
```shell
...

'''javascript
// gulp should be called like this :
// $ gulp --type production
gulp.task('scripts', function() {
  gulp.src('src/**/*.js')
    .pipe(concat('script.js'))
    .pipe(gutil.env.type === 'production' ? uglify() : gutil.noop())
    .pipe(gulp.dest('dist/'));
});
'''

## buffer(cb)

This is similar to es.wait but instead of buffering text into one string it buffers anything into an array (so very useful for file
 objects).
...
```

#### <a name="apidoc.element.gulp-util.replaceExtension"></a>[function <span class="apidocSignatureSpan">gulp-util.</span>replaceExtension (npath, ext)](#apidoc.element.gulp-util.replaceExtension)
- description and source-code
```javascript
replaceExtension = function (npath, ext) {
  if (typeof npath !== 'string') return npath;
  if (npath.length === 0) return npath;

  var nFileName = path.basename(npath, path.extname(npath))+ext;
  return path.join(path.dirname(npath), nFileName);
}
```
- example usage
```shell
...
## Usage

'''javascript
var gutil = require('gulp-util');

gutil.log('stuff happened', 'Really it did', gutil.colors.magenta('123'));

gutil.replaceExtension('file.coffee', '.js'); // file.js

var opt = {
  name: 'todd',
  file: someGulpFile
};
gutil.template('test <%= name %> <%= file.path %>', opt) // test todd /js/hi.js
'''
...
```

#### <a name="apidoc.element.gulp-util.template"></a>[function <span class="apidocSignatureSpan">gulp-util.</span>template (tmpl, data)](#apidoc.element.gulp-util.template)
- description and source-code
```javascript
template = function (tmpl, data) {
  var fn = template(tmpl, forcedSettings);

  var wrapped = function(o) {
    if (typeof o === 'undefined' || typeof o.file === 'undefined') {
      throw new Error('Failed to provide the current file as "file" to the template');
    }
    return fn(o);
  };

  return (data ? wrapped(data) : wrapped);
}
```
- example usage
```shell
...

gutil.replaceExtension('file.coffee', '.js'); // file.js

var opt = {
  name: 'todd',
  file: someGulpFile
};
gutil.template('test <%= name %> <%= file.path %>', opt) // test todd /js/hi.js
'''

### log(msg...)

Logs stuff. Already prefixed with [gulp] and all that. If you pass in multiple arguments it will join them by a space.

The default gulp coloring using gutil.colors.<color>:
...
```



# <a name="apidoc.module.gulp-util.File"></a>[module gulp-util.File](#apidoc.module.gulp-util.File)

#### <a name="apidoc.element.gulp-util.File.File"></a>[function <span class="apidocSignatureSpan">gulp-util.</span>File (file)](#apidoc.element.gulp-util.File.File)
- description and source-code
```javascript
function File(file) {
  if (!file) file = {};

  // record path change
  var history = file.path ? [file.path] : file.history;
  this.history = history || [];

  this.cwd = file.cwd || process.cwd();
  this.base = file.base || this.cwd;

  // stat = files stats object
  this.stat = file.stat || null;

  // contents = stream, buffer, or null if not read
  this.contents = file.contents || null;

  this._isVinyl = true;
}
```
- example usage
```shell
...
This is a lodash.template function wrapper. You must pass in a valid gulp file object so it is available to the user or it will
error. You can not configure any of the delimiters. Look at the [lodash docs](http://lodash.com/docs#template) for more info.

## new File(obj)

This is just [vinyl](https://github.com/wearefractal/vinyl)

'''javascript
var file = new gutil.File({
  base: path.join(__dirname, './fixtures/'),
  cwd: __dirname,
  path: path.join(__dirname, './fixtures/test.coffee')
});
'''

## noop()
...
```

#### <a name="apidoc.element.gulp-util.File.isVinyl"></a>[function <span class="apidocSignatureSpan">gulp-util.File.</span>isVinyl (file)](#apidoc.element.gulp-util.File.isVinyl)
- description and source-code
```javascript
isVinyl = function (file) {
  return file && file._isVinyl === true;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.gulp-util.File.prototype"></a>[module gulp-util.File.prototype](#apidoc.module.gulp-util.File.prototype)

#### <a name="apidoc.element.gulp-util.File.prototype.clone"></a>[function <span class="apidocSignatureSpan">gulp-util.File.prototype.</span>clone (opt)](#apidoc.element.gulp-util.File.prototype.clone)
- description and source-code
```javascript
clone = function (opt) {
  if (typeof opt === 'boolean') {
    opt = {
      deep: opt,
      contents: true
    };
  } else if (!opt) {
    opt = {
      deep: true,
      contents: true
    };
  } else {
    opt.deep = opt.deep === true;
    opt.contents = opt.contents !== false;
  }

  // clone our file contents
  var contents;
  if (this.isStream()) {
    contents = this.contents.pipe(new Stream.PassThrough());
    this.contents = this.contents.pipe(new Stream.PassThrough());
  } else if (this.isBuffer()) {
    contents = opt.contents ? cloneBuffer(this.contents) : this.contents;
  }

  var file = new File({
    cwd: this.cwd,
    base: this.base,
    stat: (this.stat ? cloneStats(this.stat) : null),
    history: this.history.slice(),
    contents: contents
  });

  // clone our custom properties
  Object.keys(this).forEach(function(key) {
    // ignore built-in fields
    if (key === '_contents' || key === 'stat' ||
      key === 'history' || key === 'path' ||
      key === 'base' || key === 'cwd') {
      return;
    }
    file[key] = opt.deep ? clone(this[key], true) : this[key];
  }, this);
  return file;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-util.File.prototype.inspect"></a>[function <span class="apidocSignatureSpan">gulp-util.File.prototype.</span>inspect ()](#apidoc.element.gulp-util.File.prototype.inspect)
- description and source-code
```javascript
inspect = function () {
  var inspect = [];

  // use relative path if possible
  var filePath = (this.base && this.path) ? this.relative : this.path;

  if (filePath) {
    inspect.push('"'+filePath+'"');
  }

  if (this.isBuffer()) {
    inspect.push(this.contents.inspect());
  }

  if (this.isStream()) {
    inspect.push(inspectStream(this.contents));
  }

  return '<File '+inspect.join(' ')+'>';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-util.File.prototype.isBuffer"></a>[function <span class="apidocSignatureSpan">gulp-util.File.prototype.</span>isBuffer ()](#apidoc.element.gulp-util.File.prototype.isBuffer)
- description and source-code
```javascript
isBuffer = function () {
  return isBuffer(this.contents);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-util.File.prototype.isDirectory"></a>[function <span class="apidocSignatureSpan">gulp-util.File.prototype.</span>isDirectory ()](#apidoc.element.gulp-util.File.prototype.isDirectory)
- description and source-code
```javascript
isDirectory = function () {
  return this.isNull() && this.stat && this.stat.isDirectory();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-util.File.prototype.isNull"></a>[function <span class="apidocSignatureSpan">gulp-util.File.prototype.</span>isNull ()](#apidoc.element.gulp-util.File.prototype.isNull)
- description and source-code
```javascript
isNull = function () {
  return isNull(this.contents);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-util.File.prototype.isStream"></a>[function <span class="apidocSignatureSpan">gulp-util.File.prototype.</span>isStream ()](#apidoc.element.gulp-util.File.prototype.isStream)
- description and source-code
```javascript
isStream = function () {
  return isStream(this.contents);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-util.File.prototype.pipe"></a>[function <span class="apidocSignatureSpan">gulp-util.File.prototype.</span>pipe (stream, opt)](#apidoc.element.gulp-util.File.prototype.pipe)
- description and source-code
```javascript
pipe = function (stream, opt) {
  if (!opt) opt = {};
  if (typeof opt.end === 'undefined') opt.end = true;

  if (this.isStream()) {
    return this.contents.pipe(stream, opt);
  }
  if (this.isBuffer()) {
    if (opt.end) {
      stream.end(this.contents);
    } else {
      stream.write(this.contents);
    }
    return stream;
  }

  // isNull
  if (opt.end) stream.end();
  return stream;
}
```
- example usage
```shell
...
Returns a stream that does nothing but pass data straight through.

'''javascript
// gulp should be called like this :
// $ gulp --type production
gulp.task('scripts', function() {
  gulp.src('src/**/*.js')
    .pipe(concat('script.js'))
    .pipe(gutil.env.type === 'production' ? uglify() : gutil.noop())
    .pipe(gulp.dest('dist/'));
});
'''

## buffer(cb)
...
```



# <a name="apidoc.module.gulp-util.PluginError"></a>[module gulp-util.PluginError](#apidoc.module.gulp-util.PluginError)

#### <a name="apidoc.element.gulp-util.PluginError.PluginError"></a>[function <span class="apidocSignatureSpan">gulp-util.</span>PluginError (plugin, message, opt)](#apidoc.element.gulp-util.PluginError.PluginError)
- description and source-code
```javascript
function PluginError(plugin, message, opt) {
  if (!(this instanceof PluginError)) throw new Error('Call PluginError using new');

  Error.call(this);

  var options = parseOptions(plugin, message, opt);
  var self = this;

  // if options has an error, grab details from it
  if (options.error) {
    // These properties are not enumerable, so we have to add them explicitly.
    arrayUniq(Object.keys(options.error).concat(nonEnumberableProperties))
      .forEach(function(prop) {
        self[prop] = options.error[prop];
      });
  }

  var properties = ['name', 'message', 'fileName', 'lineNumber', 'stack', 'showStack', 'showProperties', 'plugin'];

  // options object can override
  properties.forEach(function(prop) {
    if (prop in options) this[prop] = options[prop];
  }, this);

  // defaults
  if (!this.name) this.name = 'Error';

  if (!this.stack) {
    // Error.captureStackTrace appends a stack property which relies on the toString method of the object it is applied to.
    // Since we are using our own toString method which controls when to display the stack trace if we don't go through this
    // safety object, then we'll get stack overflow problems.
    var safety = {
      toString: function() {
        return this._messageWithDetails() + '\nStack:';
      }.bind(this)
    };
    Error.captureStackTrace(safety, arguments.callee || this.constructor);
    this.__safety = safety;
  }

  if (!this.plugin) throw new Error('Missing plugin name');
  if (!this.message) throw new Error('Missing error message');
}
```
- example usage
```shell
...
- If you pass an error in as the message the stack will be pulled from that, otherwise one will be created.
- Note that if you pass in a custom stack string you need to include the message along with that.
- Error properties will be included in 'err.toString()'. Can be omitted by including '{showProperties: false}' in the options.

These are all acceptable forms of instantiation:

'''javascript
var err = new gutil.PluginError('test', {
  message: 'something broke'
});

var err = new gutil.PluginError({
  plugin: 'test',
  message: 'something broke'
});
...
```

#### <a name="apidoc.element.gulp-util.PluginError.super_"></a>[function <span class="apidocSignatureSpan">gulp-util.PluginError.</span>super_ ()](#apidoc.element.gulp-util.PluginError.super_)
- description and source-code
```javascript
function Error() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.gulp-util.PluginError.prototype"></a>[module gulp-util.PluginError.prototype](#apidoc.module.gulp-util.PluginError.prototype)

#### <a name="apidoc.element.gulp-util.PluginError.prototype._messageDetails"></a>[function <span class="apidocSignatureSpan">gulp-util.PluginError.prototype.</span>_messageDetails ()](#apidoc.element.gulp-util.PluginError.prototype._messageDetails)
- description and source-code
```javascript
_messageDetails = function () {
  if (!this.showProperties) {
    return '';
  }

  var properties = arrayDiffer(Object.keys(this), propertiesNotToDisplay);

  if (properties.length === 0) {
    return '';
  }

  var self = this;
  properties = properties.map(function stringifyProperty(prop) {
    return '    ' + prop + ': ' + self[prop];
  });

  return 'Details:\n' + properties.join('\n');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-util.PluginError.prototype._messageWithDetails"></a>[function <span class="apidocSignatureSpan">gulp-util.PluginError.prototype.</span>_messageWithDetails ()](#apidoc.element.gulp-util.PluginError.prototype._messageWithDetails)
- description and source-code
```javascript
_messageWithDetails = function () {
  var messageWithDetails = 'Message:\n    ' + this.message;
  var details = this._messageDetails();

  if (details !== '') {
    messageWithDetails += '\n' + details;
  }

  return messageWithDetails;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-util.PluginError.prototype.toString"></a>[function <span class="apidocSignatureSpan">gulp-util.PluginError.prototype.</span>toString ()](#apidoc.element.gulp-util.PluginError.prototype.toString)
- description and source-code
```javascript
toString = function () {
  var sig = chalk.red(this.name) + ' in plugin \'' + chalk.cyan(this.plugin) + '\'';
  var detailsWithStack = function(stack) {
    return this._messageWithDetails() + '\nStack:\n' + stack;
  }.bind(this);

  var msg;
  if (this.showStack) {
    if (this.__safety) { // There is no wrapped error, use the stack captured in the PluginError ctor
      msg = this.__safety.stack;
    } else if (this._stack) {
      msg = detailsWithStack(this._stack);
    } else { // Stack from wrapped error
      msg = detailsWithStack(this.stack);
    }
  } else {
    msg = this._messageWithDetails();
  }

  return sig + '\n' + msg;
}
```
- example usage
```shell
...
## new PluginError(pluginName, message[, options])

- pluginName should be the module name of your plugin
- message can be a string or an existing error
- By default the stack will not be shown. Set 'options.showStack' to true if you think the stack is important for your error.
- If you pass an error in as the message the stack will be pulled from that, otherwise one will be created.
- Note that if you pass in a custom stack string you need to include the message along with that.
- Error properties will be included in 'err.toString()'. Can be omitted by including '{showProperties: false}' in the options.

These are all acceptable forms of instantiation:

'''javascript
var err = new gutil.PluginError('test', {
  message: 'something broke'
});
...
```



# <a name="apidoc.module.gulp-util.colors"></a>[module gulp-util.colors](#apidoc.module.gulp-util.colors)

#### <a name="apidoc.element.gulp-util.colors.hasColor"></a>[function <span class="apidocSignatureSpan">gulp-util.colors.</span>hasColor ()](#apidoc.element.gulp-util.colors.hasColor)
- description and source-code
```javascript
hasColor = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.gulp-util.colors.stripColor"></a>[function <span class="apidocSignatureSpan">gulp-util.colors.</span>stripColor (str)](#apidoc.element.gulp-util.colors.stripColor)
- description and source-code
```javascript
stripColor = function (str) {
	return typeof str === 'string' ? str.replace(ansiRegex, '') : str;
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
