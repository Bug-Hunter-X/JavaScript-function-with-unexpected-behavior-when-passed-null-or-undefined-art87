# JavaScript Unexpected Behavior with Null and Undefined

This repository demonstrates a common subtle bug in JavaScript related to handling null and undefined values in arithmetic operations.  The `foo` function is designed to add two numbers. However, its handling of null and undefined inputs is incomplete.

## Bug Description

The original `bug.js` file contains a function that handles null values correctly, returning 0.  However, it fails to correctly handle `undefined` values, resulting in `NaN` (Not a Number) in some cases.

## Solution

The `bugSolution.js` file provides a corrected version of the function.  It explicitly checks for both `null` and `undefined` values, ensuring that the function behaves predictably in all cases.

## How to Reproduce the Bug

1. Clone this repository.
2. Run `bug.js` (e.g., using Node.js).
3. Observe the output when calling `foo` with different combinations of null, undefined, and numbers.

## How to See the Solution

1. Examine `bugSolution.js` for the corrected implementation.
2. Run `bugSolution.js` and compare the output to `bug.js` to see the difference.

This example highlights the importance of comprehensive null and undefined checks in JavaScript to avoid unexpected results in your code.