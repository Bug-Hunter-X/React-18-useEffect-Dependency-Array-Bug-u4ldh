# React 18 useEffect Dependency Array Bug

This repository demonstrates a common bug related to the `useEffect` hook in React 18 and later versions.  Improperly specifying dependencies in the `useEffect` hook's array can lead to unexpected behavior such as infinite loops and performance problems.  The bug and its solution are showcased with clear code examples.

## Bug Description

The provided `bug.js` file illustrates a scenario where a component attempts to update state based on a value that's not included in the `useEffect` dependency array.  This leads to unexpected re-renders, potentially creating an infinite loop.  This is a subtle but common error.

## Solution

The `bugSolution.js` file demonstrates the correct solution.  By explicitly adding the `count` variable to the dependency array, we ensure the effect only runs when the `count` value changes, as intended.

## How to Reproduce

1. Clone this repository.
2. Navigate to the repository's directory in your terminal.
3. Run `npm install` to install the necessary dependencies.
4. Run `npm start` to start the development server.
5. Observe the behavior of the component and compare the console logs between the `bug` and `bugSolution` versions. 
