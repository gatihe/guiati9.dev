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
- Pointer to antecessor node,
- Cost of getting to current state (this value is calculated according to the search algorithm logic applied)

![Representation of two connected nodes of a Search Tree](/img/posts_img/node_representation.png)

### Nodes notation:

Adopting mathematical notation, nodes are represented by an array:
- n<sub>i</sub> = (e<sub>i</sub>, p<sub>i</sub>, g<sub>i</sub>), where:
  - e<sub>i</sub> is the current state;
  - p<sub>i</sub> is the antecessor node to node n<sub>i</sub>;
  - g<sub>i</sub> represents the cost.

## Breadth-first Search (BFS) Algorithm

### Backtracking

### Breadth-first pros

## Depth First Search Algorithm

### Depth First pros
