# ComaMaze

A Julia implementation for generating, solving, and visualising mazes using graph theory principles.


**Overview**

* **Maze Generation:** Creates random mazes by finding a spanning tree on a grid graph using a randomised Depth-First Search (DFS) algorithm.
* **Pathfinding Solver:** Solves the generated maze using the **Right-Hand Rule** based on local wall boundaries.
* **Terminal Visualisation:** Visualises the maze grid and the computed solution path directly in the terminal via custom `Base.show` overloads.


**Project Structure**

* **`src/MazeGeneration.jl`**: Main module entry point and exported functions.
* **`src/core.jl`**: Contains the `Node` and `Maze` data structures alongside basic graph constructions.
* **`src/solver.jl`**: Implements the maze solver using the Right-Hand Rule.
* **`src/visualize.jl`**: Handles terminal rendering routines and overloads `Base.show`.


**Usage Example**

```julia
using ComaMaze

m = maze(5,5)
solve(m)
