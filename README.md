# Express.js JSON Body Parsing Error

This repository demonstrates a common error encountered when working with JSON request bodies in Express.js applications.  The issue arises when an empty request body or an invalid JSON request body is sent to an endpoint that expects JSON data.

## Bug Description

When an empty request body or an invalid JSON payload is sent to the `/data` POST endpoint, the application fails to parse the request body correctly. This can lead to unexpected behavior or errors.

## Solution

The solution involves adding error handling to gracefully manage scenarios where the request body is empty or invalid JSON.  This is achieved by checking for the existence and validity of `req.body` before attempting to process it.