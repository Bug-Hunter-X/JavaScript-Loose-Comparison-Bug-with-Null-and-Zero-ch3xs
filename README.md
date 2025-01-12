# JavaScript Loose Comparison Bug

This repository demonstrates a subtle bug in JavaScript related to loose comparison (==) with null and zero.  The original code uses loose comparison which causes an unexpected result when the input is 0.

## Bug Description
The function `foo` is intended to return 0 if x is null, -1 if x is negative, and 1 otherwise. Due to loose comparison with null, the function incorrectly returns 1 when x is 0.

## Bug Solution
The solution replaces the loose comparison (==) with a strict comparison (===) to fix the incorrect behavior.  Strict comparison ensures that the type and value are both checked, leading to the correct output.

## How to reproduce
1. Clone this repository.
2. Navigate to the directory
3. run `node bug.js` and `node bugSolution.js` to see the bug and its fix respectively.
