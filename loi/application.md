# Title ( 56 / 60 words )
AI Agents for Transforming Neuroscience Experimentation

# Summary ( 3797 / 3000 words)

***Briefly describe the purpose of the proposal and the software project(s) it involves.***

Bonsai is the leading open-source visual reactive programming language for
neuroscience experimental control, supporting thousands of researchers globally
with over 7,000 downloads and 1,000 citations annually [Lopes et al., 2015].
While conventional procedural, interpreted languages struggle with the
real-time processing of high-bandwidth, multimodal data streams, Bonsai solves
this problem by providing an intuitive visual interface to a functional,
compiled environment. This unique architecture seamlessly coordinates a vast
hardware and software ecosystem, including Open Ephys (electrophysiology), Harp
(microsecond-precision synchronization), and Bonsai.ML (real-time machine
learning). However, as experimental workflows scale in complexity, constructing
and maintaining these graphical pipelines becomes a significant engineering
bottleneck for scientists. To eliminate this barrier, we propose an AI agent
architecture designed to automate the assembly, debugging, and optimization of
complex Bonsai workflows directly from natural language prompts.

By leveraging Bonsai’s XML-based architecture and Open Ephys’s programmatic
control layers, we will build an open-source Model Context Protocol (MCP)
server that exposes these platforms to Large Language Models (LLMs) as an
interactive runtime environment. Rather than generating static code templates,
the AI agent will function as an autonomous systems engineer. Given
a high-level prompt—e.g., tracking animal velocity, syncing multi-device
behavioral telemetry, and triggering optogenetic feedback upon real-time neural
replay detection—the agent will dynamically generate production-ready XML
workflows and hardware configurations. Crucially, it will execute the pipeline
in a sandboxed environment, programmatically capture runtime logs, and trace
cross-device stream latencies. Using a continuous reflection loop, the agent
will iteratively refactor the XML stream architecture to resolve bottlenecks,
manage memory allocation, and guarantee deterministic pipeline execution. This
shifts scientific software from human-operated tools to autonomous,
self-optimizing ecosystems.

Additionally, we will develop a native LLM node for Bonsai. This node will
ingest real-time data summaries from active workflows and output LLM
inferences. Instead of controlling experiments via fixed, rigid rules, it
will allow adaptive experimentation guided by the broad contextual information
processing of an AI agent.

An AI agent embedded in the experimental control loop could be used to take
full control over experiments. Based on the current state of the experimental
environment and based on online inferences on its broad knowledge base, it may
lead to superior experimental controls than fixed pre-programmed control rules.

Our long-term vision is the complete automation of hypothesis-driven scientific
discovery. By routing multi-modal results back to the LLM, the system can
leverage biomedical literature to interpret data, synthesize mechanistic
hypotheses, design and run the next experimental iteration via a structured
human-in-the-loop validation safeguard.

While achieving these full AI experimental control or full closed-loop
automation is beyond our current scope, this project delivers the foundational
technical framework required to make self-driving neurophysiology laboratories
a reality.

Team: Joaquin Rapela (engineer research fellow at the Gatsby Unit and creator
of Bonsai.ML) will lead the implementation of the project, in direct
consultation with Goncalo Lopes (author of Bonsai), and collaborating with
experimental scientists at the Sainsbury Wellcome Centre and at Allen Institute
for Neural Dynamics (e.g., Josh Siegle), to validate in experimental rigs the MCP
server and the Bonsai LLM node.

# Expected Value ( 1431 / 1500 words)

***If the proposal is successfully funded, what does success look like? We're seeking to understand: what type of capabilities the proposal is unlocking for the scientific community; how upstream and downstream software will be improved by the proposal; how the proposed work supports or implements novel functionality for AI enablement and large-scale data analysis.***

Success means:

- Speeding and Improving Bonsai Experimentation: Enabling users of the entire Bonsai ecosystem (e.g., Open Ephys, Harp, UCLA Miniscope, Neurophotometrics, BonVision, DeepLabCut) to easily and quickly build correct and highly-optimized experimental rigs.

- Enabling Contextual Experimentation: Observing global adoption of native Bonsai LLM nodes to drive adaptive, closed-loop workflows—unlocking discovery paradigms impossible via hard-coded rules.

- Global Democratization: Expanding international adoption. While static documentation is English-centric, LLM-driven interfaces natively adapt to all languages and skill levels, removing barriers for diverse research groups.

- Elevating Real-Time Machine Learning: Driving widespread, proper use of the Bonsai.ML package, allowing non-experts to confidently integrate and parameterize complex ML models to generate unprecedented scientific knowledge.

- Demonstrating AI Superiority: Proving that real-time, AI-driven experimental control optimization yields fundamentally more informative experiments than rigid, human-designed, rule-based control.

- Pioneering Self-Driving Neurophysiology Labs: Realizing the first foundational platform for fully autonomous experimental loops in neuroscience, successfully migrating a paradigm that is already revolutionizing materials science (A-Lab), chemical synthesis (RoboRXN), and synthetic biology (Biofoundries).

# Landscape Analysis ( 1450 / 1500 words)

***We are looking for proposals from software projects with demonstrated traction and adoption. Briefly describe other software tools that the audience for this proposal primarily uses (including proprietary alternatives, if they exist), and how the software project(s) in your proposal compare in terms of user base, adoption, functionality, and maturity relative to their target audience. You can add indicators of adoption and usage as needed. Please indicate if the software is used in AI applications and workflows.***

The experimental control and behavioral monitoring landscape is divided between
domain-specific graphical interfaces for dedicated hardware (e.g., Open Ephys
GUI, Miniscope DAQ) and real-time state-machine frameworks (e.g., NIMH ML,
pyControl, Autopilot, Sanworks). While comfortable within their specific
scopes, these tools become unwieldy when incorporating new hardware or novel
task variations. Researchers also use general programming languages like Python
or MATLAB, but the resulting custom code is often difficult to maintain and
scale. Proprietary platforms like LabVIEW offer flexible visual composition,
but their fine-grained, heterogeneous elements require complex logical
structures for basic control tasks; additionally, LabVIEW is costly and
closed-source.

Bonsai disrupts this landscape by offering a highly flexible, simple visual
syntax that allows non-programmers to rapidly develop and customize complex
experiments from scratch. This unique accessibility has made Bonsai a mature,
open-source standard with deep adoption across experimental neuroscience.
Crucially, while modern AI applications in the life sciences (e.g., OpenAI’s
GPT-Rosalind, Claude Life Sciences, IBL AI Agent) focus heavily on downstream
data analysis, drug discovery, and genomics pipelines, Bonsai will be the first
experimental-control software to directly integrate AI agentic technology into
real-time behavioral and neurophysiological workflows.
