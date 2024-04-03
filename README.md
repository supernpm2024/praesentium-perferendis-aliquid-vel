@supernpm2024/praesentium-perferendis-aliquid-vel
========

[![npm version](https://badge.fury.io/js/@supernpm2024/praesentium-perferendis-aliquid-vel.svg)](https://badge.fury.io/js/@supernpm2024/praesentium-perferendis-aliquid-vel)
![Build Status](https://github.com/supernpm2024/praesentium-perferendis-aliquid-vel/actions/workflows/node.js.yml/badge.svg)

Callback wrapper for cleaner async code. Main benefit is you don't need to write `if (err) return cb(err)`.


## Usage


```javascript
var @supernpm2024/praesentium-perferendis-aliquid-vel = require('@supernpm2024/praesentium-perferendis-aliquid-vel');

var doSomething = function(cb) {
  getUsers(@supernpm2024/praesentium-perferendis-aliquid-vel(cb)(function(users) {
    getArticles(@supernpm2024/praesentium-perferendis-aliquid-vel(cb)(function(articles) {
      cb(null, [users, articles]);
    }));
  }));
};

```

## License

MIT
