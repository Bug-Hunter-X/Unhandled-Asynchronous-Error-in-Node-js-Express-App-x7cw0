# Unhandled Asynchronous Error in Node.js Express App

This repository demonstrates a common error in Node.js applications: unhandled errors within asynchronous callbacks.  The `bug.js` file contains an Express.js app that simulates an asynchronous operation which might throw an error. If the random number generated is less than 0.5, an error is thrown within the `setTimeout` callback. Without proper error handling, this will cause the server to crash.

The `bugSolution.js` file shows how to correctly handle this type of asynchronous error using a `try...catch` block. 

This example highlights the importance of robust error handling in asynchronous Node.js code to prevent unexpected application crashes.