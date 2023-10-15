---
layout: two-cols
---

# Agents in Practice: Harnessing AI for Good

- Single Agent Deployment
  - Task-oriented Deployment
    - Web scenarios
    - Life scenarios
  - Innovation-oriented Deployment
  - Lifecycle-oriented Deployment
- Multi-Agents Interaction
  - Cooperative Interaction
    - Disordered cooperation
    - Ordered cooperation
  - Adversarial Interaction

::right::

- Human-Agent Interaction
  - Instructor-Executor Paradigm
    - Education
    - Health
    - Other Applications
  - Equal Partnership Paradigm
    - Empathetic Communicator
    - Human-Level Participant

---
layout: figure
hideInToc: true
figureUrl: /Scenarios_of_LLM-based_agent_applications.png
---


---
hideInToc: true
---

As an LLM-based agent, its design objective should always be beneficial to humans,
i.e., humans can **_harness AI for good_**. Specifically, we expect the agent to achieve the following
objectives:

1. Assist users in breaking free from daily tasks and repetitive labor, thereby Alleviating human work pressure and enhancing task-solving efficiency.
2. No longer necessitates users to provide explicit low-level instructions. Instead, the agent can independently analyze, plan, and solve problems.
3. After freeing users’ hands, the agent also liberates their minds to engage in exploratory and innovative work, realizing their full potential in cutting-edge scientific fields.

---
layout: figure
figureUrl: /Practical_applications_of_the_single_LLM-based_agent_in_different_scenarios.png
---

## General Ability of Single Agent

---
hideInToc: true
---

### Task-oriented Deployment

In task-oriented deployment, the agent follows high-level instructions from users, 
undertaking tasks such as goal decomposition, sequence planning of sub-goals, 
interactive exploration of the environment, until the final objective is achieved.

---
hideInToc: true
---

### Innovation-oriented Deployment

However, in a more intellectually demanding field, like cutting-edge science, the potential of agents has not been fully realized yet. This limitation mainly arises from
two challenges:
- On one hand, the inherent complexity of science poses a significant barrier.
Many domain-specific terms and multi-dimensional structures are difficult to represent using a single
text. As a result, their complete attributes cannot be fully encapsulated. This greatly weakens the
agent’s cognitive level.
- On the other hand, there is a severe lack of suitable training data in scientific domains, making it difficult for agents to comprehend the entire domain knowledge

---

### Lifecycle-oriented Deployment

Building a universally capable agent that can continuously explore, develop new skills, and maintain
a long-term life cycle in an open, unknown world is a colossal challenge.

---

## Coordinating Potential of Multiple Agents

**Motivation and Background.**
Although LLM-based agents possess commendable text under-
standing and generation capabilities, they operate as isolated entities in nature. They lack the
ability to collaborate with other agents and acquire knowledge from social interactions. This inherent
limitation restricts their potential to learn from multi-turn feedback from others to enhance their
performance. 
Moreover, they cannot be effectively deployed in complex scenarios requiring collaboration and information sharing among multiple agents.


**Potential advantages.**
Specifically, an LLM-based multi-agent system can offer several advantages.
Just as Adam Smith clearly stated in The Wealth of Nations, “The greatest improvements in the
productive powers of labor, and most of the skill, dexterity, and judgment with which it is directed or
applied, seem to be results of the division of labor.” Based on the principle of division of labor, a
single agent equipped with specialized skills and domain knowledge can engage in specific tasks. On
the one hand, agents’ skills in handling specific tasks are increasingly refined through the division of labor. On the other hand, decomposing complex tasks into multiple subtasks can eliminate the time spent switching between different processes. In the end, efficient division of labor among
multiple agents can accomplish a significantly greater workload than when there is no specialization,
substantially improving the overall system’s efficiency and output quality.

---
layout: figure
hideInToc: true
figureUrl: /Interaction_scenarios_for_multiple_LLM-based_agents.png
---


---
hideInToc: true
---

### Cooperative Interaction for Complementarity

Cooperative multi-agent systems are the most widely deployed pattern in practical usage. Within
such systems, individual agent assesses the needs and capabilities of other agents and actively seeks collaborative actions and information sharing with them [108]. This approach brings forth numerous
potential benefits, including enhanced task efficiency, collective decision improvement, and the resolution of complex real-world problems that one single agent cannot solve independently, ulti-
mately achieving the goal of synergistic complementarity. In current LLM-based multi-agent systems,
communication between agents predominantly employs natural language, which is considered the
most natural and human-understandable form of interaction.

---
hideInToc: true
---

**Disordered cooperation.** When three or more agents are present within a system, each agent is
free to express their perspectives and opinions openly. They can provide feedback and suggestions for
modifying responses related to the task at hand. This entire discussion process is uncontrolled,
lacking any specific sequence, and without introducing a standardized collaborative workflow. We
refer to this kind of multi-agent cooperation as disordered cooperation.

**Ordered cooperation.** When agents in the system adhere to specific rules, for instance, expressing their opinions one by one in a sequential manner, downstream agents only need to focus on the outputs
from upstream. This leads to a significant improvement in task completion efficiency, The entire
discussion process is highly organized and ordered. We term this kind of multi-agent cooperation as ordered cooperation. It’s worth noting that systems with only two agents, essentially engaging in a
conversational manner through a back-and-forth interaction, also fall under the category of ordered cooperation.

---
hideInToc: true
---

### Adversarial Interaction for Advancement

However,
researchers increasingly recognize that introducing concepts from game theory into
systems can lead to more robust and efficient behaviors. In competitive environments, 
agents can swiftly adjust strategies through dynamic interactions, striving to select the most advantageous or 
rational actions in response to changes caused by other agents.

By abandoning rigid beliefs and engaging in thoughtful reflection, adversarial interaction enhances the quality of responses.

The performance of the multi-agent adversarial system has shown considerable promise. However,
the system is essentially dependent on the strength of LLMs and faces several basic challenges: 
- With prolonged debate, LLM’s limited context cannot process the entire input.
- In a multi-agent environment, computational overhead significantly increases.
- Multi-agent negotiation may converge to an incorrect consensus, and all agents are firmly convinced of its accuracy.


The development of multi-agent systems is still far from being mature and feasible. **Introducing
human guides** when appropriate to compensate for agents’ shortcomings is a good choice to promote
the further advancements of agents.

---
hideInToc: true
---

### Interactive Engagement between Human and Agent

Human-agent interaction, as the name suggests, involves agents collaborating with humans to accomplish tasks. 
With the enhancement of agent capabilities, human involvement becomes progressively
essential to effectively guide and oversee agents’ actions, ensuring they align with human requirements and objectives.

---
layout: figure
hideInToc: true
figureUrl: /Two_paradigms_of_human-agent_interaction.png
---

---
hideInToc: true
---

#### Instructor-Executor Paradigm

The simplest approach involves human guidance throughout the process: humans provide clear and
specific instructions directly, while the agents’ role is to understand natural language commands from
humans and translate them into corresponding actions.

- **Quantitative feedback.** The forms of quantitative feedback mainly include absolute evaluations like binary scores 
  and ratings, as well as relative scores. Binary feedback refers to the positive and negative evaluations provided 
  by humans, which agents utilize to enhance their self-optimization.
  Comprising only two categories, this type of user feedback is often
  easy to collect, but sometimes it may oversimplify user intent by neglecting potential intermediate scenarios.
- **Qualitative feedback.** Text feedback is usually offered in natural language, particularly for responses that 
  may need improvement. The format of this feedback is quite flexible. Humans provide
  advice on how to modify outputs generated by agents, and the agents then incorporate these suggestions to refine 
  their subsequent outputs. For agents without multimodal perception capabilities, humans can also 
  act as critics, offering visual critiques, for instance. 
  Additionally, agents can utilize a memory module to store feedback for future reuse.

---
hideInToc: true
---

#### Equal Partnership Paradigm

**Empathetic communicator.** With the rapid development of AI, conversational agents have garnered
extensive attention in research fields in various forms, such as personalized custom roles and virtual chatbots.

A plethora of research endeavors have embarked on delving into the empathetic
capacities of agents. This endeavor seeks to infuse a human touch into these agents, enabling them to
detect sentiments and emotions from human expressions, ultimately crafting emotionally resonant
dialogues.

Unlike simple rule-based conversation agents, **agents with empathetic capacities can tailor their interactions to meet users’ emotional needs.**

---
hideInToc: true
---

**Human-level participant.** Furthermore, we hope that agents can be involved in the normal lives of
humans, cooperating with humans to complete tasks from a human-level perspective.

In these scenarios, agents need to first understand the beliefs, goals, and intentions of others, formulate joint action plans for their objectives, and also provide relevant suggestions to facilitate the acceptance of cooperative actions by other agents or humans. In comparison to pure agent cooperation, we desire
human involvement for two main reasons: first, to ensure interpretability, as interactions between
pure agents could generate incomprehensible language; second, to ensure controllability, as the
pursuit of agents with complete “free will” might lead to unforeseen negative consequences, carrying
the potential for disruption. Apart from gaming scenarios, agents also demonstrate human-level
capabilities in other scenarios involving human interaction, showcasing skills in strategy formulation,
negotiation, and more. Agents can collaborate with one or multiple humans, determining the shared
knowledge among the cooperative partners, identifying which information is relevant to decision-making, posing questions, and engaging in reasoning to complete tasks such as allocation, planning, and scheduling. Furthermore, agents possess persuasive abilities, dynamically influencing human viewpoints in various interactive scenarios.

---
hideInToc: true
---

The goal of the field of human-agent interaction is to learn and understand humans, develop technology and tools based on human needs, and ultimately enable comfortable, efficient, and secure interactions
between humans and agents. Currently, significant breakthroughs have been achieved in terms of
usability in this field. In the future, human-agent interaction will continue to focus on enhancing user
experience, enabling agents to better assist humans in accomplishing more complex tasks in various
domains. The ultimate aim is not to make agents more powerful but to better equip humans with agents. Considering practical applications in daily life, isolated interactions between humans and
agents are not realistic. Robots will become colleagues, assistants, and even companions. Therefore, future agents will be integrated into a social network, embodying a certain level of social value.


