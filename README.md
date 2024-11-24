# CI2024_lab3
Solve efficently a generic n^2-1 (also known as Gem Puzzle, Boss Puzzle, 15 puzzle, etc.) using path-search algorithms.  
Quality: number of actions in the solutions.  
Cost: total number of actions evaluated.  
Efficiency: Quality vs. Cost.  

## Implementation
The lab has been solved using the A* algorithm. The Manhattan distance, that is an admissible heuristic, is used: it assumes tiles can move directly to their goal positions without being blocked by other tiles but, in reality, some moves might require additional steps so the actual cost is always greater than or equal to the Manhattan distance.  
The problem is created by starting from the solution and applying a sequence of random actions, ensuring that it remains solvable.
## Performance
The quality should always align with the lowest achievable solution for each problem.
The cost can vary significantly depending on the specific problem. 
On my hardware, 3x3 grids are typically solved in just a few seconds. For 4x4 grids, the process can take up to ~20 minutes (using 10.000 `RANDOMIZE_STEPS`). Grids of 5x5 or larger require significantly more time to solve.
