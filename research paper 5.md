# Paper 1 — Notes

**Author and Title**
Prajwal L. Salins, Ganesh Anandan, Basilio Duke Ananda, Bhageerathy Reshmi, Roshan David
Jathanna — "Internet of Things-Based Wayfinding for Hospital Visitors: A Digital Solution
for Complex Health Care Infrastructures"

**URL to the Research Paper**
https://pmc.ncbi.nlm.nih.gov/articles/PMC12613019/

**Publication Record**
*Mayo Clinic Proceedings: Digital Health*, Vol. 3, Issue 4, Article 100293. Published
October 8, 2025. DOI: 10.1016/j.mcpdig.2025.100293. Open access (CC BY 4.0).

**Key Result or Finding**
A 3-phase study built and tested a browser-based hospital wayfinding tool (KH Wayfinder)
across 5 floors, 52 destinations, and 758 routes. Pre-launch, 80.5% of surveyed users said
they'd adopt a digital wayfinder. Post-launch usability testing (n=54) found 85.2% found
it easy to use, 87% reported reduced navigation time, 83.3% reported reduced stress, 94.4%
preferred it over traditional signage, and 100% would recommend it.

**Gap, Limitation, or Future Work Identified by the Authors**
The system currently lacks real-time positioning — routes were manually digitized rather
than tracked live, so it can't account for temporary closures or a visitor's actual
in-the-moment location. The authors explicitly call out future integration with Bluetooth
low energy, Wi-Fi RTT, or vision-based positioning, plus multilingual support,
voice-guided routing, and validation in other hospital types/locations with longer-term
outcome tracking (e.g., repeat visits, appointment adherence).

**Relevance to Your Project**
This is a real-world validation of the exact graph model HospitalNavigator uses
(locations as nodes, corridors as edges) — and it shows that model, deployed as a simple
web tool, measurably cuts navigation time and stress for real hospital visitors. It's the
closest real-world analog to the project's underlying use case.

**Technical Approach or Methodology**
A 3-phase mixed-methods study, not a purely computational one: (1) a pre-implementation
needs-assessment survey of hospital visitors to gauge appetite for a digital wayfinder;
(2) development of "KH Wayfinder," a browser-based tool built on a manually digitized
node/edge map of the hospital (5 floors, 52 destinations), where routes between any two
points are computed and rendered as step-by-step directions; (3) a post-implementation
pilot deployment with n=54 participants, evaluated via a structured usability
questionnaire (ease of use, time-to-destination, self-reported stress, preference vs.
signage, likelihood to recommend) analyzed with descriptive statistics.

**Dataset URL(s)**
No public dataset. The survey responses and usability-testing data were collected
directly by the authors at their hospital and are not released as an open dataset. The
underlying hospital floor plan / node-edge map was manually digitized by the authors
in-house rather than sourced from an existing public database.

