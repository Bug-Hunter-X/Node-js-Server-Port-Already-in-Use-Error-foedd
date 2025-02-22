# Node.js Server Port Already in Use Error

This repository demonstrates a common error encountered when developing Node.js applications: the 'port already in use' error.  This error occurs when the server attempts to bind to a port that is already in use by another process.

## Bug Description
The provided `bug.js` file contains a simple HTTP server that listens on port 8080. If port 8080 is already in use (e.g., by another instance of the server or a different application), the server will fail to start and throw an error.

## Solution
The `bugSolution.js` file demonstrates a solution to this problem by using the `'error'` event of the HTTP server to handle the error gracefully and provide informative feedback to the user.

## How to Reproduce the Bug
1.  Run `bug.js`.
2.  While the server is running, attempt to run `bug.js` again.  This will result in the port already in use error. (You can also run another application on port 8080)

## How to Run the Solution
1. Run `bugSolution.js`. This improved version handles the port already in use error.