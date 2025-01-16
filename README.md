# React useEffect Hook Memory Leak

This repository demonstrates a common error in React applications involving the `useEffect` hook: forgetting to include a cleanup function. This can lead to memory leaks and unexpected behavior.

## Bug
The `bug.js` file contains a component that updates the document title whenever the count changes. However, it lacks a cleanup function to reset the title when the component unmounts. This causes the title to persist even after navigating away from the component.

## Solution
The `bugSolution.js` file shows the corrected version, including a cleanup function that resets the title when the component unmounts. This prevents memory leaks and ensures the correct behavior.

## How to reproduce
1. Clone this repository.
2. Navigate to the `bug` directory.
3. Run `npm install`.
4. Run `npm start`.
5. Observe the behavior of the title when you click the button and when you navigate away from the page.