---
layout: figure-side
figureUrl: /Conceptual_framework_of_LLM-based_agent.png
figureCaption: 'Conceptual framework of LLM-based agent with three components: brain, perception, and action.'
---

# Construction of LLM-based Agents

Serving as the controller, the brain module undertakes basic tasks like memorizing, thinking,
and decision-making. The perception module perceives and processes multimodal information from the external environment,
and the action module carries out the execution using tools and influences the surroundings.

---
hideInToc: true
---

- The brain is the core of an AI agent because it not only stores knowledge and memories
  but also undertakes indispensable functions like information processing and decision-making. 
  It can present the process of reasoning and planning, and cope well with unseen tasks, exhibiting the intelligence of an agent.
- The perception module: Its core purpose is to broaden the agent’s perception space from a text-only domain to a multimodal sphere that
  includes textual, auditory, and visual modalities. This extension equips the agent to grasp and utilize
  information from its surroundings more effectively.
- The action module designed
  to expand the action space of an agent. Specifically, we empower the agent with embodied
  action ability and tool-handling skills, enabling it to adeptly adapt to environmental changes, provide
  feedback, and even influence and mold the environment.

---
layout: two-cols
---

## Brain

- Natural Language Interaction
  - High-quality generation
  - Deep understanding
- Knowledge
  - Knowledge in LLM-based agent
    - Pretrain model
    - Linguistic knowledge
    - Commensense knowledge
    - Actionable knowledge
  - Potential issues of knowledge
    - Edit wrong and outdated knowledge
    - Mitigate hallucination

::right::

- Memory
  - Memory capability
    - Raising the length limit of Transformers
    - Summarizing memory
    - Compressing mem-ories with vectors or data structures
  - Memory retrieval
    - Automated retrieval
    - Interactive retrieval
- Reasoning & Planning
  - Reasoning
  - Planning: Plan formulation、Plan reflection
- Transferability & Generalization
  - Unseen task generalization
  - In-context learning
  - Continual learning


---
hideInToc: true
---

Operating mechanism. To ensure effective communication, the ability to engage in natural language interaction is 
paramount.

After receiving the information processed by the perception
module, the brain module **first turns to storage, retrieving in knowledge and recalling from memory.**
These outcomes **aid the agent in devising plans, reasoning, and making informed
decisions.**

Additionally, the brain module **may memorize the agent’s past observations, thoughts, and actions 
in the form of summaries, vectors, or other data structures.**

Meanwhile, it can also **update the knowledge such as 
common sense and domain knowledge for future use.**

The
LLM-based agent may also adapt to unfamiliar scenarios with its inherent generalization and transfer ability. 

---
layout: two-cols
---

## Perception

- Textual Input
- Visual Input
  - Visual encoder
  - Learnable architecture
    - Query based
    - Projection based
- Auditory Input
  - Cascading manner
  - Transfer visual method
- Other Input

::right::

In the future, they could perceive and understand diverse modalities in the real world, much like humans.
For example, agents could have unique touch and smell organs, allowing them to gather more detailed information 
when interacting with objects. At the same time, agents can also have a clear sense of the temperature,
humidity, and brightness in their surroundings, enabling them to take environment-aware actions. 
Moreover, by efficiently integrating basic perceptual abilities like vision, text, and light sensitivity,
agents can develop various user-friendly perception modules for humans.

---

## Action

- Textual Output
- Tools
  - Learning tools
  - Using tools
  - Making tools
- Embodied Action
  - LLM-based Embodied actions
  - Prospective to the embodied action

---
hideInToc: true
---

### Embodied Action
In the pursuit of Artificial General Intelligence (AGI), 
the embodied agent is considered a pivotal paradigm while it strives to integrate model intelligence 
with the physical world.

_The Embodiment
hypothesis_ draws inspiration from the human intelligence development process, posing that an
agent’s intelligence arises from continuous interaction and feedback with the environment 
rather than relying solely on well-curated textbooks.

Instead, they should be capable of **actively perceiving, comprehending, and interacting with physical environments**, 
making decisions, and generating specific behaviors to modify the environment 
based on LLM’s extensive internal knowledge. 
We collectively term these as embodied actions, which enable agents’ ability to interact with 
and comprehend the world in a
manner closely resembling human behavior.

---
hideInToc: true
---

The potential of LLM-based agents for embodied actions.

- Cost efficiency
- Embodied action generalization
- Embodied action planning

Embodied actions for LLM-based agents.

- Observation
- Manipulation
- Navigation

Prospective future of the embodied action. LLM-based embodied actions are seen as the bridge
between virtual intelligence and the physical world, enabling agents to perceive and modify the environment much like humans.

- high costs of physical-world robotic operators and the scarcity of embodied datasets