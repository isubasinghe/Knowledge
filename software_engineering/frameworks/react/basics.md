# React Basics

## Basic idea

UI = `f(state)`. Components return a virtual DOM tree; React reconciles it with the live DOM. State changes trigger re-renders of the affected subtree, not the whole page.

## Key facts

- Components: function returning JSX.
- Hooks: `useState`, `useEffect`, `useMemo`, `useRef`, `useContext`, `useReducer`.
- Pure rendering: a component with the same props + state should return the same output.
- Keys identify list items for stable reconciliation.

