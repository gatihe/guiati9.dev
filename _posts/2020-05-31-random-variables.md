---
layout: post
title: "Random Variables and Probability Distribution"
excerpt: "Discrete and continuous random variables, probability distribution and some solved exercises"
categories: [statistics]
comments: true
---

The result of a probabilitic expirement can often be a count or a measure. When that occurs, its result is called a random variable.

There are two types of random variables:

- The *discrete random variables* handle values that can be counted, that means, there is a finite (or countable) number of possible results that can be counted.

- *Continuous random variables* can assume any value inside a range, that means, there are countless possible results represented through a range.

## Discrete random variables

### Discrete probability distribution

It is possible to assign a probability to each value of a discrete variable. By enumerating each value of the random variable with its corresponding probability, a probability distribution is formed.

*Definition:* A discrete probability distribution enumerates each value the random variable can take, along with its probability. A probability distribution must satisfy the following conditions: 1) A probability of each value of the discrete variable must be within the range of 0 to 1, i.e, 0 <= P(X=x) <= 1; 2) The sum of all probabilities must be equal to 1, i.e, ![Sum of probabilities](/img/posts_img/random-variables/sump.png)


For example: A company keep daily track of the number of sales of their new employees during a trial period of one hundred days. The results for a new employee are represented below in a frequency table.

| Sales per day (x) | Number of days (Frequency) | **Probabilities (P(X=x))** |
| 0 | 16 | 0.16 |
| 1 | 19 | 0.19 |
| 2 | 15 | 0.15 |
| 3 | 21 | 0.21 |
| 4 | 9 | 0.09 |
| 5 | 10 | 0.10 |
| 6 | 8 | 0.08 |
| 7 | 2 | 0.02 |
| Total | 100 | 1 |

The usual form to represent the cumulative distribution function is:
![Sum of probabilities](/img/posts_img/random-variables/distfun.png)

### Mean, Variance and Standard Deviation for discrete random variables

- The mean or mathematical expectation of a discrete random variable is given by:
![Mathematical Expectation](/img/posts_img/random-variables/mean.png)

- The variance of a discrete random variable is:
![Variance](/img/posts_img/random-variables/variance.png)

- The standard deviation is obtained by the square root of the variance, i.e,
![Standard Deviation](/img/posts_img/random-variables/stdtion.png)

#### Properties of the mathematical expectation:

1. Property 1. If X = c, where c is a constant, then E(X) = c
2. Property 2. Assume that c is a constant and X is a random variable. Then E(c * X) = c * E(X).
3. Being X and Y two random variables, then E(X+Y) = E(X) + E(Y)
  1. If Y = aX + b, where a and b are constants, then E(Y) = aE(X) + b. That means the expected value of a linear function of X.
  2. For n random variables X1, X2, ..., Xn. Then E(X1+X2+...+Xn) = E(X1) + E(X2) + ... + E(Xn).

#### Properties of the variance:

1. Property 1: If c is a constant, then Var(X+c) = Var(X).
2. Assume that c is a constant and X is a random variable. Then Var(cX) = cˆ2 * Var(X).
3. If (X, Y) is a two-dimentional random variable, and if X and Y are independent. Then Var(X+Y) = Var(X) + Var(Y).
