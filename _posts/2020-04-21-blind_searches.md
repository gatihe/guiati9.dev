---
layout: post
title: "Search Trees and Blind Search Algorithms"
excerpt: "Main concepts of blind search algorithms."
categories: [artificial intelligence]
comments: true
---

## Search Trees

As discussed earlier, in order to solve state space problems, rational agents follow search algorithms that adopt different methodologies to explore the state space and reach it's goal. The procedure of searching in a state space problem generates as an output a search tree. The shape of this tree depends on the algorithm adopted to solve the problem.

### Search Tree Structure

Search trees are composed by associated nodes that are represented by:

- Current state,
- Pointer to previous node,
- Cost of getting to current state (this value is calculated according to the search algorithm logic applied)

![Representation of two connected nodes of a Search Tree](/img/posts_img/node_representation.png)

### Nodes notation

Adopting mathematical notation, nodes are represented by an array:
- n<sub>i</sub> = (e<sub>i</sub>, p<sub>i</sub>, g<sub>i</sub>), where:
  - e<sub>i</sub> is the current state;
  - p<sub>i</sub> is the previous node to node n<sub>i</sub>;
  - g<sub>i</sub> represents the cost.

## Blind Searches

Blind searches are searching algorithms that do not use any information besides the available information on the problem definition. They start in a specific state, generate successors, check if goal state was reach and, if it wasn't, try again using the same logic.

Some characteristics of blind searches are:
 - They can only distinguish a 'non-goal state' from a 'goal state'.
 - They are used when there is no additional information about the space to be covered.
 - They distinguish themselves by the order in which nodes are expanded.

## Breadth-first Search (BFS) Algorithm

On BFS, all adjacent nodes from the initial node are expanded and so on. Here is the **algorithm** to create a BFS tree:

1. Identify initial state;
2. Set initial state as the search tree root;
3. Describe node (insert current state, previous state and path cost to current state);
4. If initial state is equal to goal state then stop tree construction;
5. Visit all adjacent states from the initial state and add them to the tree until there is no more adjacent states from initial state (always filling up node information and __checking__ if current node is equivalent to goal state).
6. Visit all adjacent nodes to the first state adjacent to the initial state and repeat the process until you reach the goal state or until the states end.

### Calculating the Cost of State Changes with BFS

When talking about blind searches, changes of state will always present cost 1 to all changes. That means that the change of states costs presents the same value for all adjacents of the current node.

![Cost of State Changes](/img/posts_img/state_change_cost.png)

### Example

![Romanian Map Represented as a Graph](/img/posts_img/romanian_map.jpg)

### BFS pros

- BFS will never reach a dead-end.
- If there is a solution, BFS will, certainly, find it.
- If there is more than one solution, a minimal solution (the one that requires the fewest steps) will be found. This characteristic is guaranteed by the fact that the longest paths are only explored after the shortest ones have been examined.

## Depth First Search Algorithm

On Depth First Search Algorithm, the nodes are explored with priority for the successors of the last node added to the tree. It begins e continues on a same path until a dead-end is found. This search method behaves according to the following algorithm:

1. Initialize tree by the initial state;
2. Find first adjacent state from current state;
3. **If** there is no adjacent state **then**:
  - return failure;
  - restart depth first search considering previous state as initial state;
4. **Else**:
  - _If_: adjacent is equal to goal state _then_: add state to the tree, exit and return the solution.
  - _Else_: Add state to the tree.
5. Make visited adjacent state the current state.
6. Repeat algorithm.

### Backtracking and State Changes Cost Calculation

![Cost of State Changes on Depth First Search](/img/posts_img/depth_first_cost_example.png)
### Depth First pros
