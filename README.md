# Search-Algorithms-in-a-Dynamic-Environment

This project involved creating different agents to navigate through mazes filled with ghosts. The mazes were generated using numpy.random, with probabilities assigned to each cell to be blocked or unblocked. The agents' survivability was evaluated based on their ability to reach the goal without being killed by ghosts. These agents at their core utilized search algorithms like BFS, DFS, A-Star Search, Bi-Directional Search based on the kind of environment they were tackling.

Agent 1 used a simple Depth First Search (DFS) algorithm to find a path from the start node to the goal. However, it did not consider the presence of ghosts and had low survivability.

Agent 2 improved upon Agent 1 by using BFS for planning the shortest path. It would replan if a ghost appeared in its path. The survivability of Agent 2 increased compared to Agent 1, but it required multiple searches and its efficiency depended on the presence of ghosts.

Agent 3 attempted to simulate Agent 2 but encountered issues with utility calculation and the wiggle problem, where it kept oscillating between two neighbors. Agent 3 performed worse than Agent 2 in terms of survivability.

Agent 4 aimed for survivability and replanned its path whenever a ghost was adjacent to its potential step. It prioritized ghost positions over path efficiency, resulting in better survivability compared to Agent 2.

Agent 5 was similar to Agent 4 but lacked knowledge of ghosts in the walls. However, this did not significantly impact its survivability, as the chances of ghosts in adjacent cells were low.

In summary, Agent 4 performed the best among the agents, prioritizing survivability over path efficiency. Agent 2 showed improved survivability compared to Agent 1 but required multiple searches. Agent 3 had issues with utility calculation and encountered the wiggle problem. Agent 5 was similar to Agent 4 but lacked knowledge of ghosts in the walls, which did not significantly affect its performance.

**Please refer to the **GhostMazeProject.pdf** for full description of this project.**
