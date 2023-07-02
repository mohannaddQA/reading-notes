# | STACK |

### analogy

Imagine you have a bunch of plates that you need to store one on top of the other. You want to put the newest plate on top and take the newest one off the stack when you need it. But there's a catch - you can only add or remove plates from the top. This simple idea of organizing plates can help us understand the concept of stacks in computer science.

### Definition:

linear data structure that follows the "Last In, First Out" (LIFO) principle. It means that the last item added to the stack is the first one to be removed. Just like the plates, we can only add or remove elements from the top of the stack.

### Operations:

- Push: Add an element to the top of the stack.
- Pop: Remove the top element from the stack.
- Peek (or Top): View the top element without removing it.

### Key Concepts:

- The top of the stack refers to the last element that was added.
- New elements are added on top, and the most recently added element is always at the top.
- Elements can only be added or removed from the top of the stack.

### Common Applications:

- Undo/Redo operations in text editors.
- Back and forward buttons in web browsers.

### Stack Implementation:

Stacks can be implemented using <b>arrays<b> or <b>linked lists<b>.

- Arrays provide efficient random access but have a fixed size.
- Linked lists allow dynamic resizing but require extra memory for node pointers.

### Time Complexity:

- Push: O(1) (constant time complexity)
- Pop: O(1) (constant time complexity)
- Peek: O(1) (constant time complexity)

### Visualization:

![stack](./stack1.png)

### Remember:

The last element added is the first one to be removed (Last In, First Out).
