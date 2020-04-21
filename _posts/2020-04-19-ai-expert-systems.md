---
layout: post
title: "Expert Systems and Inference Methods"
excerpt: "Approaching basic AI topics, such as Turing Tests and the Chinese Room Argument."
categories: [artificial intelligence]
comments: true
---



## Definition:

We call a *human expert* someone with the knowledge to solve high difficulty problems in a specific knowledge field. An __Expert System__ is a computer software that represents and simulates the knowledge of a specialty field in order to solve problems and provide recommendations.

## Characteristics:

An ES is a software that behaves as some expert in a, usually restrict, application domain. This kind of system should be able to solve problems that requires specific knowledge of a specific domain.

There are good reasons to consider simulating an human experts, once they are expensive, rare, busy, emotional and mortal.

Expert systems have a very broad application, such as:

- (Medicine) Decision support:
  - Application of standardized diagnostic methods such as interpretation of test results.

- (Medicine) Quality Assurance:
  - Audit medical decisions such as the need of some sort of procedure.

- (Agriculture) Diagnostic:
  - Expert system to identify diseases, plagues and physiological disturbs on grapevine crops.

### Pros of Expert Systems:

- Present the ability of explaining inference process.
- Present uniform structure. Each rule is an independent piece of the available knowledge.
- By separating it's knowledge from its processing, it is possible that the same project environment could be applied on different applications.

### Cons of Expert Systems:

- Work mainly with only symbolic reasoning.
- Aspects as ambiguities and conflicting rules can result on wrong results. 

## Expert Systems Architecture:

![Expert Systems Architecture](/img/posts_img/es_architecture.png)

#### Knowledge base:

The knowledge base is where the expert systems store sets of knowledge representation. It formally represents the knowledge of an specific specialty field. It represents the knowledge with pairs of condition-action (if-then).

  | If | Then |
  -----|-----
  |Condition (or premise)|action (result or conclusion)|
  |Light is green|go foward|

  The knowledge stored in the knowledge base is represented through __facts__ (incontestable knowledge) and __rules__ (conditional facts).

- Facts:
  - Men are mammal.
  - Whales are mammals.
  - Men are mortal.

- Rules:
  - __If__ animal_has_legs(x) and animal_has_beak(x), __then__ animal is bird(x).
  - __If__ temperature_over_37_degrees(x), __then__ has_fever(x).

##### Rules sintax:

- __and__: all conditions must be met for the consequents execution.
- __or__: only one of the conditions met is enough for the consequents execution.
- __not__: denial of predicate.
- __then__: establishes the consequence of the rule to be applied.

#### Working Memory:

Working memory is where facts are stored. It represents the data that are presented to the system by the beginning and during the inference.

#### Inference Engine:

The Inference Engine applies problem resolution procedures, deciding how and in which order the rules will be applied and facts will be used.

##### Foward Chaining
##### Backward Chaining

#### Interface

It is represented by the interaction with the user. There are two kinds of interface:

- Input interface: consists of input data that will provide resources to the working memory.
- Output interface: consists of the solutions and diagnostics provided. An expert system must be capable of showing its inference process and justifying its conclusions.

#### Shell

It is called shell the module composed by the expert system's inference engine and interfaces.

## Expert Systems Classification

- Interpretation: this type of ES is capable of inferring situations through the evaluation of input data like images, signals and others, via sensors. A good example would be medical systems that monitor blood pressure, heart beat, body temperature and etc.

 - Prognostic: simulate and infer probable consequences of specific scenarios. Systems that can predict demand of oil through the current geopolitical context or predict a city infrastructure damage from an earthquake.

 - Diagnostic: infer probable causes of an specific scenario. Like diseases diagnosis through symptoms.

 - Planning: they are systems able to elaborate action strategies before actions are taken. Systems that are capable to plan the production line of a factory are a good example.

 - Monitoring: systems that compares the behavior of real systems with expected ones. Example: a system that tracks data from a nuclear reactor in order to detect possible accident situations.
