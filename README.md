# React useEffect Cleanup Function Issue

This repository demonstrates a common React bug related to the useEffect hook's cleanup function not being called properly. This can lead to memory leaks if not addressed correctly. The bug and its solution are provided in separate JavaScript files.

## Bug Description
The `useEffect` hook in `bug.js` is missing `count` in the dependency array which causes the cleanup function to never execute, resulting in potential memory issues. 

## Solution
The corrected version is provided in `bugSolution.js`. By including `count` in the dependency array, the cleanup function is properly called when the component unmounts or when `count` changes. 

## How to Reproduce
1. Clone this repo.
2. Run `npm install` to install dependencies (if necessary).
3. Open `bug.js` and `bugSolution.js` to see the problem and the solution. 