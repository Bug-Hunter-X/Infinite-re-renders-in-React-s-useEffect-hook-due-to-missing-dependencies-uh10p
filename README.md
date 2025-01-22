# React useEffect Hook Bug

This repository demonstrates a common error in React's `useEffect` hook: omitting dependencies from the dependency array, leading to infinite re-renders.

## The Bug

The `bug.js` file contains a React component that uses the `useEffect` hook to log the current count to the console. However, it's missing a crucial part: the dependency array.  This causes the effect to run after every render, triggering another render, resulting in an infinite loop.