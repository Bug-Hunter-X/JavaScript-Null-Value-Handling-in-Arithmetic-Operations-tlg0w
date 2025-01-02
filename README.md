# JavaScript Null Value Handling Bug

This repository demonstrates a common, yet subtle, bug in JavaScript related to how null values are handled in arithmetic operations.

## The Bug

The `foo` function in `bug.js` attempts to add two numbers.  However, it incorrectly returns 0 if either input is null.  This is a silent failure, making the bug harder to detect.

## The Solution

The `bugSolution.js` file provides a corrected version of the `foo` function that explicitly checks for null values and handles them appropriately.  This improved version either converts null to 0 or throws an error for better error handling. 

## How to reproduce

1. Clone the repository.
2. Run `node bug.js` to observe the incorrect behavior.
3. Run `node bugSolution.js` to see the corrected behavior.