# Stack Overflow Bug in JavaScript

This repository demonstrates a common error in JavaScript: a stack overflow error caused by unbounded recursion.  The `foo` function recursively calls itself without a proper base case for sufficiently large inputs, leading to excessive function calls until the call stack is exhausted. 

The `bug.js` file contains the buggy code.  The `bugSolution.js` file provides a corrected version using iteration to avoid stack overflow issues.

## How to Reproduce

1. Clone this repository.
2. Open `bug.js` and `bugSolution.js` in your preferred JavaScript environment.
3. Run `bug.js` with a large integer as the first argument (e.g., `foo(1000, 0)`).  Observe the stack overflow error.
4. Run `bugSolution.js` with the same argument. Observe that it works correctly.