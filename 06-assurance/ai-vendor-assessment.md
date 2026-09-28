# AI Vendor Security & Governance Assessment

## 1. Purpose

This assessment provides a structured approach for evaluating third-party Artificial Intelligence providers before their services are approved for use within Austera Transport Group (ATG).

The assessment considers:

- AI governance
- Cybersecurity
- Privacy
- Data protection
- Model governance
- Generative AI security
- Identity and access
- Regulatory compliance
- Resilience
- Supply-chain risk
- Incident management
- Contractual protections

The depth of assessment must be proportionate to the risk presented by the AI service.

---

## 2. Assessment Information

| Field | Details |
|---|---|
| Vendor | |
| Product / Service | |
| Business Owner | |
| Technology Owner | |
| Assessment Owner | |
| Proposed Use Case | |
| AI Capability | |
| Data Classification | |
| AI Risk Tier | |
| Assessment Date | |
| Review Date | |

---

## 3. Assessment Rating

Each assessment question should be rated:

| Rating | Meaning |
|---|---|
| Compliant | Requirement satisfactorily addressed |
| Partially Compliant | Requirement partly addressed or compensating controls required |
| Non-Compliant | Requirement not adequately addressed |
| Not Applicable | Requirement does not apply |
| Not Assessed | Evidence has not yet been obtained |

A vendor must not be approved solely on the basis of questionnaire responses where independent evidence is required.

---

## 4. AI Governance

Determine whether the provider has established governance for the development and operation of AI.

Questions:

- Does the vendor maintain a formal AI governance framework?
- Are AI systems assigned accountable owners?
- Does the vendor perform AI risk assessments?
- Are higher-risk AI capabilities subject to enhanced governance?
- Are model changes governed?
- Does the vendor maintain Responsible AI principles?
- Are AI incidents formally managed?
- Is AI governance periodically reviewed?

### Evidence

Potential evidence includes:

- AI governance framework
- Responsible AI policy
- Risk-management methodology
- Governance committee terms of reference
- Independent assurance reports

---

## 5. AI Management System

Where appropriate, determine whether the vendor operates a structured AI management system.

Assess:

- AI policies
- Defined AI roles
- AI risk management
- AI lifecycle governance
- Performance monitoring
- Internal assurance
- Continual improvement

Where a vendor claims alignment or certification to ISO/IEC 42001, appropriate evidence should be requested.

Certification must not replace risk-based due diligence.

---

## 6. Data Ownership

Determine ownership and control of information submitted to the AI service.

Questions:

- Does ATG retain ownership of submitted information?
- Does ATG retain appropriate rights over generated outputs?
- Can the provider use ATG information for purposes unrelated to service delivery?
- Can provider personnel access ATG information?
- Are ownership provisions contractually documented?

Any ambiguity regarding data ownership must be resolved before sensitive information is processed.

---

## 7. Model Training

Determine whether ATG information may be used to train or improve provider models.

Questions:

- Are prompts used for model training?
- Are uploaded documents used for training?
- Are model responses used for training?
- Is training enabled by default?
- Can training be contractually disabled?
- Does the restriction apply to subprocessors?

Enterprise information must not be used for external model training unless explicitly authorised.

---

## 8. Data Retention

Determine:

- How long prompts are retained
- How long outputs are retained
- How uploaded documents are retained
- Whether administrators can configure retention
- Whether zero-retention options exist
- Whether deleted information remains in backups
- How deletion requests are processed

Retention must align with ATG information-governance requirements.

---

## 9. Data Residency and Sovereignty

Identify:

- Processing locations
- Storage locations
- Backup locations
- Support-access locations
- Subprocessor locations

Determine whether the provider can guarantee required geographic boundaries where applicable.

Cross-border processing must be assessed for privacy, contractual, security and regulatory implications.

---

## 10. Privacy

Assess whether the service processes personal information.

Questions include:

- What personal information may be processed?
- What is the processing purpose?
- Does the provider act as processor or controller?
- Are privacy obligations contractually defined?
- Can personal information be deleted?
- Can data-subject requests be supported?
- Are privacy incidents reported?
- Is a Privacy Impact Assessment required?

---

## 11. Security Governance

Determine whether the provider maintains an established information-security program.

Evidence may include:

- ISO/IEC 27001 certification
- SOC 2 reports
- Penetration-test summaries
- Vulnerability-management processes
- Security policies
- Independent security assessments

Certifications provide assurance evidence but do not automatically establish suitability for the proposed AI use case.

---

## 12. Identity and Access Management

Assess:

- Enterprise SSO
- MFA
- RBAC
- Administrative roles
- Privileged-access controls
- Service identities
- API authentication
- Access reviews
- User provisioning/deprovisioning
- Audit logging

Local unmanaged accounts should be avoided where enterprise federation is available.

---

## 13. Encryption and Key Management

Determine whether information is encrypted:

- In transit
- At rest
- In backups

Assess:

- Cryptographic standards
- Key management
- Key rotation
- Customer-managed key options
- Separation of tenant keys where relevant

---

## 14. Tenant Isolation

For multi-tenant AI services, determine how the provider prevents cross-customer access.

Assess:

- Logical isolation
- Data isolation
- Model-context isolation
- Vector-store isolation
- Identity boundaries
- Encryption
- Testing of tenant separation

Cross-tenant data exposure must be treated as a material security risk.

---

## 15. Model Security

Assess how production models are protected.

Questions include:

- Who can deploy or modify models?
- How is model integrity validated?
- How are model versions controlled?
- Are model changes logged?
- Are models obtained from trusted sources?
- How are model vulnerabilities handled?

---

## 16. Generative AI Security

For Generative AI services assess controls for:

- Prompt injection
- Indirect prompt injection
- Sensitive-information disclosure
- Insecure output handling
- Excessive agency
- Model manipulation
- Abuse
- Unbounded resource consumption

The provider should demonstrate security controls appropriate to the capability offered.

---

## 17. RAG Security

Where the service provides RAG capabilities, assess:

- Knowledge-source authorisation
- Document permissions
- Vector-store security
- Secure ingestion
- Data lineage
- Document deletion
- Knowledge poisoning
- Malicious embedded instructions
- Retrieval filtering

Users must not receive information they are not authorised to access.

---

## 18. AI Agent Security

Where AI agents are supported, determine:

- How agents authenticate
- How permissions are assigned
- How tools are authorised
- Whether tool allowlisting is supported
- Whether action limits exist
- Whether human approval can be enforced
- Whether agent activity is logged
- Whether autonomous activity can be disabled

Agents with enterprise-system access require enhanced assessment.

---

## 19. API Security

Where AI capabilities are accessed through APIs, assess:

- Authentication
- Authorisation
- Encryption
- Rate limiting
- Input validation
- Abuse protection
- Logging
- API-key management
- Private connectivity options

---

## 20. Logging and Auditability

Determine what telemetry is available to ATG.

Assess whether logs capture:

- User authentication
- Administrative changes
- Model access
- API activity
- Security events
- Agent actions
- Tool invocation
- Configuration changes

Determine whether logs can integrate with enterprise SIEM capabilities.

---

## 21. Security Monitoring

Determine whether the provider monitors for:

- Account compromise
- Unusual AI usage
- Prompt attacks
- Data exfiltration
- Privilege misuse
- Malicious API activity
- Model abuse
- Administrative anomalies

Clarify the provider's responsibility versus ATG's responsibility for monitoring.

---

## 22. Vulnerability Management

Assess:

- Vulnerability scanning
- Penetration testing
- Patch management
- Dependency scanning
- Container security
- Secure development
- Vulnerability disclosure
- Remediation timeframes

Material unresolved vulnerabilities must be assessed before approval.

---

## 23. AI Supply Chain

Identify material dependencies including:

- Foundation-model providers
- Cloud providers
- Model repositories
- Open-source libraries
- AI frameworks
- Data providers
- Subprocessors

The provider should maintain appropriate oversight of material supply-chain dependencies.

---

## 24. Subprocessors

Obtain a list of material subprocessors.

Assess:

- Services provided
- Data accessed
- Processing locations
- Security obligations
- Privacy obligations
- Notification of changes

Material subprocessor changes may trigger reassessment.

---

## 25. Incident Management

Determine:

- How AI security incidents are detected
- Incident-response processes
- Customer-notification processes
- Notification timeframes
- Evidence preservation
- Root-cause analysis
- Remediation
- Regulatory notification responsibilities

Contractual incident-notification requirements should be established where appropriate.

---

## 26. Resilience and Availability

Assess:

- Service availability commitments
- Redundancy
- Backup
- Disaster recovery
- Recovery objectives
- Capacity management
- Model-provider dependency
- Regional failure scenarios

Critical business processes require appropriate fallback arrangements.

---

## 27. Model Availability and Change

Determine whether the provider may:

- Retire models
- Change model versions
- Modify model behaviour
- Change safety controls
- Change pricing
- Change context limits

Assess how customers are notified of material changes.

Material model changes may require ATG reassessment.

---

## 28. Exit Strategy

ATG must understand how it can exit the service.

Assess:

- Data export
- Data deletion
- Configuration export
- Model portability
- Knowledge-base export
- Vector-data deletion
- Contract termination
- Evidence of deletion

Vendor lock-in risk should be considered during architecture assessment.

---

## 29. Regulatory and Compliance

Determine which requirements may apply to the proposed use case.

Potential considerations include:

- Privacy requirements
- Cybersecurity obligations
- Critical-infrastructure obligations
- Records management
- Sector-specific regulation
- Contractual obligations
- AI-specific regulatory requirements

Vendor compliance claims must be validated where material.

---

## 30. Contractual Protections

Contracts should address appropriate requirements including:

- Data ownership
- Permitted data use
- Model training
- Confidentiality
- Security controls
- Privacy
- Data residency
- Incident notification
- Subprocessors
- Audit rights
- Service levels
- Data deletion
- Exit arrangements

---

## 31. Risk Findings

Document material findings.

| ID | Finding | Risk | Severity | Required Treatment | Owner | Due Date |
|---|---|---|---|---|---|---|
| V-001 | | | | | | |
| V-002 | | | | | | |
| V-003 | | | | | | |

---

## 32. Residual Risk

Following treatment, determine whether residual vendor risk is:

- Low
- Moderate
- High
- Critical

Residual risk must be accepted by the appropriate authority according to the ATG governance model.

---

## 33. Assessment Outcome

Select one:

- **Approved**
- **Approved with Conditions**
- **Remediation Required**
- **Rejected**

### Conditions / Required Actions

Document any conditions that must be completed before or after deployment.

---

## 34. Approval

| Role | Name | Decision | Date |
|---|---|---|---|
| Business Owner | | | |
| Technology Owner | | | |
| Cybersecurity | | | |
| Privacy | | | |
| Data Governance | | | |
| Architecture | | | |
| AI Governance Committee | | | |

Approval requirements should reflect the AI risk tier.

---

## 35. Reassessment Triggers

Vendor reassessment should occur following material changes including:

- Significant security incident
- Material model change
- New subprocessors
- Change in data-processing location
- Change in model-training terms
- Significant architecture change
- New agent capability
- New enterprise integration
- Regulatory change
- Contract renewal

---

## 36. Framework Alignment

This assessment supports the broader ATG governance approach informed by:

- NIST AI Risk Management Framework
- ISO/IEC 42001
- NIST Cybersecurity Framework
- OWASP guidance for Generative AI security
- Enterprise security, privacy and risk requirements

Framework alignment does not replace organisation-specific legal and regulatory assessment.

---

## 37. Related Artefacts

- Enterprise AI Governance Framework
- Responsible AI Policy
- Generative AI Policy
- AI Security Standard
- AI Risk Classification Methodology
- Enterprise AI Risk Assessment
- AI Control Catalogue
- Security Control Mapping
- Enterprise AI Reference Architecture
- AI Go-Live Checklist
- AI Monitoring Framework
- AI Incident Management Framework

---

## Disclaimer

Austera Transport Group (ATG) is a fictional organisation created solely for this professional portfolio project.

This assessment is a reference model and must be adapted to specific organisational, contractual, regulatory and technology requirements.
