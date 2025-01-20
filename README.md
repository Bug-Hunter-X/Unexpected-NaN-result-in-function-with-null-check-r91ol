# JavaScript Bug: Unexpected NaN Result

This repository demonstrates a common JavaScript bug related to unexpected NaN results when dealing with null and undefined values.

## Description
The function `foo` checks if the input `a` is null and returns 0 if it is. Otherwise, it returns `a + 1`. While it correctly handles `null`, it behaves unexpectedly with `undefined`.  Instead of returning 0 (or perhaps throwing an error), it returns NaN.

## How to Reproduce
1. Clone this repository.
2. Run `bug.js` using a JavaScript runtime (e.g., Node.js).

## Solution
The solution involves adding a check for `undefined`.  This can be done using a strict equality check (`===`) or by using a more general check involving `typeof`. 
Refer to `bugSolution.js` for the corrected code.