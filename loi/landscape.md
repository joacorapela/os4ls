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
