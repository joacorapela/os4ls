Bonsai is the leading open-source visual reactive programming language for
neuroscience experimental control, supporting thousands of researchers
globally. While conventional procedural, interpreted languages struggle with
real-time processing of high-bandwidth, multimodal data streams, Bonsai
provides an intuitive visual interface to a functional, compiled environment.
This unique architecture coordinates a vast ecosystem, including Open Ephys
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
information processing of an AI agent, yielding a fundamental new type of
experimentation.

We will demonstrate the use of the Bonsai LLM node for the acceleration of the
hypothesis/experiment cycle (Box et al., 2005; see its Figure 1.2
[here](https://www.gatsby.ucl.ac.uk/~rapela/os4ls/box05-fig1.2.png)).  Most
experiments begin with a hypothesis, from which consequences are derived and an
experiment is designed and performed to test the consequences. If the
experimental outputs agree with the consequences, the hypothesis is supported
and the cycle ends. But if important differences are found, the hypothesis is
modified, new consequences are derived, a new experiment is devised, and the
cycle continues.

With the advent of LLMs, time-consuming hypothesis/experiment cycles can be
substantially accelerated. Tasks assigned to humans in these cycles (like
deriving consequences from hypothesis, designing experiments, or deriving new
hypothesis) can now be assigned to LLMs, which can assist, and eventually
substitute, human experimenters.

We will build an LLM node to assist human experimenters in the
hypothesis/experimentation cycle. This node will use the Bonsai MCP server, to
build new Bonsai experiments, and functionality from Bonsai.ML, to extract
summaries from behavioral (e.g., kinematics) and neurophysiological (e.g.,
neural latents) experimental recordings.

Recent research has used LLMs for automatic experiment building (e.g., Elteto
et al., 2026), but this research has not been able to control real behavioral
or physiological experiments.  The MCP server and the Bonsai LLM node will enable
this control for the first time.
