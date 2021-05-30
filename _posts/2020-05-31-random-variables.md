---
layout: post
title: "Random Variables and Probability Distribution"
excerpt: "Discrete and continuous random variables, probability distribution and some solved exercises"
categories: [statistics]
comments: true
---

Approaching basic AI topics, such as Turing Tests and the Chinese Room Argument.

## Definitions

Artificial Intelligence is an area of Computer Science that studies systems that simulate the human ability to reason, perceive, make decisions and solve problems. In other words, the ability to be intelligent. There are some formal definitions for AI such as:

> "[Automation of] activities related to the human thinking, activites such decision making, problem solving, learning..." (Bellman, 1956)

>"The study of mental faculties through the use of computational models" (Charniak and McDermott, 1985)

>"The study of systems that make it possible to perceive, reason and act" (Winston, 1992)

>"AI can be defined as the branch of Computer Science in charge to automate intelligent behavior" (Luger, 2004)

As we can see, AI can have multiple definitions and it may depend on which way it is going to be approached. The following content to be posted here will adopt the following definition:

> Multidisciplinary science that applies computing techniques that simulate intelligent behavior on specific activities.

## AI Paradigms

Since there is no established unifying theory or paradigm that guides AI research and development due to different points of view of researchers, there are some paradigms that are more common and usual.

* Symbolic: Knowledge representation is based on symbols. Good examples are: Expert Systems, Logical Agents, Fuzzy Logic
* Connectionism: Knowledge representation is based on how the brain works. Good examples are: Artificial Neural Nets
* Bio-Inspired: Knowledge representation is based on the simulation of behaviors found in nature. Good examples are: Genetic algorithms, Collective Intelligence, RNA.

It is not unusual to see more than one AI paradigm being applied to solve one single problem. The technique of mixing paradigms is called __Soft Computing__. The most frequent resources combined to solve problems are neural nets, fuzzy logic, bio-inspired computing and other intelligent algorithms.

## Applications

AI techniques can be used for multiple purposes, some of the most known of them are:

* Product Recommendation: - How to make custom product recommendations? How to shape buyers profiles based on navigation and shopping data?
* Web Searches: - How to locate and identify relevant information according to users searches?
* Gaming: - How to design appropriate characters behaviors? How to allow an interesting interaction with the player?

## Turing Test

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

#### Strong AI x Weak AI

This test says that if a computer software could execute tasks in a way that an expert couldn't distinguish it's performance from an human's performance, then the software would have the same capability to learn as a human has.

Some researchers say that this software wouldn't just be a model of the human mind, it would be literally a mind (__Strong AI__). This idea is not a unanimity on AI, a much more reasonable approach suggests that it consists of computers modeling and studying the human mind the same way computers can study weather, statistics or economy (__Weak AI__).

* __Strong AI:__ This approach suggests that a computer software that knows how do execute tasks just as well done as humans could, is in fact playing the role of the human mind.
* __Weak AI:__ Considers AI just a branch of Computer Science like any other.

## The Chinese Room Argument

Let's consider an unknown language to a random person, such as the Chinese. To this person, the language is merely a set of symbols without any meaning.

This person is put on a room with baskets filled with symbols that represent the Chinese language. Consider that there is also a book written in the person native language that contains rules to compose the symbols and assemble sentences in Chinese. This book indicates the rules through the shape of the symbols and does not require any logical thinking about the symbols. Therefore, to understand the book the person only needs to identify the symbols and understand how to put them together to make sentences.

In order to communicate, people fluent in Chinese from outside of the room also manipulate symbols to ask the person inside the room questions.

Even assuming that the person inside the room presents answers undistinguishable from someone who speaks Chinese, it isn't possible to state that this person really learned how to communicate in Chinese. After consulting the book of rules, the person might be able to understand the questions asked and even answer them, but this person completely ignores the Chinese idiom. Learning Chinese through this book is not possible once the meaning of the symbols were not presented on it.

A parallel with a computer would be: the software is represented by the book of rules, the baskets containing the symbols are the database, the symbols used by the people outside the room are the user input, and the symbols returned by the person in the room are represents the output interface.

The main concept of this argument that opposes to Strong AI is that if someone can't understand Chinese following only an algorithm, so the capability of manipulating symbols presented by a computer also doesn't mean that the computer "understands" Chinese. It is possible to say that computers only handles formal symbols according to the rules presented on the software.

The idea presented by the Chinese Room Argument can also be applied to other forms of cognition. __The ability to handle symbols is no guarantee of cognition, perception and understanding__ and since computers are no more than symbols handlers, the act of running a software doesn't imply cognition.

Weak AI suggests that computers can simulate some performances in specific areas in a very similar way to the humans but it doesn't make them possessors of "intelligence".
