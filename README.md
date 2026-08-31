# ComaMaze

A Julia package for generating, visualizing, and solving random mazes as spanning trees on grid graphs.
---

## Features

* **Maze Generation:** Creates $M \times N$ mazes via randomized depth-first search (DFS) to build random spanning trees.
* **Maze Solver:** Solves generated mazes using the **Right-Hand Rule** based on local wall information.
* **Terminal Visualization:** Custom `Base.show` overloading to visualize mazes and solution paths directly in the terminal.

---

## Project Structure

```text
ComaMaze/
├── Project.toml
├── Manifest.toml
└── src/
    ├── MazeGeneration.jl  # Main module & exports
    ├── core.jl            # Node & Maze structs, graph logic
    ├── solver.jl          # Right-Hand Rule maze solving algorithm
    └── visualize.jl       # MazeViz struct & terminal rendering
