---
layout: figure-side
figureUrl: /agent-society.png
figureCaption: Scenario of an envisioned society composed of AI agents, in which humans can also participate.
---

# Introduction

A general framework for LLM-based agents, comprising three main components: brain, perception, and action.

- AI agents are artificial entities that sense their environment, make decisions, and take actions.

- Actually, what the community lacks is a general and powerful model to serve as a starting point for designing AI agents that can adapt to diverse scenarios.

- Due to the versatile capabilities they demonstrate, large language models (LLMs) are regarded as potential sparks for Artificial General Intelligence (AGI), offering hope for building general AI agents.


---

# Background

## Origin of AI Agent

**Agent in philosophy.**

- In a general sense, **an “agent” is an entity with the capacity to act, and the term “agency” denotes the exercise or manifestation of this capacity**. While in a narrow sense, “agency” is usually used to refer to **the performance of intentional actions**; and correspondingly, the term “agent” denotes entities **that possess desires, beliefs, intentions, and the ability to act**. Note that agents can encompass not only individual human beings but also other entities **in both the physical and virtual world**. Importantly, the concept of an agent involves **individual autonomy**, **granting** them the ability to exercise volition, make choices, and take actions, **rather than passively reacting to external stimuli**.

---
hideInToc: true
---
## Origin of AI Agent

**From the perspective of philosophy, is artificial entities capable of agency?**

- In a general sense, if we define agents as **entities with the capacity to act**, AI systems do exhibit a form of agency. However, the term agent is more usually used to refer to entities or subjects that possess consciousness, intentionality, and the ability to act.

- With the advancement of language models, the potential emergence of artificial intentional agents
  appears more promising. In a rigorous sense, language models merely function as **conditional probability models**, using input to predict the next token.
  Different from this, **humans incorporate social and perceptual context, and speak according to their mental states**.

---
hideInToc: true
---
## Origin of AI Agent

**Introduction of agents into AI**. 

- In the realm of Philosophy, an agent can be a human, an animal, or even a concept or entity with autonomy. 
  However, in the field of artificial intelligence, an agent is a **computational entity**. 
  Due to the seemingly metaphysical nature of concepts like consciousness and desires for computational entities, 
  and given that we can only observe **the
  behavior of the machine**, many AI researchers, including Alan Turing, suggest temporarily setting
  aside the question of whether an agent is “actually” thinking or literally possesses a “mind”.
- Instead, researchers employ other attributes to help describe an agent, such as properties of autonomy,
  reactivity, pro-activeness and social ability.
  There are also researchers who held that intelligence is “in the eye of the beholder”; it is not an innate, isolated property.

- In this paper, we treat AI agents as artificial entities that are capable of perceiving their surroundings using sensors, making decisions, and then taking actions in response using actuators.

---
hideInToc: true
---

## Technological Trends in Agent Research

- Symbolic Agents.
- Reactive agents.
- Reinforcement learning-based agents.
- Agents with transfer learning and meta learning.
- Large language model-based agents.

As large language models have demonstrated impressive
emergent capabilities and have gained immense popularity, researchers have started to leverage these models to construct AI agents. Specifically, they employ LLMs as the
primary component of **brain** or **controller** of these agents and expand their perceptual and action space
through strategies such as **multimodal perception and tool utilization**. These LLM-
based agents can exhibit **reasoning and planning abilities** comparable to symbolic agents through
techniques like **Chain-of-Thought (CoT) and problem decomposition**.
They can also acquire **interactive capabilities with the environment**, akin to reactive agents, by
learning from feedback and performing new actions. Similarly, large language
models undergo pre-training on large-scale corpora and demonstrate the capacity for **few-shot and zero-shot** generalization, allowing for seamless transfer between tasks without the need to update
parameters.

---
hideInToc: true
---

## Why is LLM suitable as the primary component of an Agent’s brain?

- **Autonomy.**
- **Reactivity.**
- **Pro-activeness.**
- **Social ability.**
