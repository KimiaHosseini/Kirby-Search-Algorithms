# Kirby-Search-Algorithms

## Project Objective

The main objective of the project is to implement and evaluate several AI search algorithms within a grid environment (Grid World). The character (Kirby) must find an optimal path through this grid to collect stars while avoiding obstacles.

The project aims to demonstrate how different search algorithms perform in terms of time complexity, space complexity, optimality, and their ability to find solutions efficiently. This project is typical of AI courses as it teaches fundamental concepts about search strategies, their advantages, and disadvantages.

## Game Scenario (Grid World)

In the "Grid World" environment, Kirby (the protagonist) moves around a 2D grid. The grid represents a problem space where the task is to find a solution (path) from a start position to one or more goal positions (stars). The game is designed such that obstacles and other challenges must be navigated using AI techniques.
3. Implemented Algorithms

Several classical search algorithms are implemented in this project to solve the problem of navigating Kirby through the grid:

    Depth First Search (DFS): This is a common uninformed search algorithm that explores as far as possible along a branch before backtracking.

    Iterative Deepening Search (IDS): This combines the depth-first approach with a breadth-first approach by gradually increasing the depth limit for search, ensuring optimality like BFS but with reduced memory usage.

    Breadth First Search (BFS): This algorithm explores all possible moves one level at a time, ensuring that the shortest path is always found, though at a higher memory cost.

    Bidirectional Breadth First Search (BBFS): This variant of BFS runs two simultaneous searches from both the start and the goal, meeting in the middle to save time.

    Uniform Cost Search (UCS): An optimal, uninformed search algorithm that expands the node with the lowest cost (i.e., the path with the smallest cumulative cost so far). It’s similar to BFS but accounts for varying step costs.

    Greedy Search: This algorithm uses a heuristic to estimate the distance to the goal and always expands the node that seems closest to the goal, which doesn’t guarantee optimality.

    A*: A heuristic search algorithm that combines the strengths of UCS and Greedy Search. It uses a heuristic to guide its search but ensures that the shortest path is found by balancing the current path cost and the estimated remaining distance.

## Task Setup

The project involves setting up the grid with obstacles and goals. Kirby needs to navigate this grid, and each search algorithm dictates how Kirby explores the grid to reach the stars. Each algorithm is tested for its efficiency, effectiveness, and resource utilization.
5. Evaluation Criteria

The performance of each algorithm is measured using several criteria:

    Optimality: Does the algorithm find the shortest path?
    Time Complexity: How long does the algorithm take to find the solution (usually measured in terms of the number of nodes expanded)?
    Space Complexity: How much memory does the algorithm use (measured by the number of nodes kept in memory)?
    Completeness: Is the algorithm guaranteed to find a solution if one exists?

For example:

    DFS may find a solution quickly in some cases, but it doesn’t guarantee the shortest path and can get stuck in deep branches.
    BFS is guaranteed to find the shortest path but can require significant memory.
    A* combines the best of both worlds by using a heuristic to guide the search and ensuring optimality.

## Reporting and Analysis

In addition to coding the algorithms, the project also involves writing detailed reports. These reports analyze the behavior of each algorithm based on specific problems and scenarios.

For each algorithm, you will:

    Run the algorithm to observe how Kirby moves through the grid.
    Analyze its behavior, such as the number of nodes it visits, the path it takes, and its computational efficiency.
    Compare the performance of algorithms against each other to understand the trade-offs between time, space, and optimality.

For example, one of the reports asks whether DFS behaves rationally in this problem space and if its performance aligns with expected outcomes in terms of space and time complexity.

## Greedy Search and Heuristic Analysis

The reports also dive into heuristic-based search strategies. One such report focuses on Greedy Search and examines whether it always leads to an optimal solution.

Greedy Search uses a heuristic to estimate the closest path to the goal, but it may not always find the best path. The report also discusses what factors influence the performance of Greedy Search and under what conditions it may fail to find the optimal solution.
## Advanced Topics: A* and Optimality

Finally, the project explores more advanced search strategies like A*. A* guarantees optimality if the heuristic function used is admissible (i.e., it never overestimates the true cost to reach the goal).

This part of the project evaluates the use of A* and whether it performs better than UCS or DFS, and under what conditions it is advantageous.
## Coding and Implementation

In terms of implementation:

    The project is written in Python.
    The code includes modules for the grid environment (GridWorld), search algorithms (SearchAlgorithms.py), and the interface to run the simulations (interface.py).
    You need to modify or implement functions in these files, depending on the assignment.
