# Title ( 56 / 60 words )
AI Agents for Accelerating Neuroscience Experimentation

# Summary ( 3015 / 3000 words)

***Briefly describe the purpose of the proposal and the software project(s) it involves.***

Modern systems neuroscience requires tight, sub-millisecond synchronization
between high-density neural acquisition hardware (Open-Ephys) and complex
experimental environments managed by Bonsai—including multi-device hardware
orchestration, real-time data streaming, state-machine experimental control,
and edge machine learning inference (Bonsai.ML). Bridging these sophisticated
software ecosystems currently demands weeks of manual software engineering,
low-level performance tuning, and grueling troubleshooting by highly
specialized researchers. We propose to eliminate this technical barrier by
developing an autonomous, closed-loop AI agent framework capable of natively
synthesizing, executing, debugging, and optimizing multi-software experimental
architectures.

By leveraging the declarative, XML-based reactive architecture of Bonsai and
the programmatic control layers of Open-Ephys, we will build an open-source
Model Context Protocol (MCP) server that exposes these platforms directly to
Large Language Models (LLMs) as an interactive runtime environment. Rather than
merely generating static code templates, the AI agent will function as an
autonomous systems engineer. Given a high-level natural language prompt—such as
orchestrating an environment that tracks animal velocity, syncs multi-device
behavioral telemetry, and triggers targeted optogenetic feedback upon real-time
neural replay detection—the agent will dynamically generate the complete,
production-ready XML workflows and hardware configurations. Crucially, the
agent will execute the synthesized pipeline within a sandboxed environment,
programmatically capture runtime logs, trace data-stream latencies across
devices, and isolate compiler or hardware-handshake errors. Using a continuous
reflection loop, the agent will iteratively refactor the XML stream
architecture to resolve bottlenecks, manage memory allocation, and optimize
pipeline performance for deterministic execution. This project shifts
open-source scientific software from human-operated tools to autonomous,
self-healing, and self-optimizing ecosystems, democratizing cutting-edge
closed-loop discoveries.

Ultimately, the long-term vision of this framework is the complete automation
of hypothesis-driven scientific discovery. By routing multi-modal experimental
results back to the LLM, the system leverages a vast biomedical literature
corpus to semantically interpret results, synthesize novel mechanistic
hypotheses, and autonomously design the next experimental iteration. The agent
then dynamically generates the corresponding Bonsai XML workflows and
Open-Ephys configurations, executing them via a structured human-in-the-loop
validation safeguard. By creating a continuous, self-directed loop of automated
experimentation, analysis, and refactoring, this ecosystem establishes a new
paradigm for "self-driving labs" capable of exponentially accelerating the pace
of scientific discovery across neurophysiology and broader experimental
disciplines.

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

# Landscape Analysis ( 2 / 1500 words)

***We are looking for proposals from software projects with demonstrated traction and adoption. Briefly describe other software tools that the audience for this proposal primarily uses (including proprietary alternatives, if they exist), and how the software project(s) in your proposal compare in terms of user base, adoption, functionality, and maturity relative to their target audience. You can add indicators of adoption and usage as needed. Please indicate if the software is used in AI applications and workflows.***



