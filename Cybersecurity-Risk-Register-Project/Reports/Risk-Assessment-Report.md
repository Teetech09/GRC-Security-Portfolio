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

| Risk ID | Risk Description | Inherent Score | Inherent Rating |Provisional Residual Score |Provisional Residual Rating |
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

The assessment indicates that all identified risks require management attention, with R001 receiving the highest priority due to its Critical rating.

The residual risk scores are currently provisional and remain equal to the inherent risk scores. This is because the effectiveness of existing security controls has not been independently verified through evidence collection, control testing or formal assessment.

No reduction in risk has therefore been assumed. Residual risk ratings should be reassessed when sufficient evidence is available to demonstrate that existing or newly implemented controls are operating effectively.

The organisation should prioritise the recommended risk treatment actions and maintain supporting evidence to demonstrate control effectiveness before updating residual risk ratings.



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

Finding 2: Phishing Attacks and Employee Security Awareness

Reference: R002  
Rating: High

The simulated assessment identified potential exposure to phishing attacks due to the risk of employees interacting with malicious emails, links or attachments.

Successful phishing attacks could result in compromised user credentials, unauthorised access to organisational systems, exposure of sensitive customer information and possible business disruption.

The effectiveness of existing email security configurations and employee security awareness measures has not been independently verified.

Recommendation:

- Strengthen email security configurations to detect and filter malicious messages.
- Enforce Multi-Factor Authentication (MFA) for user accounts.
- Conduct regular employee security awareness training.
- Perform periodic phishing simulation exercises.
- Monitor phishing incidents and document lessons learned.

Finding 3: Cloud Data Protection Gaps

Reference: R003  
Rating: High

Inconsistent enforcement of AWS S3 public access restrictions and bucket policy reviews could expose sensitive customer information.

Recommendation:

- Enforce S3 Block Public Access where appropriate.
- Review bucket policies and access control lists.
- Validate effective permissions.
- Monitor configuration changes.
- Retain evidence of cloud security reviews.

  Finding 4: Ransomware Exposure and Incident Response Preparedness

Reference: R004  
Rating: High

The simulated assessment identified potential exposure to ransomware attacks that could disrupt banking operations, encrypt critical business data and affect the availability of customer-facing services.

Inadequate endpoint protection, insufficient incident detection capabilities or untested recovery procedures could increase the impact of a ransomware incident.

The effectiveness of existing endpoint protection, backup restoration and incident response controls has not been independently verified.

Recommendation:

- Strengthen endpoint protection and malware detection capabilities.
- Maintain regular and secure backups of critical business data.
- Conduct periodic backup restoration tests.
- Establish and maintain a documented ransomware incident response procedure.
- Conduct incident response tabletop exercises to evaluate organisational preparedness.



Finding 5: Inadequate Security Monitoring

Reference: R005  
Rating: High

The assumed logging environment does not have sufficient evidence of consistent monitoring, alert review and escalation.

Recommendation:

- Establish centralised security log monitoring.
- Configure alerts for suspicious activities.
- Define incident escalation procedures.
- Maintain documented monitoring and review records.

Finding 6: Third-Party Security Risk

Reference: R006  
Rating: High

Insufficient documented vendor security assessments could make it difficult to establish whether third-party payment processors adequately protect customer information.

Recommendation:

- Conduct formal vendor security assessments.
- Review relevant security assurance evidence.
- Include appropriate security requirements in vendor agreements.
- Establish periodic vendor monitoring.

Finding 7: Backup and Recovery Assurance

Reference: R007  
Rating: High

The existence of backup configurations does not establish that critical business data can be successfully restored.

Recommendation:

- Conduct scheduled restoration tests.
- Validate backup integrity.
- Document recovery procedures.
- Establish and test Recovery Time Objectives (RTOs) and Recovery Point Objectives (RPOs).

Finding 8: Unpatched System Vulnerabilities and Patch Management Gaps

Reference: R008  
Rating: High

The simulated assessment identified potential exposure arising from systems and applications that may contain unpatched security vulnerabilities.

Attackers could exploit known vulnerabilities to gain unauthorised access, compromise sensitive information, disrupt business operations or establish persistence within the organisation's technology environment.

Insufficient vulnerability tracking, delayed patch deployment, or inadequate verification of remediation could increase the organisation's exposure to known threats.

The effectiveness of existing vulnerability management and patch management controls has not been independently verified.

Recommendation:

- Establish a formal vulnerability management procedure.
- Conduct regular vulnerability scans across organisational systems.
- Prioritise vulnerabilities based on severity and business impact.
- Define patch deployment timelines and remediation responsibilities.
- Maintain a vulnerability remediation tracking register.
- Perform follow-up scans to verify that identified vulnerabilities have been successfully addressed.
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
Residual risk scores remain provisional because the effectiveness of existing security controls has not been independently verified. The assessment does not assume that documented or assumed controls are fully implemented or operating effectively.

A further assessment should be conducted after relevant evidence has been collected and control effectiveness has been evaluated. Residual risk ratings should then be updated to reflect the actual effectiveness of the controls and any remaining exposure.
This assessment is based entirely on a simulated organisational scenario.

The following limitations apply:

- NorthBridge Financial Services Ltd. is fictional.
- No actual organisational systems were accessed.
- No interviews or technical control tests were conducted.
- Existing controls are scenario assumptions rather than independently verified controls.
- Risk scores are illustrative and should not be interpreted as measured organisational exposure.
- Regulatory applicability and specific compliance obligations would require further assessment.

Residual risk scores remain provisional because the effectiveness of existing security controls has not been independently verified. The assessment does not assume that documented or assumed controls are fully implemented or operating effectively.


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

Disclaimer: This is a simulated cybersecurity GRC portfolio project created for professional learning and demonstration purposes. It does not represent an actual audit, certification, or compliance assessment of a real organisation.
