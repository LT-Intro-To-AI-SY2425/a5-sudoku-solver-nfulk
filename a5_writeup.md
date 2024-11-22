# Assignment 5 Write up

Assignment 5 can be broken up into the following parts:
1. Import the Necessary Modules:
- `copy`: For creating deep copies of objects
- `Stack` and `Queue`: Custom implementations for DFS and BFS operations
2. Utility Functions: 
- `remove_if_exists`: Removes a specified element from a list if it exists, which is used to remove the possibilites from a cell
3. Board Class:
- Represents the Sudoku board
- Consists of functions that will find the most constrained cell, and update the board, which eliminates possible solutions
4. DFS & BFS Functions:
- `DFS`: Uses depth-first search to solve the Sudoku puzzle. It works by trying to fill the most constrained cell with potential values until a solution is found or backtracks if a mistake is made
- `BFS`: Uses breadth-first search to solve the Sudoku puzzle in a similar fashion to DFS but explores nodes level by level
5. Main Execution:
- Defines two different sets of initial moves for Sudoku puzzles
- Uses both DFS and BFS to solve each puzzle and prints the results


After completing the assignment, answer the following reflection questions:

## Reflection Questions

1. How do the performance and efficiency of the Depth-First Search (DFS) and Breadth-First Search (BFS) algorithms compare when solving Sudoku puzzles? In what scenarios might one approach be preferable over the other? 
DFS uses less memory and is usually faster because it tries one solution at a time, but it can waste time on wrong paths. BFS checks all options step by step, which is safer for finding the correct solution but uses more memory and can take longer.



2. How did the choice of data structures (like the Stack for DFS and Queue for BFS) impact the implementation and functionality of the algorithms? Are there alternative data structures or design patterns that could have been used to achieve the same objectives?

Using a Stack for DFS helps it go deep into one solution at a time, while a Queue for BFS makes it explore all options level by level. Alternatives like a Priority Queue can make BFS smarter by focusing on the easiest cells first, or DFS can use recursion to simplify the code.


3. Considering the current implementation, how might the Sudoku solver be adapted or extended for larger puzzles or different types of grid-based logic games? How can the lessons learned from this assignment be applied to real-world problem-solving or optimization challenges? 
To solve larger puzzles or other grid-based games, the solver could be adapted to handle bigger boards and more rules, like using smarter ways to find the best cell to fill next. This project shows how breaking problems into small steps and using efficient tools, like queues or stacks, can help solve complex challenges in real life, like planning or scheduling tasks.