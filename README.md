# React useEffect Infinite Loop Bug

This repository demonstrates a common React bug related to the `useEffect` hook. The bug is caused by omitting a dependency from the dependency array, leading to an infinite loop.

## Bug Description

The `useEffect` hook in the provided `MyComponent` function is intended to log the current count to the console after each render. However, the `count` variable is missing from the dependency array. This means that the effect runs after every render, regardless of the changes in the `count` variable, causing the component to re-render infinitely.