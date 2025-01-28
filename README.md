# React useEffect finally block masking errors
This example demonstrates a subtle bug in a React component that uses `useEffect` to fetch data. The `finally` block, intended for cleanup, can inadvertently mask errors if the `catch` block doesn't explicitly re-throw the error.  This can lead to difficult-to-debug issues where the component appears to load successfully, but no data is displayed.

The `bug.js` file contains the buggy code. The `bugSolution.js` file provides the corrected version.