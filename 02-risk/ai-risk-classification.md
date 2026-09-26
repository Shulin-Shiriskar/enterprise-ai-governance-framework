AI Risk Classification Methodology

1. Purpose

This document defines the methodology used by Austera Transport Group (ATG) to classify Artificial Intelligence use cases according to their potential organisational impact and risk.

The classification determines the level of governance, security assurance, human oversight, testing, approval and monitoring required throughout the AI lifecycle.

The methodology is designed to support consistent and explainable risk decisions while avoiding unnecessary governance overhead for low-risk AI use cases.

⸻

2. Risk Classification Model

AI systems are classified into four tiers.

Tier	Classification	Description
Tier 1	Minimal	Low-impact AI with limited organisational exposure
Tier 2	Limited	Enterprise AI with controlled business or data exposure
Tier 3	High	AI capable of materially affecting business, customers, sensitive data or operations
Tier 4	Critical	AI capable of significant safety, critical-infrastructure, regulatory or enterprise impact

Risk classification is determined through assessment across multiple risk dimensions.

⸻

3. Risk Dimensions

Each AI use case is assessed against the following dimensions:

1. Data Sensitivity
2. Decision Impact
3. AI Autonomy
4. Cybersecurity Exposure
5. Privacy Impact
6. Safety and Operational Impact
7. Regulatory / Compliance Impact
8. External Exposure
9. Third-Party Dependency

Each dimension receives a score between 1 and 4.

⸻

4. Scoring Scale

Score	Risk Level	Meaning
1	Minimal	Low or negligible impact
2	Limited	Manageable enterprise impact
3	High	Material organisational impact
4	Critical	Severe or potentially unacceptable impact

The scoring process evaluates inherent risk before additional controls are considered.

Residual risk is assessed separately after controls have been identified and implemented.

⸻

5. Data Sensitivity

Assesses the sensitivity of information processed by the AI system.

Score	Criteria
1	Public or non-sensitive information
2	Internal organisational information
3	Confidential, commercially sensitive or personal information
4	Highly sensitive, privileged, safety-critical or security-sensitive information

Example considerations:

* Personal information
* Customer information
* Employee information
* Commercial information
* Credentials
* Security information
* Operational technology information
* Critical infrastructure information

⸻

6. Decision Impact

Assesses the consequence of decisions influenced by AI.

Score	Criteria
1	Informational assistance only
2	Supports internal business decisions
3	Materially influences customer, employee, financial or operational decisions
4	Directly influences high-impact, safety-critical or significant organisational decisions

Examples include:

Score 1: summarising public documents.

Score 2: assisting internal knowledge searches.

Score 3: recommending customer eligibility or operational actions.

Score 4: automatically controlling safety-critical infrastructure.

⸻

7. AI Autonomy

Assesses how independently the AI can act.

Score	Criteria
1	Generates information only; human initiates all actions
2	Makes recommendations requiring human approval
3	Performs defined actions with limited human intervention
4	Performs autonomous actions across systems or business processes

Agentic AI requires particular consideration because an AI agent may interact with APIs, applications, databases or cloud services.

⸻

8. Cybersecurity Exposure

Assesses the potential security attack surface.

Score	Criteria
1	Isolated or low-exposure environment
2	Internal enterprise environment
3	Connected to sensitive enterprise systems or externally accessible services
4	Privileged access, critical systems or significant external attack surface

Consider:

* Internet exposure
* API access
* Identity privileges
* System integrations
* Administrative access
* Model access
* Tool access
* RAG data sources
* Agent capabilities

⸻

9. Privacy Impact

Assesses potential impact on individuals.

Score	Criteria
1	No personal information
2	Limited personal information
3	Significant personal or sensitive information
4	Large-scale or high-impact processing of sensitive personal information

Privacy assessments must consider both information supplied to the model and information generated or inferred by the AI system.

⸻

10. Safety and Operational Impact

Assesses potential impact on business operations or physical safety.

Score	Criteria
1	No meaningful operational impact
2	Limited operational disruption
3	Significant service or operational impact
4	Safety-critical, critical-infrastructure or severe operational impact

AI integrated with operational technology requires enhanced assessment.

⸻

11. Regulatory and Compliance Impact

Assesses the potential regulatory or compliance consequence.

Score	Criteria
1	Minimal regulatory relevance
2	Existing organisational compliance obligations apply
3	Material regulatory or contractual obligations
4	Significant legal, regulatory or critical-infrastructure obligations

Relevant requirements depend on organisational context and jurisdiction.

⸻

12. External Exposure

Assesses who can interact with the AI system.

Score	Criteria
1	Restricted internal users
2	Broad internal workforce
3	Customers, partners or controlled external users
4	Publicly accessible or large-scale external interaction

Greater exposure increases the likelihood of:

* Prompt injection
* Abuse
* Data extraction
* Automated attacks
* Malicious inputs
* Reputation impact

⸻

13. Third-Party Dependency

Assesses reliance on external AI providers.

Score	Criteria
1	Internally controlled capability
2	Established enterprise provider with contractual controls
3	Material external AI dependency
4	Critical dependency with limited transparency, control or substitutability

Assessment should consider:

* Data handling
* Model training practices
* Data residency
* Sub-processors
* Availability
* Security certifications
* Contractual protections
* Incident notification
* Exit strategy

⸻

14. Base Risk Score

The initial risk score is calculated as:

Total Risk Score =
Data Sensitivity
+ Decision Impact
+ AI Autonomy
+ Cybersecurity Exposure
+ Privacy Impact
+ Safety / Operational Impact
+ Regulatory Impact
+ External Exposure
+ Third-Party Dependency

With nine dimensions scored from 1 to 4:

Minimum score = 9

Maximum score = 36

⸻

15. Base Risk Tier

Total Score	Initial Classification
9–14	Tier 1 – Minimal
15–21	Tier 2 – Limited
22–28	Tier 3 – High
29–36	Tier 4 – Critical

The numerical score provides consistency but must not be used mechanically.

Certain characteristics automatically increase governance requirements.

⸻

16. Risk Elevation Rules

Regardless of total score, an AI system must receive enhanced review where it:

* Performs safety-critical actions
* Controls critical infrastructure
* Makes high-impact decisions without meaningful human review
* Has privileged administrative access
* Processes highly sensitive information at scale
* Can autonomously execute financial or operational transactions
* Creates significant regulatory exposure
* Has material external/public exposure combined with sensitive backend access

These characteristics may elevate the system to Tier 3 or Tier 4.

⸻

17. Example Assessment — Enterprise RAG Assistant

ATG proposes an internal RAG assistant that allows employees to search approved enterprise documentation.

Dimension	Score
Data Sensitivity	2
Decision Impact	1
AI Autonomy	1
Cybersecurity Exposure	2
Privacy Impact	2
Safety / Operational Impact	1
Regulatory Impact	1
External Exposure	1
Third-Party Dependency	2
Total	13

Initial classification:

Tier 1 – Minimal

However, access controls must ensure users cannot retrieve documents they are not authorised to access.

⸻

18. Example Assessment — Customer AI Assistant

ATG proposes an AI assistant accessible to customers through its public digital platform.

Dimension	Score
Data Sensitivity	3
Decision Impact	2
AI Autonomy	2
Cybersecurity Exposure	3
Privacy Impact	3
Safety / Operational Impact	2
Regulatory Impact	2
External Exposure	4
Third-Party Dependency	2
Total	23

Initial classification:

Tier 3 – High

This use case therefore requires enhanced architecture, security, privacy and governance assessment.

⸻

19. Example Assessment — Autonomous Operational AI

ATG proposes AI capable of initiating operational actions within critical transport infrastructure.

Dimension	Score
Data Sensitivity	4
Decision Impact	4
AI Autonomy	4
Cybersecurity Exposure	4
Privacy Impact	1
Safety / Operational Impact	4
Regulatory Impact	4
External Exposure	2
Third-Party Dependency	3
Total	30

Classification:

Tier 4 – Critical

The system requires executive risk oversight and independent assurance.

⸻

20. Inherent and Residual Risk

The initial classification represents inherent AI risk.

Following identification and implementation of controls, residual risk must be assessed.

Inherent Risk
      |
      v
Control Identification
      |
      v
Control Implementation
      |
      v
Control Assurance
      |
      v
Residual Risk

Residual risk determines whether:

* The AI system can proceed
* Additional controls are required
* Formal risk acceptance is required
* The use case must be rejected

⸻

21. Reclassification Triggers

An AI system must be reclassified following material changes including:

* New model
* New AI provider
* New data source
* Increased data sensitivity
* New integration
* Increased autonomy
* New user population
* Public exposure
* Material architecture change
* New regulatory requirements
* Significant security incident
* Change in business purpose

Risk classification is therefore a lifecycle activity rather than a one-time project exercise.

⸻

22. Governance Requirements by Tier

Requirement	Tier 1	Tier 2	Tier 3	Tier 4
AI Inventory Registration	✓	✓	✓	✓
Risk Classification	✓	✓	✓	✓
Architecture Review	Optional	✓	✓	✓
Security Assessment	Basic	✓	Enhanced	Enhanced
Privacy Assessment	If applicable	If applicable	Required where relevant	Required where relevant
Threat Modelling	Optional	Risk-based	✓	✓
AI Governance Committee	—	—	✓	✓
Executive Risk Review	—	—	Risk-based	✓
Independent Assurance	—	—	Risk-based	✓
Continuous Monitoring	Basic	Standard	Enhanced	Enhanced
Periodic Reassessment	Risk-based	✓	✓	✓

⸻

23. Framework Alignment

This methodology is designed to support alignment with recognised AI, cybersecurity and risk-management practices including:

* NIST AI Risk Management Framework
* ISO/IEC 42001
* NIST Cybersecurity Framework
* ISO/IEC 27001
* OWASP guidance for Generative AI and LLM applications
* MITRE ATLAS
* Relevant Australian cybersecurity, privacy and AI governance guidance

Detailed control mappings are maintained separately within the AI Control Catalogue.

⸻

24. Classification Outcome

The classification process produces:

AI Use Case
     |
     v
Risk Dimension Assessment
     |
     v
Initial Score
     |
     v
Risk Elevation Check
     |
     v
AI Risk Tier
     |
     v
Governance Requirements
     |
     v
Required Controls
     |
     v
Approval Authority

This ensures AI governance is:

Consistent

Explainable

Risk-based

Repeatable

and

Proportionate to organisational impact.

⸻

Disclaimer

Austera Transport Group (ATG) is a fictional organisation created solely for this reference architecture and professional portfolio project.

The scoring model is a reference methodology and should be calibrated against an organisation’s specific risk appetite, legal obligations and enterprise risk framework.
