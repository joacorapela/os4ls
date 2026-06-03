Bonsai is currently the most used open-source software for neuroscience
experimental control. It is a visual reactive programming language that allows
experimentalists with little or no programming training to control
sophisticated experiments. It is used by thousands of users all around the
world (7,000 downloads per year and 1,000 citations per year of the core Bonsai
paper [Lopes et al., 2015]). Bonsai orchestrates a growing software and
hardware open-source ecosystem, such as Open Ephys hardware for
electrophysiology, Harp devices for synchronization, and the Bonsai.ML package
allowing intelligent experimental control through real-time machine learning.

Skillfully using Bonsai and the components of its ecosystem is a time-consuming
process that requires years of experience reading documentation, attending
courses, and participating in online forums. Optimally combining these
components is an even harder task. Here we propose to build an AI agent that
will automate the assembly, debugging, and optimization of Bonsai workflows
from natural language user prompts.

By leveraging the XML-based architecture of Bonsai and the programmatic control
layers of Open Ephys, we will build an open-source Model Context Protocol (MCP)
server that exposes these platforms directly to Large Language Models (LLMs) as
an interactive runtime environment. Rather than merely generating static code
templates, the AI agent will function as an autonomous systems engineer. Given
a high-level natural language prompt—such as orchestrating an environment that
tracks animal velocity, syncs multi-device behavioral telemetry, and triggers
targeted optogenetic feedback upon real-time neural replay detection—the agent
will dynamically generate the complete, production-ready XML workflows and
hardware configurations. Crucially, the agent will execute the synthesized
pipeline within a sandboxed environment, detect workflow errors,
programmatically capture runtime logs, and trace data-stream latencies across
devices. Using a continuous reflection loop, the agent will iteratively
refactor the XML stream architecture to resolve bottlenecks, manage memory
allocation, and optimize pipeline performance for optimal execution. This
project shifts open-source scientific software from human-operated tools to
autonomous, self-healing, and self-optimizing ecosystems, democratizing
cutting-edge closed-loop discoveries.

In addition, we will add a large language model (LLM) node to Bonsai. This node
will receive data summaries from Bonsai workflows as inputs and provide LLM
inferences as outputs. This node represents a paradigm shift in experimental
control; instead of controlling an experiment based on fixed, predetermined
rules, it will allow researchers to decide on the fate of the experiment based
on large-contextual-information-based inferences by the AI agent.

We will provide detailed examples of the use of this node in naturalistic,
long-duration, and continual Aeon experiments. Aeon experiments continuously
record behavioral and electrophysiological data 24/7 for weeks to months. They
are generating behavioral and electrophysiological datasets that promise to be
as relevant for neuroscience as ImageNet has been for computer vision. Bonsai
is the core experimental control software used in Aeon.

Ultimately, the long-term vision of this framework is the complete automation
of hypothesis-driven scientific discovery. By routing multi-modal experimental
results back to the LLM, the system leverages a vast biomedical literature
corpus to semantically interpret results, synthesize novel mechanistic
hypotheses, and autonomously design the next experimental iteration. The agent
then dynamically generates the corresponding Bonsai XML workflows and Open
Ephys configurations, executing them via a structured human-in-the-loop
validation safeguard. By creating a continuous, self-directed loop of automated
experimentation, analysis, and refactoring, this ecosystem establishes a new
paradigm for "self-driving labs" capable of exponentially accelerating the pace
of scientific discovery across neurophysiology and broader experimental
disciplines. While we do not aim to achieve this full long-term vision within
the scope of this project, we intend to take the critical first steps in this
direction.
