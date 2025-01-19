# Unhandled Promise Rejection in React Data Fetching

This repository demonstrates a common but subtle bug in React applications involving asynchronous data fetching and error handling. The bug stems from improper handling of promise rejections within the `useEffect` hook, leading to unexpected behavior and potential crashes.  The solution emphasizes robust error handling and state management techniques.

## Bug
The `bug.js` file shows a React component that fetches data from an API.  The issue lies in how the `.catch` block handles errors.  If the API request fails, the error message will be displayed, but the promise rejection might still cause an unhandled promise rejection in the console.  This can lead to instability in the application and make debugging more difficult.

## Solution
The `bugSolution.js` file corrects this by explicitly handling the promise rejection within the `.catch` block. This ensures that even if the API request fails, the application remains stable and the error is properly managed.

This example highlights the importance of comprehensive error handling when working with asynchronous operations in React.