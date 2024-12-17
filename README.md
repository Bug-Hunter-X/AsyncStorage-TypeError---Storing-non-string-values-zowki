# React Native AsyncStorage TypeError Bug

This repository demonstrates a common error in React Native when using AsyncStorage: attempting to store non-string values. AsyncStorage only accepts strings.  This example shows the error and its solution.

## Bug
The `bug.js` file contains code that attempts to store a JavaScript object directly in AsyncStorage. This results in a TypeError.

## Solution
The `bugSolution.js` file shows the corrected code.  Before storing the data in AsyncStorage, the object is stringified using `JSON.stringify()`. This converts the object into a string, which AsyncStorage can handle.

## How to Reproduce
1. Clone the repository.
2. Run `npm install`.
3. Run the application. Observe the error message in the console.
4. Uncomment the corrected code in `bugSolution.js` and observe that the error is resolved. 