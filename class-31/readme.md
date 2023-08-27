### Choosing the State Structure

#### Summarize the five principles for structuring state.

1. **Single Source of Truth:** Store state in a central location to avoid inconsistencies.
2. **Structured for Components:** Organize state based on component hierarchy.
3. **Immutable State:** Keep state unmodifiable and create new instances when updates are needed.
4. **Derive State:** Compute complex state from existing state to avoid redundancy.
5. **Minimize State:** Keep state minimal to improve performance and reduce bugs.

### Passing State Deeply with Context

- What problem do Contexts aim to solve?
  Contexts solve the issue of prop drilling, where props are passed through many levels of components.
- What is one technique to try before `useContext`?
  Before using `useContext`, leverage component nesting hierarchy to place components needing shared state closer to the top of the tree.
- What hook complements `useContext` for complex applications?
  The `useReducer` hook complements `useContext` for managing more complex state logic.

## Bookmark and Review

Keep these pages handy - they answer questions that show up regularly for this lab.

- [Sharing State Between Components](https://react.dev/learn/sharing-state-between-components)
- [Preserving and Resetting State](https://react.dev/learn/preserving-and-resetting-state)
