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

#### Interface

It is represented by the interaction with the user. There are two kinds of interface:

- Input interface: consists of input data that will provide resources to the working memory.
- Output interface: consists of the solutions and diagnostics provided. An expert system must be capable of showing its inference process and justifying its conclusions.

#### Shell

It is called shell the module composed by the expert system's inference engine and interfaces.

## Production Rule Systems:

During World War II, the Germans developed and used a machine called Enigma to encrypt military instructions. The cryptography of this machine was earlier considered unbreakable.
Later, Polish mathematicians were able to first break the cryptography of Enigma's in a very particular operation mode. Alan Turing's ideas made it possible to generalize this method in a way that any encrypted message from Enigma could be decrypted.

With the help of sophisticated statistical models he developed, Turing also designed a machine to automate the process of decrypting these messages, the Bombe machine.
On 1950, Turing published an article called "Computing Machinery and Intelligence" that studies the concept of intelligence on artificial systems and tries to define __when is it possible to consider that an artificial system does really possess intelligence__. He also proposed what later would become the Turing Test, which evaluates the ability of a machine to behave with intelligence just as an human being.

The movie "Imitation Game" represented it as a test played by three people, a man (A), a woman (B) and an interrogator (C). The interrogator stays in a room apart from the man and the woman and has the goal to determine which one of them is the man and which one is the woman. The man and woman are known by the interrogator as labels "X" and "Y" and the interrogator is allowed to make questions to "A" and "B" by the end of the game he must correctly associate "Y" and "X" to "A" and "B".

Turing suggests that in this game, one of them (apart from the interrogator) should be replaced with a machine. A good performance in this test is defined by the difficulty to tell the difference between the interactions and to point which one is the machine.

Every year, Cambridge University offers the Loebner Prize, where people are chosen to interact with other people and also computer softwares and try to identify when aren't they interacting with a software. The Turing Test criteria may vary once software may also vary (chatbots, games, etc). Turing has also predicted that by the year 2000 machines would easily pass this kind of tests.

In order to pass the Turing Test, the software would have to present the following abilities:
* Natural language processing
* Knowledge representation
* Automated reasoning
* Machine learning

\*The Turing Test avoids physical interaction so it can focus on it's intelligence. The "Total Turing Test" includes video signal to test the software's perception and also allow objects manipulation (robotics).

### Inference Mechanism:

### Foward Chaining
### Backward Chaining

This test says that if a computer software could execute tasks in a way that an expert couldn't distinguish it's performance from an human's performance, then the software would have the same capability to learn as a human has.

Some researchers say that this software wouldn't just be a model of the human mind, it would be literally a mind (__Strong AI__). This idea is not a unanimity on AI, a much more reasonable approach suggests that it consists of computers modeling and studying the human mind the same way computers can study weather, statistics or economy (__Weak AI__).

* __Strong AI:__ This approach suggests that a computer software that knows how do execute tasks just as well done as humans could, is in fact playing the role of the human mind.
* __Weak AI:__ Considers AI just a branch of Computer Science like any other.

## Expert Systems Classification

- Interpretation: this type of ES is capable of inferring situations through the evaluation of input data like images, signals and others, via sensors. A good example would be medical systems that monitor blood pressure, heart beat, body temperature and etc.

 - Prognostic: simulate and infer probable consequences of specific scenarios. Systems that can predict demand of oil through the current geopolitical context or predict a city infrastructure damage from an earthquake.

 - Diagnostic: infer probable causes of an specific scenario. Like diseases diagnosis through symptoms.

 - Planning: they are systems able to elaborate action strategies before actions are taken. Systems that are capable to plan the production line of a factory are a good example.

 - Monitoring: systems that compares the behavior of real systems with expected ones. Example: a system that tracks data from a nuclear reactor in order to detect possible accident situations.

## Pros and Cons
