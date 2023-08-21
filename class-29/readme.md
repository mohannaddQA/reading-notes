# Advanced State with Reducers

## Table of Contents

- [Reading](#reading)
- [Bookmark and Review](#bookmark-and-review)
-

## Reading

#### What is the motivation for adding a reducer?

The motivation for adding a reducer is to manage more complex state logic in a more organized and maintainable way. Reducers are especially useful when dealing with state that has multiple related actions and transitions. By centralizing the state transitions and logic within a reducer function, you can achieve better separation of concerns and make your codebase more predictable.

#### What are actions in the context of a reducer? How are they different than setting state directly?

In the context of a reducer, actions are objects that describe a state change in your application. An action typically includes a `type` property that indicates the type of action being performed, and it can also include additional data relevant to that action. When a component wants to update the state, it dispatches an action to the reducer. The reducer then processes the action and returns a new state based on the action's type and data.

Setting state directly involves directly modifying the state variable within a component using methods like `setState` (in the case of class components) or the `useState` hook (in the case of functional components). This approach can become less manageable as the complexity of your application grows. Using actions and reducers, on the other hand, provides a structured and standardized way to manage state changes and can be particularly beneficial for larger applications.

#### What common list operation is `useReduce` named for, and why?

The `useReducer` hook is named after the common list operation called "reduction." Reduction is a process where you iterate over a collection (such as an array) and accumulate a final result by applying a certain operation to each element. In the context of React and `useReducer`, the "reduction" concept is used to manage state transitions in a more organized manner. By using a reducer function, you can iteratively apply actions to the current state and accumulate a new state, similar to how reduction works on lists.

#### When should you switch from `useState` to `useReducer`?

You should consider switching from `useState` to `useReducer` when your component's state logic becomes more complex, involves multiple actions that can change the state, or when you need to manage state transitions in a more organized and predictable way. `useReducer` is particularly helpful when dealing with state that has intricate logic, branching, or when you want to maintain a clear separation between different aspects of state management. However, for simpler state needs, `useState` might still be sufficient and more straightforward to use.

Remember that the decision to switch from `useState` to `useReducer` depends on the complexity and requirements of your specific application's state management.

## Bookmark and Review

Make sure to bookmark the following resources, as they will provide useful information that is relevant to the lab:

- [useReducer hook](https://reactjs.org/docs/hooks-reference.html#usereducer)
- [Keeping Components Pure](https://reactjs.org/docs/react-api.html#keeping-components-pure)
- [Queueing a Series of State Updates](https://reactjs.org/docs/faq-state.html#queueing-state-updates)
