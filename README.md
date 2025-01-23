# Express.js Route Parameter Handling Error

This repository demonstrates a common error in Express.js route handlers:  failure to handle invalid input in route parameters.  The `bug.js` file shows the erroneous code, while `bugSolution.js` provides a corrected version with proper error handling.

**Bug:** The original code attempts to parse a user ID from the route parameters.  However, it lacks error handling for scenarios where the ID is not a valid integer.  This can lead to application crashes or unexpected behavior.

**Solution:** The corrected code includes error handling to check if the `userId` is a valid integer.  If it's not, a 400 Bad Request error is returned.  If the user is not found, a 404 Not Found error is returned.