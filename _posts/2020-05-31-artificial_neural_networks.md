---
layout: post
title: "Artificial Neural Networks"
excerpt: "Introduction to artificial neural networks"
categories: [artificial intelligence]
comments: true
---

## Motivation

Artificial Neural Networks are computational models based on the structure and functions of a  biological neural network. They are considered a nonlinear statistical data modeling tool that presents complex relationships between the input and the output.

## How biological neurons works

It is possible to state that the human brain is capable of: adapting through learning, behaving according to context, operating with partial knowledge, presenting high memory capacity, parallel and real-time processing. These abilities are the result of the biological neural networks acting.

The core component of the nervous system and the brain, is the neuron (nerve cell). A neuron can be defined as an electrically excitable cell that is capable of doing synapses (to processes and transmits information by electrochemical signalling).

![Simple biological neuron](/img/posts_img/simple-biological-neuron-scheme.pbm)

More specifically, the synapse occurs when the axon of a neuron and the dendrite of another neuron gather. They are capable of receiving and sending signals incredibly fast and from/to a lot of other neurons

The neuron can be seen as a device capable of receiving an input from several other neurons and propagating its output.

The human brain has about 10<sup>11</sup> neurons and each neuron makes, on average, between one and ten thousand synapses. Being the number of synapses higher than 10<sup>14</sup>, it is possible to say that the biological neural network presents high complexity.

## Definition of Artificial Neural Networks

> "An Artificial Neural Network is a massively parallel and distributed system composed of simple processing units that have a natural ability to store and use knowledge" (Bellman, 1999)

> "A artificial neural network is a circuit composed by a large quantity of simple processing units inspired on the biological neural system." (Nigrin, 1993)

## When to use Artificial Neural Networks

In practical terms, an ANN is nothing more than a mathematical model used when there is the need for modeling a system with incomplete theoretical knowledge to the point of making the traditional systematic modeling unfeasible.

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
