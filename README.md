# ⚡ Interactive Backend Runtime Visualizers

Interactive visual guides that explain how backend runtimes and request-processing systems work internally.

The project focuses on making complex concepts easier to understand through animated, step-by-step visualizations.

## Run

Open the HTML visualizations directly in your browser.

Example:

<a href="https://kirilkirkov.github.io/index.html">https://kirilkirkov.github.io/index.html</a> (Node.JS Event-Loop and Express.JS) <br>
<a href="https://kirilkirkov.github.io/php-fpm.html">https://kirilkirkov.github.io/php-fpm.html</a> (PHP-FPM)

## Visualizations

### ⚡ JavaScript Event Loop

Interactive visualization of the JavaScript Event Loop for both **Browser** and **Node.js**.

Learn how:

* Call Stack works
* Microtasks are processed
* Timers are scheduled
* Promises and `async / await` behave
* `process.nextTick()` works
* Node.js Event Loop phases are processed
* Multiple asynchronous operations can progress concurrently

Includes:

* 🎡 Animated Event Loop visualization
* 📚 Call Stack
* ⚡ Microtask Queue
* ⏱ Timers / Task Queue
* 🔁 `process.nextTick()`
* 📡 Node.js Event Loop phases
* 📝 Editable JavaScript examples
* 🖥 Live console output
* ⏯ Play / Pause / Stop
* 🐢 Adjustable animation speed
* 📱 Responsive design

---

### 🐘 Nginx & PHP-FPM

Animated visualization of the full PHP request lifecycle:

```text
Client
  ↓
Nginx
  ↓
FastCGI
  ↓
PHP-FPM
  ↓
Worker Pool
  ↓
PHP Worker
  ↓
Response
  ↓
Nginx
  ↓
Client
```

Learn how:

* Nginx handles incoming requests
* PHP requests are forwarded to PHP-FPM
* PHP-FPM manages worker processes
* One request occupies one PHP-FPM worker
* Multiple PHP requests are processed concurrently by different workers
* Requests wait when all workers are busy
* `pm.max_children` affects concurrency
* Workers become available again after the response is completed

## Purpose

This project is built as a learning tool for understanding backend internals visually instead of only reading diagrams or documentation.

The goal is to answer questions like:

> What is actually happening inside the server right now?

and:

> Why is this request waiting or executing?

## Future Visualizations

More backend concepts may be added in the future, such as:

* Redis
* Load balancing
* Worker Threads
* Message queues
* Database transactions
* Connection pools
* Horizontal scaling

## License

MIT
