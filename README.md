# Real-Time Pathfinding Visualizer

A high-performance, browser-native pathfinding engine built to visualize classic graph traversal and shortest-path algorithms. The environment dynamically adapts its structure, constraints, and rendering layers based on the selected algorithm.

## 🚀 Live Demo
Experience the pipeline live on the web: 
👉 [https://vivanshbajaj.github.io/pathfinding-visualizer/](https://vivanshbajaj.github.io/pathfinding-visualizer/)

## 🛠️ Core Engineering Features

- **Dynamic Grid Environment:** Runs a responsive 20x20 matrix with automated obstacle distribution (28% density system maze generator) while maintaining deterministic layout boundaries.
- **Asynchronous Execution Architecture:** Employs a background tracking array (`animationTimeouts`) that strictly locks down user dropdown controls mid-run, preventing event-loop race conditions. 
- **Algorithm Configurations:**
  - **BFS / DFS (Single-Target Model):** Hard-locked to 1 Start (Green) and 1 End (Red) node, tracing the single shortest path in clean **Yellow**.
  - **Dijkstra's Algorithm (Multi-Target SSSP Tree):** Scales seamlessly to 1 Start and 3 separate End points, executing parallel backtracking vectors to animate isolated routes concurrently using distinct color pipelines (**Yellow, Electric Cyan, and Neon Pink**).

## 🧰 Tech Stack
- **Structure:** HTML5 (Native DOM node generation)
- **Styling & Animations:** CSS3 (GPU-accelerated custom `@keyframes` for structural wave fluids)
- **Engine Logic:** Vanilla JavaScript (ES6+ asynchronous timers and matrix relaxation logic)

## 💻 Running Locally
1. Clone the repository:
   ```bash
   git clone [https://github.com/vivanshbajaj/pathfinding-visualizer.git](https://github.com/vivanshbajaj/pathfinding-visualizer.git)