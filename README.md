# api documentation for  [bson (v1.0.4)](https://github.com/mongodb/js-bson#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-bson.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-bson) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-bson.svg)](https://travis-ci.org/npmdoc/node-npmdoc-bson)
#### A bson parser for node.js and the browser

[![NPM](https://nodei.co/npm/bson.png?downloads=true)](https://www.npmjs.com/package/bson)

[![apidoc](https://npmdoc.github.io/node-npmdoc-bson/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-bson_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-bson/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-bson/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-bson/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Christian Amor Kvalheim",
        "email": "christkv@gmail.com"
    },
    "browser": "lib/bson/bson.js",
    "bugs": {
        "url": "https://github.com/mongodb/js-bson/issues"
    },
    "config": {
        "native": false
    },
    "contributors": [],
    "dependencies": {},
    "description": "A bson parser for node.js and the browser",
    "devDependencies": {
        "babel-core": "^6.14.0",
        "babel-loader": "^6.2.5",
        "babel-polyfill": "^6.13.0",
        "babel-preset-es2015": "^6.14.0",
        "babel-preset-stage-0": "^6.5.0",
        "babel-register": "^6.14.0",
        "benchmark": "1.0.0",
        "colors": "1.1.0",
        "nodeunit": "0.9.0",
        "webpack": "^1.13.2",
        "webpack-polyfills-plugin": "0.0.9"
    },
    "directories": {
        "lib": "./lib/bson"
    },
    "dist": {
        "shasum": "93c10d39eaa5b58415cbc4052f3e53e562b0b72c",
        "tarball": "https://registry.npmjs.org/bson/-/bson-1.0.4.tgz"
    },
    "engines": {
        "node": ">=0.6.19"
    },
    "files": [
        "lib",
        "index.js",
        "browser_build",
        "bower.json"
    ],
    "gitHead": "8dd35ca73c30a2bcab61615ccc5edd053aeb868b",
    "homepage": "https://github.com/mongodb/js-bson#readme",
    "keywords": [
        "mongodb",
        "bson",
        "parser"
    ],
    "license": "Apache-2.0",
    "main": "./index",
    "maintainers": [
        {
            "name": "octave",
            "email": "chinsay@gmail.com"
        },
        {
            "name": "christkv",
            "email": "christkv@gmail.com"
        }
    ],
    "name": "bson",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/mongodb/js-bson.git"
    },
    "scripts": {
        "build": "webpack --config ./webpack.dist.config.js",
        "test": "nodeunit ./test/node"
    },
    "version": "1.0.4"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module bson](#apidoc.module.bson)
1.  [function <span class="apidocSignatureSpan">bson.</span>BSON ()](#apidoc.element.bson.BSON)
1.  [function <span class="apidocSignatureSpan">bson.</span>BSONRegExp (pattern, options)](#apidoc.element.bson.BSONRegExp)
1.  [function <span class="apidocSignatureSpan">bson.</span>Binary (buffer, subType)](#apidoc.element.bson.Binary)
1.  [function <span class="apidocSignatureSpan">bson.</span>Code (code, scope)](#apidoc.element.bson.Code)
1.  [function <span class="apidocSignatureSpan">bson.</span>DBRef (namespace, oid, db)](#apidoc.element.bson.DBRef)
1.  [function <span class="apidocSignatureSpan">bson.</span>Decimal128 (bytes)](#apidoc.element.bson.Decimal128)
1.  [function <span class="apidocSignatureSpan">bson.</span>Double (value)](#apidoc.element.bson.Double)
1.  [function <span class="apidocSignatureSpan">bson.</span>Int32 (value)](#apidoc.element.bson.Int32)
1.  [function <span class="apidocSignatureSpan">bson.</span>Long (low, high)](#apidoc.element.bson.Long)
1.  [function <span class="apidocSignatureSpan">bson.</span>Map ()](#apidoc.element.bson.Map)
1.  [function <span class="apidocSignatureSpan">bson.</span>MaxKey ()](#apidoc.element.bson.MaxKey)
1.  [function <span class="apidocSignatureSpan">bson.</span>MinKey ()](#apidoc.element.bson.MinKey)
1.  [function <span class="apidocSignatureSpan">bson.</span>ObjectID (id)](#apidoc.element.bson.ObjectID)
1.  [function <span class="apidocSignatureSpan">bson.</span>ObjectId (id)](#apidoc.element.bson.ObjectId)
1.  [function <span class="apidocSignatureSpan">bson.</span>Symbol (value)](#apidoc.element.bson.Symbol)
1.  [function <span class="apidocSignatureSpan">bson.</span>Timestamp (low, high)](#apidoc.element.bson.Timestamp)
1.  number <span class="apidocSignatureSpan">bson.</span>BSON_BINARY_SUBTYPE_BYTE_ARRAY
1.  number <span class="apidocSignatureSpan">bson.</span>BSON_BINARY_SUBTYPE_DEFAULT
1.  number <span class="apidocSignatureSpan">bson.</span>BSON_BINARY_SUBTYPE_FUNCTION
1.  number <span class="apidocSignatureSpan">bson.</span>BSON_BINARY_SUBTYPE_MD5
1.  number <span class="apidocSignatureSpan">bson.</span>BSON_BINARY_SUBTYPE_USER_DEFINED
1.  number <span class="apidocSignatureSpan">bson.</span>BSON_BINARY_SUBTYPE_UUID
1.  number <span class="apidocSignatureSpan">bson.</span>BSON_DATA_ARRAY
1.  number <span class="apidocSignatureSpan">bson.</span>BSON_DATA_BINARY
1.  number <span class="apidocSignatureSpan">bson.</span>BSON_DATA_BOOLEAN
1.  number <span class="apidocSignatureSpan">bson.</span>BSON_DATA_CODE
1.  number <span class="apidocSignatureSpan">bson.</span>BSON_DATA_CODE_W_SCOPE
1.  number <span class="apidocSignatureSpan">bson.</span>BSON_DATA_DATE
1.  number <span class="apidocSignatureSpan">bson.</span>BSON_DATA_INT
1.  number <span class="apidocSignatureSpan">bson.</span>BSON_DATA_LONG
1.  number <span class="apidocSignatureSpan">bson.</span>BSON_DATA_MAX_KEY
1.  number <span class="apidocSignatureSpan">bson.</span>BSON_DATA_MIN_KEY
1.  number <span class="apidocSignatureSpan">bson.</span>BSON_DATA_NULL
1.  number <span class="apidocSignatureSpan">bson.</span>BSON_DATA_NUMBER
1.  number <span class="apidocSignatureSpan">bson.</span>BSON_DATA_OBJECT
1.  number <span class="apidocSignatureSpan">bson.</span>BSON_DATA_OID
1.  number <span class="apidocSignatureSpan">bson.</span>BSON_DATA_REGEXP
1.  number <span class="apidocSignatureSpan">bson.</span>BSON_DATA_STRING
1.  number <span class="apidocSignatureSpan">bson.</span>BSON_DATA_SYMBOL
1.  number <span class="apidocSignatureSpan">bson.</span>BSON_DATA_TIMESTAMP
1.  number <span class="apidocSignatureSpan">bson.</span>BSON_INT32_MAX
1.  number <span class="apidocSignatureSpan">bson.</span>BSON_INT32_MIN
1.  number <span class="apidocSignatureSpan">bson.</span>BSON_INT64_MAX
1.  number <span class="apidocSignatureSpan">bson.</span>BSON_INT64_MIN
1.  number <span class="apidocSignatureSpan">bson.</span>JS_INT_MAX
1.  number <span class="apidocSignatureSpan">bson.</span>JS_INT_MIN
1.  object <span class="apidocSignatureSpan">bson.</span>Binary.prototype
1.  object <span class="apidocSignatureSpan">bson.</span>Code.prototype
1.  object <span class="apidocSignatureSpan">bson.</span>DBRef.prototype
1.  object <span class="apidocSignatureSpan">bson.</span>Decimal128.prototype
1.  object <span class="apidocSignatureSpan">bson.</span>Double.prototype
1.  object <span class="apidocSignatureSpan">bson.</span>Int32.prototype
1.  object <span class="apidocSignatureSpan">bson.</span>Long.prototype
1.  object <span class="apidocSignatureSpan">bson.</span>ObjectID.prototype
1.  object <span class="apidocSignatureSpan">bson.</span>Symbol.prototype
1.  object <span class="apidocSignatureSpan">bson.</span>Timestamp.prototype

#### [module bson.BSONRegExp](#apidoc.module.bson.BSONRegExp)
1.  [function <span class="apidocSignatureSpan">bson.</span>BSONRegExp (pattern, options)](#apidoc.element.bson.BSONRegExp.BSONRegExp)

#### [module bson.Binary](#apidoc.module.bson.Binary)
1.  [function <span class="apidocSignatureSpan">bson.</span>Binary (buffer, subType)](#apidoc.element.bson.Binary.Binary)
1.  number <span class="apidocSignatureSpan">bson.Binary.</span>BUFFER_SIZE
1.  number <span class="apidocSignatureSpan">bson.Binary.</span>SUBTYPE_BYTE_ARRAY
1.  number <span class="apidocSignatureSpan">bson.Binary.</span>SUBTYPE_DEFAULT
1.  number <span class="apidocSignatureSpan">bson.Binary.</span>SUBTYPE_FUNCTION
1.  number <span class="apidocSignatureSpan">bson.Binary.</span>SUBTYPE_MD5
1.  number <span class="apidocSignatureSpan">bson.Binary.</span>SUBTYPE_USER_DEFINED
1.  number <span class="apidocSignatureSpan">bson.Binary.</span>SUBTYPE_UUID
1.  number <span class="apidocSignatureSpan">bson.Binary.</span>SUBTYPE_UUID_OLD

#### [module bson.Binary.prototype](#apidoc.module.bson.Binary.prototype)
1.  [function <span class="apidocSignatureSpan">bson.Binary.prototype.</span>length ()](#apidoc.element.bson.Binary.prototype.length)
1.  [function <span class="apidocSignatureSpan">bson.Binary.prototype.</span>put (byte_value)](#apidoc.element.bson.Binary.prototype.put)
1.  [function <span class="apidocSignatureSpan">bson.Binary.prototype.</span>read (position, length)](#apidoc.element.bson.Binary.prototype.read)
1.  [function <span class="apidocSignatureSpan">bson.Binary.prototype.</span>toJSON ()](#apidoc.element.bson.Binary.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">bson.Binary.prototype.</span>toString (format)](#apidoc.element.bson.Binary.prototype.toString)
1.  [function <span class="apidocSignatureSpan">bson.Binary.prototype.</span>value (asRaw)](#apidoc.element.bson.Binary.prototype.value)
1.  [function <span class="apidocSignatureSpan">bson.Binary.prototype.</span>write (string, offset)](#apidoc.element.bson.Binary.prototype.write)

#### [module bson.Code](#apidoc.module.bson.Code)
1.  [function <span class="apidocSignatureSpan">bson.</span>Code (code, scope)](#apidoc.element.bson.Code.Code)

#### [module bson.Code.prototype](#apidoc.module.bson.Code.prototype)
1.  [function <span class="apidocSignatureSpan">bson.Code.prototype.</span>toJSON ()](#apidoc.element.bson.Code.prototype.toJSON)

#### [module bson.DBRef](#apidoc.module.bson.DBRef)
1.  [function <span class="apidocSignatureSpan">bson.</span>DBRef (namespace, oid, db)](#apidoc.element.bson.DBRef.DBRef)

#### [module bson.DBRef.prototype](#apidoc.module.bson.DBRef.prototype)
1.  [function <span class="apidocSignatureSpan">bson.DBRef.prototype.</span>toJSON ()](#apidoc.element.bson.DBRef.prototype.toJSON)

#### [module bson.Decimal128](#apidoc.module.bson.Decimal128)
1.  [function <span class="apidocSignatureSpan">bson.</span>Decimal128 (bytes)](#apidoc.element.bson.Decimal128.Decimal128)
1.  [function <span class="apidocSignatureSpan">bson.Decimal128.</span>fromString (string)](#apidoc.element.bson.Decimal128.fromString)

#### [module bson.Decimal128.prototype](#apidoc.module.bson.Decimal128.prototype)
1.  [function <span class="apidocSignatureSpan">bson.Decimal128.prototype.</span>toJSON ()](#apidoc.element.bson.Decimal128.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">bson.Decimal128.prototype.</span>toString ()](#apidoc.element.bson.Decimal128.prototype.toString)

#### [module bson.Double](#apidoc.module.bson.Double)
1.  [function <span class="apidocSignatureSpan">bson.</span>Double (value)](#apidoc.element.bson.Double.Double)

#### [module bson.Double.prototype](#apidoc.module.bson.Double.prototype)
1.  [function <span class="apidocSignatureSpan">bson.Double.prototype.</span>toJSON ()](#apidoc.element.bson.Double.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">bson.Double.prototype.</span>valueOf ()](#apidoc.element.bson.Double.prototype.valueOf)

#### [module bson.Int32](#apidoc.module.bson.Int32)
1.  [function <span class="apidocSignatureSpan">bson.</span>Int32 (value)](#apidoc.element.bson.Int32.Int32)

#### [module bson.Int32.prototype](#apidoc.module.bson.Int32.prototype)
1.  [function <span class="apidocSignatureSpan">bson.Int32.prototype.</span>toJSON ()](#apidoc.element.bson.Int32.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">bson.Int32.prototype.</span>valueOf ()](#apidoc.element.bson.Int32.prototype.valueOf)

#### [module bson.Long](#apidoc.module.bson.Long)
1.  [function <span class="apidocSignatureSpan">bson.</span>Long (low, high)](#apidoc.element.bson.Long.Long)
1.  [function <span class="apidocSignatureSpan">bson.Long.</span>fromBits (lowBits, highBits)](#apidoc.element.bson.Long.fromBits)
1.  [function <span class="apidocSignatureSpan">bson.Long.</span>fromInt (value)](#apidoc.element.bson.Long.fromInt)
1.  [function <span class="apidocSignatureSpan">bson.Long.</span>fromNumber (value)](#apidoc.element.bson.Long.fromNumber)
1.  [function <span class="apidocSignatureSpan">bson.Long.</span>fromString (str, opt_radix)](#apidoc.element.bson.Long.fromString)
1.  number <span class="apidocSignatureSpan">bson.Long.</span>TWO_PWR_16_DBL_
1.  number <span class="apidocSignatureSpan">bson.Long.</span>TWO_PWR_24_DBL_
1.  number <span class="apidocSignatureSpan">bson.Long.</span>TWO_PWR_31_DBL_
1.  number <span class="apidocSignatureSpan">bson.Long.</span>TWO_PWR_32_DBL_
1.  number <span class="apidocSignatureSpan">bson.Long.</span>TWO_PWR_48_DBL_
1.  number <span class="apidocSignatureSpan">bson.Long.</span>TWO_PWR_63_DBL_
1.  number <span class="apidocSignatureSpan">bson.Long.</span>TWO_PWR_64_DBL_
1.  object <span class="apidocSignatureSpan">bson.Long.</span>INT_CACHE_
1.  object <span class="apidocSignatureSpan">bson.Long.</span>MAX_VALUE
1.  object <span class="apidocSignatureSpan">bson.Long.</span>MIN_VALUE
1.  object <span class="apidocSignatureSpan">bson.Long.</span>NEG_ONE
1.  object <span class="apidocSignatureSpan">bson.Long.</span>ONE
1.  object <span class="apidocSignatureSpan">bson.Long.</span>TWO_PWR_24_
1.  object <span class="apidocSignatureSpan">bson.Long.</span>ZERO

#### [module bson.Long.prototype](#apidoc.module.bson.Long.prototype)
1.  [function <span class="apidocSignatureSpan">bson.Long.prototype.</span>add (other)](#apidoc.element.bson.Long.prototype.add)
1.  [function <span class="apidocSignatureSpan">bson.Long.prototype.</span>and (other)](#apidoc.element.bson.Long.prototype.and)
1.  [function <span class="apidocSignatureSpan">bson.Long.prototype.</span>compare (other)](#apidoc.element.bson.Long.prototype.compare)
1.  [function <span class="apidocSignatureSpan">bson.Long.prototype.</span>div (other)](#apidoc.element.bson.Long.prototype.div)
1.  [function <span class="apidocSignatureSpan">bson.Long.prototype.</span>equals (other)](#apidoc.element.bson.Long.prototype.equals)
1.  [function <span class="apidocSignatureSpan">bson.Long.prototype.</span>getHighBits ()](#apidoc.element.bson.Long.prototype.getHighBits)
1.  [function <span class="apidocSignatureSpan">bson.Long.prototype.</span>getLowBits ()](#apidoc.element.bson.Long.prototype.getLowBits)
1.  [function <span class="apidocSignatureSpan">bson.Long.prototype.</span>getLowBitsUnsigned ()](#apidoc.element.bson.Long.prototype.getLowBitsUnsigned)
1.  [function <span class="apidocSignatureSpan">bson.Long.prototype.</span>getNumBitsAbs ()](#apidoc.element.bson.Long.prototype.getNumBitsAbs)
1.  [function <span class="apidocSignatureSpan">bson.Long.prototype.</span>greaterThan (other)](#apidoc.element.bson.Long.prototype.greaterThan)
1.  [function <span class="apidocSignatureSpan">bson.Long.prototype.</span>greaterThanOrEqual (other)](#apidoc.element.bson.Long.prototype.greaterThanOrEqual)
1.  [function <span class="apidocSignatureSpan">bson.Long.prototype.</span>isNegative ()](#apidoc.element.bson.Long.prototype.isNegative)
1.  [function <span class="apidocSignatureSpan">bson.Long.prototype.</span>isOdd ()](#apidoc.element.bson.Long.prototype.isOdd)
1.  [function <span class="apidocSignatureSpan">bson.Long.prototype.</span>isZero ()](#apidoc.element.bson.Long.prototype.isZero)
1.  [function <span class="apidocSignatureSpan">bson.Long.prototype.</span>lessThan (other)](#apidoc.element.bson.Long.prototype.lessThan)
1.  [function <span class="apidocSignatureSpan">bson.Long.prototype.</span>lessThanOrEqual (other)](#apidoc.element.bson.Long.prototype.lessThanOrEqual)
1.  [function <span class="apidocSignatureSpan">bson.Long.prototype.</span>modulo (other)](#apidoc.element.bson.Long.prototype.modulo)
1.  [function <span class="apidocSignatureSpan">bson.Long.prototype.</span>multiply (other)](#apidoc.element.bson.Long.prototype.multiply)
1.  [function <span class="apidocSignatureSpan">bson.Long.prototype.</span>negate ()](#apidoc.element.bson.Long.prototype.negate)
1.  [function <span class="apidocSignatureSpan">bson.Long.prototype.</span>not ()](#apidoc.element.bson.Long.prototype.not)
1.  [function <span class="apidocSignatureSpan">bson.Long.prototype.</span>notEquals (other)](#apidoc.element.bson.Long.prototype.notEquals)
1.  [function <span class="apidocSignatureSpan">bson.Long.prototype.</span>or (other)](#apidoc.element.bson.Long.prototype.or)
1.  [function <span class="apidocSignatureSpan">bson.Long.prototype.</span>shiftLeft (numBits)](#apidoc.element.bson.Long.prototype.shiftLeft)
1.  [function <span class="apidocSignatureSpan">bson.Long.prototype.</span>shiftRight (numBits)](#apidoc.element.bson.Long.prototype.shiftRight)
1.  [function <span class="apidocSignatureSpan">bson.Long.prototype.</span>shiftRightUnsigned (numBits)](#apidoc.element.bson.Long.prototype.shiftRightUnsigned)
1.  [function <span class="apidocSignatureSpan">bson.Long.prototype.</span>subtract (other)](#apidoc.element.bson.Long.prototype.subtract)
1.  [function <span class="apidocSignatureSpan">bson.Long.prototype.</span>toInt ()](#apidoc.element.bson.Long.prototype.toInt)
1.  [function <span class="apidocSignatureSpan">bson.Long.prototype.</span>toJSON ()](#apidoc.element.bson.Long.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">bson.Long.prototype.</span>toNumber ()](#apidoc.element.bson.Long.prototype.toNumber)
1.  [function <span class="apidocSignatureSpan">bson.Long.prototype.</span>toString (opt_radix)](#apidoc.element.bson.Long.prototype.toString)
1.  [function <span class="apidocSignatureSpan">bson.Long.prototype.</span>xor (other)](#apidoc.element.bson.Long.prototype.xor)

#### [module bson.Map](#apidoc.module.bson.Map)
1.  [function <span class="apidocSignatureSpan">bson.</span>Map ()](#apidoc.element.bson.Map.Map)

#### [module bson.MaxKey](#apidoc.module.bson.MaxKey)
1.  [function <span class="apidocSignatureSpan">bson.</span>MaxKey ()](#apidoc.element.bson.MaxKey.MaxKey)

#### [module bson.MinKey](#apidoc.module.bson.MinKey)
1.  [function <span class="apidocSignatureSpan">bson.</span>MinKey ()](#apidoc.element.bson.MinKey.MinKey)

#### [module bson.ObjectID](#apidoc.module.bson.ObjectID)
1.  [function <span class="apidocSignatureSpan">bson.</span>ObjectID (id)](#apidoc.element.bson.ObjectID.ObjectID)
1.  [function <span class="apidocSignatureSpan">bson.ObjectID.</span>ObjectId (id)](#apidoc.element.bson.ObjectID.ObjectId)
1.  [function <span class="apidocSignatureSpan">bson.ObjectID.</span>createFromHexString (string)](#apidoc.element.bson.ObjectID.createFromHexString)
1.  [function <span class="apidocSignatureSpan">bson.ObjectID.</span>createFromTime (time)](#apidoc.element.bson.ObjectID.createFromTime)
1.  [function <span class="apidocSignatureSpan">bson.ObjectID.</span>createPk ()](#apidoc.element.bson.ObjectID.createPk)
1.  [function <span class="apidocSignatureSpan">bson.ObjectID.</span>isValid (id)](#apidoc.element.bson.ObjectID.isValid)
1.  number <span class="apidocSignatureSpan">bson.ObjectID.</span>index

#### [module bson.ObjectID.prototype](#apidoc.module.bson.ObjectID.prototype)
1.  [function <span class="apidocSignatureSpan">bson.ObjectID.prototype.</span>equals (otherId)](#apidoc.element.bson.ObjectID.prototype.equals)
1.  [function <span class="apidocSignatureSpan">bson.ObjectID.prototype.</span>generate (time)](#apidoc.element.bson.ObjectID.prototype.generate)
1.  [function <span class="apidocSignatureSpan">bson.ObjectID.prototype.</span>getInc ()](#apidoc.element.bson.ObjectID.prototype.getInc)
1.  [function <span class="apidocSignatureSpan">bson.ObjectID.prototype.</span>getTimestamp ()](#apidoc.element.bson.ObjectID.prototype.getTimestamp)
1.  [function <span class="apidocSignatureSpan">bson.ObjectID.prototype.</span>get_inc ()](#apidoc.element.bson.ObjectID.prototype.get_inc)
1.  [function <span class="apidocSignatureSpan">bson.ObjectID.prototype.</span>inspect (format)](#apidoc.element.bson.ObjectID.prototype.inspect)
1.  [function <span class="apidocSignatureSpan">bson.ObjectID.prototype.</span>toHexString ()](#apidoc.element.bson.ObjectID.prototype.toHexString)
1.  [function <span class="apidocSignatureSpan">bson.ObjectID.prototype.</span>toJSON ()](#apidoc.element.bson.ObjectID.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">bson.ObjectID.prototype.</span>toString (format)](#apidoc.element.bson.ObjectID.prototype.toString)

#### [module bson.Symbol](#apidoc.module.bson.Symbol)
1.  [function <span class="apidocSignatureSpan">bson.</span>Symbol (value)](#apidoc.element.bson.Symbol.Symbol)

#### [module bson.Symbol.prototype](#apidoc.module.bson.Symbol.prototype)
1.  [function <span class="apidocSignatureSpan">bson.Symbol.prototype.</span>inspect ()](#apidoc.element.bson.Symbol.prototype.inspect)
1.  [function <span class="apidocSignatureSpan">bson.Symbol.prototype.</span>toJSON ()](#apidoc.element.bson.Symbol.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">bson.Symbol.prototype.</span>toString ()](#apidoc.element.bson.Symbol.prototype.toString)
1.  [function <span class="apidocSignatureSpan">bson.Symbol.prototype.</span>valueOf ()](#apidoc.element.bson.Symbol.prototype.valueOf)

#### [module bson.Timestamp](#apidoc.module.bson.Timestamp)
1.  [function <span class="apidocSignatureSpan">bson.</span>Timestamp (low, high)](#apidoc.element.bson.Timestamp.Timestamp)
1.  [function <span class="apidocSignatureSpan">bson.Timestamp.</span>fromBits (lowBits, highBits)](#apidoc.element.bson.Timestamp.fromBits)
1.  [function <span class="apidocSignatureSpan">bson.Timestamp.</span>fromInt (value)](#apidoc.element.bson.Timestamp.fromInt)
1.  [function <span class="apidocSignatureSpan">bson.Timestamp.</span>fromNumber (value)](#apidoc.element.bson.Timestamp.fromNumber)
1.  [function <span class="apidocSignatureSpan">bson.Timestamp.</span>fromString (str, opt_radix)](#apidoc.element.bson.Timestamp.fromString)
1.  number <span class="apidocSignatureSpan">bson.Timestamp.</span>TWO_PWR_16_DBL_
1.  number <span class="apidocSignatureSpan">bson.Timestamp.</span>TWO_PWR_24_DBL_
1.  number <span class="apidocSignatureSpan">bson.Timestamp.</span>TWO_PWR_31_DBL_
1.  number <span class="apidocSignatureSpan">bson.Timestamp.</span>TWO_PWR_32_DBL_
1.  number <span class="apidocSignatureSpan">bson.Timestamp.</span>TWO_PWR_48_DBL_
1.  number <span class="apidocSignatureSpan">bson.Timestamp.</span>TWO_PWR_63_DBL_
1.  number <span class="apidocSignatureSpan">bson.Timestamp.</span>TWO_PWR_64_DBL_
1.  object <span class="apidocSignatureSpan">bson.Timestamp.</span>INT_CACHE_
1.  object <span class="apidocSignatureSpan">bson.Timestamp.</span>MAX_VALUE
1.  object <span class="apidocSignatureSpan">bson.Timestamp.</span>MIN_VALUE
1.  object <span class="apidocSignatureSpan">bson.Timestamp.</span>NEG_ONE
1.  object <span class="apidocSignatureSpan">bson.Timestamp.</span>ONE
1.  object <span class="apidocSignatureSpan">bson.Timestamp.</span>TWO_PWR_24_
1.  object <span class="apidocSignatureSpan">bson.Timestamp.</span>ZERO

#### [module bson.Timestamp.prototype](#apidoc.module.bson.Timestamp.prototype)
1.  [function <span class="apidocSignatureSpan">bson.Timestamp.prototype.</span>add (other)](#apidoc.element.bson.Timestamp.prototype.add)
1.  [function <span class="apidocSignatureSpan">bson.Timestamp.prototype.</span>and (other)](#apidoc.element.bson.Timestamp.prototype.and)
1.  [function <span class="apidocSignatureSpan">bson.Timestamp.prototype.</span>compare (other)](#apidoc.element.bson.Timestamp.prototype.compare)
1.  [function <span class="apidocSignatureSpan">bson.Timestamp.prototype.</span>div (other)](#apidoc.element.bson.Timestamp.prototype.div)
1.  [function <span class="apidocSignatureSpan">bson.Timestamp.prototype.</span>equals (other)](#apidoc.element.bson.Timestamp.prototype.equals)
1.  [function <span class="apidocSignatureSpan">bson.Timestamp.prototype.</span>getHighBits ()](#apidoc.element.bson.Timestamp.prototype.getHighBits)
1.  [function <span class="apidocSignatureSpan">bson.Timestamp.prototype.</span>getLowBits ()](#apidoc.element.bson.Timestamp.prototype.getLowBits)
1.  [function <span class="apidocSignatureSpan">bson.Timestamp.prototype.</span>getLowBitsUnsigned ()](#apidoc.element.bson.Timestamp.prototype.getLowBitsUnsigned)
1.  [function <span class="apidocSignatureSpan">bson.Timestamp.prototype.</span>getNumBitsAbs ()](#apidoc.element.bson.Timestamp.prototype.getNumBitsAbs)
1.  [function <span class="apidocSignatureSpan">bson.Timestamp.prototype.</span>greaterThan (other)](#apidoc.element.bson.Timestamp.prototype.greaterThan)
1.  [function <span class="apidocSignatureSpan">bson.Timestamp.prototype.</span>greaterThanOrEqual (other)](#apidoc.element.bson.Timestamp.prototype.greaterThanOrEqual)
1.  [function <span class="apidocSignatureSpan">bson.Timestamp.prototype.</span>isNegative ()](#apidoc.element.bson.Timestamp.prototype.isNegative)
1.  [function <span class="apidocSignatureSpan">bson.Timestamp.prototype.</span>isOdd ()](#apidoc.element.bson.Timestamp.prototype.isOdd)
1.  [function <span class="apidocSignatureSpan">bson.Timestamp.prototype.</span>isZero ()](#apidoc.element.bson.Timestamp.prototype.isZero)
1.  [function <span class="apidocSignatureSpan">bson.Timestamp.prototype.</span>lessThan (other)](#apidoc.element.bson.Timestamp.prototype.lessThan)
1.  [function <span class="apidocSignatureSpan">bson.Timestamp.prototype.</span>lessThanOrEqual (other)](#apidoc.element.bson.Timestamp.prototype.lessThanOrEqual)
1.  [function <span class="apidocSignatureSpan">bson.Timestamp.prototype.</span>modulo (other)](#apidoc.element.bson.Timestamp.prototype.modulo)
1.  [function <span class="apidocSignatureSpan">bson.Timestamp.prototype.</span>multiply (other)](#apidoc.element.bson.Timestamp.prototype.multiply)
1.  [function <span class="apidocSignatureSpan">bson.Timestamp.prototype.</span>negate ()](#apidoc.element.bson.Timestamp.prototype.negate)
1.  [function <span class="apidocSignatureSpan">bson.Timestamp.prototype.</span>not ()](#apidoc.element.bson.Timestamp.prototype.not)
1.  [function <span class="apidocSignatureSpan">bson.Timestamp.prototype.</span>notEquals (other)](#apidoc.element.bson.Timestamp.prototype.notEquals)
1.  [function <span class="apidocSignatureSpan">bson.Timestamp.prototype.</span>or (other)](#apidoc.element.bson.Timestamp.prototype.or)
1.  [function <span class="apidocSignatureSpan">bson.Timestamp.prototype.</span>shiftLeft (numBits)](#apidoc.element.bson.Timestamp.prototype.shiftLeft)
1.  [function <span class="apidocSignatureSpan">bson.Timestamp.prototype.</span>shiftRight (numBits)](#apidoc.element.bson.Timestamp.prototype.shiftRight)
1.  [function <span class="apidocSignatureSpan">bson.Timestamp.prototype.</span>shiftRightUnsigned (numBits)](#apidoc.element.bson.Timestamp.prototype.shiftRightUnsigned)
1.  [function <span class="apidocSignatureSpan">bson.Timestamp.prototype.</span>subtract (other)](#apidoc.element.bson.Timestamp.prototype.subtract)
1.  [function <span class="apidocSignatureSpan">bson.Timestamp.prototype.</span>toInt ()](#apidoc.element.bson.Timestamp.prototype.toInt)
1.  [function <span class="apidocSignatureSpan">bson.Timestamp.prototype.</span>toJSON ()](#apidoc.element.bson.Timestamp.prototype.toJSON)
1.  [function <span class="apidocSignatureSpan">bson.Timestamp.prototype.</span>toNumber ()](#apidoc.element.bson.Timestamp.prototype.toNumber)
1.  [function <span class="apidocSignatureSpan">bson.Timestamp.prototype.</span>toString (opt_radix)](#apidoc.element.bson.Timestamp.prototype.toString)
1.  [function <span class="apidocSignatureSpan">bson.Timestamp.prototype.</span>xor (other)](#apidoc.element.bson.Timestamp.prototype.xor)



# <a name="apidoc.module.bson"></a>[module bson](#apidoc.module.bson)

#### <a name="apidoc.element.bson.BSON"></a>[function <span class="apidocSignatureSpan">bson.</span>BSON ()](#apidoc.element.bson.BSON)
- description and source-code
```javascript
BSON = function () {
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.BSONRegExp"></a>[function <span class="apidocSignatureSpan">bson.</span>BSONRegExp (pattern, options)](#apidoc.element.bson.BSONRegExp)
- description and source-code
```javascript
function BSONRegExp(pattern, options) {
  if(!(this instanceof BSONRegExp)) return new BSONRegExp();

  // Execute
  this._bsontype = 'BSONRegExp';
  this.pattern = pattern || '';
  this.options = options || '';

  // Validate options
  for(var i = 0; i < this.options.length; i++) {
    if(!(this.options[i] == 'i'
      || this.options[i] == 'm'
      || this.options[i] == 'x'
      || this.options[i] == 'l'
      || this.options[i] == 's'
      || this.options[i] == 'u'
    )) {
      throw new Error('the regular expression options [' + this.options[i] + "] is not supported");
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Binary"></a>[function <span class="apidocSignatureSpan">bson.</span>Binary (buffer, subType)](#apidoc.element.bson.Binary)
- description and source-code
```javascript
function Binary(buffer, subType) {
  if(!(this instanceof Binary)) return new Binary(buffer, subType);

  this._bsontype = 'Binary';

  if(buffer instanceof Number) {
    this.sub_type = buffer;
    this.position = 0;
  } else {
    this.sub_type = subType == null ? BSON_BINARY_SUBTYPE_DEFAULT : subType;
    this.position = 0;
  }

  if(buffer != null && !(buffer instanceof Number)) {
    // Only accept Buffer, Uint8Array or Arrays
    if(typeof buffer == 'string') {
      // Different ways of writing the length of the string for the different types
      if(typeof Buffer != 'undefined') {
        this.buffer = new Buffer(buffer);
      } else if(typeof Uint8Array != 'undefined' || (Object.prototype.toString.call(buffer) == '[object Array]')) {
        this.buffer = writeStringToArray(buffer);
      } else {
        throw new Error("only String, Buffer, Uint8Array or Array accepted");
      }
    } else {
      this.buffer = buffer;
    }
    this.position = buffer.length;
  } else {
    if(typeof Buffer != 'undefined') {
      this.buffer =  new Buffer(Binary.BUFFER_SIZE);
    } else if(typeof Uint8Array != 'undefined'){
      this.buffer = new Uint8Array(new ArrayBuffer(Binary.BUFFER_SIZE));
    } else {
      this.buffer = new Array(Binary.BUFFER_SIZE);
    }
    // Set position to start of buffer
    this.position = 0;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Code"></a>[function <span class="apidocSignatureSpan">bson.</span>Code (code, scope)](#apidoc.element.bson.Code)
- description and source-code
```javascript
function Code(code, scope) {
  if(!(this instanceof Code)) return new Code(code, scope);
  this._bsontype = 'Code';
  this.code = code;
  this.scope = scope;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.DBRef"></a>[function <span class="apidocSignatureSpan">bson.</span>DBRef (namespace, oid, db)](#apidoc.element.bson.DBRef)
- description and source-code
```javascript
function DBRef(namespace, oid, db) {
  if(!(this instanceof DBRef)) return new DBRef(namespace, oid, db);

  this._bsontype = 'DBRef';
  this.namespace = namespace;
  this.oid = oid;
  this.db = db;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Decimal128"></a>[function <span class="apidocSignatureSpan">bson.</span>Decimal128 (bytes)](#apidoc.element.bson.Decimal128)
- description and source-code
```javascript
Decimal128 = function (bytes) {
  this._bsontype = 'Decimal128';
  this.bytes = bytes;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Double"></a>[function <span class="apidocSignatureSpan">bson.</span>Double (value)](#apidoc.element.bson.Double)
- description and source-code
```javascript
function Double(value) {
  if(!(this instanceof Double)) return new Double(value);

  this._bsontype = 'Double';
  this.value = value;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Int32"></a>[function <span class="apidocSignatureSpan">bson.</span>Int32 (value)](#apidoc.element.bson.Int32)
- description and source-code
```javascript
Int32 = function (value) {
  if(!(this instanceof Int32)) return new Int32(value);

  this._bsontype = 'Int32';
  this.value = value;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Long"></a>[function <span class="apidocSignatureSpan">bson.</span>Long (low, high)](#apidoc.element.bson.Long)
- description and source-code
```javascript
function Long(low, high) {
  if(!(this instanceof Long)) return new Long(low, high);

  this._bsontype = 'Long';
<span class="apidocCodeCommentSpan">  /**
   * @type {number}
   * @ignore
   */
</span>  this.low_ = low | 0;  // force into 32 signed bits.

  /**
   * @type {number}
   * @ignore
   */
  this.high_ = high | 0;  // force into 32 signed bits.
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Map"></a>[function <span class="apidocSignatureSpan">bson.</span>Map ()](#apidoc.element.bson.Map)
- description and source-code
```javascript
function Map() { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.MaxKey"></a>[function <span class="apidocSignatureSpan">bson.</span>MaxKey ()](#apidoc.element.bson.MaxKey)
- description and source-code
```javascript
function MaxKey() {
  if(!(this instanceof MaxKey)) return new MaxKey();

  this._bsontype = 'MaxKey';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.MinKey"></a>[function <span class="apidocSignatureSpan">bson.</span>MinKey ()](#apidoc.element.bson.MinKey)
- description and source-code
```javascript
function MinKey() {
  if(!(this instanceof MinKey)) return new MinKey();

  this._bsontype = 'MinKey';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.ObjectID"></a>[function <span class="apidocSignatureSpan">bson.</span>ObjectID (id)](#apidoc.element.bson.ObjectID)
- description and source-code
```javascript
function ObjectID(id) {
  // Duck-typing to support ObjectId from different npm packages
  if(id instanceof ObjectID) return id;
  if(!(this instanceof ObjectID)) return new ObjectID(id);

  this._bsontype = 'ObjectID';

  // The most common usecase (blank id, new objectId instance)
  if(id == null || typeof id == 'number') {
    // Generate a new id
    this.id = this.generate(id);
    // If we are caching the hex string
    if(ObjectID.cacheHexString) this.__id = this.toString('hex');
    // Return the object
    return;
  }

  // Check if the passed in id is valid
  var valid = ObjectID.isValid(id);

  // Throw an error if it's not a valid setup
  if(!valid && id != null){
    throw new Error("Argument passed in must be a single String of 12 bytes or a string of 24 hex characters");
  } else if(valid && typeof id == 'string' && id.length == 24 && hasBufferType) {
    return new ObjectID(new Buffer(id, 'hex'));
  } else if(valid && typeof id == 'string' && id.length == 24) {
    return ObjectID.createFromHexString(id);
  } else if(id != null && id.length === 12) {
    // assume 12 byte string
    this.id = id;
  } else if(id != null && id.toHexString) {
    // Duck-typing to support ObjectId from different npm packages
    return id;
  } else {
    throw new Error("Argument passed in must be a single String of 12 bytes or a string of 24 hex characters");
  }

  if(ObjectID.cacheHexString) this.__id = this.toString('hex');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.ObjectId"></a>[function <span class="apidocSignatureSpan">bson.</span>ObjectId (id)](#apidoc.element.bson.ObjectId)
- description and source-code
```javascript
function ObjectID(id) {
  // Duck-typing to support ObjectId from different npm packages
  if(id instanceof ObjectID) return id;
  if(!(this instanceof ObjectID)) return new ObjectID(id);

  this._bsontype = 'ObjectID';

  // The most common usecase (blank id, new objectId instance)
  if(id == null || typeof id == 'number') {
    // Generate a new id
    this.id = this.generate(id);
    // If we are caching the hex string
    if(ObjectID.cacheHexString) this.__id = this.toString('hex');
    // Return the object
    return;
  }

  // Check if the passed in id is valid
  var valid = ObjectID.isValid(id);

  // Throw an error if it's not a valid setup
  if(!valid && id != null){
    throw new Error("Argument passed in must be a single String of 12 bytes or a string of 24 hex characters");
  } else if(valid && typeof id == 'string' && id.length == 24 && hasBufferType) {
    return new ObjectID(new Buffer(id, 'hex'));
  } else if(valid && typeof id == 'string' && id.length == 24) {
    return ObjectID.createFromHexString(id);
  } else if(id != null && id.length === 12) {
    // assume 12 byte string
    this.id = id;
  } else if(id != null && id.toHexString) {
    // Duck-typing to support ObjectId from different npm packages
    return id;
  } else {
    throw new Error("Argument passed in must be a single String of 12 bytes or a string of 24 hex characters");
  }

  if(ObjectID.cacheHexString) this.__id = this.toString('hex');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Symbol"></a>[function <span class="apidocSignatureSpan">bson.</span>Symbol (value)](#apidoc.element.bson.Symbol)
- description and source-code
```javascript
function Symbol(value) {
  if(!(this instanceof Symbol)) return new Symbol(value);
  this._bsontype = 'Symbol';
  this.value = value;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Timestamp"></a>[function <span class="apidocSignatureSpan">bson.</span>Timestamp (low, high)](#apidoc.element.bson.Timestamp)
- description and source-code
```javascript
function Timestamp(low, high) {
  if(!(this instanceof Timestamp)) return new Timestamp(low, high);
  this._bsontype = 'Timestamp';
<span class="apidocCodeCommentSpan">  /**
   * @type {number}
   * @ignore
   */
</span>  this.low_ = low | 0;  // force into 32 signed bits.

  /**
   * @type {number}
   * @ignore
   */
  this.high_ = high | 0;  // force into 32 signed bits.
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.bson.BSONRegExp"></a>[module bson.BSONRegExp](#apidoc.module.bson.BSONRegExp)

#### <a name="apidoc.element.bson.BSONRegExp.BSONRegExp"></a>[function <span class="apidocSignatureSpan">bson.</span>BSONRegExp (pattern, options)](#apidoc.element.bson.BSONRegExp.BSONRegExp)
- description and source-code
```javascript
function BSONRegExp(pattern, options) {
  if(!(this instanceof BSONRegExp)) return new BSONRegExp();

  // Execute
  this._bsontype = 'BSONRegExp';
  this.pattern = pattern || '';
  this.options = options || '';

  // Validate options
  for(var i = 0; i < this.options.length; i++) {
    if(!(this.options[i] == 'i'
      || this.options[i] == 'm'
      || this.options[i] == 'x'
      || this.options[i] == 'l'
      || this.options[i] == 's'
      || this.options[i] == 'u'
    )) {
      throw new Error('the regular expression options [' + this.options[i] + "] is not supported");
    }
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.bson.Binary"></a>[module bson.Binary](#apidoc.module.bson.Binary)

#### <a name="apidoc.element.bson.Binary.Binary"></a>[function <span class="apidocSignatureSpan">bson.</span>Binary (buffer, subType)](#apidoc.element.bson.Binary.Binary)
- description and source-code
```javascript
function Binary(buffer, subType) {
  if(!(this instanceof Binary)) return new Binary(buffer, subType);

  this._bsontype = 'Binary';

  if(buffer instanceof Number) {
    this.sub_type = buffer;
    this.position = 0;
  } else {
    this.sub_type = subType == null ? BSON_BINARY_SUBTYPE_DEFAULT : subType;
    this.position = 0;
  }

  if(buffer != null && !(buffer instanceof Number)) {
    // Only accept Buffer, Uint8Array or Arrays
    if(typeof buffer == 'string') {
      // Different ways of writing the length of the string for the different types
      if(typeof Buffer != 'undefined') {
        this.buffer = new Buffer(buffer);
      } else if(typeof Uint8Array != 'undefined' || (Object.prototype.toString.call(buffer) == '[object Array]')) {
        this.buffer = writeStringToArray(buffer);
      } else {
        throw new Error("only String, Buffer, Uint8Array or Array accepted");
      }
    } else {
      this.buffer = buffer;
    }
    this.position = buffer.length;
  } else {
    if(typeof Buffer != 'undefined') {
      this.buffer =  new Buffer(Binary.BUFFER_SIZE);
    } else if(typeof Uint8Array != 'undefined'){
      this.buffer = new Uint8Array(new ArrayBuffer(Binary.BUFFER_SIZE));
    } else {
      this.buffer = new Array(Binary.BUFFER_SIZE);
    }
    // Set position to start of buffer
    this.position = 0;
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.bson.Binary.prototype"></a>[module bson.Binary.prototype](#apidoc.module.bson.Binary.prototype)

#### <a name="apidoc.element.bson.Binary.prototype.length"></a>[function <span class="apidocSignatureSpan">bson.Binary.prototype.</span>length ()](#apidoc.element.bson.Binary.prototype.length)
- description and source-code
```javascript
function length() {
  return this.position;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Binary.prototype.put"></a>[function <span class="apidocSignatureSpan">bson.Binary.prototype.</span>put (byte_value)](#apidoc.element.bson.Binary.prototype.put)
- description and source-code
```javascript
function put(byte_value) {
  // If it's a string and a has more than one character throw an error
  if(byte_value['length'] != null && typeof byte_value != 'number' && byte_value.length != 1) throw new Error("only accepts single
 character String, Uint8Array or Array");
  if(typeof byte_value != 'number' && byte_value < 0 || byte_value > 255) throw new Error("only accepts number in a valid unsigned
 byte range 0-255");

  // Decode the byte value once
  var decoded_byte = null;
  if(typeof byte_value == 'string') {
    decoded_byte = byte_value.charCodeAt(0);
  } else if(byte_value['length'] != null) {
    decoded_byte = byte_value[0];
  } else {
    decoded_byte = byte_value;
  }

  if(this.buffer.length > this.position) {
    this.buffer[this.position++] = decoded_byte;
  } else {
    if(typeof Buffer != 'undefined' && Buffer.isBuffer(this.buffer)) {
      // Create additional overflow buffer
      var buffer = new Buffer(Binary.BUFFER_SIZE + this.buffer.length);
      // Combine the two buffers together
      this.buffer.copy(buffer, 0, 0, this.buffer.length);
      this.buffer = buffer;
      this.buffer[this.position++] = decoded_byte;
    } else {
      var buffer = null;
      // Create a new buffer (typed or normal array)
      if(Object.prototype.toString.call(this.buffer) == '[object Uint8Array]') {
        buffer = new Uint8Array(new ArrayBuffer(Binary.BUFFER_SIZE + this.buffer.length));
      } else {
        buffer = new Array(Binary.BUFFER_SIZE + this.buffer.length);
      }

      // We need to copy all the content to the new array
      for(var i = 0; i < this.buffer.length; i++) {
        buffer[i] = this.buffer[i];
      }

      // Reassign the buffer
      this.buffer = buffer;
      // Write the byte
      this.buffer[this.position++] = decoded_byte;
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Binary.prototype.read"></a>[function <span class="apidocSignatureSpan">bson.Binary.prototype.</span>read (position, length)](#apidoc.element.bson.Binary.prototype.read)
- description and source-code
```javascript
function read(position, length) {
  length = length && length > 0
    ? length
    : this.position;

  // Let's return the data based on the type we have
  if(this.buffer['slice']) {
    return this.buffer.slice(position, position + length);
  } else {
    // Create a buffer to keep the result
    var buffer = typeof Uint8Array != 'undefined' ? new Uint8Array(new ArrayBuffer(length)) : new Array(length);
    for(var i = 0; i < length; i++) {
      buffer[i] = this.buffer[position++];
    }
  }
  // Return the buffer
  return buffer;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Binary.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">bson.Binary.prototype.</span>toJSON ()](#apidoc.element.bson.Binary.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
  return this.buffer != null ? this.buffer.toString('base64') : '';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Binary.prototype.toString"></a>[function <span class="apidocSignatureSpan">bson.Binary.prototype.</span>toString (format)](#apidoc.element.bson.Binary.prototype.toString)
- description and source-code
```javascript
toString = function (format) {
  return this.buffer != null ? this.buffer.slice(0, this.position).toString(format) : '';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Binary.prototype.value"></a>[function <span class="apidocSignatureSpan">bson.Binary.prototype.</span>value (asRaw)](#apidoc.element.bson.Binary.prototype.value)
- description and source-code
```javascript
function value(asRaw) {
  asRaw = asRaw == null ? false : asRaw;

  // Optimize to serialize for the situation where the data == size of buffer
  if(asRaw && typeof Buffer != 'undefined' && Buffer.isBuffer(this.buffer) && this.buffer.length == this.position)
    return this.buffer;

  // If it's a node.js buffer object
  if(typeof Buffer != 'undefined' && Buffer.isBuffer(this.buffer)) {
    return asRaw ? this.buffer.slice(0, this.position) : this.buffer.toString('binary', 0, this.position);
  } else {
    if(asRaw) {
      // we support the slice command use it
      if(this.buffer['slice'] != null) {
        return this.buffer.slice(0, this.position);
      } else {
        // Create a new buffer to copy content to
        var newBuffer = Object.prototype.toString.call(this.buffer) == '[object Uint8Array]' ? new Uint8Array(new ArrayBuffer(this
.position)) : new Array(this.position);
        // Copy content
        for(var i = 0; i < this.position; i++) {
          newBuffer[i] = this.buffer[i];
        }
        // Return the buffer
        return newBuffer;
      }
    } else {
      return convertArraytoUtf8BinaryString(this.buffer, 0, this.position);
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Binary.prototype.write"></a>[function <span class="apidocSignatureSpan">bson.Binary.prototype.</span>write (string, offset)](#apidoc.element.bson.Binary.prototype.write)
- description and source-code
```javascript
function write(string, offset) {
  offset = typeof offset == 'number' ? offset : this.position;

  // If the buffer is to small let's extend the buffer
  if(this.buffer.length < offset + string.length) {
    var buffer = null;
    // If we are in node.js
    if(typeof Buffer != 'undefined' && Buffer.isBuffer(this.buffer)) {
      buffer = new Buffer(this.buffer.length + string.length);
      this.buffer.copy(buffer, 0, 0, this.buffer.length);
    } else if(Object.prototype.toString.call(this.buffer) == '[object Uint8Array]') {
      // Create a new buffer
      buffer = new Uint8Array(new ArrayBuffer(this.buffer.length + string.length))
      // Copy the content
      for(var i = 0; i < this.position; i++) {
        buffer[i] = this.buffer[i];
      }
    }

    // Assign the new buffer
    this.buffer = buffer;
  }

  if(typeof Buffer != 'undefined' && Buffer.isBuffer(string) && Buffer.isBuffer(this.buffer)) {
    string.copy(this.buffer, offset, 0, string.length);
    this.position = (offset + string.length) > this.position ? (offset + string.length) : this.position;
    // offset = string.length
  } else if(typeof Buffer != 'undefined' && typeof string == 'string' && Buffer.isBuffer(this.buffer)) {
    this.buffer.write(string, offset, 'binary');
    this.position = (offset + string.length) > this.position ? (offset + string.length) : this.position;
    // offset = string.length;
  } else if(Object.prototype.toString.call(string) == '[object Uint8Array]'
    || Object.prototype.toString.call(string) == '[object Array]' && typeof string != 'string') {
    for(var i = 0; i < string.length; i++) {
      this.buffer[offset++] = string[i];
    }

    this.position = offset > this.position ? offset : this.position;
  } else if(typeof string == 'string') {
    for(var i = 0; i < string.length; i++) {
      this.buffer[offset++] = string.charCodeAt(i);
    }

    this.position = offset > this.position ? offset : this.position;
  }
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.bson.Code"></a>[module bson.Code](#apidoc.module.bson.Code)

#### <a name="apidoc.element.bson.Code.Code"></a>[function <span class="apidocSignatureSpan">bson.</span>Code (code, scope)](#apidoc.element.bson.Code.Code)
- description and source-code
```javascript
function Code(code, scope) {
  if(!(this instanceof Code)) return new Code(code, scope);
  this._bsontype = 'Code';
  this.code = code;
  this.scope = scope;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.bson.Code.prototype"></a>[module bson.Code.prototype](#apidoc.module.bson.Code.prototype)

#### <a name="apidoc.element.bson.Code.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">bson.Code.prototype.</span>toJSON ()](#apidoc.element.bson.Code.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
  return {scope:this.scope, code:this.code};
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.bson.DBRef"></a>[module bson.DBRef](#apidoc.module.bson.DBRef)

#### <a name="apidoc.element.bson.DBRef.DBRef"></a>[function <span class="apidocSignatureSpan">bson.</span>DBRef (namespace, oid, db)](#apidoc.element.bson.DBRef.DBRef)
- description and source-code
```javascript
function DBRef(namespace, oid, db) {
  if(!(this instanceof DBRef)) return new DBRef(namespace, oid, db);

  this._bsontype = 'DBRef';
  this.namespace = namespace;
  this.oid = oid;
  this.db = db;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.bson.DBRef.prototype"></a>[module bson.DBRef.prototype](#apidoc.module.bson.DBRef.prototype)

#### <a name="apidoc.element.bson.DBRef.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">bson.DBRef.prototype.</span>toJSON ()](#apidoc.element.bson.DBRef.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
  return {
    '$ref':this.namespace,
    '$id':this.oid,
    '$db':this.db == null ? '' : this.db
  };
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.bson.Decimal128"></a>[module bson.Decimal128](#apidoc.module.bson.Decimal128)

#### <a name="apidoc.element.bson.Decimal128.Decimal128"></a>[function <span class="apidocSignatureSpan">bson.</span>Decimal128 (bytes)](#apidoc.element.bson.Decimal128.Decimal128)
- description and source-code
```javascript
Decimal128 = function (bytes) {
  this._bsontype = 'Decimal128';
  this.bytes = bytes;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Decimal128.fromString"></a>[function <span class="apidocSignatureSpan">bson.Decimal128.</span>fromString (string)](#apidoc.element.bson.Decimal128.fromString)
- description and source-code
```javascript
fromString = function (string) {
  // Parse state tracking
  var isNegative = false;
  var sawRadix = false;
  var foundNonZero = false;

  // Total number of significant digits (no leading or trailing zero)
  var significantDigits = 0;
  // Total number of significand digits read
  var nDigitsRead = 0;
  // Total number of digits (no leading zeros)
  var nDigits = 0;
  // The number of the digits after radix
  var radixPosition = 0;
  // The index of the first non-zero in *str*
  var firstNonZero = 0;

  // Digits Array
  var digits = [0];
  // The number of digits in digits
  var nDigitsStored = 0;
  // Insertion pointer for digits
  var digitsInsert = 0;
  // The index of the first non-zero digit
  var firstDigit = 0;
  // The index of the last digit
  var lastDigit = 0;

  // Exponent
  var exponent = 0;
  // loop index over array
  var i = 0;
  // The high 17 digits of the significand
  var significandHigh = [0, 0];
  // The low 17 digits of the significand
  var significandLow = [0, 0];
  // The biased exponent
  var biasedExponent = 0;

  // Read index
  var index = 0;

  // Trim the string
  string = string.trim();

  // Results
  var stringMatch = string.match(PARSE_STRING_REGEXP);
  var infMatch = string.match(PARSE_INF_REGEXP);
  var nanMatch = string.match(PARSE_NAN_REGEXP);

  // Validate the string
  if(!stringMatch
    && ! infMatch
    && ! nanMatch || string.length == 0) {
      throw new Error("" + string + " not a valid Decimal128 string");
  }

  // Check if we have an illegal exponent format
  if(stringMatch && stringMatch[4] && stringMatch[2] === undefined) {
    throw new Error("" + string + " not a valid Decimal128 string");
  }

  // Get the negative or positive sign
  if(string[index] == '+' || string[index] == '-') {
    isNegative = string[index++] == '-';
  }

  // Check if user passed Infinity or NaN
  if(!isDigit(string[index]) && string[index] != '.') {
    if(string[index] == 'i' || string[index] == 'I') {
      return new Decimal128(new Buffer(isNegative ? INF_NEGATIVE_BUFFER : INF_POSITIVE_BUFFER));
    } else if(string[index] == 'N') {
      return new Decimal128(new Buffer(NAN_BUFFER));
    }
  }

  // Read all the digits
  while(isDigit(string[index]) || string[index] == '.') {
    if(string[index] == '.') {
      if(sawRadix) {
        return new Decimal128(new Buffer(NAN_BUFFER));
      }

      sawRadix = true;
      index = index + 1;
      continue;
    }

    if(nDigitsStored < 34) {
      if(string[index] != '0' || foundNonZero) {
        if(!foundNonZero) {
          firstNonZero = nDigitsRead;
        }

        foundNonZero = true;

        // Only store 34 digits
        digits[digitsInsert++] = parseInt(string[index], 10);
        nDigitsStored = nDigitsStored + 1;
      }
    }

    if(foundNonZero) {
      nDigits = nDigits + 1;
    }

    if(sawRadix) {
      radixPosition = radixPosition + 1;
    }

    nDigitsRead = nDigitsRead + 1;
    index = index + 1;
  }

  if(sawRadix && !nDigitsRead) {
    throw new Error("" + string + " not a valid Decimal128 string");
  }

  // Read exponent if exists
  if(string[index] == 'e' || string[index] == 'E') {
    // Read exponent digits
    var match = string.substr(++index).match(EXPONENT_REGEX);

    // No digits read
    if(!match || !match[2]) {
      return new Decimal128(new Buffer(NAN_BUFFER));
    }

    // Get exponent
    exponent = parseInt(match[0], 10);

    // Adjust the index
    index = index + match[0].length;
  }

  // Return not a number
  if(string[index]) {
    return new Decimal128(new Buffer(NAN_BUFFER));
  }

  // Done reading input
  // Find first non-zero digit in digits
  firstDigit = 0;

  if(!nDigitsStored) {
    firstDigit = 0;
    lastDigit = 0;
    digits[0] = 0;
    nDigits = 1;
    nDigitsStored = 1;
    significantDigits = 0;
  } else {
    lastDigit = nDigitsStored - 1;
    significantDigits = nDigits;

    if(exponent != 0 && significantDigits != 1) {
      while(string[firstNonZero + significantDigits - 1] == '0') {
        significantDigits = significantDigits - 1;
      }
    }
  }

  // Normalization of ...
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.bson.Decimal128.prototype"></a>[module bson.Decimal128.prototype](#apidoc.module.bson.Decimal128.prototype)

#### <a name="apidoc.element.bson.Decimal128.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">bson.Decimal128.prototype.</span>toJSON ()](#apidoc.element.bson.Decimal128.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
  return { "$numberDecimal": this.toString() };
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Decimal128.prototype.toString"></a>[function <span class="apidocSignatureSpan">bson.Decimal128.prototype.</span>toString ()](#apidoc.element.bson.Decimal128.prototype.toString)
- description and source-code
```javascript
toString = function () {
  // Note: bits in this routine are referred to starting at 0,
  // from the sign bit, towards the coefficient.

  // bits 0 - 31
  var high;
  // bits 32 - 63
  var midh;
  // bits 64 - 95
  var midl;
  // bits 96 - 127
  var low;
  // bits 1 - 5
  var combination;
  // decoded biased exponent (14 bits)
  var biased_exponent;
  // the number of significand digits
  var significand_digits = 0;
  // the base-10 digits in the significand
  var significand = new Array(36);
  for(var i = 0; i < significand.length; i++) significand[i] = 0;
  // read pointer into significand
  var index = 0;

  // unbiased exponent
  var exponent;
  // the exponent if scientific notation is used
  var scientific_exponent;

  // true if the number is zero
  var is_zero = false;

  // the most signifcant significand bits (50-46)
  var significand_msb;
  // temporary storage for significand decoding
  var significand128 = {parts: new Array(4)};
  // indexing variables
  var i;
  var j, k;

  // Output string
  var string = [];

  // Unpack index
  var index = 0;

  // Buffer reference
  var buffer = this.bytes;

  // Unpack the low 64bits into a long
  low = buffer[index++] | buffer[index++] << 8 | buffer[index++] << 16 | buffer[index++] << 24;
  midl = buffer[index++] | buffer[index++] << 8 | buffer[index++] << 16 | buffer[index++] << 24;

  // Unpack the high 64bits into a long
  midh = buffer[index++] | buffer[index++] << 8 | buffer[index++] << 16 | buffer[index++] << 24;
  high = buffer[index++] | buffer[index++] << 8 | buffer[index++] << 16 | buffer[index++] << 24;

  // Unpack index
  var index = 0;

  // Create the state of the decimal
  var dec = {
    low: new Long(low, midl),
    high: new Long(midh, high) };

  if(dec.high.lessThan(Long.ZERO)) {
    string.push('-');
  }

  // Decode combination field and exponent
  combination = (high >> 26) & COMBINATION_MASK;

  if((combination >> 3) == 3) {
    // Check for 'special' values
    if(combination == COMBINATION_INFINITY) {
      return string.join('') + "Infinity";
    } else if(combination == COMBINATION_NAN) {
      return "NaN";
    } else {
      biased_exponent = (high >> 15) & EXPONENT_MASK;
      significand_msb = 0x08 + ((high >> 14) & 0x01);
    }
  } else {
    significand_msb = (high >> 14) & 0x07;
    biased_exponent = (high >> 17) & EXPONENT_MASK;
  }

  exponent = biased_exponent - EXPONENT_BIAS;

  // Create string of significand digits

  // Convert the 114-bit binary number represented by
  // (significand_high, significand_low) to at most 34 decimal
  // digits through modulo and division.
  significand128.parts[0] = (high & 0x3fff) + ((significand_msb & 0xf) << 14);
  significand128.parts[1] = midh;
  significand128.parts[2] = midl;
  significand128.parts[3] = low;

  if(significand128.parts[0] == 0 && significand128.parts[1] == 0
    && significand128.parts[2] == 0 && significand128.parts[3] == 0) {
      is_zero = true;
  } else {
    for(var k = 3; k >= 0; k--) {
      var least_digits = 0;
      // Peform the divide
      var result = divideu128(significand128);
      significand128 = result.quotient;
      least_digits = result.rem.low_;

      // We now have the 9 least significant digits (in base 2).
      // Convert and output to string.
      if(!least_digits) continue;

      for(var j = 8; j >= 0; j--) {
        // significand[k * 9 + j] = Math.round(least_digits % 10);
        significand[k * 9 + j] = least_digits % 10;
        // least_digits = Math.round(least_digits / 10);
        least_digits = Math.floor(least_digits / 10);
      }
    }
  }

  // Output format options:
  // Scientific - [-]d.dddE(+/-)dd or [-]dE(+/-)dd
  // Regular    - ddd.ddd

  if(is_zero) {
    significand_digits = 1;
    significand[index] = 0;
  } else {
    significand_digits = 36;
    var i = 0;

    while(!significand[index]) {
      i++;
      significand_digits = significand_digits - 1;
      index = index + 1;
    }
  }

  scientific_exponent = significand_digits - 1 + exponent;

  // The scientific exponent checks are dictated by the string conversion
  // ...
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.bson.Double"></a>[module bson.Double](#apidoc.module.bson.Double)

#### <a name="apidoc.element.bson.Double.Double"></a>[function <span class="apidocSignatureSpan">bson.</span>Double (value)](#apidoc.element.bson.Double.Double)
- description and source-code
```javascript
function Double(value) {
  if(!(this instanceof Double)) return new Double(value);

  this._bsontype = 'Double';
  this.value = value;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.bson.Double.prototype"></a>[module bson.Double.prototype](#apidoc.module.bson.Double.prototype)

#### <a name="apidoc.element.bson.Double.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">bson.Double.prototype.</span>toJSON ()](#apidoc.element.bson.Double.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
  return this.value;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Double.prototype.valueOf"></a>[function <span class="apidocSignatureSpan">bson.Double.prototype.</span>valueOf ()](#apidoc.element.bson.Double.prototype.valueOf)
- description and source-code
```javascript
valueOf = function () {
  return this.value;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.bson.Int32"></a>[module bson.Int32](#apidoc.module.bson.Int32)

#### <a name="apidoc.element.bson.Int32.Int32"></a>[function <span class="apidocSignatureSpan">bson.</span>Int32 (value)](#apidoc.element.bson.Int32.Int32)
- description and source-code
```javascript
Int32 = function (value) {
  if(!(this instanceof Int32)) return new Int32(value);

  this._bsontype = 'Int32';
  this.value = value;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.bson.Int32.prototype"></a>[module bson.Int32.prototype](#apidoc.module.bson.Int32.prototype)

#### <a name="apidoc.element.bson.Int32.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">bson.Int32.prototype.</span>toJSON ()](#apidoc.element.bson.Int32.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
  return this.value;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Int32.prototype.valueOf"></a>[function <span class="apidocSignatureSpan">bson.Int32.prototype.</span>valueOf ()](#apidoc.element.bson.Int32.prototype.valueOf)
- description and source-code
```javascript
valueOf = function () {
  return this.value;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.bson.Long"></a>[module bson.Long](#apidoc.module.bson.Long)

#### <a name="apidoc.element.bson.Long.Long"></a>[function <span class="apidocSignatureSpan">bson.</span>Long (low, high)](#apidoc.element.bson.Long.Long)
- description and source-code
```javascript
function Long(low, high) {
  if(!(this instanceof Long)) return new Long(low, high);

  this._bsontype = 'Long';
<span class="apidocCodeCommentSpan">  /**
   * @type {number}
   * @ignore
   */
</span>  this.low_ = low | 0;  // force into 32 signed bits.

  /**
   * @type {number}
   * @ignore
   */
  this.high_ = high | 0;  // force into 32 signed bits.
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Long.fromBits"></a>[function <span class="apidocSignatureSpan">bson.Long.</span>fromBits (lowBits, highBits)](#apidoc.element.bson.Long.fromBits)
- description and source-code
```javascript
fromBits = function (lowBits, highBits) {
  return new Long(lowBits, highBits);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Long.fromInt"></a>[function <span class="apidocSignatureSpan">bson.Long.</span>fromInt (value)](#apidoc.element.bson.Long.fromInt)
- description and source-code
```javascript
fromInt = function (value) {
  if (-128 <= value && value < 128) {
    var cachedObj = Long.INT_CACHE_[value];
    if (cachedObj) {
      return cachedObj;
    }
  }

  var obj = new Long(value | 0, value < 0 ? -1 : 0);
  if (-128 <= value && value < 128) {
    Long.INT_CACHE_[value] = obj;
  }
  return obj;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Long.fromNumber"></a>[function <span class="apidocSignatureSpan">bson.Long.</span>fromNumber (value)](#apidoc.element.bson.Long.fromNumber)
- description and source-code
```javascript
fromNumber = function (value) {
  if (isNaN(value) || !isFinite(value)) {
    return Long.ZERO;
  } else if (value <= -Long.TWO_PWR_63_DBL_) {
    return Long.MIN_VALUE;
  } else if (value + 1 >= Long.TWO_PWR_63_DBL_) {
    return Long.MAX_VALUE;
  } else if (value < 0) {
    return Long.fromNumber(-value).negate();
  } else {
    return new Long(
               (value % Long.TWO_PWR_32_DBL_) | 0,
               (value / Long.TWO_PWR_32_DBL_) | 0);
  }
}
```
- example usage
```shell
...
  function start() {
    // Get the Long type
    var Long = BSON.Long;
    // Create a bson parser instance
    var bson = new BSON();

    // Serialize document
    var doc = { long: Long.fromNumber(100) }

    // Serialize a document
    var data = bson.serialize(doc)
    // De serialize it again
    var doc_2 = bson.deserialize(data)
  }
</script>
...
```

#### <a name="apidoc.element.bson.Long.fromString"></a>[function <span class="apidocSignatureSpan">bson.Long.</span>fromString (str, opt_radix)](#apidoc.element.bson.Long.fromString)
- description and source-code
```javascript
fromString = function (str, opt_radix) {
  if (str.length == 0) {
    throw Error('number format error: empty string');
  }

  var radix = opt_radix || 10;
  if (radix < 2 || 36 < radix) {
    throw Error('radix out of range: ' + radix);
  }

  if (str.charAt(0) == '-') {
    return Long.fromString(str.substring(1), radix).negate();
  } else if (str.indexOf('-') >= 0) {
    throw Error('number format error: interior "-" character: ' + str);
  }

  // Do several (8) digits each time through the loop, so as to
  // minimize the calls to the very expensive emulated div.
  var radixToPower = Long.fromNumber(Math.pow(radix, 8));

  var result = Long.ZERO;
  for (var i = 0; i < str.length; i += 8) {
    var size = Math.min(8, str.length - i);
    var value = parseInt(str.substring(i, i + size), radix);
    if (size < 8) {
      var power = Long.fromNumber(Math.pow(radix, size));
      result = result.multiply(power).add(Long.fromNumber(value));
    } else {
      result = result.multiply(radixToPower);
      result = result.add(Long.fromNumber(value));
    }
  }
  return result;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.bson.Long.prototype"></a>[module bson.Long.prototype](#apidoc.module.bson.Long.prototype)

#### <a name="apidoc.element.bson.Long.prototype.add"></a>[function <span class="apidocSignatureSpan">bson.Long.prototype.</span>add (other)](#apidoc.element.bson.Long.prototype.add)
- description and source-code
```javascript
add = function (other) {
  // Divide each number into 4 chunks of 16 bits, and then sum the chunks.

  var a48 = this.high_ >>> 16;
  var a32 = this.high_ & 0xFFFF;
  var a16 = this.low_ >>> 16;
  var a00 = this.low_ & 0xFFFF;

  var b48 = other.high_ >>> 16;
  var b32 = other.high_ & 0xFFFF;
  var b16 = other.low_ >>> 16;
  var b00 = other.low_ & 0xFFFF;

  var c48 = 0, c32 = 0, c16 = 0, c00 = 0;
  c00 += a00 + b00;
  c16 += c00 >>> 16;
  c00 &= 0xFFFF;
  c16 += a16 + b16;
  c32 += c16 >>> 16;
  c16 &= 0xFFFF;
  c32 += a32 + b32;
  c48 += c32 >>> 16;
  c32 &= 0xFFFF;
  c48 += a48 + b48;
  c48 &= 0xFFFF;
  return Long.fromBits((c16 << 16) | c00, (c48 << 16) | c32);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Long.prototype.and"></a>[function <span class="apidocSignatureSpan">bson.Long.prototype.</span>and (other)](#apidoc.element.bson.Long.prototype.and)
- description and source-code
```javascript
and = function (other) {
  return Long.fromBits(this.low_ & other.low_, this.high_ & other.high_);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Long.prototype.compare"></a>[function <span class="apidocSignatureSpan">bson.Long.prototype.</span>compare (other)](#apidoc.element.bson.Long.prototype.compare)
- description and source-code
```javascript
compare = function (other) {
  if (this.equals(other)) {
    return 0;
  }

  var thisNeg = this.isNegative();
  var otherNeg = other.isNegative();
  if (thisNeg && !otherNeg) {
    return -1;
  }
  if (!thisNeg && otherNeg) {
    return 1;
  }

  // at this point, the signs are the same, so subtraction will not overflow
  if (this.subtract(other).isNegative()) {
    return -1;
  } else {
    return 1;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Long.prototype.div"></a>[function <span class="apidocSignatureSpan">bson.Long.prototype.</span>div (other)](#apidoc.element.bson.Long.prototype.div)
- description and source-code
```javascript
div = function (other) {
  if (other.isZero()) {
    throw Error('division by zero');
  } else if (this.isZero()) {
    return Long.ZERO;
  }

  if (this.equals(Long.MIN_VALUE)) {
    if (other.equals(Long.ONE) ||
        other.equals(Long.NEG_ONE)) {
      return Long.MIN_VALUE;  // recall that -MIN_VALUE == MIN_VALUE
    } else if (other.equals(Long.MIN_VALUE)) {
      return Long.ONE;
    } else {
      // At this point, we have |other| >= 2, so |this/other| < |MIN_VALUE|.
      var halfThis = this.shiftRight(1);
      var approx = halfThis.div(other).shiftLeft(1);
      if (approx.equals(Long.ZERO)) {
        return other.isNegative() ? Long.ONE : Long.NEG_ONE;
      } else {
        var rem = this.subtract(other.multiply(approx));
        var result = approx.add(rem.div(other));
        return result;
      }
    }
  } else if (other.equals(Long.MIN_VALUE)) {
    return Long.ZERO;
  }

  if (this.isNegative()) {
    if (other.isNegative()) {
      return this.negate().div(other.negate());
    } else {
      return this.negate().div(other).negate();
    }
  } else if (other.isNegative()) {
    return this.div(other.negate()).negate();
  }

  // Repeat the following until the remainder is less than other:  find a
  // floating-point that approximates remainder / other *from below*, add this
  // into the result, and subtract it from the remainder.  It is critical that
  // the approximate value is less than or equal to the real value so that the
  // remainder never becomes negative.
  var res = Long.ZERO;
  var rem = this;
  while (rem.greaterThanOrEqual(other)) {
    // Approximate the result of division. This may be a little greater or
    // smaller than the actual value.
    var approx = Math.max(1, Math.floor(rem.toNumber() / other.toNumber()));

    // We will tweak the approximate result by changing it in the 48-th digit or
    // the smallest non-fractional digit, whichever is larger.
    var log2 = Math.ceil(Math.log(approx) / Math.LN2);
    var delta = (log2 <= 48) ? 1 : Math.pow(2, log2 - 48);

    // Decrease the approximation until it is smaller than the remainder.  Note
    // that if it is too large, the product overflows and is negative.
    var approxRes = Long.fromNumber(approx);
    var approxRem = approxRes.multiply(other);
    while (approxRem.isNegative() || approxRem.greaterThan(rem)) {
      approx -= delta;
      approxRes = Long.fromNumber(approx);
      approxRem = approxRes.multiply(other);
    }

    // We know the answer can't be zero... and actually, zero would cause
    // infinite recursion since we would make no progress.
    if (approxRes.isZero()) {
      approxRes = Long.ONE;
    }

    res = res.add(approxRes);
    rem = rem.subtract(approxRem);
  }
  return res;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Long.prototype.equals"></a>[function <span class="apidocSignatureSpan">bson.Long.prototype.</span>equals (other)](#apidoc.element.bson.Long.prototype.equals)
- description and source-code
```javascript
equals = function (other) {
  return (this.high_ == other.high_) && (this.low_ == other.low_);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Long.prototype.getHighBits"></a>[function <span class="apidocSignatureSpan">bson.Long.prototype.</span>getHighBits ()](#apidoc.element.bson.Long.prototype.getHighBits)
- description and source-code
```javascript
getHighBits = function () {
  return this.high_;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Long.prototype.getLowBits"></a>[function <span class="apidocSignatureSpan">bson.Long.prototype.</span>getLowBits ()](#apidoc.element.bson.Long.prototype.getLowBits)
- description and source-code
```javascript
getLowBits = function () {
  return this.low_;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Long.prototype.getLowBitsUnsigned"></a>[function <span class="apidocSignatureSpan">bson.Long.prototype.</span>getLowBitsUnsigned ()](#apidoc.element.bson.Long.prototype.getLowBitsUnsigned)
- description and source-code
```javascript
getLowBitsUnsigned = function () {
  return (this.low_ >= 0) ?
      this.low_ : Long.TWO_PWR_32_DBL_ + this.low_;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Long.prototype.getNumBitsAbs"></a>[function <span class="apidocSignatureSpan">bson.Long.prototype.</span>getNumBitsAbs ()](#apidoc.element.bson.Long.prototype.getNumBitsAbs)
- description and source-code
```javascript
getNumBitsAbs = function () {
  if (this.isNegative()) {
    if (this.equals(Long.MIN_VALUE)) {
      return 64;
    } else {
      return this.negate().getNumBitsAbs();
    }
  } else {
    var val = this.high_ != 0 ? this.high_ : this.low_;
    for (var bit = 31; bit > 0; bit--) {
      if ((val & (1 << bit)) != 0) {
        break;
      }
    }
    return this.high_ != 0 ? bit + 33 : bit + 1;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Long.prototype.greaterThan"></a>[function <span class="apidocSignatureSpan">bson.Long.prototype.</span>greaterThan (other)](#apidoc.element.bson.Long.prototype.greaterThan)
- description and source-code
```javascript
greaterThan = function (other) {
  return this.compare(other) > 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Long.prototype.greaterThanOrEqual"></a>[function <span class="apidocSignatureSpan">bson.Long.prototype.</span>greaterThanOrEqual (other)](#apidoc.element.bson.Long.prototype.greaterThanOrEqual)
- description and source-code
```javascript
greaterThanOrEqual = function (other) {
  return this.compare(other) >= 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Long.prototype.isNegative"></a>[function <span class="apidocSignatureSpan">bson.Long.prototype.</span>isNegative ()](#apidoc.element.bson.Long.prototype.isNegative)
- description and source-code
```javascript
isNegative = function () {
  return this.high_ < 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Long.prototype.isOdd"></a>[function <span class="apidocSignatureSpan">bson.Long.prototype.</span>isOdd ()](#apidoc.element.bson.Long.prototype.isOdd)
- description and source-code
```javascript
isOdd = function () {
  return (this.low_ & 1) == 1;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Long.prototype.isZero"></a>[function <span class="apidocSignatureSpan">bson.Long.prototype.</span>isZero ()](#apidoc.element.bson.Long.prototype.isZero)
- description and source-code
```javascript
isZero = function () {
  return this.high_ == 0 && this.low_ == 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Long.prototype.lessThan"></a>[function <span class="apidocSignatureSpan">bson.Long.prototype.</span>lessThan (other)](#apidoc.element.bson.Long.prototype.lessThan)
- description and source-code
```javascript
lessThan = function (other) {
  return this.compare(other) < 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Long.prototype.lessThanOrEqual"></a>[function <span class="apidocSignatureSpan">bson.Long.prototype.</span>lessThanOrEqual (other)](#apidoc.element.bson.Long.prototype.lessThanOrEqual)
- description and source-code
```javascript
lessThanOrEqual = function (other) {
  return this.compare(other) <= 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Long.prototype.modulo"></a>[function <span class="apidocSignatureSpan">bson.Long.prototype.</span>modulo (other)](#apidoc.element.bson.Long.prototype.modulo)
- description and source-code
```javascript
modulo = function (other) {
  return this.subtract(this.div(other).multiply(other));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Long.prototype.multiply"></a>[function <span class="apidocSignatureSpan">bson.Long.prototype.</span>multiply (other)](#apidoc.element.bson.Long.prototype.multiply)
- description and source-code
```javascript
multiply = function (other) {
  if (this.isZero()) {
    return Long.ZERO;
  } else if (other.isZero()) {
    return Long.ZERO;
  }

  if (this.equals(Long.MIN_VALUE)) {
    return other.isOdd() ? Long.MIN_VALUE : Long.ZERO;
  } else if (other.equals(Long.MIN_VALUE)) {
    return this.isOdd() ? Long.MIN_VALUE : Long.ZERO;
  }

  if (this.isNegative()) {
    if (other.isNegative()) {
      return this.negate().multiply(other.negate());
    } else {
      return this.negate().multiply(other).negate();
    }
  } else if (other.isNegative()) {
    return this.multiply(other.negate()).negate();
  }

  // If both Longs are small, use float multiplication
  if (this.lessThan(Long.TWO_PWR_24_) &&
      other.lessThan(Long.TWO_PWR_24_)) {
    return Long.fromNumber(this.toNumber() * other.toNumber());
  }

  // Divide each Long into 4 chunks of 16 bits, and then add up 4x4 products.
  // We can skip products that would overflow.

  var a48 = this.high_ >>> 16;
  var a32 = this.high_ & 0xFFFF;
  var a16 = this.low_ >>> 16;
  var a00 = this.low_ & 0xFFFF;

  var b48 = other.high_ >>> 16;
  var b32 = other.high_ & 0xFFFF;
  var b16 = other.low_ >>> 16;
  var b00 = other.low_ & 0xFFFF;

  var c48 = 0, c32 = 0, c16 = 0, c00 = 0;
  c00 += a00 * b00;
  c16 += c00 >>> 16;
  c00 &= 0xFFFF;
  c16 += a16 * b00;
  c32 += c16 >>> 16;
  c16 &= 0xFFFF;
  c16 += a00 * b16;
  c32 += c16 >>> 16;
  c16 &= 0xFFFF;
  c32 += a32 * b00;
  c48 += c32 >>> 16;
  c32 &= 0xFFFF;
  c32 += a16 * b16;
  c48 += c32 >>> 16;
  c32 &= 0xFFFF;
  c32 += a00 * b32;
  c48 += c32 >>> 16;
  c32 &= 0xFFFF;
  c48 += a48 * b00 + a32 * b16 + a16 * b32 + a00 * b48;
  c48 &= 0xFFFF;
  return Long.fromBits((c16 << 16) | c00, (c48 << 16) | c32);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Long.prototype.negate"></a>[function <span class="apidocSignatureSpan">bson.Long.prototype.</span>negate ()](#apidoc.element.bson.Long.prototype.negate)
- description and source-code
```javascript
negate = function () {
  if (this.equals(Long.MIN_VALUE)) {
    return Long.MIN_VALUE;
  } else {
    return this.not().add(Long.ONE);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Long.prototype.not"></a>[function <span class="apidocSignatureSpan">bson.Long.prototype.</span>not ()](#apidoc.element.bson.Long.prototype.not)
- description and source-code
```javascript
not = function () {
  return Long.fromBits(~this.low_, ~this.high_);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Long.prototype.notEquals"></a>[function <span class="apidocSignatureSpan">bson.Long.prototype.</span>notEquals (other)](#apidoc.element.bson.Long.prototype.notEquals)
- description and source-code
```javascript
notEquals = function (other) {
  return (this.high_ != other.high_) || (this.low_ != other.low_);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Long.prototype.or"></a>[function <span class="apidocSignatureSpan">bson.Long.prototype.</span>or (other)](#apidoc.element.bson.Long.prototype.or)
- description and source-code
```javascript
or = function (other) {
  return Long.fromBits(this.low_ | other.low_, this.high_ | other.high_);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Long.prototype.shiftLeft"></a>[function <span class="apidocSignatureSpan">bson.Long.prototype.</span>shiftLeft (numBits)](#apidoc.element.bson.Long.prototype.shiftLeft)
- description and source-code
```javascript
shiftLeft = function (numBits) {
  numBits &= 63;
  if (numBits == 0) {
    return this;
  } else {
    var low = this.low_;
    if (numBits < 32) {
      var high = this.high_;
      return Long.fromBits(
                 low << numBits,
                 (high << numBits) | (low >>> (32 - numBits)));
    } else {
      return Long.fromBits(0, low << (numBits - 32));
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Long.prototype.shiftRight"></a>[function <span class="apidocSignatureSpan">bson.Long.prototype.</span>shiftRight (numBits)](#apidoc.element.bson.Long.prototype.shiftRight)
- description and source-code
```javascript
shiftRight = function (numBits) {
  numBits &= 63;
  if (numBits == 0) {
    return this;
  } else {
    var high = this.high_;
    if (numBits < 32) {
      var low = this.low_;
      return Long.fromBits(
                 (low >>> numBits) | (high << (32 - numBits)),
                 high >> numBits);
    } else {
      return Long.fromBits(
                 high >> (numBits - 32),
                 high >= 0 ? 0 : -1);
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Long.prototype.shiftRightUnsigned"></a>[function <span class="apidocSignatureSpan">bson.Long.prototype.</span>shiftRightUnsigned (numBits)](#apidoc.element.bson.Long.prototype.shiftRightUnsigned)
- description and source-code
```javascript
shiftRightUnsigned = function (numBits) {
  numBits &= 63;
  if (numBits == 0) {
    return this;
  } else {
    var high = this.high_;
    if (numBits < 32) {
      var low = this.low_;
      return Long.fromBits(
                 (low >>> numBits) | (high << (32 - numBits)),
                 high >>> numBits);
    } else if (numBits == 32) {
      return Long.fromBits(high, 0);
    } else {
      return Long.fromBits(high >>> (numBits - 32), 0);
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Long.prototype.subtract"></a>[function <span class="apidocSignatureSpan">bson.Long.prototype.</span>subtract (other)](#apidoc.element.bson.Long.prototype.subtract)
- description and source-code
```javascript
subtract = function (other) {
  return this.add(other.negate());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Long.prototype.toInt"></a>[function <span class="apidocSignatureSpan">bson.Long.prototype.</span>toInt ()](#apidoc.element.bson.Long.prototype.toInt)
- description and source-code
```javascript
toInt = function () {
  return this.low_;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Long.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">bson.Long.prototype.</span>toJSON ()](#apidoc.element.bson.Long.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
  return this.toString();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Long.prototype.toNumber"></a>[function <span class="apidocSignatureSpan">bson.Long.prototype.</span>toNumber ()](#apidoc.element.bson.Long.prototype.toNumber)
- description and source-code
```javascript
toNumber = function () {
  return this.high_ * Long.TWO_PWR_32_DBL_ +
         this.getLowBitsUnsigned();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Long.prototype.toString"></a>[function <span class="apidocSignatureSpan">bson.Long.prototype.</span>toString (opt_radix)](#apidoc.element.bson.Long.prototype.toString)
- description and source-code
```javascript
toString = function (opt_radix) {
  var radix = opt_radix || 10;
  if (radix < 2 || 36 < radix) {
    throw Error('radix out of range: ' + radix);
  }

  if (this.isZero()) {
    return '0';
  }

  if (this.isNegative()) {
    if (this.equals(Long.MIN_VALUE)) {
      // We need to change the Long value before it can be negated, so we remove
      // the bottom-most digit in this base and then recurse to do the rest.
      var radixLong = Long.fromNumber(radix);
      var div = this.div(radixLong);
      var rem = div.multiply(radixLong).subtract(this);
      return div.toString(radix) + rem.toInt().toString(radix);
    } else {
      return '-' + this.negate().toString(radix);
    }
  }

  // Do several (6) digits each time through the loop, so as to
  // minimize the calls to the very expensive emulated div.
  var radixToPower = Long.fromNumber(Math.pow(radix, 6));

  var rem = this;
  var result = '';
  while (true) {
    var remDiv = rem.div(radixToPower);
    var intval = rem.subtract(remDiv.multiply(radixToPower)).toInt();
    var digits = intval.toString(radix);

    rem = remDiv;
    if (rem.isZero()) {
      return digits + result;
    } else {
      while (digits.length < 6) {
        digits = '0' + digits;
      }
      result = '' + digits + result;
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Long.prototype.xor"></a>[function <span class="apidocSignatureSpan">bson.Long.prototype.</span>xor (other)](#apidoc.element.bson.Long.prototype.xor)
- description and source-code
```javascript
xor = function (other) {
  return Long.fromBits(this.low_ ^ other.low_, this.high_ ^ other.high_);
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.bson.Map"></a>[module bson.Map](#apidoc.module.bson.Map)

#### <a name="apidoc.element.bson.Map.Map"></a>[function <span class="apidocSignatureSpan">bson.</span>Map ()](#apidoc.element.bson.Map.Map)
- description and source-code
```javascript
function Map() { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.bson.MaxKey"></a>[module bson.MaxKey](#apidoc.module.bson.MaxKey)

#### <a name="apidoc.element.bson.MaxKey.MaxKey"></a>[function <span class="apidocSignatureSpan">bson.</span>MaxKey ()](#apidoc.element.bson.MaxKey.MaxKey)
- description and source-code
```javascript
function MaxKey() {
  if(!(this instanceof MaxKey)) return new MaxKey();

  this._bsontype = 'MaxKey';
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.bson.MinKey"></a>[module bson.MinKey](#apidoc.module.bson.MinKey)

#### <a name="apidoc.element.bson.MinKey.MinKey"></a>[function <span class="apidocSignatureSpan">bson.</span>MinKey ()](#apidoc.element.bson.MinKey.MinKey)
- description and source-code
```javascript
function MinKey() {
  if(!(this instanceof MinKey)) return new MinKey();

  this._bsontype = 'MinKey';
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.bson.ObjectID"></a>[module bson.ObjectID](#apidoc.module.bson.ObjectID)

#### <a name="apidoc.element.bson.ObjectID.ObjectID"></a>[function <span class="apidocSignatureSpan">bson.</span>ObjectID (id)](#apidoc.element.bson.ObjectID.ObjectID)
- description and source-code
```javascript
function ObjectID(id) {
  // Duck-typing to support ObjectId from different npm packages
  if(id instanceof ObjectID) return id;
  if(!(this instanceof ObjectID)) return new ObjectID(id);

  this._bsontype = 'ObjectID';

  // The most common usecase (blank id, new objectId instance)
  if(id == null || typeof id == 'number') {
    // Generate a new id
    this.id = this.generate(id);
    // If we are caching the hex string
    if(ObjectID.cacheHexString) this.__id = this.toString('hex');
    // Return the object
    return;
  }

  // Check if the passed in id is valid
  var valid = ObjectID.isValid(id);

  // Throw an error if it's not a valid setup
  if(!valid && id != null){
    throw new Error("Argument passed in must be a single String of 12 bytes or a string of 24 hex characters");
  } else if(valid && typeof id == 'string' && id.length == 24 && hasBufferType) {
    return new ObjectID(new Buffer(id, 'hex'));
  } else if(valid && typeof id == 'string' && id.length == 24) {
    return ObjectID.createFromHexString(id);
  } else if(id != null && id.length === 12) {
    // assume 12 byte string
    this.id = id;
  } else if(id != null && id.toHexString) {
    // Duck-typing to support ObjectId from different npm packages
    return id;
  } else {
    throw new Error("Argument passed in must be a single String of 12 bytes or a string of 24 hex characters");
  }

  if(ObjectID.cacheHexString) this.__id = this.toString('hex');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.ObjectID.ObjectId"></a>[function <span class="apidocSignatureSpan">bson.ObjectID.</span>ObjectId (id)](#apidoc.element.bson.ObjectID.ObjectId)
- description and source-code
```javascript
function ObjectID(id) {
  // Duck-typing to support ObjectId from different npm packages
  if(id instanceof ObjectID) return id;
  if(!(this instanceof ObjectID)) return new ObjectID(id);

  this._bsontype = 'ObjectID';

  // The most common usecase (blank id, new objectId instance)
  if(id == null || typeof id == 'number') {
    // Generate a new id
    this.id = this.generate(id);
    // If we are caching the hex string
    if(ObjectID.cacheHexString) this.__id = this.toString('hex');
    // Return the object
    return;
  }

  // Check if the passed in id is valid
  var valid = ObjectID.isValid(id);

  // Throw an error if it's not a valid setup
  if(!valid && id != null){
    throw new Error("Argument passed in must be a single String of 12 bytes or a string of 24 hex characters");
  } else if(valid && typeof id == 'string' && id.length == 24 && hasBufferType) {
    return new ObjectID(new Buffer(id, 'hex'));
  } else if(valid && typeof id == 'string' && id.length == 24) {
    return ObjectID.createFromHexString(id);
  } else if(id != null && id.length === 12) {
    // assume 12 byte string
    this.id = id;
  } else if(id != null && id.toHexString) {
    // Duck-typing to support ObjectId from different npm packages
    return id;
  } else {
    throw new Error("Argument passed in must be a single String of 12 bytes or a string of 24 hex characters");
  }

  if(ObjectID.cacheHexString) this.__id = this.toString('hex');
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.ObjectID.createFromHexString"></a>[function <span class="apidocSignatureSpan">bson.ObjectID.</span>createFromHexString (string)](#apidoc.element.bson.ObjectID.createFromHexString)
- description and source-code
```javascript
function createFromHexString(string) {
  // Throw an error if it's not a valid setup
  if(typeof string === 'undefined' || string != null && string.length != 24) {
    throw new Error("Argument passed in must be a single String of 12 bytes or a string of 24 hex characters");
  }

  // Use Buffer.from method if available
  if(hasBufferType) return new ObjectID(new Buffer(string, 'hex'));

  // Calculate lengths
  var array = new _Buffer(12);
  var n = 0;
  var i = 0;

  while (i < 24) {
    array[n++] = decodeLookup[string.charCodeAt(i++)] << 4 | decodeLookup[string.charCodeAt(i++)]
  }

  return new ObjectID(array);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.ObjectID.createFromTime"></a>[function <span class="apidocSignatureSpan">bson.ObjectID.</span>createFromTime (time)](#apidoc.element.bson.ObjectID.createFromTime)
- description and source-code
```javascript
function createFromTime(time) {
  var buffer = new Buffer([0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0, 0]);
  // Encode time into first 4 bytes
  buffer[3] = time & 0xff;
  buffer[2] = (time >> 8) & 0xff;
  buffer[1] = (time >> 16) & 0xff;
  buffer[0] = (time >> 24) & 0xff;
  // Return the new objectId
  return new ObjectID(buffer);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.ObjectID.createPk"></a>[function <span class="apidocSignatureSpan">bson.ObjectID.</span>createPk ()](#apidoc.element.bson.ObjectID.createPk)
- description and source-code
```javascript
function createPk() {
  return new ObjectID();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.ObjectID.isValid"></a>[function <span class="apidocSignatureSpan">bson.ObjectID.</span>isValid (id)](#apidoc.element.bson.ObjectID.isValid)
- description and source-code
```javascript
function isValid(id) {
  if(id == null) return false;

  if(typeof id == 'number') {
    return true;
  }

  if(typeof id == 'string') {
    return id.length == 12 || (id.length == 24 && checkForHexRegExp.test(id));
  }

  if(id instanceof ObjectID) {
    return true;
  }

  if(id instanceof _Buffer) {
    return true;
  }

  // Duck-Typing detection of ObjectId like objects
  if(id.toHexString) {
    return id.id.length == 12 || (id.id.length == 24 && checkForHexRegExp.test(id.id));
  }

  return false;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.bson.ObjectID.prototype"></a>[module bson.ObjectID.prototype](#apidoc.module.bson.ObjectID.prototype)

#### <a name="apidoc.element.bson.ObjectID.prototype.equals"></a>[function <span class="apidocSignatureSpan">bson.ObjectID.prototype.</span>equals (otherId)](#apidoc.element.bson.ObjectID.prototype.equals)
- description and source-code
```javascript
function equals(otherId) {
  var id;

  if(otherId instanceof ObjectID) {
    return this.toString() == otherId.toString();
  } else if(typeof otherId == 'string' && ObjectID.isValid(otherId) && otherId.length == 12 && this.id instanceof _Buffer) {
    return otherId === this.id.toString('binary');
  } else if(typeof otherId == 'string' && ObjectID.isValid(otherId) && otherId.length == 24) {
    return otherId.toLowerCase() === this.toHexString();
  } else if(typeof otherId == 'string' && ObjectID.isValid(otherId) && otherId.length == 12) {
    return otherId === this.id;
  } else if(otherId != null && (otherId instanceof ObjectID || otherId.toHexString)) {
    return otherId.toHexString() === this.toHexString();
  } else {
    return false;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.ObjectID.prototype.generate"></a>[function <span class="apidocSignatureSpan">bson.ObjectID.prototype.</span>generate (time)](#apidoc.element.bson.ObjectID.prototype.generate)
- description and source-code
```javascript
generate = function (time) {
  if ('number' != typeof time) {
    time = ~~(Date.now()/1000);
  }

  // Use pid
  var pid = (typeof process === 'undefined' ? Math.floor(Math.random() * 100000) : process.pid) % 0xFFFF;
  var inc = this.get_inc();
  // Buffer used
  var buffer = new Buffer(12);
  // Encode time
  buffer[3] = time & 0xff;
  buffer[2] = (time >> 8) & 0xff;
  buffer[1] = (time >> 16) & 0xff;
  buffer[0] = (time >> 24) & 0xff;
  // Encode machine
  buffer[6] = MACHINE_ID & 0xff;
  buffer[5] = (MACHINE_ID >> 8) & 0xff;
  buffer[4] = (MACHINE_ID >> 16) & 0xff;
  // Encode pid
  buffer[8] = pid & 0xff;
  buffer[7] = (pid >> 8) & 0xff;
  // Encode index
  buffer[11] = inc & 0xff;
  buffer[10] = (inc >> 8) & 0xff;
  buffer[9] = (inc >> 16) & 0xff;
  // Return the buffer
  return buffer;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.ObjectID.prototype.getInc"></a>[function <span class="apidocSignatureSpan">bson.ObjectID.prototype.</span>getInc ()](#apidoc.element.bson.ObjectID.prototype.getInc)
- description and source-code
```javascript
getInc = function () {
  return this.get_inc();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.ObjectID.prototype.getTimestamp"></a>[function <span class="apidocSignatureSpan">bson.ObjectID.prototype.</span>getTimestamp ()](#apidoc.element.bson.ObjectID.prototype.getTimestamp)
- description and source-code
```javascript
getTimestamp = function () {
  var timestamp = new Date();
  var time = this.id[3] | this.id[2] << 8 | this.id[1] << 16 | this.id[0] << 24;
  timestamp.setTime(Math.floor(time) * 1000);
  return timestamp;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.ObjectID.prototype.get_inc"></a>[function <span class="apidocSignatureSpan">bson.ObjectID.prototype.</span>get_inc ()](#apidoc.element.bson.ObjectID.prototype.get_inc)
- description and source-code
```javascript
get_inc = function () {
  return ObjectID.index = (ObjectID.index + 1) % 0xFFFFFF;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.ObjectID.prototype.inspect"></a>[function <span class="apidocSignatureSpan">bson.ObjectID.prototype.</span>inspect (format)](#apidoc.element.bson.ObjectID.prototype.inspect)
- description and source-code
```javascript
inspect = function (format) {
  // Is the id a buffer then use the buffer toString method to return the format
  if(this.id && this.id.copy) {
    return this.id.toString(typeof format === 'string' ? format : 'hex');
  }

  // if(this.buffer )
  return this.toHexString();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.ObjectID.prototype.toHexString"></a>[function <span class="apidocSignatureSpan">bson.ObjectID.prototype.</span>toHexString ()](#apidoc.element.bson.ObjectID.prototype.toHexString)
- description and source-code
```javascript
toHexString = function () {
  if(ObjectID.cacheHexString && this.__id) return this.__id;

  var hexString = '';
  if(!this.id || !this.id.length) {
    throw new Error('invalid ObjectId, ObjectId.id must be either a string or a Buffer, but is [' + JSON.stringify(this.id) + ']');
  }

  if(this.id instanceof _Buffer) {
    hexString = convertToHex(this.id);
    if(ObjectID.cacheHexString) this.__id = hexString;
    return hexString;
  }

  for (var i = 0; i < this.id.length; i++) {
    hexString += hexTable[this.id.charCodeAt(i)];
  }

  if(ObjectID.cacheHexString) this.__id = hexString;
  return hexString;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.ObjectID.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">bson.ObjectID.prototype.</span>toJSON ()](#apidoc.element.bson.ObjectID.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
  return this.toHexString();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.ObjectID.prototype.toString"></a>[function <span class="apidocSignatureSpan">bson.ObjectID.prototype.</span>toString (format)](#apidoc.element.bson.ObjectID.prototype.toString)
- description and source-code
```javascript
toString = function (format) {
  // Is the id a buffer then use the buffer toString method to return the format
  if(this.id && this.id.copy) {
    return this.id.toString(typeof format === 'string' ? format : 'hex');
  }

  // if(this.buffer )
  return this.toHexString();
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.bson.Symbol"></a>[module bson.Symbol](#apidoc.module.bson.Symbol)

#### <a name="apidoc.element.bson.Symbol.Symbol"></a>[function <span class="apidocSignatureSpan">bson.</span>Symbol (value)](#apidoc.element.bson.Symbol.Symbol)
- description and source-code
```javascript
function Symbol(value) {
  if(!(this instanceof Symbol)) return new Symbol(value);
  this._bsontype = 'Symbol';
  this.value = value;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.bson.Symbol.prototype"></a>[module bson.Symbol.prototype](#apidoc.module.bson.Symbol.prototype)

#### <a name="apidoc.element.bson.Symbol.prototype.inspect"></a>[function <span class="apidocSignatureSpan">bson.Symbol.prototype.</span>inspect ()](#apidoc.element.bson.Symbol.prototype.inspect)
- description and source-code
```javascript
inspect = function () {
  return this.value;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Symbol.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">bson.Symbol.prototype.</span>toJSON ()](#apidoc.element.bson.Symbol.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
  return this.value;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Symbol.prototype.toString"></a>[function <span class="apidocSignatureSpan">bson.Symbol.prototype.</span>toString ()](#apidoc.element.bson.Symbol.prototype.toString)
- description and source-code
```javascript
toString = function () {
  return this.value;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Symbol.prototype.valueOf"></a>[function <span class="apidocSignatureSpan">bson.Symbol.prototype.</span>valueOf ()](#apidoc.element.bson.Symbol.prototype.valueOf)
- description and source-code
```javascript
valueOf = function () {
  return this.value;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.bson.Timestamp"></a>[module bson.Timestamp](#apidoc.module.bson.Timestamp)

#### <a name="apidoc.element.bson.Timestamp.Timestamp"></a>[function <span class="apidocSignatureSpan">bson.</span>Timestamp (low, high)](#apidoc.element.bson.Timestamp.Timestamp)
- description and source-code
```javascript
function Timestamp(low, high) {
  if(!(this instanceof Timestamp)) return new Timestamp(low, high);
  this._bsontype = 'Timestamp';
<span class="apidocCodeCommentSpan">  /**
   * @type {number}
   * @ignore
   */
</span>  this.low_ = low | 0;  // force into 32 signed bits.

  /**
   * @type {number}
   * @ignore
   */
  this.high_ = high | 0;  // force into 32 signed bits.
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Timestamp.fromBits"></a>[function <span class="apidocSignatureSpan">bson.Timestamp.</span>fromBits (lowBits, highBits)](#apidoc.element.bson.Timestamp.fromBits)
- description and source-code
```javascript
fromBits = function (lowBits, highBits) {
  return new Timestamp(lowBits, highBits);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Timestamp.fromInt"></a>[function <span class="apidocSignatureSpan">bson.Timestamp.</span>fromInt (value)](#apidoc.element.bson.Timestamp.fromInt)
- description and source-code
```javascript
fromInt = function (value) {
  if (-128 <= value && value < 128) {
    var cachedObj = Timestamp.INT_CACHE_[value];
    if (cachedObj) {
      return cachedObj;
    }
  }

  var obj = new Timestamp(value | 0, value < 0 ? -1 : 0);
  if (-128 <= value && value < 128) {
    Timestamp.INT_CACHE_[value] = obj;
  }
  return obj;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Timestamp.fromNumber"></a>[function <span class="apidocSignatureSpan">bson.Timestamp.</span>fromNumber (value)](#apidoc.element.bson.Timestamp.fromNumber)
- description and source-code
```javascript
fromNumber = function (value) {
  if (isNaN(value) || !isFinite(value)) {
    return Timestamp.ZERO;
  } else if (value <= -Timestamp.TWO_PWR_63_DBL_) {
    return Timestamp.MIN_VALUE;
  } else if (value + 1 >= Timestamp.TWO_PWR_63_DBL_) {
    return Timestamp.MAX_VALUE;
  } else if (value < 0) {
    return Timestamp.fromNumber(-value).negate();
  } else {
    return new Timestamp(
               (value % Timestamp.TWO_PWR_32_DBL_) | 0,
               (value / Timestamp.TWO_PWR_32_DBL_) | 0);
  }
}
```
- example usage
```shell
...
  function start() {
    // Get the Long type
    var Long = BSON.Long;
    // Create a bson parser instance
    var bson = new BSON();

    // Serialize document
    var doc = { long: Long.fromNumber(100) }

    // Serialize a document
    var data = bson.serialize(doc)
    // De serialize it again
    var doc_2 = bson.deserialize(data)
  }
</script>
...
```

#### <a name="apidoc.element.bson.Timestamp.fromString"></a>[function <span class="apidocSignatureSpan">bson.Timestamp.</span>fromString (str, opt_radix)](#apidoc.element.bson.Timestamp.fromString)
- description and source-code
```javascript
fromString = function (str, opt_radix) {
  if (str.length == 0) {
    throw Error('number format error: empty string');
  }

  var radix = opt_radix || 10;
  if (radix < 2 || 36 < radix) {
    throw Error('radix out of range: ' + radix);
  }

  if (str.charAt(0) == '-') {
    return Timestamp.fromString(str.substring(1), radix).negate();
  } else if (str.indexOf('-') >= 0) {
    throw Error('number format error: interior "-" character: ' + str);
  }

  // Do several (8) digits each time through the loop, so as to
  // minimize the calls to the very expensive emulated div.
  var radixToPower = Timestamp.fromNumber(Math.pow(radix, 8));

  var result = Timestamp.ZERO;
  for (var i = 0; i < str.length; i += 8) {
    var size = Math.min(8, str.length - i);
    var value = parseInt(str.substring(i, i + size), radix);
    if (size < 8) {
      var power = Timestamp.fromNumber(Math.pow(radix, size));
      result = result.multiply(power).add(Timestamp.fromNumber(value));
    } else {
      result = result.multiply(radixToPower);
      result = result.add(Timestamp.fromNumber(value));
    }
  }
  return result;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.bson.Timestamp.prototype"></a>[module bson.Timestamp.prototype](#apidoc.module.bson.Timestamp.prototype)

#### <a name="apidoc.element.bson.Timestamp.prototype.add"></a>[function <span class="apidocSignatureSpan">bson.Timestamp.prototype.</span>add (other)](#apidoc.element.bson.Timestamp.prototype.add)
- description and source-code
```javascript
add = function (other) {
  // Divide each number into 4 chunks of 16 bits, and then sum the chunks.

  var a48 = this.high_ >>> 16;
  var a32 = this.high_ & 0xFFFF;
  var a16 = this.low_ >>> 16;
  var a00 = this.low_ & 0xFFFF;

  var b48 = other.high_ >>> 16;
  var b32 = other.high_ & 0xFFFF;
  var b16 = other.low_ >>> 16;
  var b00 = other.low_ & 0xFFFF;

  var c48 = 0, c32 = 0, c16 = 0, c00 = 0;
  c00 += a00 + b00;
  c16 += c00 >>> 16;
  c00 &= 0xFFFF;
  c16 += a16 + b16;
  c32 += c16 >>> 16;
  c16 &= 0xFFFF;
  c32 += a32 + b32;
  c48 += c32 >>> 16;
  c32 &= 0xFFFF;
  c48 += a48 + b48;
  c48 &= 0xFFFF;
  return Timestamp.fromBits((c16 << 16) | c00, (c48 << 16) | c32);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Timestamp.prototype.and"></a>[function <span class="apidocSignatureSpan">bson.Timestamp.prototype.</span>and (other)](#apidoc.element.bson.Timestamp.prototype.and)
- description and source-code
```javascript
and = function (other) {
  return Timestamp.fromBits(this.low_ & other.low_, this.high_ & other.high_);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Timestamp.prototype.compare"></a>[function <span class="apidocSignatureSpan">bson.Timestamp.prototype.</span>compare (other)](#apidoc.element.bson.Timestamp.prototype.compare)
- description and source-code
```javascript
compare = function (other) {
  if (this.equals(other)) {
    return 0;
  }

  var thisNeg = this.isNegative();
  var otherNeg = other.isNegative();
  if (thisNeg && !otherNeg) {
    return -1;
  }
  if (!thisNeg && otherNeg) {
    return 1;
  }

  // at this point, the signs are the same, so subtraction will not overflow
  if (this.subtract(other).isNegative()) {
    return -1;
  } else {
    return 1;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Timestamp.prototype.div"></a>[function <span class="apidocSignatureSpan">bson.Timestamp.prototype.</span>div (other)](#apidoc.element.bson.Timestamp.prototype.div)
- description and source-code
```javascript
div = function (other) {
  if (other.isZero()) {
    throw Error('division by zero');
  } else if (this.isZero()) {
    return Timestamp.ZERO;
  }

  if (this.equals(Timestamp.MIN_VALUE)) {
    if (other.equals(Timestamp.ONE) ||
        other.equals(Timestamp.NEG_ONE)) {
      return Timestamp.MIN_VALUE;  // recall that -MIN_VALUE == MIN_VALUE
    } else if (other.equals(Timestamp.MIN_VALUE)) {
      return Timestamp.ONE;
    } else {
      // At this point, we have |other| >= 2, so |this/other| < |MIN_VALUE|.
      var halfThis = this.shiftRight(1);
      var approx = halfThis.div(other).shiftLeft(1);
      if (approx.equals(Timestamp.ZERO)) {
        return other.isNegative() ? Timestamp.ONE : Timestamp.NEG_ONE;
      } else {
        var rem = this.subtract(other.multiply(approx));
        var result = approx.add(rem.div(other));
        return result;
      }
    }
  } else if (other.equals(Timestamp.MIN_VALUE)) {
    return Timestamp.ZERO;
  }

  if (this.isNegative()) {
    if (other.isNegative()) {
      return this.negate().div(other.negate());
    } else {
      return this.negate().div(other).negate();
    }
  } else if (other.isNegative()) {
    return this.div(other.negate()).negate();
  }

  // Repeat the following until the remainder is less than other:  find a
  // floating-point that approximates remainder / other *from below*, add this
  // into the result, and subtract it from the remainder.  It is critical that
  // the approximate value is less than or equal to the real value so that the
  // remainder never becomes negative.
  var res = Timestamp.ZERO;
  var rem = this;
  while (rem.greaterThanOrEqual(other)) {
    // Approximate the result of division. This may be a little greater or
    // smaller than the actual value.
    var approx = Math.max(1, Math.floor(rem.toNumber() / other.toNumber()));

    // We will tweak the approximate result by changing it in the 48-th digit or
    // the smallest non-fractional digit, whichever is larger.
    var log2 = Math.ceil(Math.log(approx) / Math.LN2);
    var delta = (log2 <= 48) ? 1 : Math.pow(2, log2 - 48);

    // Decrease the approximation until it is smaller than the remainder.  Note
    // that if it is too large, the product overflows and is negative.
    var approxRes = Timestamp.fromNumber(approx);
    var approxRem = approxRes.multiply(other);
    while (approxRem.isNegative() || approxRem.greaterThan(rem)) {
      approx -= delta;
      approxRes = Timestamp.fromNumber(approx);
      approxRem = approxRes.multiply(other);
    }

    // We know the answer can't be zero... and actually, zero would cause
    // infinite recursion since we would make no progress.
    if (approxRes.isZero()) {
      approxRes = Timestamp.ONE;
    }

    res = res.add(approxRes);
    rem = rem.subtract(approxRem);
  }
  return res;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Timestamp.prototype.equals"></a>[function <span class="apidocSignatureSpan">bson.Timestamp.prototype.</span>equals (other)](#apidoc.element.bson.Timestamp.prototype.equals)
- description and source-code
```javascript
equals = function (other) {
  return (this.high_ == other.high_) && (this.low_ == other.low_);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Timestamp.prototype.getHighBits"></a>[function <span class="apidocSignatureSpan">bson.Timestamp.prototype.</span>getHighBits ()](#apidoc.element.bson.Timestamp.prototype.getHighBits)
- description and source-code
```javascript
getHighBits = function () {
  return this.high_;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Timestamp.prototype.getLowBits"></a>[function <span class="apidocSignatureSpan">bson.Timestamp.prototype.</span>getLowBits ()](#apidoc.element.bson.Timestamp.prototype.getLowBits)
- description and source-code
```javascript
getLowBits = function () {
  return this.low_;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Timestamp.prototype.getLowBitsUnsigned"></a>[function <span class="apidocSignatureSpan">bson.Timestamp.prototype.</span>getLowBitsUnsigned ()](#apidoc.element.bson.Timestamp.prototype.getLowBitsUnsigned)
- description and source-code
```javascript
getLowBitsUnsigned = function () {
  return (this.low_ >= 0) ?
      this.low_ : Timestamp.TWO_PWR_32_DBL_ + this.low_;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Timestamp.prototype.getNumBitsAbs"></a>[function <span class="apidocSignatureSpan">bson.Timestamp.prototype.</span>getNumBitsAbs ()](#apidoc.element.bson.Timestamp.prototype.getNumBitsAbs)
- description and source-code
```javascript
getNumBitsAbs = function () {
  if (this.isNegative()) {
    if (this.equals(Timestamp.MIN_VALUE)) {
      return 64;
    } else {
      return this.negate().getNumBitsAbs();
    }
  } else {
    var val = this.high_ != 0 ? this.high_ : this.low_;
    for (var bit = 31; bit > 0; bit--) {
      if ((val & (1 << bit)) != 0) {
        break;
      }
    }
    return this.high_ != 0 ? bit + 33 : bit + 1;
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Timestamp.prototype.greaterThan"></a>[function <span class="apidocSignatureSpan">bson.Timestamp.prototype.</span>greaterThan (other)](#apidoc.element.bson.Timestamp.prototype.greaterThan)
- description and source-code
```javascript
greaterThan = function (other) {
  return this.compare(other) > 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Timestamp.prototype.greaterThanOrEqual"></a>[function <span class="apidocSignatureSpan">bson.Timestamp.prototype.</span>greaterThanOrEqual (other)](#apidoc.element.bson.Timestamp.prototype.greaterThanOrEqual)
- description and source-code
```javascript
greaterThanOrEqual = function (other) {
  return this.compare(other) >= 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Timestamp.prototype.isNegative"></a>[function <span class="apidocSignatureSpan">bson.Timestamp.prototype.</span>isNegative ()](#apidoc.element.bson.Timestamp.prototype.isNegative)
- description and source-code
```javascript
isNegative = function () {
  return this.high_ < 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Timestamp.prototype.isOdd"></a>[function <span class="apidocSignatureSpan">bson.Timestamp.prototype.</span>isOdd ()](#apidoc.element.bson.Timestamp.prototype.isOdd)
- description and source-code
```javascript
isOdd = function () {
  return (this.low_ & 1) == 1;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Timestamp.prototype.isZero"></a>[function <span class="apidocSignatureSpan">bson.Timestamp.prototype.</span>isZero ()](#apidoc.element.bson.Timestamp.prototype.isZero)
- description and source-code
```javascript
isZero = function () {
  return this.high_ == 0 && this.low_ == 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Timestamp.prototype.lessThan"></a>[function <span class="apidocSignatureSpan">bson.Timestamp.prototype.</span>lessThan (other)](#apidoc.element.bson.Timestamp.prototype.lessThan)
- description and source-code
```javascript
lessThan = function (other) {
  return this.compare(other) < 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Timestamp.prototype.lessThanOrEqual"></a>[function <span class="apidocSignatureSpan">bson.Timestamp.prototype.</span>lessThanOrEqual (other)](#apidoc.element.bson.Timestamp.prototype.lessThanOrEqual)
- description and source-code
```javascript
lessThanOrEqual = function (other) {
  return this.compare(other) <= 0;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Timestamp.prototype.modulo"></a>[function <span class="apidocSignatureSpan">bson.Timestamp.prototype.</span>modulo (other)](#apidoc.element.bson.Timestamp.prototype.modulo)
- description and source-code
```javascript
modulo = function (other) {
  return this.subtract(this.div(other).multiply(other));
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Timestamp.prototype.multiply"></a>[function <span class="apidocSignatureSpan">bson.Timestamp.prototype.</span>multiply (other)](#apidoc.element.bson.Timestamp.prototype.multiply)
- description and source-code
```javascript
multiply = function (other) {
  if (this.isZero()) {
    return Timestamp.ZERO;
  } else if (other.isZero()) {
    return Timestamp.ZERO;
  }

  if (this.equals(Timestamp.MIN_VALUE)) {
    return other.isOdd() ? Timestamp.MIN_VALUE : Timestamp.ZERO;
  } else if (other.equals(Timestamp.MIN_VALUE)) {
    return this.isOdd() ? Timestamp.MIN_VALUE : Timestamp.ZERO;
  }

  if (this.isNegative()) {
    if (other.isNegative()) {
      return this.negate().multiply(other.negate());
    } else {
      return this.negate().multiply(other).negate();
    }
  } else if (other.isNegative()) {
    return this.multiply(other.negate()).negate();
  }

  // If both Timestamps are small, use float multiplication
  if (this.lessThan(Timestamp.TWO_PWR_24_) &&
      other.lessThan(Timestamp.TWO_PWR_24_)) {
    return Timestamp.fromNumber(this.toNumber() * other.toNumber());
  }

  // Divide each Timestamp into 4 chunks of 16 bits, and then add up 4x4 products.
  // We can skip products that would overflow.

  var a48 = this.high_ >>> 16;
  var a32 = this.high_ & 0xFFFF;
  var a16 = this.low_ >>> 16;
  var a00 = this.low_ & 0xFFFF;

  var b48 = other.high_ >>> 16;
  var b32 = other.high_ & 0xFFFF;
  var b16 = other.low_ >>> 16;
  var b00 = other.low_ & 0xFFFF;

  var c48 = 0, c32 = 0, c16 = 0, c00 = 0;
  c00 += a00 * b00;
  c16 += c00 >>> 16;
  c00 &= 0xFFFF;
  c16 += a16 * b00;
  c32 += c16 >>> 16;
  c16 &= 0xFFFF;
  c16 += a00 * b16;
  c32 += c16 >>> 16;
  c16 &= 0xFFFF;
  c32 += a32 * b00;
  c48 += c32 >>> 16;
  c32 &= 0xFFFF;
  c32 += a16 * b16;
  c48 += c32 >>> 16;
  c32 &= 0xFFFF;
  c32 += a00 * b32;
  c48 += c32 >>> 16;
  c32 &= 0xFFFF;
  c48 += a48 * b00 + a32 * b16 + a16 * b32 + a00 * b48;
  c48 &= 0xFFFF;
  return Timestamp.fromBits((c16 << 16) | c00, (c48 << 16) | c32);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Timestamp.prototype.negate"></a>[function <span class="apidocSignatureSpan">bson.Timestamp.prototype.</span>negate ()](#apidoc.element.bson.Timestamp.prototype.negate)
- description and source-code
```javascript
negate = function () {
  if (this.equals(Timestamp.MIN_VALUE)) {
    return Timestamp.MIN_VALUE;
  } else {
    return this.not().add(Timestamp.ONE);
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Timestamp.prototype.not"></a>[function <span class="apidocSignatureSpan">bson.Timestamp.prototype.</span>not ()](#apidoc.element.bson.Timestamp.prototype.not)
- description and source-code
```javascript
not = function () {
  return Timestamp.fromBits(~this.low_, ~this.high_);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Timestamp.prototype.notEquals"></a>[function <span class="apidocSignatureSpan">bson.Timestamp.prototype.</span>notEquals (other)](#apidoc.element.bson.Timestamp.prototype.notEquals)
- description and source-code
```javascript
notEquals = function (other) {
  return (this.high_ != other.high_) || (this.low_ != other.low_);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Timestamp.prototype.or"></a>[function <span class="apidocSignatureSpan">bson.Timestamp.prototype.</span>or (other)](#apidoc.element.bson.Timestamp.prototype.or)
- description and source-code
```javascript
or = function (other) {
  return Timestamp.fromBits(this.low_ | other.low_, this.high_ | other.high_);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Timestamp.prototype.shiftLeft"></a>[function <span class="apidocSignatureSpan">bson.Timestamp.prototype.</span>shiftLeft (numBits)](#apidoc.element.bson.Timestamp.prototype.shiftLeft)
- description and source-code
```javascript
shiftLeft = function (numBits) {
  numBits &= 63;
  if (numBits == 0) {
    return this;
  } else {
    var low = this.low_;
    if (numBits < 32) {
      var high = this.high_;
      return Timestamp.fromBits(
                 low << numBits,
                 (high << numBits) | (low >>> (32 - numBits)));
    } else {
      return Timestamp.fromBits(0, low << (numBits - 32));
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Timestamp.prototype.shiftRight"></a>[function <span class="apidocSignatureSpan">bson.Timestamp.prototype.</span>shiftRight (numBits)](#apidoc.element.bson.Timestamp.prototype.shiftRight)
- description and source-code
```javascript
shiftRight = function (numBits) {
  numBits &= 63;
  if (numBits == 0) {
    return this;
  } else {
    var high = this.high_;
    if (numBits < 32) {
      var low = this.low_;
      return Timestamp.fromBits(
                 (low >>> numBits) | (high << (32 - numBits)),
                 high >> numBits);
    } else {
      return Timestamp.fromBits(
                 high >> (numBits - 32),
                 high >= 0 ? 0 : -1);
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Timestamp.prototype.shiftRightUnsigned"></a>[function <span class="apidocSignatureSpan">bson.Timestamp.prototype.</span>shiftRightUnsigned (numBits)](#apidoc.element.bson.Timestamp.prototype.shiftRightUnsigned)
- description and source-code
```javascript
shiftRightUnsigned = function (numBits) {
  numBits &= 63;
  if (numBits == 0) {
    return this;
  } else {
    var high = this.high_;
    if (numBits < 32) {
      var low = this.low_;
      return Timestamp.fromBits(
                 (low >>> numBits) | (high << (32 - numBits)),
                 high >>> numBits);
    } else if (numBits == 32) {
      return Timestamp.fromBits(high, 0);
    } else {
      return Timestamp.fromBits(high >>> (numBits - 32), 0);
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Timestamp.prototype.subtract"></a>[function <span class="apidocSignatureSpan">bson.Timestamp.prototype.</span>subtract (other)](#apidoc.element.bson.Timestamp.prototype.subtract)
- description and source-code
```javascript
subtract = function (other) {
  return this.add(other.negate());
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Timestamp.prototype.toInt"></a>[function <span class="apidocSignatureSpan">bson.Timestamp.prototype.</span>toInt ()](#apidoc.element.bson.Timestamp.prototype.toInt)
- description and source-code
```javascript
toInt = function () {
  return this.low_;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Timestamp.prototype.toJSON"></a>[function <span class="apidocSignatureSpan">bson.Timestamp.prototype.</span>toJSON ()](#apidoc.element.bson.Timestamp.prototype.toJSON)
- description and source-code
```javascript
toJSON = function () {
  return this.toString();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Timestamp.prototype.toNumber"></a>[function <span class="apidocSignatureSpan">bson.Timestamp.prototype.</span>toNumber ()](#apidoc.element.bson.Timestamp.prototype.toNumber)
- description and source-code
```javascript
toNumber = function () {
  return this.high_ * Timestamp.TWO_PWR_32_DBL_ +
         this.getLowBitsUnsigned();
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Timestamp.prototype.toString"></a>[function <span class="apidocSignatureSpan">bson.Timestamp.prototype.</span>toString (opt_radix)](#apidoc.element.bson.Timestamp.prototype.toString)
- description and source-code
```javascript
toString = function (opt_radix) {
  var radix = opt_radix || 10;
  if (radix < 2 || 36 < radix) {
    throw Error('radix out of range: ' + radix);
  }

  if (this.isZero()) {
    return '0';
  }

  if (this.isNegative()) {
    if (this.equals(Timestamp.MIN_VALUE)) {
      // We need to change the Timestamp value before it can be negated, so we remove
      // the bottom-most digit in this base and then recurse to do the rest.
      var radixTimestamp = Timestamp.fromNumber(radix);
      var div = this.div(radixTimestamp);
      var rem = div.multiply(radixTimestamp).subtract(this);
      return div.toString(radix) + rem.toInt().toString(radix);
    } else {
      return '-' + this.negate().toString(radix);
    }
  }

  // Do several (6) digits each time through the loop, so as to
  // minimize the calls to the very expensive emulated div.
  var radixToPower = Timestamp.fromNumber(Math.pow(radix, 6));

  var rem = this;
  var result = '';
  while (true) {
    var remDiv = rem.div(radixToPower);
    var intval = rem.subtract(remDiv.multiply(radixToPower)).toInt();
    var digits = intval.toString(radix);

    rem = remDiv;
    if (rem.isZero()) {
      return digits + result;
    } else {
      while (digits.length < 6) {
        digits = '0' + digits;
      }
      result = '' + digits + result;
    }
  }
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.bson.Timestamp.prototype.xor"></a>[function <span class="apidocSignatureSpan">bson.Timestamp.prototype.</span>xor (other)](#apidoc.element.bson.Timestamp.prototype.xor)
- description and source-code
```javascript
xor = function (other) {
  return Timestamp.fromBits(this.low_ ^ other.low_, this.high_ ^ other.high_);
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
