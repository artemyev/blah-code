[![very bullgit](https://img.shields.io/badge/very-bullgit-1393d5.svg?style=flat)](https://bullg.it/)
[![npm version](https://img.shields.io/npm/v/blah-code.svg?style=flat)](https://www.npmjs.org/package/blah-code)
[![Build Status](https://travis-ci.org/bullgit/blah-code.svg?branch=master)](https://travis-ci.org/bullgit/blah-code)
[![devDependency Status](https://david-dm.org/bullgit/blah-code/dev-status.svg)](https://david-dm.org/bullgit/blah-code#info=devDependencies)
[![XO code style](https://img.shields.io/badge/code_style-XO-5ed9c7.svg)](https://github.com/sindresorhus/xo)
[![Unicorn approved](https://img.shields.io/badge/unicorn-approved-ff69b4.svg?style=flat)](https://www.youtube.com/watch?v=ihXfH-zR8qA&feature=youtu.be&t=10s)

# blah-code

> Encode and decode blah code

[Demotime](https://bullg.it/blah-code/) :rabbit:

As UMD module this runs almost everywhere [AMD (e.g RequireJS), CommonJS (Nodeland, browserify) and with good ol’ globals].

Uses ECMAScript 5.1 intensively. So you need [es5-shim](https://github.com/es-shims/es5-shim) in case you want to use in old Browsers (IE < 9).


## Install

```bash
$ npm install --save blah-code
```

or even:

```bash
$ bower install --save blah-code
```

## Usage

### CommonJS example:

```javascript
var blahCode = require('blah-code');

blahCode.encode('Hi there! What’s up?'); // → blaa bluh. blah bleh bluuh. […]

blahCode.decode('blaa bluh. blah bleh bluuh. blaah bluh. blah blah blehh. blah bleh bleeh. blah bleh blah. blah blah bleeh. blah bleh blah. blaah blaah. blaah bluh. blahh blaa. blah bleh bleeh. blee blaa. blah blah blehh. blahh bluh blah blaa. blah blah bluuh. blaah bluh. blah blah blaa. blah blah bluh. blehh blaah'); // -> hi there! whats up?
```

### Global scope example:

```html
<script src="blah-code.min.js"></script>
<script src="myFile.js"></script>
```

```javascript
// myFile.js

blahCode.encode('Hi there! What’s up?'); // → blaa bluh. blah bleh bluuh. […]
```

## API

Accepts a `string` and returns a `string`:

### blahCode.encode()

Returns the blah code representation of the given text:

```javascript
blahCode.encode('Hi there! What’s up?');
```

There is an optional parameter that you can use to switch from blah-code to ape-code. Just use:

```javascript
blahCode.encode('Hi there! What’s up?', 'ooks');
```

### blahCode.decode()

Returns regular text of the given blah code:

```javascript
blahCode.decode('blaa bluh. blah bleh bluuh. blaah bluh.');
```

There is an optional parameter that you can use to switch from blah-code to ape-code. Just use:

```javascript
blahCode.decode('Oook! Ook!. Ook? Ook Oook. Ook?! Ook!.', 'ooks');
```

## Contributing

See [CONTRIBUTING.md](CONTRIBUTING.md)

## Related

- [blah-code-cli](https://github.com/bullgit/blah-code-cli) - CLI for this module

## License

MIT © [Michael Kühnel](http://michael-kuehnel.de)

