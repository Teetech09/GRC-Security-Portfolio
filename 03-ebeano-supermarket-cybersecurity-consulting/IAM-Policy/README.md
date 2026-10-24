
 Deliverable 1: Identity and Access Management (IAM) Policy

Ebeano Supermarket Cybersecurity Consulting Project

Project Category: Governance, Risk and Compliance (GRC) / Cybersecurity Consulting  
Business: Ebeano Supermarket — Simulated Case Study  
Workforce: 28 Employees  
Document Type: Proposed IAM Policy  
Deliverable: 1 of 5  
Status: Proposed — Not Implemented

---

1. Executive Summary

Ebeano Supermarket is modeled as a growing retail business with multiple outlets in Africa. The business uses cloud-based Point-of-Sale (POS) systems, staff tablets, kitchen terminals, customer Wi-Fi, inventory systems, and social media accounts.

The original educational project brief described eight employees. This expanded portfolio scenario assumes 28 employees across eight job categories to demonstrate more comprehensive access governance and internal security controls.

The business faces several cybersecurity and operational risks, including:

- Weak and shared passwords.
- Unauthorized access to POS and financial systems.
- Unattended staff tablets.
- Phishing and social engineering attacks.
- Ransomware and business disruption.
- Unauthorized POS device substitution and payment diversion.
- Insider fraud and misuse of privileged access.

This proposed IAM policy establishes rules for authentication, authorization, employee access management, privileged accounts, dual control, segregation of duties, job rotation, mandatory leave, and monitoring.

The objective is to protect business systems and financial transactions while maintaining practical, affordable security controls.

 2. Policy Purpose and Objectives

The purpose of this policy is to ensure that employees access only the systems and information necessary to perform their assigned duties.

The policy aims to:

1. Replace shared employee accounts with individual accounts wherever supported.
2. Implement Role-Based Access Control (RBAC) and least privilege.
3. Enforce strong passwords and Multi-Factor Authentication (MFA).
4. Establish segregation of duties for sensitive activities.
5. Apply dual control to high-risk financial and administrative transactions.
6. Introduce job rotation and mandatory leave for sensitive duties.
7. Protect POS devices, payment settings, and financial records.
8. Establish employee onboarding, access changes, and offboarding procedures.
9. Monitor user activity and conduct periodic access reviews.
10. Improve accountability and reduce the likelihood of fraud and unauthorized access.

3. Scope and Organizational Structure

This policy applies to all 28 employees, business accounts, company-managed devices, and relevant third-party service providers.

3.1 Proposed Staff Distribution

| Staff Role | Number | Primary Responsibilities |
|---|---:|---|
| Store Manager | 1 | Business oversight, financial approvals, and security governance |
| Assistant Managers / Supervisors | 2 | Daily operations, staff supervision, and approved transaction reviews |
| Chefs / Kitchen Staff | 5 | Food preparation and kitchen order processing |
| Floor Sales Representatives | 10 | Customer assistance and authorized sales transactions |
| Cashiers | 5 | Payment processing and transaction recording |
| Inventory / Stock Officers | 2 | Stock management, verification, and reporting |
| Social Media / Marketing Staff | 2 | Marketing campaigns and social media management |
| IT Support / Systems Administrator | 1 | Network, device, and systems administration |
| Total | 28 | |

This staffing structure is an educational assumption rather than a verified description of a real supermarket.

 4. IAM Governance Principles

 4.1 Least Privilege

Employees must receive only the permissions required for their responsibilities.

For example, marketing staff must not access POS administration, and cashiers must not modify merchant settlement accounts.

 4.2 Role-Based Access Control (RBAC)

Access must be assigned according to approved job roles.

Any exception must be documented, justified, approved, and periodically reviewed.

4.3 Individual Accountability

Each employee must use a unique account wherever supported.

Shared employee credentials are prohibited where individual account functionality is available.

4.4 Segregation of Duties (SoD)

Critical activities must be divided among different authorized individuals to reduce fraud, errors, and misuse of access.

Examples include:

- Cashiers process payments but do not independently approve high-risk refunds.
- Inventory officers record stock adjustments, while supervisors approve significant changes.
- IT administrators maintain systems but do not independently authorize financial transactions.
- Managers approve sensitive changes but should not bypass required independent verification.

 4.5 Dual Control (Four-Eyes Principle)

Dual control requires two separate authorized employees to participate in or independently verify high-risk activities.

| Sensitive Activity | Initiator | Independent Approver / Verifier |
|---|---|---|
| High-value POS refund | Cashier | Manager or authorized supervisor |
| Settlement bank account change | Authorized administrator | Store Manager, with independent verification |
| POS device replacement | IT Administrator | Manager or authorized supervisor |
| Significant inventory adjustment | Inventory Officer | Assistant Manager |
| Privileged access assignment | IT Administrator | Store Manager |
| High-risk payment reversal | Authorized cashier | Manager or authorized supervisor |

The initiator and approver must be different individuals.

Approval records should be retained, and the system should technically enforce dual approval where supported.

Policy requirement: No employee may independently initiate, approve, and complete a high-risk transaction.

4.6 Job Rotation

Job rotation involves periodically reassigning employees to different authorized duties to improve accountability and help identify irregularities.

The supermarket should:

- Rotate cashier assignments where practical.
- Rotate stock verification responsibilities.
- Alternate supervisory review duties between assistant managers.
- Ensure replacement employees are trained before receiving new duties.
- Review and remove temporary access after assignments end.
- Preserve segregation of duties during rotation.

A proposed rotation schedule is every three to six months for suitable sensitive roles, subject to staffing and operational requirements.

4.7 Mandatory Leave

Employees handling sensitive financial, payment, inventory, or administrative responsibilities should take planned leave according to applicable employment rules.

During the employee's absence:

- An authorized replacement performs the relevant duties.
- Outstanding transactions and records are independently reviewed.
- Unusual discrepancies are escalated.
- Access may be temporarily adjusted where appropriate.
- Normal permissions are restored only after the temporary assignment is completed.

Mandatory leave is intended to support fraud detection and business continuity, not to imply employee wrongdoing.

4.8 Default Deny

Access must be denied unless explicitly approved and assigned.

4.9 Need-to-Know

Employees may access sensitive business information only when it is necessary for their assigned responsibilities.

5. Role-Based Access Control Matrix

Access Legend

- Admin: Authorized administration.
- Approve: Authorized business approval.
- Operate: Routine operational access.
- View: Read-only access.
- Support: Restricted technical maintenance.
- None: No access.

| Employee Role | POS | Kitchen | Inventory | Social Media | Network Admin |
|---|---|---|---|---|---|
| Store Manager | Approve / View | View if needed | View / Approve | Approve | None |
| Assistant Managers | View / Approve | View if needed | View / Approve | None | None |
| Chefs / Kitchen Staff | None | Operate | None | None | None |
| Floor Sales Representatives | Operate | None | None | None | None |
| Cashiers | Operate | None | None | None | None |
| Inventory Officers | Limited inventory-related functions | None | Operate | None | None |
| Social Media Staff | None | None | None | Operate | None |
| IT Administrator | Support | Support | Support | None | Admin |

The POS platform's actual capabilities must be reviewed before these permissions are implemented.

Technical support access must not automatically grant financial approval privileges.

6. Password and Credential Management

6.1 Password Requirements

Employees must:

1. Use unique passwords for each business system.
2. Use passwords of at least 15 characters where supported.
3. Prefer memorable passphrases.
4. Avoid common, predictable, or previously compromised passwords.
5. Never share passwords through messaging apps, paper notes, or unsecured files.
6. Store credentials in an approved password manager.
7. Report suspected credential compromise immediately.
8. Replace vendor default credentials before devices are deployed.

Routine password changes are not required without evidence of compromise, unless mandated by applicable system or contractual requirements.

6.2 Shared Organizational Accounts

Where individual accounts are unavailable:

- Access must be explicitly authorized.
- Credentials must be stored in an approved password manager.
- Access must be restricted to designated employees.
- Available activity logs must be reviewed.
- Credentials must be rotated after relevant staff departures or suspected compromise.

The business should prioritize replacing shared accounts with individually attributable access.

 7. Multi-Factor Authentication (MFA)

MFA must be required for privileged and sensitive accounts wherever the platform supports it.

| Account / System | MFA Requirement |
|---|---|
| Store Manager | Mandatory |
| Assistant Managers with privileged access | Mandatory |
| Cloud POS Administration | Mandatory where supported |
| Social Media Accounts | Mandatory |
| IT Administrator | Mandatory |
| Router Administration | Enable where supported |
| General POS User Accounts | Enable where supported |

Preferred methods include passkeys, security keys, and authenticator applications.

SMS authentication should be treated as a fallback where stronger options are unavailable.

Unexpected MFA prompts must be reported immediately.

8. Employee Access Lifecycle Management

8.1 Onboarding

1. Manager approves the employee's role.
2. IT creates an individual account where supported.
3. Approved RBAC permissions are assigned.
4. MFA is configured where required.
5. Staff receive security awareness training.
6. Assigned devices are recorded in the asset register.
7. Access approval records are retained.

 8.2 Role Changes

1. Review current access.
2. Remove unnecessary permissions.
3. Obtain approval for additional permissions.
4. Check for segregation-of-duties conflicts.
5. Document temporary or permanent changes.

 8.3 Offboarding

1. Disable employee accounts promptly.
2. Revoke active sessions where supported.
3. Remove POS, social media, and cloud access.
4. Recover assigned devices and access cards.
5. Rotate any shared credentials the employee could access.
6. Update access and asset inventories.

9. POS Security and Payment Fraud Prevention

 9.1 Approved POS Devices

The supermarket must maintain an inventory of authorized POS devices.

Each record should include:

- Device serial number.
- Merchant or payment provider identifier.
- Assigned outlet.
- Assigned custodian.
- Device status.
- Date of registration or replacement.

Staff must not substitute personal POS devices for approved company payment terminals.

 9.2 Payment Settlement Controls

- Restrict settlement account changes.
- Require independent approval and verification of bank details.
- Record configuration changes.
- Apply dual control to high-risk refunds and reversals.
- Investigate unexplained transaction discrepancies.

 9.3 Daily Transaction Reconciliation

An authorized supervisor or manager should compare:

- POS transaction records.
- Daily sales reports.
- Refund and reversal records.
- Payment provider settlement reports.
- Bank settlement records.

Unexplained differences must be escalated.

9.4 Physical POS Verification

At the beginning of each shift, designated staff should verify that the approved POS device is present and shows no signs of substitution or tampering.

Suspicious devices must not be used until verified by authorized personnel.

10. Privileged Access Management

Privileged accounts must receive stronger protection.

Required controls include:

- Separate administrative and routine accounts where supported.
- MFA for privileged access.
- Manager approval before elevated access is granted.
- Restricted remote administration.
- Logging of administrative changes.
- Monthly privileged access reviews.
- Prompt removal of unused privileged accounts.
- Time-limited elevated permissions where supported.

The IT Administrator must not independently approve financial transactions or changes to payment settlement accounts.

11. Monitoring, Reviews, and Internal Controls

| Control Activity | Responsible Role | Proposed Frequency |
|---|---|---|
| POS exception review | Manager / Supervisor | Daily |
| Payment reconciliation | Manager / Authorized Supervisor | Daily |
| POS device verification | Assigned Custodian | Each shift |
| POS inventory review | Manager / IT Administrator | Weekly |
| User access review | Manager / IT Administrator | Monthly |
| Privileged access review | Manager / IT Administrator | Monthly |
| Social media access review | Manager / Marketing Lead | Monthly |
| Job rotation review | Manager | Every 3–6 months |
| Mandatory leave planning | Manager | Annually |
| IAM policy review | Manager / IT Administrator | Annually and after major changes |

Independent reviewers must not approve their own transactions.

 12. Incident Reporting and Response

Employees must report:

- Suspicious login attempts.
- Unexpected MFA prompts.
- Lost or stolen tablets.
- Unrecognized POS devices.
- Unauthorized refunds.
- Suspected payment diversion.
- Compromised passwords.
- Suspicious messages requesting credentials.
- Unexplained inventory or settlement discrepancies.

The authorized response team should:

1. Record the report.
2. Assess the potential impact.
3. Restrict affected accounts or devices where necessary.
4. Preserve logs and transaction records.
5. Investigate and escalate appropriately.
6. Restore normal operations after containment.
7. Document lessons learned.

13. Policy Ownership and Responsibilities

| Role | IAM Responsibility |
|---|---|
| Store Manager | Policy approval, risk ownership, sensitive access authorization |
| Assistant Managers | Operational oversight and independent approvals |
| IT Administrator | Account provisioning, technical controls, logging, and access changes |
| Cashiers | Authorized payment processing and incident reporting |
| Inventory Officers | Stock recording and discrepancy reporting |
| Marketing Staff | Secure management of approved social media access |
| All Employees | Compliance with access rules and timely incident reporting |

14. Implementation Priorities

| Priority | Security Control | Expected Benefit |
|---|---|---|
| Critical | Individual employee accounts | Improves accountability |
| Critical | MFA for privileged accounts | Reduces account compromise |
| Critical | POS device verification | Reduces payment diversion risk |
| High | Dual control for refunds and settlement changes | Reduces single-person fraud opportunities |
| High | Segregation of duties | Limits conflicting permissions |
| High | Restricted privileged access | Reduces administrative misuse |
| High | Onboarding and offboarding procedures | Reduces unauthorized access |
| Medium | Password manager | Improves credential security |
| Medium | Monthly access reviews | Identifies excessive permissions |
| Medium | Job rotation | Supports independent review and fraud detection |
| Medium | Mandatory leave | Supports accountability and continuity |
| Medium | Device inventory | Improves asset tracking |

15. Expected Business Benefits

If implemented effectively, the proposed IAM policy would help Ebeano Supermarket:

- Protect customer payment operations.
- Reduce unauthorized system access.
- Improve accountability across 28 employees.
- Reduce opportunities for insider fraud.
- Detect suspicious financial and inventory activity.
- Strengthen management oversight.
- Improve employee access governance.
- Establish practical security controls suitable for a growing retail business.

16. Policy Review and Approval

Policy Owner: Store Manager  
Technical Custodian: IT Support / Systems Administrator  
Review Frequency: At least annually, and after major operational or security changes  
Approval Status: Pending — Simulated Scenario

The policy should be reviewed and formally approved before implementation in a real business.

17. Implementation Status and Disclaimer

Status: Proposed — Not Implemented

This IAM policy was developed for an educational cybersecurity consulting project.

The original project brief described eight employees. This expanded portfolio version assumes a 28-person workforce and introduces additional controls to demonstrate IAM governance, segregation of duties, dual control, job rotation, and fraud prevention.

The recommendations are proposed controls. They do not represent verified deployment in a live supermarket environment.

---

Project: Ebeano Supermarket Cybersecurity Consulting  
Category: GRC / Identity and Access Management  
Deliverable: 1 of 5 — IAM Policy
  

