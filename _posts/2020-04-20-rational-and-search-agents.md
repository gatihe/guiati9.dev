---
layout: post
title: "Rational and Search Agents"
excerpt: "Approaching basic AI topics, such as Turing Tests and the Chinese Room Argument."
categories: [artificial intelligence]
comments: true
---


# Rational Agents

## Definition:

>A **agent** is any entity that is capable of perceiving its environment through sensors, execute data and knowledge processing tasks and acts on it through effectors - Russel & Norvig, 2004.

A _human agent_ has eyes, ears, and other organs as sensors, and also have hands, legs, mouth and other body parts that are considered effectors. A _robotic agent_ could have cameras, signal or wave detects acting like sensors and engines as effectors.

A generic agent is composed by:
- Perceptions: Originated from the environment and captured by agents through its sensors.
- Sensors: Mechanisms that allows the agent to capture perceptions.
- Environment: Domain which agent interacts with.
- Actions: Tasks that effects the environment, based on perceptions and executed by the agents.
- Effectors: Allow the agent to execute its actions.
- Performance: Success measure instrument of an agent.

Rational agents present 'rationality', which can be defined as the fulfillment of the performance criteria according the ambient, possible actions and its perceptions.

To each sequence of perceptions, a rational agent should do what would maximize its performance measure, based on its set of perceptions, knowledge and sequence of actions.

Racionality depends of, at least, four items:
- Performance measure that defines the success rate of the agent.
- All of what the agent has already perceived, or perceptual history.
- Knowledge of the environment.
- Actions for the agent to execute.

A rational agent acts by updating its memory through perception (gathering all knowledge available about the environment) then evaluating, according to its memory, the best action to be taken and, finally, acting. The pseudocode below shows a function that describes the rational agent generically:

```
def agent(perception):
    memory = []
    memory = update_memory(memory, perception)
    action = choose_best_action(memory)
    return action
```


## Applications of Rational Agents:

|Agent type|Performance measurement|Environment|Sensors|Effectors|
|-----|-----|-----|-----|-----|
|Medical Diagnosis Systems|Healthy pacient, lower costs|Pacient, hospital, team|Keyboard input for symptoms, findings and pacient answers|Output questions, diagnostics|
|Satelite image analysis system|Correct assumption of image category|Broadcast link of orbiting satelite|Arrays of colors in pixels|Output image categorization|
|Piece selection robot|Percentage of pieces inside correct trays|Running machines with pieces, trays|Camera, articulated angular sensors|Articulated arm and hand|


## Types of Rational Agents:

#### Simple Reactive Agent:

The simple reactive agent choose its actions according to its current perception, completely ignoring the past perceptions (perception history). It is the simplest kind of agent once it has very limited intelligence.

#### Reactive Agent with Internal State:

This kind of agent is able to store its perception history, environment representations, interaction history and the earlier actions history, which makes it possible to use information beyond the current perception.

#### Goal-based Agent:

Goal-based agents have, as their most important characteristic, the need to be set to accomplish a goal. So, it is capable of storing information just like reactive agents with internal state, but the actions have as a parameter reaching an specific goal and should only stop when the goal is accomplished. It works until an previously set condition is reached.

#### Utility-based Agent (_optimizer_):

This type of agent works based on a sense of utility. It also has goals and the ability to store and process information, but its actions are affected on the idea choosing, from a set of predicted possible futures, the best one according to its goal and also prioritize goals (in case there is more than one).

#### Learning Agent

Learning agents are capable of acquire knowledge while facing new contexts (combinations of environment conditions and perceptions). In order to act, a learning agent will perceive the environment with sensors, compare the current environment and learn from its differences and similarities and, only then, act.
