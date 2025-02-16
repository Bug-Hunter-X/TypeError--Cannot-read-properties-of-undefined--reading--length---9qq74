# Javascript Bug: TypeError: Cannot read properties of undefined (reading 'length')
This repository contains a simple JavaScript example demonstrating a common error: the `TypeError: Cannot read properties of undefined (reading 'length')`.  This error occurs when trying to access the `length` property of a variable that is `undefined`.

## Bug Description
The provided JavaScript function `foo` aims to check if the input `x` is null and if it's not return its length.  However, it fails to handle the case where `x` is `undefined`, leading to a `TypeError`.  Undefined values do not possess a `length` property, resulting in the error.

## How to Reproduce
1. Clone this repository.
2. Open `bug.js`.
3. Run the code.  The function will throw an error if you call `foo` with `undefined` as an argument.

## Solution
The solution involves adding a check for `undefined` values in the `foo` function.  This ensures that the code gracefully handles different input types, avoiding the TypeError.