# React useEffect Infinite Loop Bug

This repository demonstrates a common error in React applications involving the `useEffect` hook: creating an infinite render loop by omitting the dependency array.

The `bug.js` file shows the problematic code, where the `useEffect` hook runs after every render because the dependency array is missing.  This leads to an infinite loop, constantly updating the count and rendering the component.

The `bugSolution.js` file provides the corrected version, adding the `count` variable to the dependency array.  This ensures the effect only runs when the `count` value changes.