# api documentation for  [nlp_compromise (v6.5.3)](https://github.com/nlp-compromise/nlp_compromise#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-nlp_compromise.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-nlp_compromise) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-nlp_compromise.svg)](https://travis-ci.org/npmdoc/node-npmdoc-nlp_compromise)
#### natural language processing in the browser

[![NPM](https://nodei.co/npm/nlp_compromise.png?downloads=true)](https://www.npmjs.com/package/nlp_compromise)

[![apidoc](https://npmdoc.github.io/node-npmdoc-nlp_compromise/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-nlp_compromise_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-nlp_compromise/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-nlp_compromise/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-nlp_compromise/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Spencer Kelly",
        "email": "spencermountain@gmail.com",
        "url": "http://spencermounta.in"
    },
    "bugs": {
        "url": "https://github.com/nlp-compromise/nlp_compromise/issues"
    },
    "dependencies": {},
    "description": "natural language processing in the browser",
    "devDependencies": {
        "babel-preset-es2015": "6.9.0",
        "babelify": "7.3.0",
        "browserify": "13.0.1",
        "derequire": "^2.0.3",
        "grunt-cli": "1.2.0",
        "grunt-contrib-watch": "1.0.0",
        "grunt-eslint": "19.0.0",
        "grunt-filesize": "0.0.7",
        "grunt-run": "0.6.0",
        "http-server": "0.9.0",
        "nlp-corpus": "latest",
        "tap-spec": "4.1.1",
        "tape": "4.6.0",
        "uglify-js": "2.7.0"
    },
    "directories": {},
    "dist": {
        "shasum": "7720b67daab7b486509057ef1d5eff9a3db091bb",
        "tarball": "https://registry.npmjs.org/nlp_compromise/-/nlp_compromise-6.5.3.tgz"
    },
    "files": [
        "builds/",
        "src/",
        "nlp.d.ts"
    ],
    "gitHead": "994c61750b725eb8508b417472a422b17293ef10",
    "homepage": "https://github.com/nlp-compromise/nlp_compromise#readme",
    "license": "MIT",
    "main": "./builds/nlp_compromise.js",
    "maintainers": [
        {
            "name": "spencermountain",
            "email": "spencermountain@gmail.com"
        }
    ],
    "name": "nlp_compromise",
    "optionalDependencies": {},
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git://github.com/nlp-compromise/nlp_compromise.git"
    },
    "scripts": {
        "build": "grunt build",
        "build_windows": "grunt build_windows",
        "coverage": "grunt coverage",
        "demo": "grunt demo",
        "demo_windows": "grunt demo_windows",
        "test": "./node_modules/tape/bin/tape ./test/unit_test/**/*_test.js | tap-spec",
        "watch": "grunt watch"
    },
    "typings": "./nlp.d.ts",
    "version": "6.5.3"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module nlp_compromise](#apidoc.module.nlp_compromise)
1.  [function <span class="apidocSignatureSpan">nlp_compromise.</span>adjective (s)](#apidoc.element.nlp_compromise.adjective)
1.  [function <span class="apidocSignatureSpan">nlp_compromise.</span>adverb (s)](#apidoc.element.nlp_compromise.adverb)
1.  [function <span class="apidocSignatureSpan">nlp_compromise.</span>date (s)](#apidoc.element.nlp_compromise.date)
1.  [function <span class="apidocSignatureSpan">nlp_compromise.</span>lexicon (obj)](#apidoc.element.nlp_compromise.lexicon)
1.  [function <span class="apidocSignatureSpan">nlp_compromise.</span>noun (s)](#apidoc.element.nlp_compromise.noun)
1.  [function <span class="apidocSignatureSpan">nlp_compromise.</span>organization (s)](#apidoc.element.nlp_compromise.organization)
1.  [function <span class="apidocSignatureSpan">nlp_compromise.</span>person (s)](#apidoc.element.nlp_compromise.person)
1.  [function <span class="apidocSignatureSpan">nlp_compromise.</span>place (s)](#apidoc.element.nlp_compromise.place)
1.  [function <span class="apidocSignatureSpan">nlp_compromise.</span>plugin (obj)](#apidoc.element.nlp_compromise.plugin)
1.  [function <span class="apidocSignatureSpan">nlp_compromise.</span>question (s)](#apidoc.element.nlp_compromise.question)
1.  [function <span class="apidocSignatureSpan">nlp_compromise.</span>sentence (s, options)](#apidoc.element.nlp_compromise.sentence)
1.  [function <span class="apidocSignatureSpan">nlp_compromise.</span>statement (s)](#apidoc.element.nlp_compromise.statement)
1.  [function <span class="apidocSignatureSpan">nlp_compromise.</span>term (s)](#apidoc.element.nlp_compromise.term)
1.  [function <span class="apidocSignatureSpan">nlp_compromise.</span>text (s, options)](#apidoc.element.nlp_compromise.text)
1.  [function <span class="apidocSignatureSpan">nlp_compromise.</span>value (s)](#apidoc.element.nlp_compromise.value)
1.  [function <span class="apidocSignatureSpan">nlp_compromise.</span>verb (s)](#apidoc.element.nlp_compromise.verb)
1.  object <span class="apidocSignatureSpan">nlp_compromise.</span>fns

#### [module nlp_compromise.fns](#apidoc.module.nlp_compromise.fns)
1.  [function <span class="apidocSignatureSpan">nlp_compromise.fns.</span>endsWith (str, suffix)](#apidoc.element.nlp_compromise.fns.endsWith)
1.  [function <span class="apidocSignatureSpan">nlp_compromise.fns.</span>expand_prefixes (list, obj)](#apidoc.element.nlp_compromise.fns.expand_prefixes)
1.  [function <span class="apidocSignatureSpan">nlp_compromise.fns.</span>expand_suffixes (list, obj)](#apidoc.element.nlp_compromise.fns.expand_suffixes)
1.  [function <span class="apidocSignatureSpan">nlp_compromise.fns.</span>extend (a, b)](#apidoc.element.nlp_compromise.fns.extend)
1.  [function <span class="apidocSignatureSpan">nlp_compromise.fns.</span>flatten (arr)](#apidoc.element.nlp_compromise.fns.flatten)
1.  [function <span class="apidocSignatureSpan">nlp_compromise.fns.</span>isFunction (obj)](#apidoc.element.nlp_compromise.fns.isFunction)
1.  [function <span class="apidocSignatureSpan">nlp_compromise.fns.</span>pluck (arr, str)](#apidoc.element.nlp_compromise.fns.pluck)
1.  [function <span class="apidocSignatureSpan">nlp_compromise.fns.</span>reverseObj (obj)](#apidoc.element.nlp_compromise.fns.reverseObj)
1.  [function <span class="apidocSignatureSpan">nlp_compromise.fns.</span>startsWith (str, prefix)](#apidoc.element.nlp_compromise.fns.startsWith)
1.  [function <span class="apidocSignatureSpan">nlp_compromise.fns.</span>titlecase (str)](#apidoc.element.nlp_compromise.fns.titlecase)
1.  [function <span class="apidocSignatureSpan">nlp_compromise.fns.</span>toObj (arr)](#apidoc.element.nlp_compromise.fns.toObj)



# <a name="apidoc.module.nlp_compromise"></a>[module nlp_compromise](#apidoc.module.nlp_compromise)

#### <a name="apidoc.element.nlp_compromise.adjective"></a>[function <span class="apidocSignatureSpan">nlp_compromise.</span>adjective (s)](#apidoc.element.nlp_compromise.adjective)
- description and source-code
```javascript
adjective = function (s) {
  return new models.Adjective(s);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nlp_compromise.adverb"></a>[function <span class="apidocSignatureSpan">nlp_compromise.</span>adverb (s)](#apidoc.element.nlp_compromise.adverb)
- description and source-code
```javascript
adverb = function (s) {
  return new models.Adverb(s);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nlp_compromise.date"></a>[function <span class="apidocSignatureSpan">nlp_compromise.</span>date (s)](#apidoc.element.nlp_compromise.date)
- description and source-code
```javascript
date = function (s) {
  return new models.Date(s);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nlp_compromise.lexicon"></a>[function <span class="apidocSignatureSpan">nlp_compromise.</span>lexicon (obj)](#apidoc.element.nlp_compromise.lexicon)
- description and source-code
```javascript
lexicon = function (obj) {
  obj = obj || {};
  var lex = _dereq_('./lexicon.js');

  Object.keys(obj).forEach(function (k) {
    lex[k] = obj[k];
  });

  return lex;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nlp_compromise.noun"></a>[function <span class="apidocSignatureSpan">nlp_compromise.</span>noun (s)](#apidoc.element.nlp_compromise.noun)
- description and source-code
```javascript
noun = function (s) {
  return new models.Noun(s);
}
```
- example usage
```shell
...
> 'npm install nlp_compromise'

> '<script src="https://unpkg.com/nlp_compromise@latest/builds/nlp_compromise.min.js"></script>'

'''javascript
let nlp = require('nlp_compromise'); // or nlp = window.nlp_compromise

nlp.noun('dinosaur').pluralize();
// 'dinosaurs'

nlp.verb('speak').conjugate();
// { past: 'spoke',
//   infinitive: 'speak',
//   gerund: 'speaking',
//   actor: 'speaker',
...
```

#### <a name="apidoc.element.nlp_compromise.organization"></a>[function <span class="apidocSignatureSpan">nlp_compromise.</span>organization (s)](#apidoc.element.nlp_compromise.organization)
- description and source-code
```javascript
organization = function (s) {
  return new models.Organization(s);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nlp_compromise.person"></a>[function <span class="apidocSignatureSpan">nlp_compromise.</span>person (s)](#apidoc.element.nlp_compromise.person)
- description and source-code
```javascript
person = function (s) {
  return new models.Person(s);
}
```
- example usage
```shell
...

nlp.text('Tony Hawk did a kickflip').people();
// [ Person { text: 'Tony Hawk' ..} ]

nlp.noun('vacuum').article();
// 'a'

nlp.person('Tony Hawk').pronoun();
// 'he'

nlp.value('five hundred and sixty').number;
// 560

nlp.text(require('nlp-corpus').text.friends()).topics()//11 seasons of friends
// [ { count: 2523, text: 'ross' },
...
```

#### <a name="apidoc.element.nlp_compromise.place"></a>[function <span class="apidocSignatureSpan">nlp_compromise.</span>place (s)](#apidoc.element.nlp_compromise.place)
- description and source-code
```javascript
place = function (s) {
  return new models.Place(s);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nlp_compromise.plugin"></a>[function <span class="apidocSignatureSpan">nlp_compromise.</span>plugin (obj)](#apidoc.element.nlp_compromise.plugin)
- description and source-code
```javascript
plugin = function (obj) {
  obj = obj || {};
  // if obj is a function, pass it an instance of this nlp library
  if (fns.isFunction(obj)) {
    // run it in this current context
    obj = obj.call(this, this);
  }
  //apply each plugin to the correct prototypes
  Object.keys(obj).forEach(function (k) {
    Object.keys(obj[k]).forEach(function (method) {
      models[k].prototype[method] = obj[k][method];
    });
  });
}
```
- example usage
```shell
...
//   { count: 1411, text: 'rachel' },
//   ....
'''
#Plugin/Mixins
we've also got a modest, though ambitious [plugin ecosystem](https://github.com/nlp-compromise/nlp_compromise/wiki/Plugins):
'''javascript
//US-UK localization
nlp.plugin(require('nlp-locale'))
nlp.term('favourite').toAmerican()
// 'favorite'

//syllable hyphenization
nlp.plugin(require('nlp-syllables'));
var t2 = nlp.term('houston texas');
t2.syllables()
...
```

#### <a name="apidoc.element.nlp_compromise.question"></a>[function <span class="apidocSignatureSpan">nlp_compromise.</span>question (s)](#apidoc.element.nlp_compromise.question)
- description and source-code
```javascript
question = function (s) {
  return new models.Question(s);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nlp_compromise.sentence"></a>[function <span class="apidocSignatureSpan">nlp_compromise.</span>sentence (s, options)](#apidoc.element.nlp_compromise.sentence)
- description and source-code
```javascript
sentence = function (s, options) {
  return new models.Sentence(s, options);
}
```
- example usage
```shell
...

[![CodacyBadge](https://api.codacy.com/project/badge/grade/82cc8ebd98b64ed199d7be6021488062)](https://www.codacy.com/app/spencerkelly86
/nlp_compromise)
[![npm version](https://badge.fury.io/js/nlp_compromise.svg)](https://www.npmjs.com/package/nlp_compromise)
[![downloads](https://img.shields.io/npm/dm/nlp_compromise.svg)](https://www.npmjs.com/package/nlp_compromise)

**nlp_compromise** does NLP in the browser.
'''javascript
nlp.sentence('She sells seashells').to_past().text()
// 'She sold seashells'
'''
### Yup,
* **<150k** js file
* **86%** on the [Penn treebank](http://www.cis.upenn.edu/~treebank/)
* keypress speed, constant-time.
* caniuse, uhuh. **IE9+**
...
```

#### <a name="apidoc.element.nlp_compromise.statement"></a>[function <span class="apidocSignatureSpan">nlp_compromise.</span>statement (s)](#apidoc.element.nlp_compromise.statement)
- description and source-code
```javascript
statement = function (s) {
  return new models.Statement(s);
}
```
- example usage
```shell
...
//   present: 'speaks',
//   future: 'will speak',
//   perfect: 'have spoken',
//   pluperfect: 'had spoken',
//   future_perfect: 'will have spoken'
// }

nlp.statement('She sells seashells').negate().text()
// 'She doesn't sell seashells'

nlp.sentence('I fed the dog').replace('the [Noun]', 'the cat').text()
// 'I fed the cat'

nlp.text('Tony Hawk did a kickflip').people();
// [ Person { text: 'Tony Hawk' ..} ]
...
```

#### <a name="apidoc.element.nlp_compromise.term"></a>[function <span class="apidocSignatureSpan">nlp_compromise.</span>term (s)](#apidoc.element.nlp_compromise.term)
- description and source-code
```javascript
term = function (s) {
  return new models.Term(s);
}
```
- example usage
```shell
...
//   ....
'''
#Plugin/Mixins
we've also got a modest, though ambitious [plugin ecosystem](https://github.com/nlp-compromise/nlp_compromise/wiki/Plugins):
'''javascript
//US-UK localization
nlp.plugin(require('nlp-locale'))
nlp.term('favourite').toAmerican()
// 'favorite'

//syllable hyphenization
nlp.plugin(require('nlp-syllables'));
var t2 = nlp.term('houston texas');
t2.syllables()
//[ [ 'hous', 'ton' ], [ 'tex', 'as' ] ]
...
```

#### <a name="apidoc.element.nlp_compromise.text"></a>[function <span class="apidocSignatureSpan">nlp_compromise.</span>text (s, options)](#apidoc.element.nlp_compromise.text)
- description and source-code
```javascript
text = function (s, options) {
  return new models.Text(s, options);
}
```
- example usage
```shell
...

[![CodacyBadge](https://api.codacy.com/project/badge/grade/82cc8ebd98b64ed199d7be6021488062)](https://www.codacy.com/app/spencerkelly86
/nlp_compromise)
[![npm version](https://badge.fury.io/js/nlp_compromise.svg)](https://www.npmjs.com/package/nlp_compromise)
[![downloads](https://img.shields.io/npm/dm/nlp_compromise.svg)](https://www.npmjs.com/package/nlp_compromise)

**nlp_compromise** does NLP in the browser.
'''javascript
nlp.sentence('She sells seashells').to_past().text()
// 'She sold seashells'
'''
### Yup,
* **<150k** js file
* **86%** on the [Penn treebank](http://www.cis.upenn.edu/~treebank/)
* keypress speed, constant-time.
* caniuse, uhuh. **IE9+**
...
```

#### <a name="apidoc.element.nlp_compromise.value"></a>[function <span class="apidocSignatureSpan">nlp_compromise.</span>value (s)](#apidoc.element.nlp_compromise.value)
- description and source-code
```javascript
value = function (s) {
  return new models.Value(s);
}
```
- example usage
```shell
...

nlp.noun('vacuum').article();
// 'a'

nlp.person('Tony Hawk').pronoun();
// 'he'

nlp.value('five hundred and sixty').number;
// 560

nlp.text(require('nlp-corpus').text.friends()).topics()//11 seasons of friends
// [ { count: 2523, text: 'ross' },
//   { count: 1922, text: 'joey' },
//   { count: 1876, text: 'god' },
//   { count: 1411, text: 'rachel' },
...
```

#### <a name="apidoc.element.nlp_compromise.verb"></a>[function <span class="apidocSignatureSpan">nlp_compromise.</span>verb (s)](#apidoc.element.nlp_compromise.verb)
- description and source-code
```javascript
verb = function (s) {
  return new models.Verb(s);
}
```
- example usage
```shell
...

'''javascript
let nlp = require('nlp_compromise'); // or nlp = window.nlp_compromise

nlp.noun('dinosaur').pluralize();
// 'dinosaurs'

nlp.verb('speak').conjugate();
// { past: 'spoke',
//   infinitive: 'speak',
//   gerund: 'speaking',
//   actor: 'speaker',
//   present: 'speaks',
//   future: 'will speak',
//   perfect: 'have spoken',
...
```



# <a name="apidoc.module.nlp_compromise.fns"></a>[module nlp_compromise.fns](#apidoc.module.nlp_compromise.fns)

#### <a name="apidoc.element.nlp_compromise.fns.endsWith"></a>[function <span class="apidocSignatureSpan">nlp_compromise.fns.</span>endsWith (str, suffix)](#apidoc.element.nlp_compromise.fns.endsWith)
- description and source-code
```javascript
endsWith = function (str, suffix) {
  //if suffix is regex
  if (suffix && suffix instanceof RegExp) {
    if (str.match(suffix)) {
      return true;
    }
  }
  //if suffix is a string
  if (str && suffix && str.indexOf(suffix, str.length - suffix.length) !== -1) {
    return true;
  }
  return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nlp_compromise.fns.expand_prefixes"></a>[function <span class="apidocSignatureSpan">nlp_compromise.fns.</span>expand_prefixes (list, obj)](#apidoc.element.nlp_compromise.fns.expand_prefixes)
- description and source-code
```javascript
expand_prefixes = function (list, obj) {
  let keys = Object.keys(obj);
  let l = keys.length;
  for (let i = 0; i < l; i++) {
    const arr = obj[keys[i]].split(',');
    for (let i2 = 0; i2 < arr.length; i2++) {
      list.push(keys[i] + arr[i2]);
    }
  }
  return list;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nlp_compromise.fns.expand_suffixes"></a>[function <span class="apidocSignatureSpan">nlp_compromise.fns.</span>expand_suffixes (list, obj)](#apidoc.element.nlp_compromise.fns.expand_suffixes)
- description and source-code
```javascript
expand_suffixes = function (list, obj) {
  let keys = Object.keys(obj);
  let l = keys.length;
  for (let i = 0; i < l; i++) {
    const arr = obj[keys[i]].split(',');
    for (let i2 = 0; i2 < arr.length; i2++) {
      list.push(arr[i2] + keys[i]);
    }
  }
  return list;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nlp_compromise.fns.extend"></a>[function <span class="apidocSignatureSpan">nlp_compromise.fns.</span>extend (a, b)](#apidoc.element.nlp_compromise.fns.extend)
- description and source-code
```javascript
extend = function (a, b) {
  const keys = Object.keys(b);
  for(let i = 0; i < keys.length; i++) {
    a[keys[i]] = b[keys[i]];
  }
  return a;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nlp_compromise.fns.flatten"></a>[function <span class="apidocSignatureSpan">nlp_compromise.fns.</span>flatten (arr)](#apidoc.element.nlp_compromise.fns.flatten)
- description and source-code
```javascript
flatten = function (arr) {
  let all = [];
  arr.forEach(function(a) {
    all = all.concat(a);
  });
  return all;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nlp_compromise.fns.isFunction"></a>[function <span class="apidocSignatureSpan">nlp_compromise.fns.</span>isFunction (obj)](#apidoc.element.nlp_compromise.fns.isFunction)
- description and source-code
```javascript
isFunction = function (obj) {
  return Object.prototype.toString.call(obj) === '[object Function]';
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nlp_compromise.fns.pluck"></a>[function <span class="apidocSignatureSpan">nlp_compromise.fns.</span>pluck (arr, str)](#apidoc.element.nlp_compromise.fns.pluck)
- description and source-code
```javascript
pluck = function (arr, str) {
  arr = arr || [];
  return arr.map(function(o) {
    return o[str];
  });
}
```
- example usage
```shell
...
//add all names
addArr(Object.keys(firstNames.all), 'Person');
//overwrite to MalePerson, FemalePerson
addArr(firstNames.male, 'MalePerson');
addArr(firstNames.female, 'FemalePerson');
//add irregular nouns
const irregNouns = require('./data/irregular_nouns.js');
addArr(fns.pluck(irregNouns, 0), 'Noun');
addArr(fns.pluck(irregNouns, 1), 'Plural');

addObj(require('./data/misc.js'));
addObj(require('./data/multiples.js'));
addObj(require('./data/phrasal_verbs.js'));
//add named holidays, like 'easter'
Object.keys(require('./data/holidays.js')).forEach(function(k) {
...
```

#### <a name="apidoc.element.nlp_compromise.fns.reverseObj"></a>[function <span class="apidocSignatureSpan">nlp_compromise.fns.</span>reverseObj (obj)](#apidoc.element.nlp_compromise.fns.reverseObj)
- description and source-code
```javascript
reverseObj = function (obj) {
  return Object.keys(obj).reduce(function(h, k) {
    h[obj[k]] = k;
    return h;
  }, {});
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nlp_compromise.fns.startsWith"></a>[function <span class="apidocSignatureSpan">nlp_compromise.fns.</span>startsWith (str, prefix)](#apidoc.element.nlp_compromise.fns.startsWith)
- description and source-code
```javascript
startsWith = function (str, prefix) {
  if (str && str.length && str.substr(0, 1) === prefix) {
    return true;
  }
  return false;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nlp_compromise.fns.titlecase"></a>[function <span class="apidocSignatureSpan">nlp_compromise.fns.</span>titlecase (str)](#apidoc.element.nlp_compromise.fns.titlecase)
- description and source-code
```javascript
titlecase = function (str) {
  if (!str) {
    return '';
  }
  str = str.toLowerCase();
  return str.charAt(0).toUpperCase() + str.slice(1);
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.nlp_compromise.fns.toObj"></a>[function <span class="apidocSignatureSpan">nlp_compromise.fns.</span>toObj (arr)](#apidoc.element.nlp_compromise.fns.toObj)
- description and source-code
```javascript
toObj = function (arr) {
  return arr.reduce(function(h, a) {
    h[a] = true;
    return h;
  }, {});
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
