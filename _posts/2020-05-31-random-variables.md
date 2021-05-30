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
