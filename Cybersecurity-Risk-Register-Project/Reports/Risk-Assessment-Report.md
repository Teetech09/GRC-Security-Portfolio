Cybersecurity Risk Assessment Report

Organisation: NorthBridge Financial Services Ltd.  
Industry: Financial Services  
Assessment Type: Simulated Cybersecurity Risk Assessment  
Prepared By: GRC Analyst (Portfolio Project)  
Assessment Date:12 November 2026  
Report Classification: Portfolio Demonstration


1. Executive Summary

This report presents the findings of a simulated cybersecurity risk assessment conducted for NorthBridge Financial Services Ltd., a fictional Canadian financial services organisation.

The assessment was designed to identify potential cybersecurity threats, evaluate organisational vulnerabilities, review assumed existing security controls and recommend appropriate risk treatment actions.

Eight cybersecurity risks were identified across key business and technology areas, including identity and access management, cloud security, ransomware, security monitoring, third-party security, backup and recovery, and vulnerability management.

The assessment identified:

- 1 Critical risk.
- 7 High risks.
- 0 Medium risks.
- 0 Low risks.

The results indicate that the simulated organisation requires prioritised attention to identity and access management, protection of customer information, incident response and operational resilience.

Recommended actions include strengthening employee offboarding procedures, enforcing cloud security configurations, improving security monitoring, conducting vendor assessments and regularly testing backup restoration.

All findings and scores are illustrative and are not based on an actual organisational audit.

2. Background

NorthBridge Financial Services Ltd. is a fictional financial services organisation providing digital banking and payment services to customers.

Its assumed technology environment includes:

- AWS cloud infrastructure.
- Microsoft 365.
- Digital banking applications.
- Identity and access management systems.
- Third-party payment processors.
- Cloud-based customer information storage.

Given the sensitivity of financial and customer information, effective cybersecurity risk management is important for protecting business operations, customer trust and information assets.

Management has requested a simulated risk assessment to identify potential areas of exposure and recommend suitable security improvements.

3. Assessment Objectives

The objectives of this assessment are to:

1. Identify key cybersecurity risks affecting the organisation.
2. Evaluate the likelihood and potential impact of identified risks.
3. Assess inherent and residual risk levels.
4. Identify assumed existing controls and potential control gaps.
5. Map identified risks to relevant cybersecurity frameworks.
6. Recommend risk treatment actions.
7. Support management decision-making through documented risk information.

4. Assessment Scope

The assessment covers the following areas:

| Assessment Area | Focus |
|---|---|
| Identity and Access Management | User access, account lifecycle and employee offboarding |
| Security Awareness | Phishing and employee security awareness |
| Cloud Security | AWS S3 permissions and customer data protection |
| Incident Response | Ransomware preparedness and response |
| Security Monitoring | Logging, alerting and incident detection |
| Third-Party Security | Vendor assessments and payment processor security |
| Backup and Recovery | Backup availability and restoration testing |
| Vulnerability Management | Vulnerability identification and patch remediation |

The assessment focuses on cybersecurity risks associated with the organisation's assumed technology environment.

5. Assessment Methodology

A qualitative risk assessment methodology was used.

Each risk was evaluated using a five-point likelihood scale and a five-point impact scale.

Risk Score = Likelihood × Impact

The assessment considers two risk levels:

Inherent Risk: The potential risk before considering existing security controls.

Residual Risk: The remaining risk after considering existing controls.

The following project-specific risk classifications were applied:

| Score | Risk Rating |
|---|---|
| 1–4 | Low |
| 5–9 | Medium |
| 10–16 | High |
| 17–25 | Critical |

The scoring methodology is documented separately in `risk_scoring_methodology.md`.

6. Risk Assessment Results

Eight cybersecurity risks were identified during the simulated assessment.

| Risk ID | Risk Description | Inherent Score | Inherent Rating | Residual Score | Residual Rating |
|---|---|---:|---|---:|---|
| R001 | Former employees retain active system accounts | 20 | Critical | 20 | Critical |
| R002 | Employees fall victim to phishing attacks | 16 | High | 16 | High |
| R003 | Sensitive customer data exposed through AWS S3 misconfiguration | 15 | High | 15 | High |
| R004 | Ransomware disrupts banking operations | 15 | High | 15 | High |
| R005 | Security incidents go undetected due to inadequate monitoring | 12 | High | 12 | High |
| R006 | Third-party payment processor exposes customer information | 15 | High | 15 | High |
| R007 | Backups are unavailable or unusable during recovery | 15 | High | 15 | High |
| R008 | Unpatched vulnerabilities allow attackers to compromise systems | 16 | High | 16 | High |

6.1 Risk Distribution

| Risk Rating | Number of Risks |
|---|---:|
| Critical | 1 |
| High | 7 |
| Medium | 0 |
| Low | 0 |
| Total | 8 |

The assessment indicates that all identified risks require management attention, with R001 receiving the highest priority due to its Critical rating.

7. Key Findings and Observations

Finding 1: Identity and Access Management Weaknesses

Reference: R001  
Rating: Critical

The simulated assessment identified a potential weakness in the employee offboarding process.

Former employees retaining active accounts could create opportunities for unauthorised access to business systems and sensitive customer information.

Recommendation:

- Establish a documented employee offboarding procedure.
- Ensure timely deactivation of accounts following termination.
- Introduce periodic user access reviews.
- Maintain evidence of account deactivation and approval.

Finding 2: Cloud Data Protection Gaps

Reference: R003  
Rating: High

Inconsistent enforcement of AWS S3 public access restrictions and bucket policy reviews could expose sensitive customer information.

Recommendation:

- Enforce S3 Block Public Access where appropriate.
- Review bucket policies and access control lists.
- Validate effective permissions.
- Monitor configuration changes.
- Retain evidence of cloud security reviews.

Finding 3: Inadequate Security Monitoring

Reference: R005  
Rating: High

The assumed logging environment does not have sufficient evidence of consistent monitoring, alert review and escalation.

Recommendation:

- Establish centralised security log monitoring.
- Configure alerts for suspicious activities.
- Define incident escalation procedures.
- Maintain documented monitoring and review records.

Finding 4: Third-Party Security Risk

Reference: R006  
Rating: High

Insufficient documented vendor security assessments could make it difficult to establish whether third-party payment processors adequately protect customer information.

Recommendation:

- Conduct formal vendor security assessments.
- Review relevant security assurance evidence.
- Include appropriate security requirements in vendor agreements.
- Establish periodic vendor monitoring.

Finding 5: Backup and Recovery Assurance

Reference: R007  
Rating: High

The existence of backup configurations does not establish that critical business data can be successfully restored.

**Recommendation:**

- Conduct scheduled restoration tests.
- Validate backup integrity.
- Document recovery procedures.
- Establish and test Recovery Time Objectives (RTOs) and Recovery Point Objectives (RPOs).

8. Recommended Risk Treatment Priorities

The following actions are recommended based on the simulated risk ratings.

| Priority | Risk ID | Recommended Action | Target Timeline |
|---|---|---|---|
| 1 | R001 | Strengthen employee offboarding and access deactivation | 30 days |
| 2 | R003 | Enforce AWS S3 access restrictions and review permissions | 14 days |
| 3 | R002 | Improve phishing awareness and simulation exercises | 45 days |
| 4 | R008 | Establish vulnerability remediation deadlines and tracking | 30 days |
| 5 | R004 | Improve ransomware preparedness and incident response testing | 60 days |
| 6 | R006 | Conduct third-party security assessments | 45 days |
| 7 | R007 | Perform backup restoration and recovery testing | 30 days |
| 8 | R005 | Improve security monitoring and alert review procedures | 30 days |

The proposed actions are documented in the accompanying `risk_treatment_plan.csv`.

9. Framework Alignment

The identified risks were mapped to relevant references within:

- NIST Cybersecurity Framework (CSF) 2.0.
- ISO/IEC 27001:2022 Annex A.

The framework mapping demonstrates how the identified risks relate to recognised cybersecurity practices and information security controls.

Refer to `framework-mapping/nist_iso_mapping.md` for the detailed mapping.

Framework alignment does not establish that the organisation has implemented or complied with the referenced controls.

10. Limitations and Assumptions

This assessment is based entirely on a simulated organisational scenario.

The following limitations apply:

- NorthBridge Financial Services Ltd. is fictional.
- No actual organisational systems were accessed.
- No interviews or technical control tests were conducted.
- Existing controls are scenario assumptions rather than independently verified controls.
- Risk scores are illustrative and should not be interpreted as measured organisational exposure.
- Regulatory applicability and specific compliance obligations would require further assessment.

Residual risk scores have therefore not been reduced based on unverified control effectiveness.

11. Conclusion

The simulated assessment identified eight cybersecurity risks, including one Critical risk and seven High risks.

The findings demonstrate the importance of effective identity and access management, cloud security, employee awareness, security monitoring, third-party risk management, backup assurance and vulnerability remediation.

Management should prioritise the proposed treatment actions, assign accountable risk owners and require supporting evidence before considering remediation complete.

Risk assessments should also be reviewed periodically and updated when significant changes occur in the organisation's technology environment, threat landscape or business operations.

12. Supporting Project Documents

| Document | Location |
|---|---|
| Main Project Documentation | `README.md` |
| Risk Register | `risk-register/risk_register.csv` |
| Risk Scoring Methodology | `risk-register/risk_scoring_methodology.md` |
| Risk Treatment Plan | `risk-register/risk_treatment_plan.csv` |
| Framework Mapping | `framework-mapping/nist_iso_mapping.md` 

Disclaimer: This is a simulated cybersecurity GRC portfolio project created for professional learning and demonstration purposes. It does not represent an actual audit, certification or compliance assessment of a real organisation.
