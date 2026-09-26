# Generative AI Policy

## 1. Purpose

This policy establishes mandatory requirements for the secure, responsible and authorised use of Generative Artificial Intelligence across Austera Transport Group (ATG).

Generative AI can significantly improve productivity, knowledge discovery, software development, analysis and customer services. However, it introduces risks including sensitive information disclosure, inaccurate output, prompt injection, excessive agency, intellectual-property exposure and inappropriate reliance on generated content.

This policy establishes requirements for managing these risks.

---

## 2. Scope

This policy applies to Generative AI capabilities including:

- Large Language Models (LLMs)
- Enterprise copilots
- AI assistants
- Retrieval-Augmented Generation (RAG)
- Generative AI APIs
- AI coding assistants
- Document-generation systems
- Image-generation systems
- AI agents
- AI-enabled SaaS applications

It applies to employees, contractors, consultants, delivery partners and third parties using Generative AI for ATG-related activities.

---

## 3. Approved AI Services

Organisational information may only be processed using AI services approved for the relevant information classification and business purpose.

Approval must consider:

- Security
- Privacy
- Data handling
- Model training practices
- Identity integration
- Data residency
- Retention
- Contractual protections
- Monitoring
- Regulatory requirements

Consumer AI accounts must not be assumed to provide the same protections as approved enterprise AI services.

---

## 4. Data Protection

Users must not enter sensitive organisational information into unapproved Generative AI services.

This may include:

- Personal information
- Confidential information
- Commercially sensitive information
- Credentials
- Passwords
- API keys
- Security configurations
- Source code
- Internal architecture
- Critical infrastructure information
- Privileged or legally protected information

Information supplied to AI must comply with its existing classification and handling requirements.

---

## 5. Enterprise Data and Model Training

ATG information must not be used to train external AI models unless explicitly authorised.

Where third-party Generative AI is used, ATG must understand:

- Whether prompts are retained
- Whether responses are retained
- Whether organisational data is used for model training
- Whether humans can access submitted data
- Where data is processed
- How data can be deleted
- Which subprocessors are involved

Appropriate contractual and technical controls must be established.

---

## 6. Prompt Security

Prompts may contain sensitive business context and must therefore be treated as information assets.

Applications must protect:

- System prompts
- Prompt templates
- Hidden instructions
- Security instructions
- Business rules
- Sensitive contextual information

Users must not attempt to bypass organisational AI controls through prompt manipulation.

---

## 7. Prompt Injection

Applications using Generative AI must consider both direct and indirect prompt-injection attacks.

Potential controls include:

- Input validation
- Content filtering
- Prompt isolation
- Instruction hierarchy
- Tool restrictions
- Data-source validation
- Output validation
- Least privilege
- Human approval for sensitive actions

Prompt injection must be treated as an application security risk rather than solely as a model-quality issue.

---

## 8. AI Output Validation

Generative AI output must be treated as untrusted until appropriately validated.

Potential issues include:

- Hallucination
- Fabricated references
- Incorrect facts
- Insecure code
- Misleading recommendations
- Inappropriate content
- Manipulated responses

Validation requirements must be proportional to the impact of the output.

Material business decisions must not rely solely on unverified Generative AI output.

---

## 9. Retrieval-Augmented Generation

RAG systems must maintain enterprise access controls when retrieving organisational information.

RAG implementations must consider:

- Authorised knowledge sources
- Document classification
- User permissions
- Index security
- Vector-store security
- Document-level access
- Data lineage
- Data freshness
- Poisoned documents
- Malicious embedded instructions

A user must not gain access to information through AI that they would not otherwise be authorised to access.

---

## 10. Vector Databases and Embeddings

Embeddings and vector stores must be treated according to the sensitivity of the source information.

Controls must consider:

- Authentication
- Authorisation
- Encryption
- Network access
- Tenant isolation
- Backup
- Retention
- Deletion
- Logging

Embedding data must not be assumed to be non-sensitive merely because it is not stored in its original document format.

---

## 11. AI Agents

AI agents capable of interacting with enterprise systems require enhanced controls.

Agents must operate using:

- Dedicated identities where appropriate
- Least privilege
- Approved tools
- Restricted API permissions
- Defined action boundaries
- Comprehensive logging
- Human approval for high-impact actions

Agents must not receive unrestricted access to enterprise systems merely for implementation convenience.

---

## 12. Tool Invocation

Where an AI agent can invoke tools or APIs, each tool must be explicitly authorised.

Examples include:

- Email
- Databases
- Cloud platforms
- Business applications
- File repositories
- APIs
- Automation platforms
- Operational systems

High-impact tool actions should require additional validation or human approval.

---

## 13. Agent Identity

AI agents must have identifiable and auditable identities where technically feasible.

Agent activity must be distinguishable from human activity.

Shared administrative credentials must not be used by autonomous AI agents.

---

## 14. Human-in-the-Loop Controls

Human approval must be considered for actions that may:

- Transfer funds
- Modify sensitive information
- Delete information
- Change infrastructure
- Communicate externally
- Affect customer outcomes
- Affect employees
- Impact operations
- Create safety consequences

The required level of human oversight must reflect the impact of the action.

---

## 15. AI-Generated Software Code

AI-generated code must follow existing software-development and security processes.

Required controls may include:

- Developer review
- Peer review
- Unit testing
- Integration testing
- Static analysis
- Dependency scanning
- Vulnerability scanning
- Secrets detection
- Software composition analysis
- Change approval

AI-generated code must not be automatically promoted into production without appropriate validation.

---

## 16. Intellectual Property

Users must consider intellectual-property and licensing risks associated with Generative AI.

Users must not intentionally provide copyrighted, confidential or proprietary third-party material to AI systems where doing so would breach applicable rights or obligations.

Generated content must be reviewed before material external or commercial use.

---

## 17. External Publication

AI-generated content intended for external publication must receive appropriate human review.

Review should consider:

- Accuracy
- Confidentiality
- Reputation
- Intellectual property
- Privacy
- Regulatory requirements
- Brand requirements

AI-generated content must not be represented as independently verified where it has not been validated.

---

## 18. Customer-Facing Generative AI

Customer-facing Generative AI requires enhanced assurance.

Controls should include:

- Content safety
- Prompt-injection protection
- Abuse prevention
- Rate limiting
- Authentication where appropriate
- Privacy controls
- Logging
- Output validation
- Escalation mechanisms
- Human support pathways

Users should be informed where appropriate that they are interacting with AI.

---

## 19. Generative AI Security Logging

Enterprise Generative AI applications must maintain sufficient telemetry to investigate security and operational events.

Logging may include:

- User identity
- Model requested
- Request timestamp
- Security events
- Guardrail violations
- Agent actions
- Tool invocation
- Administrative changes
- Errors

Prompt and response logging must consider privacy and data sensitivity.

Sensitive information must not be unnecessarily duplicated into monitoring platforms.

---

## 20. Model Selection

Models must be selected according to business and risk requirements rather than capability alone.

Selection considerations include:

- Security
- Privacy
- Accuracy
- Performance
- Cost
- Data handling
- Deployment model
- Model transparency
- Availability
- Support
- Regulatory requirements

Higher capability does not automatically make a model appropriate for every use case.

---

## 21. Model Changes

Material model changes may require reassessment.

Examples include:

- Changing model provider
- Major model-version change
- Moving between hosted and externally managed models
- Material change in model behaviour
- Introduction of multimodal capability
- Introduction of tool use
- Introduction of agentic functionality

---

## 22. Third-Party Generative AI

Third-party Generative AI services must undergo appropriate vendor assessment.

Assessment must consider:

- Data ownership
- Training practices
- Data retention
- Data residency
- Security
- Privacy
- Subprocessors
- Incident notification
- Service availability
- Model changes
- Exit arrangements

---

## 23. Prohibited Uses

Unless specifically authorised through appropriate governance, Generative AI must not be used to:

- Circumvent security controls
- Generate or expose credentials
- Access information beyond user authorisation
- Make uncontrolled high-impact decisions
- Autonomously modify critical systems
- Process sensitive information using unapproved services
- Impersonate individuals deceptively
- Bypass organisational governance processes

---

## 24. Incident Management

Potential Generative AI incidents include:

- Sensitive information leakage
- Prompt-injection compromise
- Unauthorised data retrieval
- Agent performing unauthorised actions
- Knowledge-base poisoning
- Model compromise
- Inappropriate customer output
- Significant hallucination affecting business operations
- Third-party AI breach

Incidents must be handled through established organisational incident-management processes.

---

## 25. Monitoring and Reassessment

Generative AI systems must be monitored according to risk.

Reassessment is required following material changes to:

- Model
- Provider
- Data
- RAG sources
- Agent permissions
- Tools
- Integrations
- User population
- Business purpose
- External exposure

---

## 26. Roles and Responsibilities

### Business Owner
Owns the approved business purpose and business risk.

### Technology Owner
Owns technical operation and lifecycle.

### AI Delivery Team
Implements approved AI capabilities and controls.

### Enterprise Architecture
Assures architecture alignment and design.

### Cybersecurity
Defines and assures Generative AI security controls.

### Data Governance
Governs enterprise data used by Generative AI.

### Privacy
Assesses privacy implications.

### AI Governance Committee
Provides oversight for higher-risk use cases.

---

## 27. Compliance

Non-compliant Generative AI services may be:

- Blocked
- Suspended
- Restricted
- Subject to remediation
- Escalated for governance review

Material non-compliance must be reported through appropriate governance channels.

---

## 28. Related Artefacts

- Responsible AI Policy
- AI Security Standard
- Acceptable AI Use Policy
- Enterprise AI Governance Framework
- AI Risk Classification Methodology
- Enterprise AI Risk Assessment
- AI Vendor Assessment
- AI Control Catalogue

---

## Disclaimer

Austera Transport Group (ATG) is a fictional organisation created solely for this professional portfolio project.

This policy is a reference model and should be adapted to an organisation's specific legal, regulatory, security and operational requirements.
