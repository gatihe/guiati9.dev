---
layout: post
title: "Heuristic Searches"
excerpt: "Main concepts of blind search algorithms."
categories: [artificial intelligence]
comments: true
---

## Motivation

Although blind searches are very useful, these algorithms provides only a single way to expand nodes and search a solution for finding a way to the goal state. In many cases, applying these methods are impractical due to the high quantity of nodes to be expanded before finding a solution (the bigger the state space, the greater the complexity).

When talking about search algorithms, solution is defined as a path from the initial state to the goal state. An __optimal solution__ is the one that presents the lower cost of all the existent solutions.

Search algorithms can have its performance measured by:
- Completeness: the ability to provide a solution if it exists.
- Optimality: the ability to find an optimal solution.
- Time Complexity: time spent to find a solution.
- Space (Storage) Complexity: needed memory to find a solution.

## Heuristics

The extra information about the problem being solved by the search algorithm is called __heuristic__ and the search methods that use these information are called __heuristic search methods__.

In order to systematically solve complex problems, it usually necessary to build methods that no longer guarantee the optimal solution but that almost always find a very good solution. The reason is that the heuristics usually points to interesting directions but can not provide points of interest for certain contexts.

Good heuristics functions are hard to be implemented because its hard to predict with precision the value of a specific solution. Also, in state space searches it isn't always easy, or even possible, to stablish a mathematical value to a change of state.

## Evaluation Function

## Greedy Algorithms

### Best-first Search Algorithm

### A* Search Algorithm
