# Pathfinding Visualizer

A client-side web application that visualizes Breadth-First Search (BFS), Depth-First Search (DFS), and Dijkstra's algorithm on a 20x20 grid.

## Live Demo
You can run the visualizer live here: [https://vivanshbajaj.github.io/pathfinding-visualizer/](https://vivanshbajaj.github.io/pathfinding-visualizer/)

## Features

* **Algorithmic Behavior:**
    * **BFS & DFS:** Finds a path from the source to a single destination, rendering the final path in yellow.
    * **Dijkstra's Algorithm:** Solves the Single-Source Shortest Path (SSSP) problem for 3 separate destinations concurrently. Each destination's path is tracked independently and rendered in a unique color (Yellow, Cyan, and Pink).
* **Grid Interactions:**
    * Manual wall allocation via cell clicking.
    * Automated random maze generation using a 28% wall density constraint, automatically skipping start and target nodes.
* **State Locking & Cleanup:** Prevents asynchronous race conditions by disabling the algorithm selector during runtime execution. Interaction with clear or reset triggers clears all active `setTimeout` identifiers to halt ongoing animation queues instantly.

## Tech Stack

* **HTML5:** Dynamic DOM element generation for the grid canvas.
* **CSS3:** Custom `@keyframes` animations to handle the search frontier wave and shortest path highlights.
* **JavaScript (ES6):** Pure vanilla implementation of graph theory algorithms and asynchronous animation loops.

## Local Setup

1. Clone the repository:
   ```bash
   git clone [https://github.com/vivanshbajaj/pathfinding-visualizer.git](https://github.com/vivanshbajaj/pathfinding-visualizer.git)