# Readings: Redux - Combined Reducers

### Multiple Reducers Example

- **Why create multiple reducers?**

  - Creating multiple reducers in Redux is beneficial for managing the complexity of your application's state. Each reducer can handle a specific slice of the overall state, making it more modular and easier to maintain.

- **How would you combine multiple reducers?**

  - You can combine multiple reducers using Redux's `combineReducers` utility function. `combineReducers` takes an object as an argument, where each key-value pair represents a specific slice of the state and its corresponding reducer function.

- **How will you manage state as an immutable object? Why?**
  - In Redux, it is recommended to manage state as an immutable object to ensure predictable behavior and facilitate debugging. When you modify the state, you create a new copy of it with the desired changes instead of directly mutating the existing state. This immutability helps prevent unintended side effects and supports debugging.

### Redux Docs: Using Combined Reducers

- **combineReducers is a utility function to simplify the most common use case when writing **\_ \_\_\_**.**

  - `combineReducers` is a utility function to simplify the most common use case when writing Redux reducers.

- **Explain how combineReducers assembles the new state tree.**

  - `combineReducers` assembles the new state tree by taking an object where each key represents a specific slice of the state and its corresponding reducer function. When an action is dispatched, `combineReducers` calls each reducer with the corresponding slice of the state and the action, then combines the results into a single state object.

- **How would you define initial state in an app using combineReducers?**
  - You can define the initial state for an app using `combineReducers` by providing an initial state object as the second argument to the `createStore` function when setting up your Redux store. This initial state object should have keys corresponding to the slices of the state defined in your reducers.

### Redux Docs: Combined Reducer Syntax

- **Why will you want to split your reducing functions as your app becomes more complex?**

  - As your app becomes more complex, splitting your reducing functions into smaller, focused reducers becomes important for maintainability and scalability. Each reducer should be responsible for a specific part of the application's state, making it easier to reason about and modify the state handling logic.

- **The **\_** helper function turns an object whose values are different reducing functions into a single reducing function you can pass to \_\_\_\_.**

  - The `combineReducers` helper function turns an object whose values are different reducing functions into a single reducing function you can pass to the `createStore` function to create the Redux store.

- **What is a popular convention when naming reducers?**
  - A popular convention when naming reducers is to use descriptive names that reflect the state slice they manage. For example, if you have a reducer managing the user authentication state, you might name it `authReducer`. Using clear and meaningful names helps maintain code clarity and readability.
