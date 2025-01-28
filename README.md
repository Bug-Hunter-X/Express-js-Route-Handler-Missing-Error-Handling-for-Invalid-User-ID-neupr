# Express.js Route Handler Missing Error Handling for Invalid User ID

This repository demonstrates a common error in Express.js route handlers:  missing error handling for invalid input.  Specifically, this example shows a route that fetches a user by ID but fails to handle cases where the ID is not a valid integer.

## Bug

The `bug.js` file contains an Express.js route handler that fetches a user by ID.  It attempts to parse the ID as an integer, but it doesn't check if the input is actually a number. This can lead to errors if a non-numeric ID is provided.

## Solution

The `bugSolution.js` file demonstrates the correct approach. It includes error handling to check if the ID is a number and returns a 400 Bad Request error if it is not.