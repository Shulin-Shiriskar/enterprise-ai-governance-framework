Enterprise AI Risk Assessment

1. Purpose

This assessment is used to identify, analyse and document risks associated with Artificial Intelligence use cases across Austera Transport Group (ATG).

It supports:

* AI risk classification
* Architecture review
* Cybersecurity assessment
* Privacy assessment
* Data governance
* Third-party assessment
* Control selection
* Residual risk determination
* Governance approval

The assessment should be completed before production approval and reassessed following material changes to the AI system.

⸻

2. Assessment Information

Field	Response
AI Use Case	
Business Owner	
Technology Owner	
Solution / Product Name	
Business Unit	
AI Provider	
Model / Service	
Assessment Date	
Assessor	
Initial Risk Tier	
Target Production Date	
Next Review Date	

⸻

3. Business Context

3.1 What business problem is the AI system intended to solve?

Document the business objective and expected outcome.

Response:

⸻

3.2 Who will use the system?

Examples:

* Employees
* Customers
* Partners
* Suppliers
* Public users
* System-to-system integrations

Response:

⸻

3.3 What happens if the AI produces an incorrect result?

Consider:

* Financial impact
* Customer impact
* Operational impact
* Reputation
* Safety
* Regulatory consequences

Response:

⸻

3.4 Is AI necessary for this use case?

Could the business objective reasonably be achieved using conventional automation, search, analytics or deterministic rules?

Response:

⸻

4. AI Capability

4.1 What type of AI capability is being used?

Select all that apply:

* Generative AI
* Large Language Model
* Machine Learning
* Predictive Analytics
* Computer Vision
* Natural Language Processing
* Retrieval-Augmented Generation
* AI Agent
* Enterprise Copilot
* Third-party AI SaaS
* Other

Details:

⸻

4.2 Which model or AI service is being used?

Document:

* Provider
* Model
* Version where applicable
* Hosting model
* Deployment location

Response:

⸻

4.3 Can the AI initiate actions?

* No — information generation only
* Recommendations only
* Actions require human approval
* Limited autonomous actions
* Broad autonomous actions

Details:

⸻

5. Data Assessment

5.1 What information will the AI process?

Select all that apply:

* Public
* Internal
* Confidential
* Commercially sensitive
* Personal information
* Sensitive personal information
* Security-sensitive information
* Operational information
* Critical infrastructure information
* Credentials / secrets

⸻

5.2 Where does the data originate?

Examples:

* Enterprise databases
* Documents
* SharePoint
* Data lake
* APIs
* SaaS platforms
* Customer input
* Internet
* Operational systems

Response:

⸻

5.3 Is organisational information used to train or fine-tune the model?

* No
* Yes
* Unknown

If yes, explain:

⸻

5.4 Is Retrieval-Augmented Generation used?

* No
* Yes

If yes, document:

* Knowledge sources
* Vector database
* Indexing process
* Access-control model
* Document-level permissions
* Data refresh process

⸻

5.5 Can the AI retrieve information a user would not otherwise be authorised to access?

* No
* Yes
* Unknown

If yes or unknown, remediation is required before production.

⸻

6. Privacy Assessment

6.1 Does the AI process personal information?

* No
* Yes

6.2 Does the AI infer information about individuals?

* No
* Yes
* Unknown

6.3 Is personal information sent to an external AI provider?

* No
* Yes

6.4 Is a Privacy Impact Assessment required?

* No
* Yes
* To be determined by Privacy

6.5 Are users informed about relevant AI processing?

* Yes
* No
* Not applicable

Privacy observations:

⸻

7. Identity and Access Management

7.1 How do users authenticate?

Examples:

* Enterprise identity
* SSO
* Managed identity
* Service principal
* API credentials
* Local account

Response:

⸻

7.2 Is MFA enforced where appropriate?

* Yes
* No
* Not applicable

⸻

7.3 How is authorisation implemented?

Examples:

* RBAC
* ABAC
* Application roles
* Document-level permissions

Response:

⸻

7.4 Does the AI system have privileged access?

* No
* Yes

If yes, document justification and controls:

⸻

7.5 Are machine identities and secrets securely managed?

* Yes
* No
* Not applicable

⸻

8. AI Agent Assessment

Complete this section where AI agents are used.

8.1 What tools can the agent invoke?

Examples:

* APIs
* Databases
* Email
* File systems
* Cloud services
* Business applications
* Automation platforms

Response:

⸻

8.2 Can the agent modify enterprise information?

* No
* Yes

⸻

8.3 Can the agent execute transactions?

* No
* Yes

⸻

8.4 Can the agent create, modify or delete cloud resources?

* No
* Yes

⸻

8.5 Are sensitive actions subject to human approval?

* Yes
* No
* Not applicable

⸻

8.6 Is agent access based on least privilege?

* Yes
* No

⸻

9. Cybersecurity Assessment

Assess exposure to:

* Prompt injection
* Indirect prompt injection
* Sensitive information disclosure
* Insecure output handling
* Excessive agency
* Model abuse
* API attacks
* Identity compromise
* Data poisoning
* Knowledge-base poisoning
* Model supply-chain compromise
* Denial of service
* Credential leakage
* Malicious file ingestion
* Unauthorised model access

Security observations:

⸻

10. Network and Integration Security

10.1 Is the AI system publicly accessible?

* No
* Yes

10.2 Are backend services privately accessible where appropriate?

* Yes
* No
* Not applicable

10.3 Are APIs authenticated and authorised?

* Yes
* No
* Not applicable

10.4 Is traffic encrypted?

* Yes
* No

10.5 Are external integrations controlled through approved gateways?

* Yes
* No
* Not applicable

Architecture observations:

⸻

11. Model and Prompt Security

11.1 Are system prompts protected from unauthorised modification?

* Yes
* No
* Not applicable

11.2 Are controls implemented against prompt injection?

* Yes
* No

11.3 Are model inputs validated?

* Yes
* No

11.4 Are model outputs validated before downstream use?

* Yes
* No

11.5 Are content-safety controls implemented where appropriate?

* Yes
* No
* Not applicable

⸻

12. Human Oversight

12.1 Does AI influence significant decisions?

* No
* Yes

12.2 Is human review required before material actions?

* Yes
* No
* Not applicable

12.3 Can a human override the AI?

* Yes
* No

12.4 Is responsibility for final decisions clearly defined?

* Yes
* No

12.5 Are users informed of AI limitations?

* Yes
* No
* Not applicable

⸻

13. Third-Party AI Assessment

Where an external AI provider is used, assess:

Question	Yes	No	Unknown
Enterprise data ownership defined?			
Provider prevented from training on enterprise data where required?			
Data residency understood?			
Retention understood?			
Data deletion supported?			
Encryption implemented?			
Identity integration supported?			
Security certifications reviewed?			
Sub-processors identified?			
Incident notification defined?			
Service availability requirements defined?			
Exit strategy established?			

Vendor observations:

⸻

14. Logging and Monitoring

Determine whether the solution records appropriate:

* Authentication events
* Authorisation failures
* Administrative changes
* Model requests
* Model responses where appropriate
* Agent actions
* Tool invocation
* Security events
* Guardrail violations
* Sensitive-data events
* Model errors
* Performance metrics

Logs must be protected according to their information sensitivity.

⸻

15. Model and Operational Monitoring

15.1 Is model behaviour monitored?

* Yes
* No

15.2 Is model performance monitored?

* Yes
* No

15.3 Is model drift relevant?

* Yes
* No

15.4 Are abnormal AI behaviours detectable?

* Yes
* No

15.5 Are security events integrated with enterprise monitoring?

* Yes
* No

⸻

16. Resilience and Failure

16.1 What happens if the AI service becomes unavailable?

Response:

⸻

16.2 Is there a manual or deterministic fallback?

* Yes
* No
* Not required

⸻

16.3 What happens if the model produces incorrect information?

Response:

⸻

16.4 Can the AI capability be disabled without disrupting unrelated services?

* Yes
* No

⸻

17. Regulatory and Compliance Assessment

Identify applicable obligations.

Potential considerations include:

* Privacy obligations
* Cybersecurity requirements
* Critical infrastructure obligations
* Records management
* Industry regulation
* Contractual obligations
* Data residency
* Internal policy
* AI-specific regulatory requirements

Applicable requirements:

⸻

18. Risk Dimension Scoring

Following assessment, score each risk dimension.

Risk Dimension	Score 1–4	Rationale
Data Sensitivity		
Decision Impact		
AI Autonomy		
Cybersecurity Exposure		
Privacy Impact		
Safety / Operational Impact		
Regulatory Impact		
External Exposure		
Third-Party Dependency		
Total Inherent Risk Score		

⸻

19. Risk Elevation Check

Does the system:

* Perform safety-critical actions?
* Control critical infrastructure?
* Make high-impact decisions without meaningful human review?
* Have privileged administrative access?
* Process highly sensitive information at scale?
* Execute autonomous financial or operational transactions?
* Create significant regulatory exposure?
* Combine public exposure with sensitive backend access?

If Yes to any item, enhanced governance review is required regardless of numerical score.

⸻

20. Identified Risks

ID	Risk	Impact	Likelihood	Inherent Rating	Owner
AI-R01					
AI-R02					
AI-R03					

⸻

21. Required Controls

Control ID	Required Control	Control Owner	Status	Evidence
AI-C01				
AI-C02				
AI-C03				

⸻

22. Residual Risk Assessment

Following implementation and assurance of controls:

Risk ID	Inherent Risk	Controls	Residual Risk	Risk Owner	Decision
					

Possible decisions:

* Accept
* Further Treatment Required
* Escalate
* Reject

⸻

23. Governance Recommendation

Final Risk Tier

Tier: __________________

Recommendation

* Approved
* Approved with Conditions
* Remediation Required
* Escalation Required
* Rejected

Conditions / Required Actions

⸻

24. Approval Record

Role	Name	Decision	Date
Business Owner			
Enterprise Architecture			
Cybersecurity			
Data Governance			
Privacy			
Enterprise Risk			
AI Governance Committee			
Executive Risk Authority			

Only roles required by the applicable AI risk tier need to provide approval.

⸻

25. Reassessment Triggers

This assessment must be reviewed following material changes including:

* Model replacement
* Model version change with material behavioural impact
* New data source
* Increased data sensitivity
* New integration
* Increased AI autonomy
* New user population
* Public exposure
* Significant architecture change
* Significant AI incident
* New regulatory obligation
* Material change in business purpose

⸻

26. Assessment Outcome

The assessment process follows:

Business Use Case
       |
       v
AI Capability Assessment
       |
       v
Data / Privacy / Security Assessment
       |
       v
Risk Dimension Scoring
       |
       v
Inherent Risk
       |
       v
Control Selection
       |
       v
Control Implementation & Assurance
       |
       v
Residual Risk
       |
       v
Governance Decision

The objective is not to eliminate all AI risk.

The objective is to ensure AI risk is:

Known → Assessed → Controlled → Owned → Accepted → Monitored

⸻

Disclaimer

Austera Transport Group (ATG) is a fictional organisation created solely for this reference architecture and professional portfolio project.

This assessment is a reference model and should be adapted to an organisation’s legal, regulatory, operational and enterprise risk requirements.
