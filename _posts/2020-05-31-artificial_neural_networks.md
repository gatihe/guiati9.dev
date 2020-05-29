---
layout: post
title: "Artificial Neural Networks"
excerpt: "Introduction to artificial neural networks"
categories: [artificial intelligence]
comments: true
---

## Motivation


## How biological neurons works

The extra information about the problem being solved by the search algorithm is called __heuristic__ and the search methods that use these information are called __heuristic search methods__.

In order to systematically solve complex problems, it usually necessary to build methods that no longer guarantee the optimal solution but that almost always find a very good solution. The reason is that the heuristics usually points to interesting directions but can not provide points of interest for certain contexts.

A problem may present an exact solution, but the computational cost can derail the process. For AI problems the optimal solution is rarely required and a __good approximation__ will normally be accepted.

Good heuristics functions are hard to be implemented because its hard to predict with precision the value of a specific solution. Also, in state space searches it isn't always easy, or even possible, to stablish a mathematical value to a change of state.

There are two ways of incorporate heuristic knowledge to a search method:
- Altering the rules: The rules set for a system may not limit itself to the possible actions, but also add a set of "reasonable actions" specified by the author of the rules.
- Evaluation functions: A evaluation function should provide for a specific node on the search process the best possible estimate of this node being in a desired path to the solution. This estimate should be quantifiable.

## Artificial Neural Networks

It is important to state that evaluation functions are not the same thing as heuristic functions. The __evaluation function (f(n))__ measures the cost of a specific node, while the __heuristic function (h(n))__ measures the estimated cost of the cheapest path from the current node to goal node.

An evaluation function is represented by:

- f(n) = g(n) + h(n)
  - g(n) = accumulated cost of state changes up to the current node;
  - h(n) = estimated cost of the current node until the goal state.


## When to use Artificial Neural Networks

Greedy algorithm is a term used to define a search algorithm that always tries to move closer to the goal state in every step of the solution. It is possible for the algorithm to tell if the successor node will bring it closer or farther from the solution by using evaluation functions.

### Best-first Search Algorithm

This algorithm is based on the estimation of proximity from the goal state. It __analyzes the current node adjacent nodes and chooses the closest to the goal state__ according to the adjacent nodes evaluation functions.

In this case, the node evaluation function is equal to its heuristic function: f(n) = h(n)

It is recommended to use the best-first algorithm when there is the possibility do estimate the distances to the goal.

The Best-First algorithm usually provides __non optimal solution__. Even providing good results, there might be better ones among the possible solutions. Also, it is considered a __non complete solution__ once it can enter a loop state if it doesn't detect repeated nodes, meaning that it may not even find a solution.

## McCulloch-Pitts Neuron

The A* Algorithm evaluates nodes combining the cost to reach each node (g(n)) and the estimate cost to go from that node to the goal node (h(n)).

- f(n) = g(n) + h(n)
  - g(n) = accumulated cost of state changes up to the current node;
  - h(n) = estimated cost of the current node until the goal state.

In order to find the cheapest solution, the algorithm select the nodes with the lowest value of f(n).

This algorithm works with two list of states: _Open_ and _Closed_:

- The open list is a priority queue and it stores nodes that haven't been visited yet or that present some enhancement on total cost.
- The closed list stores already visited states.

A* Algorithm:

1. Consider P as the initial state.
2. Calculate _f_, _g_ and _h_ for P.
3. Add P to _open_ list (By this point P is the only element on this list).
4. Being M the best node from OPEN_LIST (lowest _f_):
  - __If__ M is equal to goal state, __then__ finalize and return path.
  - __If__ OPEN_LIST is empty, __then__ finalize and return error.
5. To each C node connected to M (successors list):
  - Calculate _f_, _g_ and _h_ for C.
  - __If__ C is not in OPEN_LIST or CLOSED_LIST __then__ add C to OPEN_LIST.
  - __If__ C is in OPEN_LIST or CLOSED_LIST and presents the lowest cost __then__  remove C from OPEN_LIST or CLOSED_LIST and add C to OPEN_LIST.
6. Move M from OPEN_LIST to CLOSED_LIST and head back to step 4.




## Perceptron

### Weighs

### Activation functions


## ANN Architecture

## Single Layer ANNs

## Nonlinearly separable classifications

## Multilayer perceptron

## How to build an ANN

## Classification evaluation metrics
