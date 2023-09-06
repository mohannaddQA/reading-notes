# Redux

#### 1. First Principle of Redux

The first principle of Redux is that the entire application state is stored in a single JavaScript object called the "state tree" or simply the "store." This store is the single source of truth for the entire application, making it easy to access and manage the state of the application.

#### 2. Store and Reducers

- **What is a Store?**: In Redux, a "store" is a JavaScript object that holds the entire state of your application. It represents the current state of your application's data.

- **Reducers**: Reducers are pure functions used within the store to specify how the state should change in response to actions. They take the current state and an action as arguments and return a new state based on the action. Reducers ensure that the state is updated in an immutable way.

#### 3. `createStore` Methods

`createStore` provides several methods to interact with the store:

- `getState()`: Used to retrieve the current state from the store. It returns the current state object.

- `dispatch(action)`: Dispatches actions to the store, triggering reducers to update the state based on the action's type and payload.

- `subscribe(listener)`: Registers a callback function to be called when the state in the store is updated. Useful for reacting to state changes.

#### 4. `combineReducers()`

Explain to a non-technical recruiter what `combineReducers()` does and why it is useful:

`combineReducers()` is a utility function that combines multiple reducer functions into a single reducer. Each reducer typically manages a different part of the application state, making code organization and maintenance easier. It modularizes state management and improves scalability.
