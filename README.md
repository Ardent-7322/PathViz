# PathViz

Welcome to PathViz! I built this application because I was fascinated by pathfinding algorithms, and I wanted to visualize them in action. I hope you enjoy playing around with this visualization tool as much as I enjoyed building it. You can access it here (use Google Chrome!): [PathViz](https://github.com/Ardent-7322/PathViz/tree/master).

## Meet the Algorithms

This application supports the following algorithms:

### Dijkstra's Algorithm (weighted)
- **For Everyone:** Think of Dijkstra's Algorithm as the ultimate GPS. It always finds the shortest route from your starting point to your destination.
- **Technical Details:** It guarantees the shortest path by exploring all possible routes in a weighted graph where each edge has a cost.

### A* Search (weighted)
- **For Everyone:** A* Search is like a GPS with a sense of direction. It finds the shortest path faster by guessing which routes might be quicker.
- **Technical Details:** It uses heuristics (educated guesses) to speed up the process, combining the cost to get to the node and an estimate of the cost to get to the destination.

### Greedy Best-first Search (weighted)
- **For Everyone:** This algorithm is like a person who always takes the road that looks the most promising without considering if it’s the best overall route.
- **Technical Details:** It prioritizes nodes that seem to lead directly to the target, based on heuristics, but it doesn’t guarantee the shortest path.

### Swarm Algorithm (weighted)
- **For Everyone:** Imagine a group of ants spreading out from the start and converging towards the food source. That’s how the Swarm Algorithm works.
- **Technical Details:** It mixes Dijkstra's thoroughness with A*’s heuristic approach, exploring around the start and converging towards the target without guaranteeing the shortest path.

### Convergent Swarm Algorithm (weighted)
- **For Everyone:** Similar to the Swarm Algorithm, but it moves even faster by heavily relying on guesses about the best routes.
- **Technical Details:** It’s a more heuristic-heavy version of the Swarm Algorithm, trading some accuracy for speed.

### Bidirectional Swarm Algorithm (weighted)
- **For Everyone:** Imagine ants starting from both the start and the food source, meeting in the middle. That’s the Bidirectional Swarm.
- **Technical Details:** It applies the Swarm Algorithm from both ends, speeding up the process but not guaranteeing the shortest path.

### Breadth-first Search (unweighted)
- **For Everyone:** This method checks all possible routes layer by layer. Think of it as exploring all streets in a neighborhood before moving to the next layer.
- **Technical Details:** It guarantees the shortest path in an unweighted graph by exploring all nodes at the present "depth" before moving on to nodes at the next depth level.

### Depth-first Search (unweighted)
- **For Everyone:** This is like someone who picks a path and follows it until they hit a dead end, then backtracks to try another path.
- **Technical Details:** It explores as far as possible along each branch before backtracking, which doesn’t guarantee the shortest path and can be inefficient for pathfinding.

## Maze Generation

In addition to pathfinding algorithms, I implemented a **Recursive Division** Maze Generation algorithm:
- **For Everyone:** This method creates a maze by repeatedly splitting areas into smaller sections with walls, similar to how you might divide a room using partitions.
- **Technical Details:** It works by recursively splitting the grid and adding walls with gaps, creating a complex maze structure.

## More about the Swarm Algorithm

The Swarm Algorithm is a unique method co-developed with my colleague, Hussein Farah. It blends Dijkstra's methodical exploration with A*'s heuristic guidance:
- **For Everyone:** It balances exploring nearby areas and moving towards the goal, much like a character in a video game tracking a boss while keeping an eye on nearby enemies.
- **Technical Details:** The algorithm updates nodes' distances from the start while considering their estimated distance to the target, forming a triangle-like search pattern. We named it "Swarm" due to its potential application in video games for managing multiple targets and threats.
