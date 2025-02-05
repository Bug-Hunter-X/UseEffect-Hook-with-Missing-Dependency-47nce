# React useEffect Hook with Missing Dependency

This repository demonstrates a common React bug: an infinite loop caused by a missing dependency in the `useEffect` hook.

The `bug.js` file contains the buggy code, where the `useEffect` hook is missing the `count` dependency. This causes the effect to run on every render, leading to an infinite loop of console logs and potential performance issues.  The `bugSolution.js` provides the corrected code.

## How to reproduce

1. Clone this repository.
2. Run `npm install` to install the dependencies.
3. Run `npm start` to start the development server.
4. Observe the infinite loop in the browser's console.

## Solution

The solution involves adding the `count` variable as a dependency to the `useEffect` hook.  This ensures that the effect only runs when the value of `count` changes.