# Unhandled Exception in Asynchronous Node.js Server

This repository demonstrates a common error in Node.js where an unhandled exception within an asynchronous operation can cause the server to crash. The `bug.js` file contains the problematic code, while `bugSolution.js` provides a solution using error handling.

## Problem

The server simulates an asynchronous operation (using `setTimeout`) that randomly either succeeds or throws an error.  If an error occurs, it's not caught, leading to a crash.

## Solution

The solution involves using a `try...catch` block within the asynchronous operation to handle potential errors gracefully. This prevents the server from crashing and allows for more robust error handling.