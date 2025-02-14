# Unexpected State Updates in React's useState Hook

This repository demonstrates a common yet subtle bug in React applications involving the `useState` hook. The problem arises from the asynchronous nature of state updates in React.  When you call `setCount` multiple times in quick succession, the subsequent calls might overwrite previous updates leading to unexpected results.  The example shows a counter that should increment by 2 on each click but instead only increments by 1.

## How to reproduce

1. Clone this repository.
2. Run `npm install`.
3. Run `npm start`.
4. Observe the counter's behavior.  It will increment by one, not two.