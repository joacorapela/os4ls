# Title ( 56 / 60 words )
AI Agents for Transforming Neuroscience Experimentation

# Summary ( 2892 / 3000 words)

***Briefly describe the purpose of the proposal and the software project(s) it involves.***

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

# Expected Value ( 1426 / 1500 words)

***If the proposal is successfully funded, what does success look like? We're seeking to understand: what type of capabilities the proposal is unlocking for the scientific community; how upstream and downstream software will be improved by the proposal; how the proposed work supports or implements novel functionality for AI enablement and large-scale data analysis.***

If successfully funded, success will look like:

1. Unlocking Ecosystem Capabilities: Enabling Bonsai users (e.g., Open Ephys, Harp, UCLA Miniscope) to rapidly build correct and optimized experimental architectures.

2. Upstream & Downstream Software Improvement: Upstream classic ML pipelines for processing raw data, like state-space models to extract kinematics information from raw video data, or variational-Bayes models to infer latent variables from Neuropixels recordings, will be empowered by streaming low-dimensional summaries into downstream LLM Bonsai nodes. This natively bridges high-dimensional raw data acquisition with modern AI orchestration.

3. Novel Functionality for AI Enablement: Driving adoption of native Bonsai LLM nodes to power adaptive, closed-loop workflows impossible via hard-coded rules.

4. Global Democratization: Expanding international adoption. While static documentation is English-centric, LLM-driven interfaces natively adapt to all languages and skill levels, removing barriers for diverse research groups.

5. Elevating Real-Time Machine Learning: Driving widespread use of Bonsai.ML, allowing non-experts to confidently integrate complex ML models to generate scientific knowledge.

6. Validating AI-Driven Workflows: Providing initial proof-of-concept evidence that LLM Bonsai nodes yield measurably more responsive and informative paradigms than conventional, static workflows.

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

# Work Plan ( 853 / 750 words)

***To complete this section, please download or make a copy of the [provided template](https://docs.google.com/document/d/1QeloUWQCiDwTPzZlJQ55tKHAoTHztuhIqSm90aEkuWo/edit?tab=t.0) (by selecting File->Download or File->Make a Copy), complete the required sections, and upload as a single PDF.***

[Project name] is a widely used open source [tool category] for [research area], maintained by a [multi-institution community]. This request supports a [N]-month effort to [headline aim], organized around the two goals below. The engineering work sits within our published roadmap: Goal 1 corresponds to milestone [x.y] on our public issue tracker, and Goal 2 builds on a working prototype released in [year]. Beyond the requested funds, our institution contributes [X] of the lead maintainer's time, continuous integration credits, and existing test infrastructure. We will pair development with two community activities: a half-day tutorial at [conference] aimed at [target audience], and a remote contributor sprint to onboard and mentor new maintainers. All code will be developed in the open under [license], with releases published in [registry].

# Goals, Outcomes, Milestones and Deliverables (up to 5 goals)


## Goal 1: Interoperability with community standards
**Outcome**: Users move data between [project name] and the rest of their ecosystem without lossy, manual format conversion, so it fits cleanly into standard analysis workflows.
**Milestones & Deliverables**:
1.1  Add native read/write support for the community-standard data format(s). [Year 1]
1.2  Produce migration guidance and interactive notebooks demonstrating interoperability. [Year 1]
**Success indicators**:
Native support for [standard format] released and validated against reference datasets. [Year 2]
[N] tutorials or notebooks published and adopted in community training. [Year 2]


## Goal 2: AI-native, agent-callable interfaces
**Outcome**: [project name] becomes a composable building block that automated pipelines and AI agents can call directly through a stable interface.
**Milestones & Deliverables**:
2.1  Define and document a stable programmatic interface covering core operations. [Year 1]
2.2  Release stable version of agent-callable endpoints. [Year 1]
**Success indicators**:
At least [N] downstream tools or pipelines adopt the new interface [Year 2].



# Budget Description

Enter the amount requested in USD per year (whole numbers only) as well as the budget requested for all years. The numbers should match those described in the Budget Description to follow. Please note that for track 1, the maximum amount requested is 50,000 USD  total over two years (25,000 USD/per year).  For track 2, the maximum amount requested is ,000,000 total over two years(00,000 USD/per year).

Amount for Year 1: 125000

Amount for Year 2: 125000

Total Amount: 250000

Budget Description:

Upload the description of the costs to be funded by this grant at a high level in narrative and tabular form, outlining costs for personnel (including names, if known), supplies, equipment, travel, meetings/hackathons/sprints, subcontracts, other costs, and up to 10% indirect costs (excluding equipment and subcontracts). Upload as .pdf and/or .xlsx file formats.

Budget Description:

Recent Financial Support ( 221 / 1500 words)

List active and recently completed grants (previous two calendar years - 2025 and 2026) as well as in-kind support the PI and any co-PIs have received to directly or indirectly support work related to this proposal, including the software project(s) listed in the proposal, including: their duration, total amount in USD (for grants), and source of funding (maximum 1,500 characters)
1. The creation of [Bonsai.ML](https://bonsai-rx.org/machinelearning/) was supported by the Biotechnology and Biomedical Sciences Research Council award [BB/W019132/1](https://gtr.ukri.org/projects?ref=BB%2FW019132%2F1).
