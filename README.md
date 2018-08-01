## queue-node

* A simple queue structure for nodejs.

#### GET START

##### INSTALL
```shell
$ npm install queue-node --save
```

##### IMPORT and INIT and USAGE
```javascript
const Queue = require('queue-node');

/**
 * size<Number>: queue size
 * callback<Function>: jobs when queue full
 *   data<Array>: the data queue
 *   onerror<Function>: callback when error
 */
const queue = new Queue(1000, (data, onerror) => {
  if (err) {
      onerror();
  }

  // do sthing
});

// push
const array = [a, b, c];
queue.push(...array);
```
