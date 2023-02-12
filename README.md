# Promise-chaining-

const promise = new Promise(resolve => setTimeout(resolve, 5000));
promise
 // 5 seconds later
 .then(() => 2)
 // returning a value from a then callback will cause
 // the new promise to resolve with this value
 .then(value => { /* value === 2 */ });
