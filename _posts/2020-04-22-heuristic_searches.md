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

A problem may present an exact solution, but the computational cost can derail the process. For AI problems the optimal solution is rarely required and a __good approximation__ will normally be accepted.

Good heuristics functions are hard to be implemented because its hard to predict with precision the value of a specific solution. Also, in state space searches it isn't always easy, or even possible, to stablish a mathematical value to a change of state.

There are two ways of incorporate heuristic knowledge to a search method:
- Altering the rules: The rules set for a system may not limit itself to the possible actions, but also add a set of "reasonable actions" specified by the author of the rules.
- Evaluation functions: A evaluation function should provide for a specific node on the search process the best possible estimate of this node being in a desired path to the solution. This estimate should be quantifiable.

## Evaluation Function

It is important to state that evaluation functions are not the same thing as heuristic functions. The __evaluation function (f(n))__ measures the cost of a specific node, while the __heuristic function (h(n))__ measures the estimated cost of the cheapest path from the current node to goal node.

An evaluation function is represented by:

- f(n) = g(n) + h(n)
  - g(n) = accumulated cost of state changes up to the current node;
  - h(n) = estimated cost of the current node until the goal state.


## Greedy Algorithms

Greedy algorithm is a term used to define a search algorithm that always tries to move closer to the goal state in every step of the solution. It is possible for the algorithm to tell if the successor node will bring it closer or farther from the solution by using evaluation functions.

### Best-first Search Algorithm

This algorithm is based on the estimation of proximity from the goal state. It __analyzes the current node adjacent nodes and chooses the closest to the goal state__ according to the adjacent nodes evaluation functions.

It is recommended to use the best-first algorithm when there is the possibility do estimate the distances to the goal.




### A* Search Algorithm
