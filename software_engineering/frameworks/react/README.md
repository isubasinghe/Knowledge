# react

## Basic idea

A declarative JavaScript UI library: describe the UI as a function of state; React diffs the resulting virtual DOM against the previous one and applies the minimal real-DOM patches.

## Key facts

- Components: functions returning JSX (sugar for `React.createElement`).
- State: `useState`, `useReducer`; side effects: `useEffect`.
- Reconciliation via virtual DOM; keys identify list items across renders.
- Unidirectional data flow (props down, events up).

