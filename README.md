# Graph Traversal (DFS and BFS): Implementation & Time Analysis

A Jupyter notebook implementing and analyzing **Depth-First Search (DFS)** and **Breadth-First Search (BFS)** on a graph in Python, using an adjacency-list representation.

## Features
- Simple `Graph` class using an adjacency list (undirected)
- DFS implemented both recursively and iteratively (explicit stack)
- BFS implemented iteratively (queue-based)
- Interactive user input for building a custom graph (edges + starting node)
- Real runtime measurement using Python's `time` module
- Time and space complexity analysis for both algorithms
- Graph visualizations (via `networkx`/`matplotlib`) showing traversal order
- Bonus: BFS-based shortest path (fewest edges) between two nodes in an unweighted graph
- Runtime comparison on random graphs of increasing size (100 to 20,000 nodes), with a line chart

## Getting Started
1. Clone the repo
2. Install dependencies: `pip install jupyter matplotlib networkx`
3. Open `graph_dfs_bfs_analysis.ipynb` in Jupyter Notebook, JupyterLab, or Google Colab
4. Run the cells top to bottom — demo cells use a sample graph by default; swap in `get_user_edges()` / `get_user_start_node(nodes)` (no arguments) to build and traverse your own graph

## Complexity Summary

| Algorithm | Time Complexity | Space Complexity | Data Structure Used | Guarantees Shortest Path (unweighted)? |
|-----------|--------------------|---------------------|------------------------|--------------------------------------------|
| DFS       | O(V + E)            | O(V)                 | Stack (or recursion)   | No                                          |
| BFS       | O(V + E)            | O(V)                 | Queue                  | Yes                                         |

Where `V` = number of vertices (nodes), `E` = number of edges.

Both algorithms visit every vertex and edge exactly once, giving the same asymptotic `O(V + E)` time complexity. Use DFS for deep exploration, cycle detection, or topological sorting; use BFS when you need the shortest path in an unweighted graph or level-by-level exploration.

## License
MIT
