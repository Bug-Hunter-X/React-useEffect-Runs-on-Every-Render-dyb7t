# React useEffect Runs on Every Render

This repository demonstrates a common React bug where the `useEffect` hook runs on every render, leading to performance issues. The solution shows how to fix this by correctly specifying the dependencies array.

## Bug

The `useEffect` hook in `bug.js` lacks a proper dependency array.  This results in the effect running on every render, which can cause unexpected behavior and performance problems.

## Solution

`bugSolution.js` corrects the issue by specifying the `count` state variable in the dependency array, ensuring the effect only runs when `count` changes.