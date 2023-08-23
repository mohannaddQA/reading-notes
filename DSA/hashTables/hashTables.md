# | HASH TABLE |

### Analogy

Think of a hash table as a magical recipe book in a library's kitchen. Each recipe has a unique name (key) and lists ingredients and instructions (values). To find a recipe quickly, you don't search the whole book; instead, you consult the index, which lists the page number where each recipe is. This index is created using a secret code (hash function) that converts recipe names into page numbers.

### Definition

A hash table is a data structure that stores key-value pairs, allowing efficient insertion, retrieval, and deletion. It uses a hash function to map keys to indices in an array. This enables quick access to values based on their keys.

### Operations

- Insertion: Add a new key-value pair to the hash table.
- Lookup: Retrieve the value associated with a given key.
- Deletion: Remove a key-value pair from the hash table.

### Key Concepts

- Hash Function: A mathematical function that converts keys into indices within the array.
- Hash Collisions: When two different keys map to the same index due to the limited number of indices. Various techniques handle collisions.
- Buckets: The array slots where key-value pairs are stored. Multiple pairs can be in the same bucket.
- Load Factor: The ratio of occupied buckets to the total number of buckets, which affects efficiency.
- Chaining: A collision resolution technique where each bucket contains a linked list of key-value pairs.
- Open Addressing: A collision resolution technique where collisions are resolved by placing items in the next available slot.

### Common Applications

- Databases: Indexing and data retrieval.
- Caches: Fast access to frequently used data.
- Language Interpreters: Storing variables and their values.

### Hash Table Implementation

Hash tables can be implemented using arrays and linked lists.

- Arrays hold the buckets, where each bucket can hold multiple key-value pairs.
- Linked lists inside buckets manage collisions.

### Time Complexity

The time complexity of hash table operations is usually O(1) on average.

- Insertion: O(1) on average (can degrade to O(n) in worst cases).
- Lookup: O(1) on average (can degrade to O(n) in worst cases).
- Deletion: O(1) on average (can degrade to O(n) in worst cases).

### Visualization:

![visualization](./vis.png)
