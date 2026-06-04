Bonsai is the leading open-source visual reactive programming language for
neuroscience experimental control, used by thousands worldwide (7,000
downloads/year; 1,000 citations/year [Lopes et al., 2015]). Scientists mainly
know procedural, interpreted programming languages, but these are not
well-suited to real-time processing of multimodal data streams. Bonsai solves
this problem by giving users a visual entry point to a functional, compiled
programming language that interfaces with a broad hardware and software
ecosystem for neuroscience experimental control, including Open Ephys
(electrophysiology hardware), Harp (hardware synchronization, and Bonsai.ML
(real-time ML). But as workflows grow in complexity, they become hard for
scientists to build and maintain. We propose an AI agent to automate the
assembly, debugging, and optimization of complex Bonsai workflows directly from
natural language prompts.

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
