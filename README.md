# React Race Condition Bug

This repository demonstrates a common race condition bug in React applications involving asynchronous `setState` calls.  The bug occurs because `setState` is asynchronous; the component might re-render before the state is updated.

The `bug.js` file contains the buggy code. The `bugSolution.js` file provides a solution using functional updates to prevent this race condition.

## How to Reproduce

1. Clone this repository.
2. Run `npm install` to install the necessary packages.
3. Run `npm start` to start the development server.
4. Click the button. Observe that the console log might display an outdated value for the count before the UI is updated.