# Missing Content-Type Header in Node.js HTTP Response

This repository demonstrates a common error in Node.js HTTP servers: omitting the `Content-Type` header in the response.  This can lead to unexpected behavior and errors on the client-side because the client might not know how to interpret the response body.

## Bug

The `bug.js` file shows a simple HTTP server that lacks the crucial `Content-Type` header.  This causes the client to potentially misinterpret the response, leading to errors or unexpected behavior.

## Solution

The `bugSolution.js` file demonstrates the correct way to set the `Content-Type` header.  By specifying the content type (e.g., `text/plain`, `application/json`), you ensure the client correctly interprets the response.

## How to reproduce

1. Clone this repository.
2. Navigate to the repository directory.
3. Run `node bug.js`. 
4. Observe the potential issues when accessing the server using a browser or other HTTP client.
5. Run `node bugSolution.js` and see how it addresses the problem.