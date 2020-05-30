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

In practical terms, an ANN is nothing more than a mathematical model used when there is the need for modeling a system with incomplete theoretical knowledge to the point of making the traditional systematic modeling unfeasible. The problems that can be solved by artificial neural networks, usually present:

- Variables with unknown relationship or mathematically intractable.
- Multidimensionality.

We can use Artificial Neural Networks to make predictions through sets of values but they are mainly used as a classification tool.

## McCulloch-Pitts Neuron

The very first artificial neuron model used on artificial neural networks was proposed by McCulloch and Pitts in _A logical calculus of the ideas immanent in nervous activity_ on 1943. It assumed that the neuron presents a logical function. The proposed structure was an abstraction of the real neural activity on real neural systems and, although very simple, it was proven extremely versatile and easy to modify. It served as inspiration to most of future connectionist models developed.

![McCulloch-Pitts Neuron](/img/posts_img/mcculloch-pitts-model.gif)

## Perceptron

On 1958, Frank Rosenblatt introduced the concept of perceptron, which is a cognitive model that consists on sensorial units connected to a single layer of McCulloch-Pitts neurons, adding the idea of adjustable synapses.

![Rosenblatt's Perceptron](/img/posts_img/perceptron.png)

- x<sub>n</sub>: input values
- w<sub>n</sub>: it represents the synaptic weights and have the purpose to amplify or attenuate the input from a neuron
- Weighted Summation: represents the sum of all inputs considering their weights.
- Step/Activation Function: the main goal of activation function is to make neural networks non-linear.
- Output: is the result of the activation function applied to the weighted summation

## Layers

Usually layers are classified in three groups:

- Input layer: where inputs are presented to the ANN;
- Middle/Hidden layers: where most of proccessing is done, through the usage of weighted connections;
- Output layer: where the final result is concluded and presented.

### One Middle Layer ANNs

Artificial neural networks that are composed by a single middle layer can be used to solve linearly separable problems, that is, problems that can be separated by a line segment to represent the division of classes.

Like the AND logical function:



### Multilayer Perceptrons

Non linearly separable problems, by the other hand, can be solved by ANNs composed by multilayers perceptrons, that is, ANNs that have more than one hidden layer.

![Rosenblatt's Perceptron](/img/posts_img/multilayer_perceptron.jpeg)

## General procedure for building an ANN

1. Collect input data
- Choose/build a dataset with meaningful data and clean it.

2. Separate input datasets
- Training dataset: This dataset will be used to create the classifier;
- Test dataset: Refers to data used after building the ANN in order to verify its performance.

3. Define the network setup:
- Select the neural paradigm according to the ANN application;
- Define the topology to be adopted, that is, the number of layers, the number of units in each layer, etc;
- Choose the training algorithm.

4. Training:
- The classifier should be created in a way that is capable of describe and distinguish an already know set of classes and values. The predictor is created using a labeled training dataset, that is, the ANN output for each input array is already known.

5. Testing:
- Once the predictor has been created, it is needed to evaluate its performance when applied to data that wasn't used during the training process, known as testing datasets.

## ANN Generalization

Independently of the adopted classifier, it should be trained using a specific training dataset. As a result, the classifier's performance depends on both the number of training examples and the specific values ​​of the examples, that is, the quality of the training dataset.

A classification system should be able to classify future test examples that do not belong to the training dataset. The ability to generalize classifiers refers to its performance when classifying test patterns that were not used during the training stage. 

## Classification evaluation metrics
