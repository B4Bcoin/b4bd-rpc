B4Bcoin-rpc.js
===============

A client library to connect to B4Bcoin RPC in JavaScript.

## Get Started

b4bd-rpc.js runs on [node](http://nodejs.org/)

```bash
npm install b4bd-rpc
```

## Examples

```javascript

var RpcClient = require('b4bd-rpc');
// var RpcClient = require('./');

var config = {
  protocol: 'http',
  user: 'user',
  pass: 'pass',
  host: '127.0.0.1',
  port: '8667',
};

var rpc = new RpcClient(config);


rpc.getDifficulty(function(error, parsedBuf) {
  console.log(parsedBuf);
});


rpc.listaddressesbyasset('TEST', function(error, parsedBuf) {
  console.log(parsedBuf);
});


```
