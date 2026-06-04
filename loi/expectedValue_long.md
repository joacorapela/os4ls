If funded, this project democratizes experimentation, allowing Bonsai users to
translate natural language into error-free and highly-optimized Bonsai
workflows in minutes. Offloading systems engineering to an autonomous loop lets
researchers scale assay complexity without manual bottlenecks, timing delays,
or memory glitches.

Contributions to the Bonsai ecosystem and Bonsai.ML: The Bonsai MCP server will
boost the complete Bonsai ecosystem (e.g., Open Ephys, Harp, UCLA
Miniscope, Neurophotometrics, BonVision, DeepLabCut), with a especial impact on
real-time machine learning via Bonsai.ML. Most Bonsai users lack the machine
learning expertise to seamlessly integrate ML models into their rigs
or optimally tune their parameters. The Bonsai MCP server lowers this barrier
by clearly demonstrating how Bonsai.ML packages can elevate specific workflows
and directly assisting users with optimal model parameterization.

An AI agent embedded in the experimental control loop could be used to take
full control over experiments, based on the current state of the experimental
environment and based on online inferences on its broad knowledge base. We may
realise that AI-based control is far superior than human-based one. AI is being
used for experimental control in other domains (e.g., materials science --
A-LAB --, chemical synthesis -- RoboRXN --, synthetic biology -- Biofunders --)
but, as far as we know, it has not been used in neuroscience.

Our long-term vision is the complete automation of hypothesis-driven scientific
discovery. By routing multi-modal results back to the LLM, the system can
leverage biomedical literature to interpret data, synthesize mechanistic
hypotheses, design and run the next experimental iteration via a structured
human-in-the-loop validation safeguard.

While achieving these full AI experimental control or full closed-loop
automation is beyond our current scope, this project delivers the foundational
technical framework required to make self-driving neurophysiology laboratories
a reality.

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
