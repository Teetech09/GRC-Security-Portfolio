 Deliverable 5: Top Three Cybersecurity Risks and Affordable Mitigation Strategies

Ebeano Supermarket Cybersecurity Consulting Project

Category: Governance, Risk and Compliance (GRC) / Cybersecurity Risk Management  
Business: Ebeano Supermarket — Simulated Case Study  
Workforce: 28 Employees  
Deliverable:5 of 5  
Status: Proposed — Not Implemented


1. Executive Summary

Ebeano Supermarket is modeled as a growing retail business with 28 employees, cloud-based Point-of-Sale (POS) systems, customer Wi-Fi, staff tablets, kitchen terminals, inventory systems, and social media accounts.

The business faces cybersecurity and operational risks that could affect financial transactions, customer trust, business continuity, and the availability of critical services.

This assessment identifies the three highest-priority risks in the simulated scenario:

1. POS Payment Fraud and Unauthorized Device Substitution
2. Phishing, Credential Theft, and Account Compromise
3. Ransomware and Unauthorized Access Through Poor Network Segmentation

The assessment evaluates the potential likelihood and business impact of each risk, recommends affordable controls, and establishes an implementation roadmap.

The objective is to help supermarket management make informed, risk-based security decisions without requiring an expensive enterprise cybersecurity program.

2. Risk Assessment Objectives

The objectives are to:

- Identify the most significant cybersecurity threats to the supermarket.
- Evaluate business impact and likelihood.
- Prioritize risks requiring immediate attention.
- Recommend affordable and practical mitigation measures.
- Assign responsibility for risk treatment.
- Estimate residual risk after proposed controls.
- Establish a phased implementation roadmap.
- Support management decision-making and accountability.

3. Assessment Scope

The assessment covers the following business assets and processes:

- POS terminals and payment processing.
- Staff tablets and workstations.
- Cloud-based business applications.
- Employee accounts and credentials.
- Customer and staff Wi-Fi.
- Kitchen and inventory systems.
- Social media accounts.
- Network infrastructure.
- Sensitive operational and financial information.

This is a qualitative, scenario-based assessment. No live vulnerability scanning, penetration testing, site inspection, or technical validation has been performed.

4. Risk Assessment Methodology

A simple 5 × 5 qualitative risk matrix is used.

Risk is calculated as:

Risk Score = Likelihood × Impact

 4.1 Likelihood Scale

| Score | Rating | Description |
|---|---|---|
| 1 | Rare | Unlikely under normal circumstances |
| 2 | Unlikely | Possible but not expected frequently |
| 3 | Possible | Could occur under realistic conditions |
| 4 | Likely | Expected to occur without adequate controls |
| 5 | Almost Certain | Highly likely or repeatedly expected |

4.2 Impact Scale

| Score | Rating | Description |
|---|---|---|
| 1 | Insignificant | Minimal disruption or financial loss |
| 2 | Minor | Limited operational or financial impact |
| 3 | Moderate | Noticeable disruption or recoverable loss |
| 4 | Major | Significant financial loss or service interruption |
| 5 | Severe | Critical financial, operational, or reputational damage |

 4.3 Risk Rating Thresholds

| Risk Score | Risk Level | Recommended Response |
|---|---|---|
| 1–4 | Low | Monitor and maintain controls |
| 5–9 | Medium | Plan and implement improvements |
| 10–16 | High | Prioritize mitigation |
| 17–25 | Critical | Immediate management attention |

The scoring thresholds are proposed for this educational scenario.

5. Top Three Cybersecurity Risks

Risk 1: POS Payment Fraud and Unauthorized Device Substitution

Risk ID: EBS-R01  
Risk Category: Financial Fraud / Physical and Cybersecurity  
Affected Assets: POS Terminals, Payment Accounts, Financial Records

 Risk Description

An unauthorized individual or dishonest employee could replace an approved POS terminal with a personal or fraudulent device.

Customers may unknowingly make payments into an unauthorized merchant account rather than the supermarket's legitimate account.

Weak device verification procedures, insufficient supervision, and inadequate transaction reconciliation could allow the fraud to continue undetected.

Potential Business Impact

- Direct financial losses.
- Payment diversion.
- Customer complaints.
- Reconciliation discrepancies.
- Reputational damage.
- Disruption of checkout operations.

Inherent Risk Assessment

Likelihood: 4 — Likely  
**Impact:** 5 — Severe  
**Risk Score:** 4 × 5 = **20 — Critical**

 Recommended Mitigation Controls

1. Maintain an approved POS asset register.
2. Label and verify POS terminals at the beginning of each shift.
3. Record merchant identifiers and device serial numbers.
4. Require dual control for POS replacement.
5. Independently verify settlement account changes.
6. Reconcile daily sales with payment provider and bank settlement reports.
7. Train cashiers to recognize suspicious devices.
8. Restrict access to POS configuration and administration.
9. Investigate unexplained payment discrepancies promptly.

 Affordable Implementation Approach

The supermarket can begin with printed asset labels, a spreadsheet-based POS register, daily verification checklists, and management approval procedures.

These controls require limited technology investment and can significantly improve accountability.

Proposed Residual Risk

Likelihood:2 — Unlikely  
Impact: 5 — Severe  
Residual Score: 2 × 5 = 10 — High

Even after controls are introduced, a successful payment diversion incident could still have severe consequences. Continued monitoring is necessary.

---

 Risk 2: Phishing, Credential Theft, and Account Compromise

Risk ID: EBS-R02  
Risk Category: Social Engineering / Identity Security  
Affected Assets: Employee Accounts, Cloud Applications, Social Media, Business Email

Risk Description

Employees may receive fraudulent emails, text messages, social media messages, or calls designed to obtain passwords, MFA codes, financial information, or unauthorized payments.

Attackers may impersonate suppliers, brand representatives, managers, or IT support personnel.

Shared passwords and limited awareness can increase the likelihood of successful account compromise.

Potential Business Impact

- Unauthorized access to business accounts.
- Fraudulent supplier payments.
- Social media account takeover.
- Disclosure of sensitive business information.
- Unauthorized POS activity.
- Reputational damage.

Inherent Risk Assessment

Likelihood: 4 — Likely  
Impact: 4 — Major  
Risk Score: 4 × 4 = 16 — High

Recommended Mitigation Controls

1. Require MFA for sensitive and privileged accounts.
2. Use individual employee accounts.
3. Implement role-based access control.
4. Train employees to identify phishing messages.
5. Verify unusual payment requests independently.
6. Use an approved password manager.
7. Restrict administrative permissions.
8. Conduct periodic access reviews.
9. Establish a simple suspicious-message reporting procedure.
10. Conduct management-approved phishing simulations.

Affordable Implementation Approach

The supermarket can begin with authenticator applications, short monthly security briefings, supplier verification procedures, and existing platform security settings.

 Proposed Residual Risk

Likelihood: 2 — Unlikely  
Impact: 4 — Major  
Residual Score: 2 × 4 = 8 — Medium

Phishing cannot be completely eliminated, but awareness, MFA, and access restrictions can reduce the likelihood of successful attacks.



Risk 3: Ransomware and Unauthorized Access Through Poor Network Segmentation

Risk ID: EBS-R03  
Risk Category: Network Security / Business Continuity  
Affected Assets: Guest Wi-Fi, POS Devices, Staff Tablets, Kitchen Terminals, Network Infrastructure

Risk Description

If customer Wi-Fi and operational systems share an inadequately protected network, compromised devices may be able to communicate with sensitive business systems.

Weak network segmentation, unpatched devices, and excessive access permissions may increase opportunities for unauthorized access or malware propagation.

A ransomware incident could interrupt payment processing, inventory operations, or other essential services.

Potential Business Impact

- Checkout and payment disruption.
- Loss of access to operational systems.
- Business downtime.
- Recovery expenses.
- Potential data exposure.
- Customer dissatisfaction.

 Inherent Risk Assessment

Likelihood:3 — Possible  
Impact: 5 — Severe  
Risk Score: 3 × 5 = 15 — High

Recommended Mitigation Controls

1. Separate guest Wi-Fi from operational networks.
2. Isolate POS devices using appropriate network segmentation.
3. Configure firewall rules to deny unnecessary inter-network traffic.
4. Restrict network administration.
5. Apply security updates to supported devices.
6. Deploy endpoint protection where appropriate.
7. Maintain protected, tested backups of important business data.
8. Restrict unnecessary administrative privileges.
9. Monitor suspicious network activity.
10. Develop and test a basic incident response and recovery procedure.

Affordable Implementation Approach

The supermarket should first check whether its existing router supports guest isolation, firewall rules, and VLANs.

Where existing equipment is insufficient, upgrades should be phased according to business risk and budget.

Proposed Residual Risk

Likelihood:2 — Unlikely  
Impact: 4 — Major  
Residual Score: 2 × 4 = 8 — Medium

Network segmentation reduces potential lateral movement, while backups and recovery planning may reduce the impact of an incident.



6. Consolidated Risk Register

| Risk ID | Risk Description | Inherent Likelihood | Inherent Impact | Inherent Score | Inherent Rating | Proposed Residual Score | Residual Rating |
|---|---|---:|---:|---:|---|---:|---|
| EBS-R01 | POS Payment Fraud and Device Substitution | 4 | 5 | 20 | Critical | 10 | High |
| EBS-R02 | Phishing and Credential Compromise | 4 | 4 | 16 | High | 8 | Medium |
| EBS-R03 | Ransomware and Poor Network Segmentation | 3 | 5 | 15 | High | 8 | Medium |

Important: Residual risk scores estimate the risk assuming recommended controls are implemented and operate effectively. They are not verified results.

7. Risk Heat Map

The following matrix shows the initial risk positions.

| Likelihood \\ Impact | 1 | 2 | 3 | 4 | 5 |
|---|---|---|---|---|---|
| 5 — Almost Certain | — | — | — | — | — |
| 4 — Likely | — | — | — | R02 | R01 |
| 3 — Possible | — | — | — | — | R03 |
| 2 — Unlikely | — | — | — | — | — |
| 1 — Rare | — | — | — | — | — |

R01: POS Payment Fraud  
R02:Phishing and Credential Compromise  
R03: Ransomware and Network Exposure

 8. Risk Treatment and Ownership

| Risk ID | Risk Treatment | Proposed Risk Owner | Supporting Roles |
|---|---|---|---|
| EBS-R01 | Mitigate | Store Manager | Cashiers, Supervisors, IT Administrator |
| EBS-R02 | Mitigate | Store Manager | IT Administrator, All Employees |
| EBS-R03 | Mitigate | Store Manager | IT Administrator, Supervisors |

The Store Manager is responsible for approving risk treatment decisions and accepting any remaining risk.

The IT Administrator provides technical support, while supervisors and employees carry out operational controls.

9. Affordable Security Implementation Roadmap

 Phase 1: Immediate Actions — First 30 Days

Priority: Critical

- Establish an approved POS device register.
- Introduce POS verification at the start of each shift.
- Require dual approval for high-risk payment changes.
- Enable MFA on sensitive accounts.
- Replace shared credentials where supported.
- Separate customer Wi-Fi from business systems where existing equipment allows.
- Deliver an initial five-minute phishing awareness briefing.

Expected Outcome: Reduced exposure to payment fraud, account compromise, and unauthorized network access.

Phase 2: Short-Term Improvements — Days 31–60

**Priority: High**

- Review employee access permissions.
- Implement or improve network firewall restrictions.
- Restrict POS administration.
- Establish daily payment reconciliation procedures.
- Secure staff tablets and network equipment.
- Introduce visitor and contractor procedures.
- Review software update practices.
- Establish protected backups for essential business information.

Expected Outcome: Improved operational accountability and reduced opportunities for unauthorized access.

 Phase 3: Medium-Term Improvements — Days 61–90

Priority: Medium to High

- Test backup restoration.
- Review network segmentation effectiveness.
- Conduct an approved phishing awareness exercise.
- Introduce a formal incident reporting register.
- Review POS device inventory and reconciliation records.
- Assess whether Mobile Device Management is affordable.
- Establish job rotation and mandatory leave procedures.
- Review unresolved risks and update the risk register.

Expected Outcome: Improved monitoring, recovery readiness, and ongoing risk governance.

10. Cost-Conscious Control Prioritization

| Security Measure | Relative Cost | Risk Reduction Value |
|---|---|---|
| POS verification checklist | Low | High |
| Spreadsheet-based asset register | Low | High |
| MFA using supported applications | Low | High |
| Monthly staff awareness briefing | Low | High |
| Supplier payment verification | Low | High |
| Dual approval procedures | Low | High |
| Device auto-lock settings | Low | Medium to High |
| Guest Wi-Fi isolation using existing equipment | Low if supported | High |
| Protected backup solution | Low to Moderate | High |
| Managed firewall / VLAN-capable equipment | Moderate | High |
| Mobile Device Management | Moderate | Medium to High |

Actual costs depend on existing equipment, software subscriptions, service providers, and the number of supermarket outlets.

11. Key Risk Indicators and Monitoring

| Indicator | Proposed Monitoring Frequency | Responsible Role |
|---|---|---|
| Unverified POS devices | Each shift | Cashier / Supervisor |
| Unexplained payment discrepancies | Daily | Store Manager |
| Suspicious messages reported | Monthly | IT Administrator |
| Privileged accounts without MFA | Monthly | IT Administrator |
| Inactive employee accounts | Monthly | IT Administrator |
| Unauthorized guest-to-business connectivity | After network changes and periodically | IT Administrator |
| Backup restoration failures | Quarterly | IT Administrator |
| Overdue critical security actions | Monthly | Store Manager |

12. Risk Acceptance and Escalation

Risk acceptance should be a documented management decision.

- Critical risks: Require immediate management attention and a documented treatment plan.
- High risks: Require prioritized mitigation and management oversight.
- Medium risks: Require scheduled treatment and periodic monitoring.
- Low risks: May be monitored under routine controls.

Any residual risk that exceeds the supermarket's approved risk tolerance must be escalated to the Store Manager.

Risk acceptance should not be used to bypass applicable legal, contractual, or payment provider requirements.

13. Management Recommendations

Based on this simulated assessment, the following actions are recommended:

1. Protect payment revenue first. Establish POS verification, dual control, and daily reconciliation.
2. Protect employee identities. Implement MFA, individual accounts, and regular awareness training.
3. Separate customer and business networks. Prioritize guest Wi-Fi isolation and protect the POS network.
4. Improve accountability. Maintain access, asset, incident, and risk registers.
5. Review progress regularly. Track completion of high-priority security actions and update the risk assessment.

The recommended approach emphasizes affordable administrative and technical controls before major infrastructure investments.

14. Expected Business Benefits

If implemented effectively, the recommended controls could:

- Reduce payment fraud opportunities.
- Improve protection of employee accounts.
- Limit unauthorized access to business systems.
- Reduce operational disruption.
- Improve incident detection and response.
- Support management accountability.
- Strengthen customer confidence.
- Establish a foundation for continuous cybersecurity improvement.

 15. Limitations and Assumptions

This assessment is based on an educational case study and the expanded 28-employee workforce assumption.

The following information has not been independently verified:

- Existing network configuration.
- Actual POS device inventory.
- Current security controls.
- Employee access permissions.
- Historical incident records.
- Business financial exposure.
- Available security budget.
- Actual number and configuration of outlets.

Risk scores represent professional judgment applied to the simulated scenario, not measurements from a live environment.

16. Implementation Status and Disclaimer

Status: Proposed — Not Implemented

This risk assessment was prepared for a simulated cybersecurity consulting portfolio engagement.

No live risk assessment, penetration test, physical inspection, employee training, or security control deployment has been performed.

All recommendations, scores, and projected outcomes are illustrative and require validation before implementation in a real business environment.



Project: Ebeano Supermarket Cybersecurity Consulting  
Category: GRC / Cybersecurity Risk Management  
Deliverable: 5 of 5 — Top Three Cybersecurity Risks and Affordable Mitigation Strategies
