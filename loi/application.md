# Title ( 56 / 60 words )
AI Agents for Accelerating Neuroscience Experimentation

# Summary ( 2864 / 3000 words)

***Briefly describe the purpose of the proposal and the software project(s) it involves.***

Bonsai is the leading open-source visual reactive programming language for neuroscience experimental control, used by thousands worldwide (7,000 downloads/year; 1,000 citations/year [Lopes et al., 2015]). It orchestrates an expanding software and hardware ecosystem, including Open Ephys (electrophysiology), Harp (hardware synchronization), and Bonsai.ML (real-time machine learning). However, masterfully configuring and optimizing these interconnected components requires years of specialized experience. We propose an AI agent to automate the assembly, debugging, and optimization of complex Bonsai workflows directly from natural language prompts.

By leveraging Bonsai’s XML-based architecture and Open Ephys’s programmatic control layers, we will build an open-source Model Context Protocol (MCP) server that exposes these platforms to Large Language Models (LLMs) as an interactive runtime environment. Rather than generating static code templates, the AI agent will function as an autonomous systems engineer. Given a high-level prompt—e.g., tracking animal velocity, syncing multi-device behavioral telemetry, and triggering optogenetic feedback upon real-time neural replay detection—the agent will dynamically generate production-ready XML workflows and hardware configurations. Crucially, it will execute the pipeline in a sandboxed environment, programmatically capture runtime logs, and trace cross-device stream latencies. Using a continuous reflection loop, the agent will iteratively refactor the XML stream architecture to resolve bottlenecks, manage memory allocation, and guarantee deterministic pipeline execution. This shifts scientific software from human-operated tools to autonomous, self-optimizing ecosystems.

Additionally, we will develop a native LLM node for Bonsai. This node will ingest real-time data summaries from active workflows and output LLM inferences. Instead of controlling experiments via fixed, rigid rules, it enables adaptive experimentation guided by the broad contextual information processing of an AI agent.

We will validate this node within naturalistic, long-duration, 24/7 continual Aeon experiments. Aeon datasets promise to be as transformative for neuroscience as ImageNet was for computer vision, and Bonsai serves as its core control software.

Our long-term vision is the complete automation of hypothesis-driven scientific discovery. By routing multi-modal results back to the LLM, the system can leverage biomedical literature to interpret data, synthesize mechanistic hypotheses, design and run the next experimental iteration via a structured human-in-the-loop validation safeguard. While achieving this full closed-loop automation is beyond our current scope, this project delivers the foundational technical framework required to make self-driving neurophysiology laboratories a reality.

# Expected Value ( 1401 / 1500 words)

***If the proposal is successfully funded, what does success look like? We're seeking to understand: what type of capabilities the proposal is unlocking for the scientific community; how upstream and downstream software will be improved by the proposal; how the proposed work supports or implements novel functionality for AI enablement and large-scale data analysis.***

If funded, this project democratizes instrumentation, allowing experimentalists
to translate natural language into error-free Bonsai configurations in minutes.
Offloading systems engineering to an autonomous loop lets researchers scale
assay complexity without manual bottlenecks, timing delays, or memory glitches.

Upstream Optimization: Project Aeon generates massive continuous datasets whose
scale mirrors ImageNet in computer vision. However, month-long sessions are
vulnerable to data loss from configuration drift. Deploying LLM nodes into the
Bonsai runtime, guided by real-time probabilistic inferences from Bonsai.ML,
allows the system to adjust parameters mid-session, preventing the catastrophic
waste of improperly collected data.

Downstream Growth: Our Model Context Protocol (MCP) framework provides an open,
standardized data playground for external ML developers. This allows the global
community to seamlessly integrate, benchmark, and deploy their real-time tools
into active experimental ecosystems using Bonsai's streaming data.

AI Enablement: This project treats LLMs as active runtime nodes within live,
high-bandwidth data streams. This establishes the foundational infrastructure
for fully autonomous, closed-loop "self-driving laboratories" capable of
generating, testing, and refining hypotheses dynamically, compressing research
cycles from months into single sessions.

# Landscape Analysis ( 1646 / 1500 words)

***We are looking for proposals from software projects with demonstrated traction and adoption. Briefly describe other software tools that the audience for this proposal primarily uses (including proprietary alternatives, if they exist), and how the software project(s) in your proposal compare in terms of user base, adoption, functionality, and maturity relative to their target audience. You can add indicators of adoption and usage as needed. Please indicate if the software is used in AI applications and workflows.***

The large field of technologies serving experimental control and behaviour monitoring is
traditionally occupied either by domain-specific graphical user interfaces for control and recording
of specific devices and experiment types (e.g. Open Ephys GUI , Miniscope DAQ Software) or by
real-time control frameworks for specifying task logic using state machine or similar formalisms
(e.g. NIMH ML , pyControl , Autopilot , Sanworks).

These dedicated interfaces are typically very comfortable for experimenters in the specific domain
for which the tool is designed, but can become unwieldy with the introduction of a new device or
task variation from outside their usual scope. Alternatively, one can use a more general
programming language such as Python or MATLAB, with the disadvantage of the code being harder
to understand, maintain, and change.

Programming languages like LabVIEW straddle the middle ground and provide a high-level, flexible
visual interface for composing data acquisition and control systems. Unlike Bonsai, however, the
graphical elements of Lab-VIEW are heterogeneous and very fine grained, thus requiring long and
complex logical structures to implement even a simple experimental control system. LabVIEW is
not free nor open source.

By providing an extremely simple, yet fl�exible visual syntax, Bonsai provides the opportunity for
even complete non-programmers to design and successfully customise relatively complex
experiments from the ground up. It is this capability in particular which has made Bonsai such an
attractive standard tool in experimental neuroscience. In addition, Bonsai is free and open source.
