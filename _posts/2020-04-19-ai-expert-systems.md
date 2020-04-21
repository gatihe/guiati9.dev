---
layout: post
title: "Expert Systems and Inference Methods"
excerpt: "Approaching basic AI topics, such as Turing Tests and the Chinese Room Argument."
categories: [artificial intelligence]
comments: true
---



## Definition:

We call a *human expert* someone with the knowledge to solve high difficulty problems in a specific knowledge field. An *Expert System* is a computer software that represents and simulates the knowledge of a specialty field in order to solve problems and provide recommendations.

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

## Expert Systems Components:

- Knowledge base
- Work memory
- Inference engine
- Interface

## Expert Systems Architecture:

AI techniques can be used for multiple purposes, some of the most known of them are:

* Product Recommendation: - How to make custom product recommendations? How to shape buyers profiles based on navigation and shopping data?
* Web Searches: - How to locate and identify relevant information according to users searches?
* Gaming: - How to design appropriate characters behaviors? How to allow an interesting interaction with the player?

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

A parallel with a computer would be: the software is represented by the book of rules, the baskets containing the symbols are the database, the symbols used by the people outside the room are the user input, and the symbols returned by the person in the room are represents the output interface.

The main concept of this argument that opposes to Strong AI is that if someone can't understand Chinese following only an algorithm, so the capability of manipulating symbols presented by a computer also doesn't mean that the computer "understands" Chinese. It is possible to say that computers only handles formal symbols according to the rules presented on the software.

The idea presented by the Chinese Room Argument can also be applied to other forms of cognition. __The ability to handle symbols is no guarantee of cognition, perception and understanding__ and since computers are no more than symbols handlers, the act of running a software doesn't imply cognition.

Weak AI suggests that computers can simulate some performances in specific areas in a very similar way to the humans but it doesn't make them possessors of "intelligence".
