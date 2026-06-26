Bonsai is the leading open-source visual reactive programming language for
neuroscience experimental control, supporting thousands of researchers globally
(>7,000 downloads, >1,000 citations/year [Lopes et al., 2015]). While
conventional procedural, interpreted languages struggle with real-time
processing of high-bandwidth, multimodal data streams, Bonsai provides an
intuitive visual interface to a functional, compiled environment. This unique
architecture coordinates a vast ecosystem, including Open Ephys
(electrophysiology), Harp (microsecond synchronization), and Bonsai.ML
(real-time ML). However, as workflows scale, constructing and maintaining
graphical pipelines becomes a major engineering bottleneck. We propose an AI
agent architecture to automate the assembly, debugging, and optimization of
complex Bonsai workflows directly from natural language prompts.

Leveraging Bonsai’s XML architecture and Open Ephys’s control layers, we will
build an open-source Model Context Protocol (MCP) server that exposes these
platforms to Large Language Models (LLMs) as an interactive runtime. Rather
than generating static code templates, the AI agent will function as an
autonomous systems engineer. Given a high-level prompt—e.g., tracking animal
velocity, syncing telemetry, and triggering optogenetic feedback on neural
replay detection—the agent will dynamically generate production-ready XML
workflows. It will execute pipelines in a sandbox, capture logs, and trace
stream latencies. Using a continuous reflection loop, it will iteratively
refactor the XML stream architecture to resolve bottlenecks and guarantee
deterministic pipeline execution.

Additionally, we will develop a native LLM node for Bonsai. This node will
ingest real-time data summaries from active workflows to output live
inferences. Instead of controlling experiments via rigid, pre-programmed rules,
this enables adaptive experimentation guided by the broad contextual
information processing of an AI agent, yielding fundamentally more informative
results.

Our long-term vision is the complete automation of hypothesis-driven scientific
discovery. By routing multi-modal results back to the LLM, the system can
leverage biomedical literature to interpret data, synthesize hypotheses, and
run the next experimental iteration via a structured human-in-the-loop
safeguard. While full closed-loop automation is beyond our current scope, this
project delivers the foundational technical framework to make self-driving
neurophysiology laboratories a reality.

Team: Joaquin Rapela (research fellow, Gatsby Unit; creator of Bonsai.ML) will
lead implementation, consulting with Goncalo Lopes (author of Bonsai) and
collaborating with scientists at the Sainsbury Wellcome Centre and Allen
Institute for Neural Dynamics (e.g., Josh Siegle) to validate the MCP server
and LLM node in live experimental rigs.
