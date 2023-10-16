# Agent Society: From Individuality to Sociality

- Behavior and Personality
  - Social Behavior
    - Individual behaviors
    - Group behaviors
  - Personality
    - Cognition
    - Emotion
    - Character
- Social Environment
  - Text-based Environment
  - Virtual Sandbox Environment
  - Physical Environment
- Society Simulation

---

## Behavior and Personality of LLM-based Agents


For an extended period, sociologists have frequently conducted social experiments to observe specific
social phenomena within controlled environments. Notable examples include the Hawthorne Experiment and the Stanford Prison Experiment. Subsequently, researchers began employing animals in social simulations, exemplified by the Mouse Utopia Experiment. However, these experiments
invariably utilized living organisms as participants, made it difficult to carry out various interventions,
lack flexibility, and inefficient in terms of time. Thus, researchers and practitioners envision an interactive artificial society wherein human behavior can be performed through trustworthy agents.
From sandbox games such as The Sims to the concept of Metaverse, we can see how “simulated society” is defined in people’s minds: environment and the individuals interacting in it. Behind
each individual can be a piece of program, a real human, or a LLM-based agent as described in the previous sections. Then, the interaction between individuals also contributes to the birth of sociality.

---
layout: figure
hideInToc: true
figureUrl: /Overview_of_Simulated_Agent_Society.png
---

---
hideInToc: true
---

### Social Behavior

LLM-based agents have exhibited spontaneous social behaviors
in an environment where both cooperation and competition coexist. The emergent behaviors intertwine to shape the social interactions.

**Foundational individual behaviors.** Individual behaviors arise through the interplay between internal cognitive processes and external environmental factors. These behaviors form the basis of
how agents operate and develop as individuals within society. They can be classified into three core dimensions:

1. Input behaviors
2. Internalizing behaviors
3. Output behaviors

---
hideInToc: true
---

**Dynamic group behaviors.** A group is essentially a gathering of two or more individuals participating in shared activities within a defined social context. The attributes of a group are never
static; instead, they evolve due to member interactions and environmental influences. This flexibility
gives rise to numerous group behaviors, each with a distinctive impact on the larger societal group.
The categories of group behaviors include:

1. Positive group behaviors
   are actions that foster unity, collaboration, and collective well-being.
2. Neutral group behaviors. In human society, strong personal values vary widely and tend toward
   individualism and competitiveness. In contrast, LLMs which are designed with an emphasis on
   being “helpful, honest, and harmless” often demonstrate a tendency towards neutrality.
   This alignment with neutral values leads to conformity behaviors including mimicry, spectating,
   and reluctance to oppose majorities.
3. Negative group behaviors can undermine the effectiveness and coherence of an agent group.
   Conflict and disagreement arising from heated debates or disputes among agents may lead to
   internal tensions. Furthermore, recent studies have revealed that agents may exhibit confrontational
   actions and even resort to destructive behaviors, such as destroying other agents or the environment in pursuit of efficiency gains.

---
hideInToc: true
---

### Personality

Recent advances in LLMs have provided glimpses of human-like intelligence. Just as human
personality emerges through socialization, agents also exhibit a form of personality that develops
through interactions with the group and the environment. The widely accepted definition of personality refers to cognitive, emotional, and character traits that shape behaviors.

1. Cognitive abilities. Cognitive abilities generally refer to the mental processes of gaining knowledge
   and comprehension, including thinking, judging, and problem-solving. Recent studies have started
   leveraging cognitive psychology methods to investigate emerging sociological personalities of LLM-
   based agents through various lenses.
2. Emotional intelligence.
   Emotions, distinct from cognitive abilities, involve subjective feelings and
   mood states such as joy, sadness, fear, and anger. With the increasing potency of LLMs, LLM-based
   agents are now demonstrating not only sophisticated reasoning and cognitive tasks but also a nuanced
   understanding of emotions. Recent research has explored the emotional intelligence (EI) of LLMs, including emotion recognition, interpretation, and understanding.
   These advances highlight the growing potential of LLMs to exhibit emotional intelligence, a crucial facet of achieving AGI.

---
hideInToc: true
---

3. Character portrayal. While cognition involves mental abilities and emotion relates to subjective experiences, the narrower concept of personality typically pertains to distinctive character patterns.
   Recent work has also explored customizable character portrayal in LLM-based agents. By
   optimizing LLMs through careful techniques, users can align with desired profiles and shape diverse
   and relatable agents. One effective approach is prompt engineering, which involves the concise
   summaries that encapsulate desired character traits, interests, or other attributes. These
   prompts serve as cues for LLM-based agents, directing their responses and behaviors to align with
   the outlined character portrayal. Furthermore, personality-enriched datasets can also be used to train
   and fine-tune LLM-based agents.

--- 

## Environment for Agent Society

In the context of simulation, the whole society consists of not only solitary agents but also the
environment where agents inhabit, sense, and act. The environment impacts sensory inputs,
action space, and interactive potential of agents. In turn, agents influence the state of the environment
through their behaviors and decisions. As shown in Figure 12, for a single agent, the environment refers to other autonomous agents, human actors, and external factors. It provides the necessary
resources and stimuli for agents.

---
hideInToc: true
---

### Text-based Environment

Since LLMs primarily rely on language as their input and output format, the text-based environment
serves as the most natural platform for agents to operate in. It is shaped by natural language
descriptions without direct involvement of other modalities. Agents exist in the text world and rely on textual resources to perceive, reason, and take actions.

---
hideInToc: true
---

### Virtual Sandbox Environment

The virtual sandbox environment provides a visualized and extensible platform for agent society,
bridging the gap between simulation and reality. The key features of sandbox environments are: 

- Visualization. Unlike the text-based environment, the virtual sandbox displays a panoramic view
  of the simulated setting. This visual representation can range from a simple 2D graphical interface to a fully immersive 3D modeling, depending on the complexity of the simulated society. Multiple
  elements collectively transform abstract simulations into visible landscapes.
- Extensibility. The environment demonstrates a remarkable degree of extensibility, facilitating the construction and deployment of diverse scenarios. At a basic level, agents can manipulate the physical elements within the environment, including the overall design and layout of architecture.

---
hideInToc: true
---

### Physical Environment

In contrast, the physical environment refers to the tangible and real-world surroundings which consist of actual physical objects and spaces. For instance, within
a household physical environment, tangible surfaces and spaces can be occupied by realworld objects such as plates. This physical reality is significantly more complex, posing additional
challenges for LLM-based agents:

- Sensory perception and processing. The physical environment introduces a rich tapestry of sensory inputs with real-world objects. It incorporates visual, auditory
  and spatial senses. While this diversity enhances interactivity and sensory immersion, it also introduces the complexity of simultaneous perception. Agents must process sensory inputs to
  interact effectively with their surroundings.
- Motion control. Unlike virtual environments, physical spaces impose realistic constraints on actions through embodiment. Action sequences generated by LLM-based agents should be adaptable
  to the environment. It means that the physical environment necessitates executable and grounded motion control.

---

## Society Simulation with LLM-based Agents

The concept of “Simulated Society” in this section serves as a dynamic system where agents engage
in intricate interactions within a well-defined environment. Recent research on simulated societies has followed two primary lines, namely, exploring the boundaries of the collective intelligence
capabilities of LLM-based agents and using them to accelerate discoveries in the social sciences.

---
hideInToc: true
---

### Key Properties and Mechanism of Agent Society

Social simulation can be categorized into macro-level simulation and micro-level simulation.

In the macro-level simulation, also known as system-based simulation, researchers model the overall
state of the system of the simulated society. 

While micro-level simulation, also known as
agent-based simulation or Multi-Agent Systems (MAS), indirectly simulates society by modeling
individuals. With the development of LLM-based agents, micro-level simulation has gained prominence recently. 

In this article, we characterize that the “Agent Society” refers to an **open, persistent, situated, and organized** framework where LLM-based agents interact with each other in a defined environment. Each of these attributes plays a pivotal role in shaping the
harmonious appearance of the simulated society.

---
hideInToc: true
---

- Open. One of the defining features of simulated societies lies in their openness, both in terms of
  their constituent agents and their environmental components. Agents, the primary actors within such
  societies, have the flexibility to enter or leave the environment without disrupting its operational
  integrity. Furthermore, this feature extends to the environment itself, which can be expanded
  by adding or removing entities in the virtual or physical world, along with adaptable resources like
  tool APIs. Additionally, humans can also participate in societies by assuming the role of an agent or serving as the “inner voice” guiding these agents. This inherent openness adds another level of complexity to the simulation, blurring the lines between simulation and reality.
-  Persistent. We expect persistence and sustainability from the simulated society. While individual agents within the society exercise autonomy in their actions over each time step, the
   overall organizational structure persists through time, to a degree detached from the transient behaviors of individual agents. This persistence creates an environment where agents’ decisions and behaviors accumulate, leading to a coherent societal trajectory that develops through time. The system operates independently, contributing to society’s stability while accommodating the
   dynamic nature of its participants.

---
hideInToc: true
---

- Situated. The situated nature of the society emphasizes its existence and operation within a distinct environment. This environment is artificially or automatically constructed in advance, and agents execute their behaviors and interactions effectively within it. A noteworthy aspect of this attribute is that agents possess an awareness of their spatial context, understanding their location within the environment and the objects within their field of view. This awareness contributes to their ability to interact proactively and contextually.
- Organized. The simulated society operates within a meticulously organized framework, mirroring
  the systematic structure present in the real world. Just as the physical world adheres to physics principles, the simulated society operates within predefined rules and limitations. In the simu-lated world, agents interact with the environment in a limited action space, while objects in the environment transform in a limited state space. All of these rules determine how agents operate,
  facilitating the communication connectivity and information transmission pathways, among other aspects in simulation. This organizational framework ensures that operations are coherent
  and comprehensible, ultimately leading to an ever-evolving yet enduring simulation that mirrors
  the intricacies of real-world systems.

---
hideInToc: true
---

### Insights from Agent Society

In the realm of social science, the pursuit of generalized representations
of individuals, groups, and their intricate dynamics has long been a shared objective. The
emergence of LLM-based agents allows us to take a more microscopic view of simulated society,
which leads to more discoveries from the new representation.

---
hideInToc: true
---

**Organized productive cooperation.**
Society simulation offers valuable insights into innovative collaboration patterns, which have the potential to enhance real-world management strategies. Research
has demonstrated that within this simulated society, the integration of diverse experts introduces a
multifaceted dimension of individual intelligence. When dealing with complex tasks, such
as software development or consulting, the presence of agents with various backgrounds, abilities,
and experiences facilitates creative problem-solving. Furthermore, diversity functions as a system of checks and balances, effectively preventing and rectifying errors through interaction, ultimately improving the adaptability to various tasks. Through numerous iterations of interactions and debates among agents, individual errors like hallucination or degeneration of thought (DoT) are corrected by the group [112].
Efficient communication also plays a pivotal role in such a large and complex collaborative group.
For example, MetaGPT has artificially formulated communication styles with reference to
standardized operating procedures (SOPs), validating the effectiveness of empirical methods. Park et al. observed agents working together to organize a Valentine’s Day party through spontaneous communication in a simulated town.

---
hideInToc: true
---

**Propagation in social networks.**
As simulated social systems can model what might happen in the
real world, they can be used as a reference for predicting social processes. Unlike traditional empirical
approaches, which heavily rely on time-series data and holistic modeling, agent-based simulations offer a unique advantage by providing more interpretable and endogenous perspectives for researchers. Here we focus on its application to modeling propagation in social networks.
The first crucial aspect to be explored is the development of interpersonal relationships in simulated
societies. For instance, agents who are not initially connected as friends have the potential to establish
connections through intermediaries. Once a network of relationships is established, our attention
shifts to the dissemination of information within this social network, along with the underlying
attitudes and emotions associated with it. S proposes a user-demographic inference module for capturing both the number of people aware of a particular message and the collective sentiment prevailing among the crowd. This same approach extends to modeling cultural transmission and the spread of infectious diseases. By employing LLM-based agents to model individual
behaviors, implementing various intervention strategies, and monitoring population changes over
time, these simulations empower researchers to gain deeper insights into the intricate processes that underlie various social phenomena of propagation.

---
hideInToc: true
---

**Ethical decision-making and game theory.**
Simulated societies offer a dynamic platform for
the investigation of intricate decision-making processes, encompassing decisions influenced by
ethical and moral principles. Taking Werewolf game and murder mystery games as
examples, researchers explore the capabilities of LLM-based agents when confronted with challenges of deceit, trust, and incomplete information. These complex decision-making scenarios also intersect
with game theory, where we frequently encounter moral dilemmas pertaining to individual and collective interests, such as Nash Equilibria. Through the modeling of diverse scenarios, researchers
acquire valuable insights into how agents prioritize values like honesty, cooperation, and fairness
in their actions. In addition, agent simulations not only provide an understanding of existing moral values but also contribute to the development of philosophy by serving as a basis for understanding
how these values evolve and develop over time. Ultimately, these insights contribute to the refinement
of LLM-based agents, ensuring their alignment with human values and ethical standards.

---
hideInToc: true
---

**Policy formulation and improvement.** The emergence of LLM-based agents has profoundly
transformed our approach to studying and comprehending intricate social systems. However, despite
those interesting facets mentioned earlier, numerous unexplored areas remain, underscoring the
potential for investigating diverse phenomena. One of the most promising avenues for investigation
in simulated society involves exploring various economic and political states and their impacts on
societal dynamics. Researchers can simulate a wide array of economic and political systems by
configuring agents with differing economic preferences or political ideologies. This in-depth analysis
can provide valuable insights for policymakers seeking to foster prosperity and promote societal well-being. As concerns about environmental sustainability grow, we can also simulate scenarios
involving resource extraction, pollution, conservation efforts, and policy interventions. These
findings can assist in making informed decisions, foreseeing potential repercussions, and formulating
policies that aim to maximize positive outcomes while minimizing unintended adverse effects.

---
hideInToc: true
---

### Ethical and Social Risks in Agent Society

- **Unexpected social harm.**
  Simulated societies carry the risk of generating unexpected social
  phenomena that may cause considerable public outcry and social harm. These phenomena span
  from individual-level issues like discrimination, isolation, and bullying, to broader concerns such as oppressive slavery and antagonism
- **Stereotypes and prejudice.**
- **Privacy and security.**
- **Over-reliance and addictiveness.**

