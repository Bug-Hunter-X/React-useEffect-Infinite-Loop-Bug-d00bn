# React useEffect Infinite Loop Bug

This repository demonstrates a common bug in React applications involving the `useEffect` hook.  The issue arises from an incorrectly defined dependency array, leading to an infinite loop.  The solution provides a corrected version with the proper dependency array.

## Bug Description

The provided `bug.js` file contains a React component that uses `useEffect` to log the count state to the console. However, because the dependency array is empty or missing, useEffect runs after every render, causing the count to continuously increment and trigger re-renders indefinitely.

## Solution

The `bugSolution.js` file presents the correct implementation where the dependency array includes `count`. This ensures that the `useEffect` runs only when the `count` value actually changes.

## How to reproduce

1. Clone this repository.
2. Navigate to the project directory.
3. Run `npm install`
4. Run `npm start`
5. Observe the behavior in your browser's console and compare the output of both versions.
