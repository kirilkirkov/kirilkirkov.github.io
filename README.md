# ⚡ JavaScript Event Loop Visualizer

Interactive visualization of the JavaScript Event Loop for both **Browser** and **Node.js**.

The goal is to make asynchronous JavaScript easier to understand by showing what actually happens with callbacks, queues, the Call Stack, microtasks, timers, and Node.js Event Loop phases.

## Features

* 🌐 Browser Event Loop visualization
* 🟢 Node.js Event Loop visualization
* 📚 Call Stack
* ⚡ Microtask Queue
* ⏱ Timers / Task Queue
* 🔁 `process.nextTick()`
* 📡 Node.js phases: `timers → pending → poll → check → close`
* 🎡 Animated Event Loop wheel
* 🎯 Visual callback lifecycle
* 📝 Editable JavaScript examples
* 🖥 Live console output
* ⏯ Play / Pause / Stop
* 🐢 Adjustable animation speed
* 📱 Responsive design

## Examples

Explore common async JavaScript behavior with:

```js
console.log('A');

setTimeout(() => console.log('B'), 0);

Promise.resolve()
  .then(() => console.log('C'));

console.log('D');
```

Output:

```text
A
D
C
B
```

The visualizer shows **why** this execution order happens.

## Purpose

Built as a learning tool for understanding:

* JavaScript concurrency
* Event Loop scheduling
* Promises and microtasks
* `async / await`
* timers
* Node.js Event Loop phases
* `process.nextTick()`
* `setImmediate()`

## Run

Open `index.html` in your browser.

No backend required.

## License

MIT
