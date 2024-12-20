# Express.js Server Crash: Unhandled Database Query Errors

This repository demonstrates a common error in Express.js applications: unhandled errors during database queries.  The `bug.js` file shows the problematic code, which lacks proper error handling and can cause the server to crash.  The `bugSolution.js` file provides a corrected version with improved error handling.

**Problem:**
The original code attempts to fetch user data from a database. However, it fails to handle potential errors from the database query.  If the database query fails (e.g., due to a network issue or invalid user ID), the server crashes.  Asynchronous operations are not properly handled leading to silent failures.

**Solution:**
The solution involves adding comprehensive error handling. The `bugSolution.js` file demonstrates how to catch and handle potential database errors, preventing the server from crashing and providing informative error responses to the client.