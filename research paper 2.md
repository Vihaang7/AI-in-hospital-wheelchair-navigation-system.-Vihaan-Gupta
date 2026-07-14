# Paper 4 — Notes

**Author and Title**
Yiwen Zhu, Lihe Liu, Jiaqian Yu, Di Zhang — "LLM-Based Multi-Agent Orchestration: A
Survey of Frameworks, Communication Protocols, and Emerging Patterns"

**URL to the Research Paper**
https://doi.org/10.3390/fi18060326

**Publication Record**
*Future Internet* (MDPI), Vol. 18, Issue 6, Article 326. Published June 15, 2026.
DOI: 10.3390/fi18060326. Open access (CC BY).

**Key Result or Finding**
Proposes a two-dimensional taxonomy for LLM multi-agent orchestration — 3 coordination
topologies (centralized, decentralized, hierarchical) × 1 adaptivity axis (static vs.
dynamic-adaptive) — and maps six major frameworks (LangGraph, CrewAI, AutoGen/Microsoft
Agent Framework, OpenAI Agents SDK, MetaGPT, DSPy) onto it. Finds LangGraph's
checkpoint-per-mutation, typed-state model gives it the strongest rollback/audit
guarantees of the frameworks surveyed, at the cost of a more verbose setup than
higher-level frameworks like CrewAI.

**Gap, Limitation, or Future Work Identified by the Authors**
Vendor-reported adoption and benchmark figures (marked † throughout the survey) lack
independent peer-reviewed replication as of the paper's March 2026 literature cutoff.
Screening for the survey was performed by a single reviewer, a documented potential
source of selection bias. Cross-framework benchmark numbers aren't directly comparable,
since each was measured under different model versions and task subsets. The authors
close by naming 8 open challenges, including the lack of a standardized six-dimension
evaluation framework for multi-agent coordination *quality* itself.

**Relevance to Your Project**
This survey directly categorizes the kind of pipeline built for HospitalNavigator — a
linear Resolver → Routing → Accessibility → Concierge graph with conditional
short-circuit edges — as a "(centralized/hierarchical, static)" configuration in its own
taxonomy. Its discussion of LangGraph's typed-state-plus-checkpoint model versus
conversation-based alternatives (like AutoGen) explains why building `NavState` as an
explicit, error-checked dict was a reasonable choice for auditability over a more
free-form conversational agent design.

**Technical Approach or Methodology**
A narrative literature survey (explicitly not a formal PRISMA-style systematic review,
since the authors judged registered protocols and dual-reviewer screening impractical for
such a fast-moving field). They searched six databases — Scopus, Web of Science, IEEE
Xplore, ACM Digital Library, arXiv, and Google Scholar — over the window January 2022
to March 2026, using a Boolean query combining terms like "LLM agent," "AI agent," and
"autonomous agent" with orchestration-related terms. Screened sources include
peer-reviewed papers, preprints, and framework documentation/industry reports (the last
two carry real weight here since production frameworks evolve faster than the
peer-reviewed literature). Findings were synthesized into a taxonomy (3 topologies × 1
adaptivity axis) and a structured comparison table of 6 frameworks across state
management, token cost, failure recovery, and design philosophy.

**Dataset URL(s)**
This is a survey paper, not an empirical study with a dataset — its "data" is the corpus
of literature and framework documentation it searched and screened. The databases it
searched are public and can be accessed directly:
- Scopus: https://www.scopus.com
- Web of Science: https://www.webofscience.com
- IEEE Xplore: https://ieeexplore.ieee.org
- ACM Digital Library: https://dl.acm.org
- arXiv: https://arxiv.org
- Google Scholar: https://scholar.google.com
The authors do not report releasing their specific screened-paper list/corpus as a
separate downloadable file.

