# Node.js Server Port Already in Use Error

This repository demonstrates a common error in Node.js development where a server fails to start because the port is already in use.  The error is handled using error event listener and checks for port availability. 

## The Problem

When you attempt to start a Node.js HTTP server on a port that's already occupied by another process (e.g., another server or application), the `server.listen()` method will throw an error. This typically results in the server failing to start.

## The Solution

This solution uses error event listener to gracefully handle the error case when a port is already in use.  The alternative solution involves checking for port availability before starting the server, to avoid the error altogether.
