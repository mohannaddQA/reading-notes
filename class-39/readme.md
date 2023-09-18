# Readings: Redux - Additional Topics

### Redux Toolkit (RTK)

- **What concerns are addressed by Redux Toolkit?**

  - Redux Toolkit addresses concerns related to boilerplate code in Redux applications. It provides a set of tools and utilities to simplify common Redux tasks, such as reducing repetitive code and managing the store's setup.

- **What does `configureStore()` do?**

  - `configureStore()` is a function provided by Redux Toolkit. It simplifies the store configuration process in Redux. It sets up the Redux store with sensible defaults, including setting up the Redux DevTools Extension for easier debugging. Developers can customize the store's behavior by passing an object with configuration options to `configureStore()`.

- **How would I use `createSlice()`?**

  - `createSlice()` is used to create a Redux slice, which is a collection of reducers and actions for a specific part of the state. To use it, you define an initial state object, a set of reducer functions that specify how the state should change, and automatically generate corresponding action creators. Here's a basic example:

    ```javascript
    import { createSlice } from "@reduxjs/toolkit";

    const initialState = {
      value: 0,
    };

    const counterSlice = createSlice({
      name: "counter",
      initialState,
      reducers: {
        increment: (state) => {
          state.value += 1;
        },
        decrement: (state) => {
          state.value -= 1;
        },
      },
    });

    // You can now use counterSlice.reducer and counterSlice.actions in your Redux setup.
    ```

### MobX

- **What is Mobx?**

  - MobX is a state management library for JavaScript applications, primarily used for building reactive user interfaces. It allows you to create observable state objects, which automatically track and update the user interface when the state changes. MobX follows the reactive programming paradigm and offers a simple way to manage complex application states.

- **How does MobX make it “impossible” to produce an inconsistent state?**

  - MobX ensures consistency in application state by enforcing a strict rule: The state can only be modified within MobX-tracked functions. Any change made to the state outside of these functions will not trigger reactivity. This makes it "impossible" to produce an inconsistent state because MobX guarantees that all state changes happen in a predictable and controlled manner.

- **How would we build a reactive user interface?**

  - To build a reactive user interface with MobX, you follow these steps:

    1. Define observable state: Create observable objects or variables to represent your application state.
    2. Create reactions: Define functions or components that react to changes in the observable state.
    3. Modify state: Use MobX actions to modify the observable state.
    4. Observe updates: MobX will automatically update any reactions (UI components) when the observed state changes, ensuring a reactive user interface.

    Here's a simplified example:

    ```javascript
    import { observable, action, autorun } from "mobx";

    // Define observable state
    const appState = observable({
      count: 0,
    });

    // Create a reaction (autorun)
    autorun(() => {
      console.log(`Count: ${appState.count}`);
    });

    // Modify state using actions
    const increment = action(() => {
      appState.count += 1;
    });

    increment(); // This will trigger the autorun and update the UI.
    ```
