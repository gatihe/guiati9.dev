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



## Application of Rational Agents:

|Agent type|Performance measurement|Environment|Sensors|Effectors|
|_____|_____|_____|_____|_____|
|Medical Diagnosis Systems|Healthy pacient, lower costs|Pacient, hospital, team|Keyboard input for symptoms, findings and pacient answers|Output questions, diagnostics|
|Satelite image analysis system|Correct assumption of image category|Broadcast link of orbiting satelite|Arrays of colors in pixels|Output image categorization|
|Piece selection robot|Percentage of pieces inside correct trays|Running machines with pieces, trays|Camera, articulated angular sensors|Articulated arm and hand|
||||||
||||||
