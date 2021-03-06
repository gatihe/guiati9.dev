---
layout: post
title: "Artificial Neural Networks"
excerpt: "Introduction to artificial neural networks"
categories: [artificial intelligence]
comments: true
---

## Motivation

When it comes to Artificial Inteligence, the __symbolic approach__, also known as GOFAI (Good old-fashioned AI) is represented by techniques that aims to model the mind with representations (symbols) such as deductive reasoning, logical inference and search algorithms. As a mutual excludent alternative, there is the __connectionist approach__, which gets its name from the typical network topology that most part of its algorithms present. The most commonly technique adopted by the connectionist approach is the usage of Artificial Neural Networks.

Artificial Neural Networks consists of models based on the structure and functions of a  biological neural network. They are considered a nonlinear statistical data modeling tool that presents complex relationships between the input and the output.

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

### Single Layer Perceptrons

Artificial neural networks that are composed by a single middle layer can be used to solve linearly separable problems, that is, problems that can be separated by a line segment to represent the division of classes.

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

The classification evaluation metrics aim to provide a quantitative value of a classifier's quality, most commonly it focuses on estimating the generalization performance, that is, how well the classifier will perform on data not used in training.

### Evaluation Metrics for Binary Problems

The problem is considered binary when the classification output is divided in only two classes (whether something is or isn't some other thing). It is usually associated with the idea of a target class, that is, the class that fits the value that is trying to be predicted.

Some good examples of binary problems are to predict whether the received message is a spam or not, or whether a loan is going to be approved or not. For these examples, the target classes would be , respectively, spam and approved.

The target class is also called __positive class__, which implies the existence of a __negative class__. Both positive and negative classes allow the definition of specific metrics related to each one.

#### True:
- __TP (true positive)__: object classified as positive that really belongs to the positive class.
- __TN (true negative)__: object classified as negative that really belongs to the negative class.

#### False:
- __FP (false positive)__: object classified as positive when it actually belongs to the negative class (it is also known as type 1 error).
- __FN (false negative)__: object classified as negative when it actually belongs to the positive class (it is also known as type 2 error).

A good way to fully present the performance of a binary classification algorithm is to build a matrix that relates the desired classes with the predicted classes.

The __confusion matrix__ (also known as contingency or error matrix) presents the original classes and the predicted classes:


||Predicted positive class|Predicted negative class|
Original positive class|TP|FN
Original negative class|FP|TN

Once the confusion matrix is defined, it gets easier to calculate the __accuracy of the classifier__. The accuracy is represented through the division of the correct classifications by the total of classified items.

- __ACC__ = TP + TN / TP + FP + TN + FN

And the __error rate__ is given by:

- __Error__ = 1 - ACC

It is also possible to determine two other important evaluation metrics, the __true positive rate (TPR)__ and __false positive rate (FPR)__.

- __TPR__ = TP / TP + FN (corresponds to the percentage of positive objects correctly classified as positive)

- __FPR__ = FP / FP + TN (corresponds to the percentage of negative objects incorrectly classified as positive)
