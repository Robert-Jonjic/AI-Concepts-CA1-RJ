
# Pathfinding Algorithms Comparison

This project compares three pathfinding algorithms—Breadth-First Search (BFS), Dijkstra's Algorithm, and A*—for finding the most efficient path from **Tipperary** to **Sligo** using a weighted graph of Irish cities. Each algorithm provides timing statistics to measure efficiency.

## What’s in the Jupyter Notebook

The notebook contains:
1. **Graph Setup**: Defines cities as nodes and distances as edges.
2. **Algorithm Implementations**:
   - **BFS** for shortest unweighted path.
   - **Dijkstra's Algorithm** for shortest weighted path.
   - **A* Algorithm** for optimized pathfinding with heuristic guidance.
3. **Testing and Results**: Compares the path and execution time of each algorithm.

## Table of Contents

- [Graph Setup](#graph-setup)
- [Algorithms Implemented](#algorithms-implemented)
- [Results](#results)
- [Conclusion](#conclusion)
- [Requirements](#requirements)
- [How to Run](#how-to-run)

## Graph Setup

The graph is represented as a dictionary, with heuristic values for A* providing straight-line distance estimates to Sligo.

## Algorithms Implemented

- **BFS**: Simple path search without considering edge weights.
- **Dijkstra's**: Finds the shortest weighted path using a priority queue.
- **A\***: Optimizes pathfinding with heuristics for faster searches.

## Results

| Algorithm   | Path                                           | Time (seconds)           |
|-------------|------------------------------------------------|---------------------------|
| **BFS**     | `['Tipperary', 'Limerick', 'Galway', 'Castlebar', 'Sligo']` | 1.7e-05                  |
| **Dijkstra**| `['Tipperary', 'Limerick', 'Galway', 'Castlebar', 'Sligo']` | 9.55e-05                 |
| **A\***     | `['Tipperary', 'Limerick', 'Galway', 'Castlebar', 'Sligo']` | 5.33e-05                 |

## Conclusion

Each algorithm produced the same path, with BFS being the fastest in this setup, followed by A*, and Dijkstra's being slightly slower.

## Requirements

- **Python 3.x**
- **Jupyter Notebook**
- Basic libraries: `time`, `queue`

## How to Run

1. **Install Jupyter Notebook** (if not already installed):
   ```bash
   pip install jupyter
   ```

2. **Clone or Download the Repository**:
   ```bash
   git clone <repository-url>
   ```
   Navigate to the folder containing `CA1_pathfinding_comparison.ipynb`.

3. **Start Jupyter Notebook**:
   ```bash
   jupyter notebook
   ```
   This opens Jupyter in your browser. Open the notebook and select **Run All** from the **Cell** menu to execute all cells.

4. **View Results**: Observe paths and timings printed in the output cells for each algorithm.

---

This README.md provides an overview of the project, the setup, and clear instructions on running the notebook.
