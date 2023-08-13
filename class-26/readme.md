# React Quick Start Guide

Welcome to the React Quick Start guide! This document aims to provide you with a quick refresher on React and its fundamental concepts.

### What are the building blocks of a React app?

- Components: These are the fundamental building blocks in React. They represent the elements of the page and thier behavior.
- JSX: A syntax extension for JavaScript that allows you to write HTML-like code in your JavaScript files.
- Props: Used to pass data from parent to child components.
- State: Represents mutable data that affects the component's behavior and rendering.
- Lifecycle methods: Special methods for executing code at various stages of a component's lifecycle.
- Virtual DOM: A virtual representation of the actual DOM that React uses to optimize updates.

### What is the difference between an HTML element and a React component?

An HTML element is a native browser element (`<div>`, `<p>`), while a React component is a reusable piece of UI that can contain one or more HTML elements. Components allow you to create complex UI structures and manage behavior efficiently.

### What is JSX and why do we use it?

JSX is a syntax extension for JavaScript that lets you write HTML-like code within your JavaScript files. It simplifies UI creation and gets transpiled into regular JavaScript by tools like Babel.

### Describe the process of embedding JavaScript expressions in JSX.

You can embed JavaScript expressions in JSX using curly braces `{}`. For instance, to embed a variable named `count`, you can write: `{count}`.

### Does React or JSX have any special features for iteration or conditional logic?

React provides special features for iteration and conditional logic using JavaScript expressions. You can use JavaScript's `map()` function for iteration and conditional statements (`if` or ternary operators) directly within JSX.

### How does React know to respond to a user’s inputs?

React responds to user inputs through event handlers. Event handlers update component state or trigger actions, leading to UI updates.

### What word indicates that a React component manages data with a Hook?

"useState."

### How can two react components share data?

Data can be shared between React components through props (for parent-to-child communication) and a concept called "state lifting" (for lifting state up from child to parent components). You can also use external state management libraries like Redux or the Context API for more complex scenarios.

## Render and Commit

### What are the three steps of refreshing a React UI?

1. Receive new data: Components receive new data or state.
2. Re-render: Components re-render based on the updated data or state.
3. Update the DOM: React updates the Virtual DOM and compares it with the actual DOM to make efficient changes.

### How do you trigger updates to a component after the initial render?

Updates to a component after the initial render can be triggered by modifying its state using functions like `setState` (in class components) or state update functions (in functional components with Hooks).

### Does React recreate DOM nodes on every rerender?

No, React does not recreate all DOM nodes on every re-render. It uses the Virtual DOM to efficiently update only the necessary parts of the actual DOM.

### After React has updated the DOM, what still needs to happen before the user sees the change?

Before the user sees DOM changes, React performs a process called "committing." During this process, React updates the actual DOM based on changes made to the Virtual DOM. Once the committing process is complete, the user sees the updated UI.
