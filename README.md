# Subtle Null Handling Bug in JavaScript

This repository demonstrates a common, yet subtle, bug in JavaScript related to null value handling.  The `foo` function is designed to return 0 if either input `a` or `b` is null. However, it contains a flaw in how it handles the scenario where *both* inputs are null.

The `bug.js` file contains the buggy code.  The `bugSolution.js` file provides a corrected version.

## How to Reproduce
1. Clone this repository.
2. Open `bug.js`.
3. Run the code using a JavaScript interpreter (like Node.js).
4. Observe the unexpected output when calling `foo(null, null)`. 

## Solution
The solution involves adding a specific check to handle the case of both parameters being null simultaneously.