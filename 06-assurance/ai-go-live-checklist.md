# AI Go-Live Assurance Checklist

## 1. Purpose

This checklist defines the minimum assurance activities required before an Artificial Intelligence solution is approved for production within Austera Transport Group (ATG).

The checklist provides a final governance gate confirming that business, architecture, cybersecurity, data, privacy, operational and AI-specific risks have been appropriately addressed.

---

## 2. Solution Information

| Field | Details |
|---|---|
| AI Solution | |
| Business Owner | |
| Technology Owner | |
| Delivery Team | |
| AI Capability | |
| Model / Provider | |
| AI Risk Tier | |
| Data Classification | |
| Target Environment | |
| Planned Go-Live Date | |
| Assessment Date | |

---

## 3. Checklist Status

Use the following status values:

| Status | Meaning |
|---|---|
| Complete | Requirement satisfied |
| Partial | Requirement partially satisfied |
| Not Complete | Requirement outstanding |
| N/A | Requirement does not apply |
| Risk Accepted | Outstanding requirement formally accepted |

Material outstanding requirements must not be marked complete without supporting evidence.

---

# 4. Governance Readiness

- [ ] AI use case has been formally registered.
- [ ] Business Owner has been identified.
- [ ] Technology Owner has been identified.
- [ ] AI risk classification has been completed.
- [ ] Required AI risk assessment has been completed.
- [ ] Governance approvals required for the risk tier have been obtained.
- [ ] Material risks have identified owners.
- [ ] Residual risks have been formally accepted.
- [ ] Exceptions have been documented and approved.
- [ ] Review/reassessment date has been established.

### Evidence

Examples:

- AI inventory record
- Risk assessment
- Risk register
- Governance approval
- Risk acceptance
- Exception record

---

# 5. Architecture Readiness

- [ ] Solution architecture has been documented.
- [ ] Architecture review has been completed.
- [ ] Data flows are documented.
- [ ] Trust boundaries are identified.
- [ ] Model/provider selection is documented.
- [ ] Integration architecture has been reviewed.
- [ ] RAG architecture has been reviewed where applicable.
- [ ] Agent architecture has been reviewed where applicable.
- [ ] Material architecture decisions are recorded.
- [ ] Production architecture aligns with approved design.

### Evidence

Examples:

- Solution Architecture Document
- Architecture diagrams
- Architecture Decision Records
- Architecture Review Board approval

---

# 6. Identity and Access Management

- [ ] Enterprise authentication is implemented where applicable.
- [ ] MFA requirements are satisfied.
- [ ] RBAC is configured.
- [ ] Least privilege has been validated.
- [ ] Administrative access is restricted.
- [ ] Workload identities are configured.
- [ ] AI agent identities are defined where applicable.
- [ ] Shared credentials have been removed or formally approved.
- [ ] Joiner/mover/leaver processes are supported.
- [ ] Privileged access is auditable.

---

# 7. Network Security

- [ ] Required network segmentation is implemented.
- [ ] Private connectivity is implemented where required.
- [ ] Internet exposure has been approved.
- [ ] Firewall rules have been reviewed.
- [ ] WAF protection is implemented where applicable.
- [ ] API ingress is controlled.
- [ ] Outbound connectivity is appropriately restricted.
- [ ] DNS architecture is validated.
- [ ] DDoS protection has been considered.
- [ ] Unnecessary public endpoints have been removed.

---

# 8. Data Governance

- [ ] Data sources are approved.
- [ ] Data ownership is identified.
- [ ] Data classification has been completed.
- [ ] Data access is authorised.
- [ ] Data minimisation has been applied.
- [ ] Retention requirements are defined.
- [ ] Data deletion processes are defined.
- [ ] Data lineage is understood.
- [ ] Data residency requirements are satisfied.
- [ ] Records-management requirements are addressed.

---

# 9. Privacy

- [ ] Personal information processed by the AI system is identified.
- [ ] Privacy assessment has been completed where required.
- [ ] Collection and processing purpose is documented.
- [ ] Data minimisation has been applied.
- [ ] Retention is appropriate.
- [ ] Third-party privacy implications have been assessed.
- [ ] Cross-border processing has been assessed.
- [ ] Required notices or consent mechanisms are implemented.
- [ ] Privacy risks have been treated or accepted.

---

# 10. Model Assurance

- [ ] Production model is approved.
- [ ] Model provider is approved.
- [ ] Model version is recorded.
- [ ] Model limitations are documented.
- [ ] Model access is restricted.
- [ ] Material model risks have been assessed.
- [ ] Model change process is defined.
- [ ] Model retirement/replacement process is understood.
- [ ] Model performance has been validated for the intended purpose.

---

# 11. Generative AI Security

Where Generative AI is used:

- [ ] Prompt-injection risk has been assessed.
- [ ] Indirect prompt injection has been considered.
- [ ] System prompts are protected where required.
- [ ] Sensitive-information disclosure controls are implemented.
- [ ] AI output is treated as untrusted.
- [ ] Output validation is implemented where required.
- [ ] Content-safety controls are configured where applicable.
- [ ] Abuse controls are implemented.
- [ ] Model access is appropriately restricted.
- [ ] Security testing has been completed.

---

# 12. RAG Assurance

Where Retrieval-Augmented Generation is used:

- [ ] Knowledge sources are approved.
- [ ] Source-system permissions are preserved where required.
- [ ] Document ingestion is controlled.
- [ ] Documents are classified.
- [ ] Vector store is secured.
- [ ] Embeddings are appropriately protected.
- [ ] Knowledge poisoning risk has been assessed.
- [ ] Malicious document content has been considered.
- [ ] Data freshness processes are defined.
- [ ] Document removal/deletion is supported.
- [ ] Retrieval results have been tested for unauthorised disclosure.

---

# 13. AI Agent Assurance

Where AI agents are used:

- [ ] Agent identity is defined.
- [ ] Agent permissions follow least privilege.
- [ ] Approved tools are allowlisted.
- [ ] Tool/API permissions are documented.
- [ ] High-impact actions are identified.
- [ ] Human approval gates are implemented where required.
- [ ] Transaction/action limits are configured where appropriate.
- [ ] Agent activity is logged.
- [ ] Agent actions are distinguishable from human actions.
- [ ] Kill-switch or disable capability exists.
- [ ] Failure behaviour has been tested.

---

# 14. API and Integration Security

- [ ] APIs use appropriate authentication.
- [ ] API authorisation has been validated.
- [ ] TLS is enforced.
- [ ] Request validation is implemented.
- [ ] Rate limiting is configured where appropriate.
- [ ] API abuse controls are implemented.
- [ ] API secrets are securely managed.
- [ ] Integration identities follow least privilege.
- [ ] API logging is enabled.
- [ ] Downstream systems validate AI-generated input.

---

# 15. Secrets Management

- [ ] Secrets are stored in an approved secrets-management platform.
- [ ] Credentials are not embedded in source code.
- [ ] Credentials are not embedded in prompts.
- [ ] Credentials are not exposed in logs.
- [ ] Secret rotation is supported.
- [ ] Managed/workload identity is used where practical.

---

# 16. Secure Development

- [ ] Source code is stored in approved version control.
- [ ] Peer review has been completed.
- [ ] SAST has been completed where applicable.
- [ ] Dependency scanning has been completed.
- [ ] Secrets scanning has been completed.
- [ ] Container scanning has been completed where applicable.
- [ ] Vulnerabilities have been remediated or accepted.
- [ ] Production deployment follows approved CI/CD processes.
- [ ] Infrastructure as Code has been reviewed where applicable.

---

# 17. Security Testing

Security testing must be proportionate to AI risk.

- [ ] Authentication testing completed.
- [ ] Authorisation testing completed.
- [ ] API security testing completed.
- [ ] Prompt-injection testing completed where applicable.
- [ ] Sensitive-data disclosure testing completed.
- [ ] RAG access-control testing completed where applicable.
- [ ] Agent boundary testing completed where applicable.
- [ ] Penetration testing completed where required.
- [ ] High/Critical findings are resolved or formally accepted.

---

# 18. Logging and Monitoring

- [ ] Authentication events are logged.
- [ ] Administrative activity is logged.
- [ ] Model usage is observable.
- [ ] API activity is logged.
- [ ] Agent actions are logged.
- [ ] Tool invocation is logged where applicable.
- [ ] Security events are centrally monitored.
- [ ] Alerting is configured.
- [ ] Logging avoids unnecessary sensitive-data duplication.
- [ ] Log retention requirements are defined.

---

# 19. AI Monitoring

Where appropriate, monitoring includes:

- [ ] Model performance.
- [ ] Response quality.
- [ ] Guardrail violations.
- [ ] Prompt attacks.
- [ ] Model usage.
- [ ] Token/resource consumption.
- [ ] Abnormal retrieval.
- [ ] Agent behaviour.
- [ ] Model drift.
- [ ] User feedback.

Monitoring thresholds and escalation processes must be defined.

---

# 20. Incident Management

- [ ] AI-specific incident scenarios have been identified.
- [ ] Incident-response ownership is defined.
- [ ] Security escalation pathways are documented.
- [ ] Privacy escalation pathways are documented.
- [ ] Relevant telemetry is available for investigation.
- [ ] AI capability can be disabled where required.
- [ ] Vendor escalation process is documented.
- [ ] Evidence-preservation requirements are understood.

---

# 21. Resilience and Recovery

- [ ] Availability requirements are defined.
- [ ] AI provider failure has been considered.
- [ ] API failure behaviour is defined.
- [ ] Timeout behaviour is defined.
- [ ] Invalid AI output behaviour is defined.
- [ ] RAG failure behaviour is defined.
- [ ] Agent failure behaviour is defined.
- [ ] Critical processes have appropriate fallback arrangements.
- [ ] Backup/recovery requirements are addressed.
- [ ] Recovery procedures have been tested where required.

---

# 22. Third-Party Assurance

Where external AI providers are used:

- [ ] Vendor assessment has been completed.
- [ ] Security assurance has been reviewed.
- [ ] Privacy requirements have been reviewed.
- [ ] Model-training terms are understood.
- [ ] Data-retention terms are understood.
- [ ] Data-residency arrangements are understood.
- [ ] Subprocessors are understood.
- [ ] Incident-notification requirements are established.
- [ ] Exit arrangements are defined.
- [ ] Contractual risks are accepted.

---

# 23. Operational Readiness

- [ ] Production support owner is identified.
- [ ] Support model is documented.
- [ ] Operational procedures exist.
- [ ] Monitoring dashboards are available.
- [ ] Alert ownership is defined.
- [ ] Runbooks are available.
- [ ] Escalation paths are documented.
- [ ] Capacity/cost monitoring is configured.
- [ ] Known limitations are documented.
- [ ] Operational teams have received required training.

---

# 24. Business Readiness

- [ ] Business Owner accepts the solution.
- [ ] Users have appropriate training.
- [ ] AI limitations have been communicated.
- [ ] Human-review responsibilities are understood.
- [ ] User guidance is available.
- [ ] Support pathways are communicated.
- [ ] Expected business outcomes are measurable.

---

# 25. Compliance and Records

- [ ] Applicable regulatory requirements have been assessed.
- [ ] Contractual requirements have been assessed.
- [ ] Required governance evidence is retained.
- [ ] Records-management obligations are addressed.
- [ ] Required audit evidence is available.

---

# 26. Outstanding Risks and Actions

| ID | Outstanding Item | Risk | Owner | Due Date | Status |
|---|---|---|---|---|---|
| GL-001 | | | | | |
| GL-002 | | | | | |
| GL-003 | | | | | |

No material outstanding item should be silently accepted.

---

# 27. Go-Live Decision

Select one:

- **Approved for Production**
- **Approved with Conditions**
- **Go-Live Deferred**
- **Rejected**

### Conditions

Document any conditions, risk acceptances or post-go-live actions.

---

# 28. Approval

| Role | Name | Decision | Date |
|---|---|---|---|
| Business Owner | | | |
| Technology Owner | | | |
| Enterprise Architecture | | | |
| Cybersecurity | | | |
| Data Governance | | | |
| Privacy | | | |
| Enterprise Risk | | | |
| AI Governance Committee | | | |

Required approvers must reflect the AI risk tier.

---

# 29. Post-Go-Live Review

A post-production review should be scheduled according to risk.

The review should consider:

- Production incidents
- Security alerts
- User feedback
- Model performance
- AI quality
- Guardrail effectiveness
- Unexpected behaviour
- Cost and utilisation
- Outstanding risks
- Required control improvements

Tier 3 and Tier 4 AI systems should receive enhanced post-production review.

---

# 30. Assurance Traceability

The go-live gate completes the assurance chain:

**Business Use Case  
↓  
Risk Classification  
↓  
Risk Assessment  
↓  
Policy Requirements  
↓  
Security Controls  
↓  
Architecture Review  
↓  
Testing & Evidence  
↓  
Go-Live Assurance  
↓  
Production Monitoring  
↓  
Periodic Reassessment**

---

# 31. Related Artefacts

- Enterprise AI Governance Framework
- AI Risk Classification Methodology
- Enterprise AI Risk Assessment
- AI Risk Register
- Responsible AI Policy
- Generative AI Policy
- AI Security Standard
- AI Control Catalogue
- AI Vendor Security & Governance Assessment
- Enterprise AI Reference Architecture
- AI Monitoring Framework
- AI Incident Management Framework

---

## Disclaimer

Austera Transport Group (ATG) is a fictional organisation created solely for this professional portfolio project.

This checklist is a reference assurance model and must be adapted to an organisation's specific technology, risk, regulatory and operational requirements.
