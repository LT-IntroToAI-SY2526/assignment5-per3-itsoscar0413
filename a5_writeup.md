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

1. What are some things that you learned through this assignment? Think about the concepts of backtracking, constraint satisfaction, and search algorithms. Were there any particular challenges you faced while implementing the Board class methods or the DFS/BFS functions? How did you overcome them?

### I learned how the search algorithms like DFS or BFS can help solve complex problems that are constraint and involve multiple steps. It further helped me understand backtracking, because especially if you backtracked everything manually it would take a long time, having code to do it both saves time and also allows to see if there's multiple solutions, or if it's just one. When you created the update function, especially because I couldn't run the code due to me being out, it made it a bit harder to interpret the code and understand it's meaning so I had to infer and use logic while readin the code to make it make sense, but it did make sense! And to help further my understanding, when I came back on monday and reviewed the update function, my understanding helped polish those thoughts.

2. How can you apply what you learned in this assignment to future programs or projects? Consider other types of problems that involve searching through possibilities, making decisions, and backtracking when those decisions don't work out. Can you think of real-world scenarios where DFS or BFS might be useful? What about other constraint satisfaction problems?

### Using the idea of backtracking, and mainly BFS, instead of spending time on one long pathway and if it ends up not working then time is wasted, it's better to do it briefly and see if it works or not. Being able to backtrack is extremely crucial in finding errors when something doesn't work. Although DFS is able to find more errors with details, BFS would be more convenient when it comes to doing someting quick like a school assignment or possible career when it comes to orgainzing stuff. But in a real world scenario with time present, DFS is best for finding all possible solutions. 

3. Explain how the Stack and Queue classes work and why they are important for DFS and BFS algorithms. Describe the difference between LIFO (Last In First Out) and FIFO (First In First Out) data structures. How does using a Stack versus a Queue change the way the search algorithm explores possible solutions? Why is one data structure better suited for depth-first search and the other for breadth-first search?

### 1) The stack and queue classes are special data structures that help make the algorithms work, and they're special because it allows the algorithm to do more. 2a) LIFO makes the most recent item added is the next thing to be explored, and it allows the "branch" to be dived deeply before it being removed. 2b) FIFO makes it so the first item added is the one to be explored first, that way it's all viewed briefly before going deeper. 3) Using stack vs queue changes the way the code apporaches the problem it is currently facing when searching for solutions. 4) Stack allows the code to explore possibilities deeply and with detail which alligns with DFS, while queue is brief and broad, and can help find the fastest/minimum path which goes with BFS. 