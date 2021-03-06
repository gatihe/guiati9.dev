---
layout: post
title: "Fuzzy Logic and Production Rules"
excerpt: "Fuzzy set theory, membership functions, fuzzification and production rules"
categories: [artificial intelligence]
comments: true
---

## Introduction

While applying classical logic to solve problems it is possible to identify that it values bivalent analysis (the objects used are either true or false), that is, it presents low tolerance with limit values that end up being excluded. But the real life requires multivalent thinking in order to be better studied, it isn't 'all black and white'.

Some examples that enforce the concept of multivalent approach are:
- In judicial matters, a judge and the jury must consider the degree of guilt of an accused depending on the laws and evidence against the accused;
- Classification of healthy patients;
- Classification of objects as 'large';
- Classification of people as 'tall'.

*Fuzzy logic* aims to capture different degrees of truth that exists in real life. Some formal definitions are:

> Fuzzy logic is capable of combining the inaccuracy associated with natural events and the computational power of machines to produce systems with smart, robust and flexible results. - COX, Earl. Fuzzy logic for business and industry - 1995

>Fuzzy logic allows the development of systems that represents human decisions, to which the conventional (boolean) math and logic is proven to be insufficient or inefficient. - VON ALTROCK, Constantin. Fuzzy logic and neuroFuzzy applications in busines and finance - 1996

It is possible to tell if a concept is fuzzy or not if it should not be defined in an extreme way. Concepts like 'healthy', 'depressed' and 'tall' are good examples, once there are not only 'tall' and 'not tall' people in the world. There are degrees of certainty (or doubt) to which people can be classified as 'tall' or 'not tall'.

The Fuzzy Logic was first proposed by Zadeh, who demonstrates this concept through the Fuzzy Set Theory.

## Classical Set Theory

Formal representations of the Set Theory:

- Set: set of objects that shares some common specific characteristic. According to Classical Set Theory a object can only present two different relationship with a set, that is, it may or may not be an element of the set.

- Membership: An element _x_ is an element of set A: x E A.

- Characteristic function: Establishes the membership relationship between an element _x_ and a set A.

Being A a set and f its characteristic function:
```
f(x) =  { 1 if x E A}
        { 0 if x ˜E A}
```
A is also formally represented as:

A = {x E X \| f(x) = 1}

And the characteristic function A(x) (or f(x)) is represented by:

f(x): X -> {0,1}

Graphically, f(x) is given by:

![f(x) Graph](/img/posts_img/fxgraph.png)

## Fuzzy Set Theory

By the previous classical set representations, it is possible to identify a sudden change of values (0 to 1) with no transition values (values between 0 and 1). This behavior makes it harder to capture real life situations. Fuzzy logic proposes a different approach to mitigate this limitation.

Fuzzy sets allow its elements to interact with them in multiple ways (more ways that 'belongs' and 'does not belong').

A fuzzy set A defined on a domain X is defined by a membership function f<sub>A</sub> which maps elements of X for the range [0,1].

A: Fuzzy Set

X: Domain

A: X -> [0,1] or A = {x E X \| A(x) = 1}

__Membership function__: f<sub>A</sub>(x): X -> [0,1]

This way, the membership function designates, to each element x that belongs to X, a real number to f<sub>A</sub>(x) from the range [0,1]. The result represents element's x membership degree to set A, that is, how much possible is it for x element to belong to the A set.



### Types of Membership Functions

```
f(x) : X -> [0,1],
- f(x) = 0,
- 0 < f(x) < 1
f(x) = 1
```

##### Triangular Membership Function

```
f(x) = {0 if x<=a}
       {(x-a)/(m-a) if x E [a,m]}
       {(b-x)/(b-m) if x E[m,b]}
       {0 if x >= b}

```
![Triangular Graph](/img/posts_img/triangular_function.png)

##### Trapezoidal Membership Function

```
f(x) = {0 if x <- a}
       {(x-a)/(m-a) if x E [a,m]}
       {1 if x E [m,n]}
       {(b-x)/(b-n) if E [n,b]}
       {0 if x >= b}
```

![Trapezoidal Graph](/img/posts_img/trapezoidal_function.png)

##### Example:

### Linguistic Variables

A linguistic variable is a variable whose default values are words rather than numbers. It is represented by the elements:
- X: variable name
- T(X): Set of values assumed by variable X.

Every linguistic values form a set of terms.

Example:

Being X = age
T(age) = {Young, very young, mature, old, sort of old, child}

or

X:temperature
T(temperature) = {high, medium, low}

Each one of T(x) values represents a __fuzzy set__ with a membership function associated to it.

### Fuzzification

Fuzzification is the process of creating fuzzy sets. It consists on:

1. Find a concept to be fuzzified.
2. Convert concept into a linguistic variable.
3. Designate reasonable linguistic variables to this variable.
4. Each one of the values is a fuzzy set defined by its own membership function.

##### Logical operations with fuzzy sets

- Union:

Being A and B two fuzzy sets:

The membership function that represents the union between two fuzzy sets is given by __f<sub>AUB</sub>(x) = max {f<sub>A</sub>(x),f<sub>B</sub>(x)__ or __f<sub>AUB</sub>(x) = f<sub>A</sub>(x) U f<sub>B</sub>(x)__.

- Intersection:

Being A and B two fuzzy sets:

The membership function that represents the intersection between two fuzzy sets is given by __f<sub>A∩B</sub>(x) = min {f<sub>A</sub>(x), f<sub>B</sub>(x)}__ or __f<sub>A∩B</sub>(x) = f<sub>A∩B</sub>(x) = f<sub>A</sub>(x) ∩ f<sub>b</sub>(x)__.

## Production Rules

In a fuzzy system the knowledge is represented through fuzzy rules (or propositions). Fuzzy rules are statements that relates the variables to fuzzy sets.

A rule is given by __Antecedent -> Consequent__, being:

- __Antecedent__: one or more clauses linked through fuzzy operators (AND, OR, NOT).
- __Consequent__: the conclusion.

The difference of statements from the symbolic to connectionist logic is that the antecedent and the consequent are now __linguistic variable__ values. As per example:

If __blood_pressure__ is __high__ and __individual_age__ is __elder__;
Then __health_insurance_cost__ is __very_high__

Being the linguistic values:

- blood_pressure(b) = {low, average, high}
- indiviual_age(i) = {young, adult, elder}
- heal_insurance_cost = {low, average, high, very high

The fuzzy reasoning, which simulates human characteristics, is executed through inference, which allows drawing conclusions based on known facts.

### Steps to Create Fuzzy Production Rules

1. Create linguistic variables;
2. Choose domain values to the input linguistic variables;
3. Choose domain values to the output linguistic variable;
4. Associate fuzzy sets to each variable;
5. Create membership functions to each varaiable
6. Define fuzzy rules
