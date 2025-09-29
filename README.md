# Stack in C++
## Name: Maitraiyee Vashistha
## PRN: 24070123057
## Division: ENTC-A3
## Title: Understanding Stack in C++
-----

## Aim
To study the concept of Stack in C++ and implement operations like **push**, **pop**, and **display**.

## Tools Used
- GNU g++ compiler (local compilation)  
- Any online C++ compiler (e.g., Programiz, GeeksforGeeks IDE)  

---

## Theory

### Stack – Definition
A **Stack** is a linear data structure that follows the **LIFO (Last-In, First-Out)** principle.  
- The **last element inserted** into the stack is the **first one to be removed**.  
- It is similar to a stack of plates: the last plate placed on the stack is the first one taken off.  

### Basic Operations
1. **Push** – Adds an element to the top of the stack.  
2. **Pop** – Removes the element from the top of the stack.  
3. **Peek/Top** – Returns the top element without removing it.  
4. **Display** – Shows all elements in the stack from top to bottom.  

### Representation
- A stack can be implemented using:  
  - **Arrays** (static stack, fixed size).  
  - **Linked Lists** (dynamic stack, flexible size).  

- A variable `top` is used to track the index of the last inserted element.  
- Initial value: `top = -1` (empty stack).  

### Memory Storage
- Array-based stacks require **contiguous memory**.  
- Linked-list-based stacks store elements in **non-contiguous memory**, connected by pointers.  

### Stack Behavior
- **Overflow** occurs if a push operation is attempted on a full stack.  
- **Underflow** occurs if a pop operation is attempted on an empty stack.  

---

## Applications of Stacks
- **Expression Evaluation & Conversion** (Infix to Postfix/Prefix).  
- **Function Calls / Recursion** (Call stack).  
- **Undo/Redo Operations** in text editors.  
- **Balanced Parentheses Checking** in compilers.  
- **Depth-First Search (DFS)** in graph algorithms.  

---

## Algorithm

1. **Start**  
2. Define a class `Stack` with array and `top` index.  
3. Initialize `top = -1` (empty stack).  
4. **Push Operation**:  
   - If `top >= MAX - 1` → Overflow.  
   - Else increment `top` and insert value.  
5. **Pop Operation**:  
   - If `top < 0` → Underflow.  
   - Else remove element and decrement `top`.  
6. **Display Operation**:  
   - Traverse array from `0` to `top` and print elements.  
7. In `main()`, perform multiple push and pop operations.  
8. **End**  

---

## Conclusion
Stacks are simple yet powerful data structures that strictly follow the **LIFO principle**.  
Using arrays, we can efficiently implement push, pop, and display operations, while handling overflow and underflow.  
They are widely used in **expression evaluation, function call tracking, undo/redo operations, and graph algorithms**, making them fundamental in computer science.
