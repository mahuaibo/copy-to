copy-to
=======

copy an object's properties to another one

## Install

```
npm install copy-to
```

## Usage

```js
var copy = require('copy-to');

var src = {
  _name: 'foo',
  set name(val) {
    this._name = val;
  },
  get name() {
    return this._name;
  },
  show: function () {
    console.log(this._name);
  }
};

var des = {
  _name: 'bar'
};

copy(src).to(des);
copy(src).toCover(des);
```

## License
MIT
