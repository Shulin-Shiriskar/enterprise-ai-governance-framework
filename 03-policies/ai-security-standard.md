# AI Security Standard

## 1. Purpose

This standard defines mandatory cybersecurity requirements for Artificial Intelligence systems deployed or used by Austera Transport Group (ATG).

It translates the Enterprise AI Governance Framework and Responsible AI Policy into technical security requirements covering:

- Identity and access management
- Network security
- Data protection
- Model security
- Generative AI security
- Retrieval-Augmented Generation (RAG)
- AI agents
- API and integration security
- Secrets management
- Logging and monitoring
- Secure development
- Supply-chain security
- Incident response

The objective is to ensure AI capabilities are designed, implemented and operated using security-by-design and Zero Trust principles.

---

# 2. Scope

This standard applies to:

- Generative AI applications
- Large Language Models
- Machine Learning platforms
- Enterprise copilots
- RAG solutions
- AI agents
- AI APIs
- Vector databases
- AI-enabled SaaS
- Model hosting platforms
- AI development environments
- AI integrations with enterprise systems

It applies to internally developed, cloud-hosted and third-party AI capabilities.

---

# 3. Security Principles

AI systems must follow the following principles:

1. Verify explicitly.
2. Apply least privilege.
3. Assume AI inputs and outputs may be hostile.
4. Protect enterprise data throughout the AI lifecycle.
5. Minimise attack surface.
6. Isolate high-risk workloads.
7. Maintain traceability.
8. Implement defence in depth.
9. Design for compromise.
10. Continuously monitor AI behaviour and access.

---

# 4. Identity and Access Management

## AI-SEC-001 — Enterprise Identity

Enterprise AI systems must integrate with approved organisational identity services where technically feasible.

Local identities should be avoided where enterprise identity integration is available.

---

## AI-SEC-002 — Strong Authentication

Administrative and privileged access to AI platforms must use strong authentication, including MFA where supported and appropriate.

---

## AI-SEC-003 — Role-Based Access

Access must be granted according to defined roles and business requirements.

RBAC or equivalent mechanisms must be used where supported.

---

## AI-SEC-004 — Least Privilege

Users, applications, models and AI agents must receive only the permissions necessary to perform their approved functions.

---

## AI-SEC-005 — Workload Identity

Machine-to-machine AI integrations should use managed or workload identities where supported.

Long-lived static credentials should be avoided.

---

## AI-SEC-006 — Privileged Access

Privileged access to AI infrastructure must be:

- Restricted
- Auditable
- Time-bound where supported
- Separated from standard user access

---

# 5. AI Agent Identity

## AI-SEC-007 — Dedicated Agent Identity

AI agents interacting with enterprise systems must use identifiable service or workload identities where technically feasible.

Agent activity must be distinguishable from human activity.

---

## AI-SEC-008 — Agent Permission Boundaries

AI agents must have explicitly defined permission boundaries.

Agents must not receive unrestricted administrative permissions unless formally approved through exception and risk-acceptance processes.

---

## AI-SEC-009 — Sensitive Agent Actions

High-impact agent actions must require additional safeguards such as:

- Human approval
- Transaction limits
- Policy validation
- Step-up authentication
- Restricted APIs

---

# 6. Network Security

## AI-SEC-010 — Network Segmentation

AI workloads must be appropriately segmented from unrelated enterprise systems according to risk.

---

## AI-SEC-011 — Private Connectivity

Private connectivity should be used for sensitive AI services where supported and justified by risk.

Examples include:

- Private endpoints
- Private service connectivity
- Internal APIs
- Private model endpoints

---

## AI-SEC-012 — Internet Exposure

Internet-facing AI services must be explicitly approved and protected by appropriate controls.

Controls may include:

- Web Application Firewall
- API gateway
- DDoS protection
- Rate limiting
- Bot/abuse protection
- Authentication

---

## AI-SEC-013 — Egress Control

Outbound connectivity from sensitive AI workloads must be controlled according to business requirements.

Unrestricted internet egress should be avoided for high-risk workloads.

---

# 7. API and Integration Security

## AI-SEC-014 — API Authentication

AI APIs must require appropriate authentication unless explicitly designed and approved for anonymous access.

---

## AI-SEC-015 — API Authorisation

Authentication alone must not grant unrestricted access.

Authorisation must validate whether the calling identity is permitted to perform the requested action.

---

## AI-SEC-016 — API Protection

Externally exposed AI APIs must implement controls appropriate to risk, including:

- Rate limiting
- Request validation
- Authentication
- Authorisation
- Abuse detection
- Logging

---

## AI-SEC-017 — Input Validation

Data entering AI applications through APIs, files, prompts or integrations must be treated as untrusted input.

---

# 8. Data Protection

## AI-SEC-018 — Data Classification

Information processed by AI must retain its organisational data classification.

AI processing does not reduce existing protection requirements.

---

## AI-SEC-019 — Encryption in Transit

Sensitive information must be encrypted in transit using approved cryptographic protocols.

---

## AI-SEC-020 — Encryption at Rest

Sensitive AI data must be encrypted at rest using approved platform capabilities.

---

## AI-SEC-021 — Data Minimisation

AI applications must access only information required for the approved business purpose.

---

## AI-SEC-022 — Model Training Protection

Enterprise data must not be used for external model training unless explicitly authorised.

---

# 9. Secrets Management

## AI-SEC-023 — Approved Secrets Store

API keys, tokens, certificates and credentials used by AI systems must be stored in approved secrets-management platforms.

Secrets must not be stored in:

- Source code
- Prompt templates
- Configuration repositories
- Plain-text files
- Container images

---

## AI-SEC-024 — Secret Rotation

Secrets must support rotation according to organisational security requirements.

---

## AI-SEC-025 — Credential Logging

Credentials, tokens and secrets must not be included in AI prompts, model outputs or application logs.

---

# 10. Generative AI Security

## AI-SEC-026 — Treat Model Output as Untrusted

LLM output must be treated as untrusted input before being passed to downstream systems.

---

## AI-SEC-027 — Prompt Injection

Generative AI applications must assess the risk of:

- Direct prompt injection
- Indirect prompt injection
- Instruction manipulation
- Jailbreaking
- Malicious contextual content

Controls must be proportional to application risk.

---

## AI-SEC-028 — System Prompt Protection

System prompts containing security controls, business rules or sensitive context must be protected against unauthorised access and modification.

---

## AI-SEC-029 — Output Validation

AI output used to trigger business or technical actions must be validated before execution.

---

## AI-SEC-030 — Content Safety

Customer-facing or externally accessible Generative AI should implement appropriate content-safety controls.

---

# 11. Retrieval-Augmented Generation Security

## AI-SEC-031 — Authorised Knowledge Sources

RAG systems must retrieve information only from approved knowledge sources.

---

## AI-SEC-032 — Permission Preservation

RAG solutions must preserve source-system authorisation boundaries where required.

Users must not retrieve information through AI that they are not authorised to access directly.

---

## AI-SEC-033 — Vector Store Protection

Vector databases must implement appropriate:

- Authentication
- Authorisation
- Encryption
- Network controls
- Logging
- Backup protection

---

## AI-SEC-034 — Knowledge-Base Integrity

Processes must exist to prevent or detect unauthorised modification and poisoning of trusted AI knowledge sources.

---

## AI-SEC-035 — Document Ingestion

Documents ingested into RAG systems must be validated according to risk.

Externally supplied documents must be treated as potentially hostile.

---

# 12. AI Agent Security

## AI-SEC-036 — Tool Allowlisting

AI agents must only invoke explicitly approved tools and APIs.

---

## AI-SEC-037 — Action Boundaries

Agent actions must be constrained according to approved business functions.

---

## AI-SEC-038 — Human Approval

High-impact actions must require human approval where automated execution could create unacceptable risk.

---

## AI-SEC-039 — Transaction Limits

Where appropriate, autonomous agents must implement limits governing:

- Transaction value
- Action frequency
- Data volume
- Resource creation
- External communication

---

## AI-SEC-040 — Agent Audit Trail

Agent decisions and tool invocations must generate sufficient audit information to support investigation.

---

# 13. Model Security

## AI-SEC-041 — Approved Models

Production applications must use approved models and model providers.

---

## AI-SEC-042 — Model Integrity

Where models are self-hosted, mechanisms must exist to validate model provenance and integrity.

---

## AI-SEC-043 — Model Access

Access to deploy, modify or replace production models must be restricted.

---

## AI-SEC-044 — Model Change Management

Material model changes must follow change-management and reassessment requirements.

---

# 14. Secure AI Development

## AI-SEC-045 — Source Control

AI application code and configuration must be maintained in approved source-control systems.

---

## AI-SEC-046 — Peer Review

Material production code changes must undergo appropriate review.

---

## AI-SEC-047 — Security Testing

AI applications must undergo security testing appropriate to risk.

Testing may include:

- SAST
- DAST
- Dependency scanning
- Secrets scanning
- API testing
- Prompt-injection testing
- Access-control testing
- AI red-team testing

---

## AI-SEC-048 — Dependency Security

AI libraries, frameworks and dependencies must be managed through approved software supply-chain processes.

---

# 15. CI/CD Security

## AI-SEC-049 — Controlled Deployment

Production AI deployment must occur through approved deployment processes.

---

## AI-SEC-050 — Pipeline Credentials

CI/CD credentials must use secure identity and secrets-management practices.

---

## AI-SEC-051 — Security Gates

Higher-risk AI systems should include automated security checks within CI/CD pipelines.

---

# 16. Logging

## AI-SEC-052 — Security Logging

AI applications must record sufficient security telemetry.

Depending on risk, logs may include:

- Authentication
- Authorisation failures
- Administrative changes
- Model access
- Agent actions
- Tool invocation
- Security-policy violations
- Errors

---

## AI-SEC-053 — Sensitive Logging

Sensitive prompts and model responses must not be indiscriminately logged.

Logging design must consider privacy, security and investigation requirements.

---

## AI-SEC-054 — Log Integrity

Security logs must be protected against unauthorised modification and deletion.

---

# 17. Security Monitoring

## AI-SEC-055 — Central Monitoring

Security-relevant AI telemetry should integrate with enterprise security-monitoring capabilities where appropriate.

---

## AI-SEC-056 — Detection Use Cases

Monitoring should consider detection of:

- Repeated prompt attacks
- Unusual model usage
- Excessive data retrieval
- Privilege misuse
- Abnormal agent activity
- Unexpected tool invocation
- Sensitive-data exposure
- Administrative changes

---

## AI-SEC-057 — Alerting

Material security events must generate appropriate alerts and incident-response actions.

---

# 18. Third-Party AI Security

## AI-SEC-058 — Security Assessment

Third-party AI services must undergo security assessment proportional to risk.

---

## AI-SEC-059 — Data Handling

Security assessment must determine how the provider:

- Processes data
- Stores data
- Protects data
- Retains data
- Deletes data
- Uses data for model training

---

## AI-SEC-060 — Incident Notification

Material AI providers must have appropriate contractual or operational mechanisms for notifying ATG of relevant security incidents.

---

# 19. AI Supply Chain

## AI-SEC-061 — Component Provenance

AI models, libraries, containers and dependencies must originate from trusted sources.

---

## AI-SEC-062 — Vulnerability Management

Known vulnerabilities affecting AI platforms and dependencies must be managed according to enterprise vulnerability-management requirements.

---

## AI-SEC-063 — Third-Party Components

AI solutions must maintain appropriate visibility of material third-party components and dependencies.

---

# 20. Resilience

## AI-SEC-064 — Failure Design

AI applications must define behaviour when:

- Models are unavailable
- APIs fail
- Responses time out
- Guardrails reject requests
- AI output is invalid

---

## AI-SEC-065 — Safe Failure

AI failure must not automatically create unsafe or insecure system behaviour.

---

## AI-SEC-066 — Kill Switch

High-risk autonomous AI capabilities must provide mechanisms to disable or restrict autonomous actions when required.

---

# 21. Incident Response

## AI-SEC-067 — AI Security Incidents

AI-specific scenarios must be incorporated into incident-response planning.

Potential incidents include:

- Prompt-injection compromise
- Sensitive information disclosure
- Model compromise
- Agent privilege misuse
- Knowledge-base poisoning
- Credential leakage
- Unauthorised model access
- Third-party AI compromise

---

## AI-SEC-068 — Evidence Preservation

Relevant AI security logs and evidence must be preserved according to incident-response requirements.

---

# 22. Security Assurance by Risk Tier

| Security Requirement | Tier 1 | Tier 2 | Tier 3 | Tier 4 |
|---|:---:|:---:|:---:|:---:|
| Identity Review | Basic | ✓ | ✓ | ✓ |
| Security Assessment | Basic | ✓ | Enhanced | Enhanced |
| Threat Modelling | Risk-based | Risk-based | ✓ | ✓ |
| API Security Review | If applicable | ✓ | ✓ | ✓ |
| Prompt-Injection Testing | If applicable | Risk-based | ✓ | ✓ |
| Agent Security Review | If applicable | ✓ | ✓ | ✓ |
| Security Logging | Basic | ✓ | Enhanced | Enhanced |
| Penetration Testing | Risk-based | Risk-based | ✓ | ✓ |
| Independent Security Assurance | — | — | Risk-based | ✓ |
| Continuous Security Monitoring | Basic | Standard | Enhanced | Enhanced |

---

# 23. Exceptions

Where a mandatory security requirement cannot be implemented, a formal exception is required.

The exception must document:

- Control identifier
- Business justification
- Security risk
- Compensating controls
- Risk owner
- Expiry date
- Remediation plan

High-risk exceptions must be escalated according to the AI Governance Operating Model.

---

# 24. Control Traceability

Each security requirement is assigned a unique control identifier:

`AI-SEC-###`

These identifiers enable traceability between:

**Policy → Standard → Risk → Control → Implementation → Evidence → Assurance**

Control mappings to recognised security and AI frameworks are maintained separately within the AI Control Catalogue.

---

# 25. Related Artefacts

- Responsible AI Policy
- Generative AI Policy
- Acceptable AI Use Policy
- Enterprise AI Governance Framework
- Enterprise AI Risk Assessment
- AI Control Catalogue
- AI Vendor Assessment
- AI Go-Live Checklist
- AI Incident Management Framework

---

## Disclaimer

Austera Transport Group (ATG) is a fictional organisation created solely for this professional portfolio project.

This standard is a reference security model and must be tailored to an organisation's architecture, threat profile, regulatory obligations and risk appetite.
