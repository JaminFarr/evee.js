# evee.js
The lightweight es6 event library.

Evee is a beautiful, lightweight event library, written in clean JavaScript (ES6).

## How to use
```js
// Get evee
var evee = require('./evee')();

// Subscribe to the 'onUpdate' event
evee.subscribe('onUpdate', e => {
  console.log('Ticks: ' + e.data);
});

var ticks = 0;
while(true) {

  // Dispatch the 'onUpdate' event
  evee.dispatch('onUpdate', ++ticks);
}
```

As you can see, evee is really easy to use!   
Start using evee today and fire events at nearly the speed of light<sup>1</sup> :)


<sup>1</sup> <sub>This is probably not true, but who knows.</sub>