
# MediHealth Clinic — Incident Response Plan

## 1. Document Control

| Item | Details |
|---|---|
| Plan ID | MHC-PLAN-003 |
| Version | 1.0 |
| Status | Proposed — educational portfolio |
| Author | Titilayo Yusuf |
| Proposed owner | IT lead |
| Approval authority | Clinic management |
| Review | Annually and after significant incidents or changes |

## 2. Purpose

Provide a coordinated process for identifying, assessing, containing, and recovering from cybersecurity incidents.

The priorities are to protect patient safety, limit information exposure, preserve evidence, and restore trustworthy services.

## 3. Scope

This plan covers suspected or confirmed incidents involving:

- Phishing and compromised accounts.
- Malware and ransomware.
- Unauthorised access to patient information.
- Unauthorised changes to records.
- Lost or stolen devices.
- Disruption of clinic systems.
- Unauthorised physical access affecting information or equipment.

An EHR outage requires assessment. Hardware failure alone does not establish a cyberattack, although it may require continuity and recovery procedures.

## 4. Preparation

Before adopting this plan, management must:

- Assign response roles and deputies.
- Confirm reporting channels and escalation contacts.
- Establish an alternative communication method if email is unavailable or compromised.
- Arrange EHR vendor and external technical support.
- Maintain an asset inventory and relevant logging.
- Approve clinical downtime and emergency access procedures.
- Make protected copies of essential response instructions available during outages.

Contact details belong in a restricted operational contact list. Do not publish them in the public portfolio.

## 5. Roles and Responsibilities

| Proposed role | Responsibility |
|---|---|
| Incident coordinator | Coordinate actions, maintain the incident record, and escalate decisions. |
| IT lead | Investigate technical issues, preserve evidence, and carry out authorised containment and recovery. |
| Clinical operations lead | Assess effects on care and activate approved downtime procedures. |
| Clinic management | Authorise major operational decisions, resources, and external communications. |
| Designated privacy or legal adviser | Assess notification obligations and advise on sensitive information handling. |
| EHR vendor or external specialist | Provide support within agreed access and evidence-handling boundaries. |
| Employees | Report concerns promptly and follow response instructions. |

One person may hold more than one role in a small clinic. Responsibilities and deputies must still be clear.

## 6. Reporting an Incident

Employees should report immediately through the approved route when they notice:

- A suspicious email or unexpected authentication prompt.
- Credentials entered into an unfamiliar website.
- Unexpected file encryption or a ransom message.
- Missing equipment.
- Unusual access to records.
- Unexplained changes to patient information.
- Unexpected system disruption.

Include:

- What happened.
- When it was noticed.
- The affected device, account, or service.
- Any action already taken.
- Whether patient care appears affected.

Do not include passwords or unnecessary patient information.

Staff must not investigate independently, contact suspected attackers, or publish incident details.

## 7. Initial Assessment

The incident coordinator and IT lead should:

1. Create an incident identifier.
2. Record the report and discovery time, including timezone.
3. Establish known facts and distinguish them from assumptions.
4. Identify affected systems, accounts, and information.
5. Assess immediate effects on patient care.
6. Determine whether the activity is an incident or another operational issue.
7. Assign severity and initiate the required response.

Update the assessment as evidence changes.

## 8. Severity and Escalation

| Severity | Example | Proposed escalation |
|---|---|---|
| Critical | Widespread ransomware, major suspected record alteration, or an outage threatening safe care | Immediately notify IT, clinical leadership, and management; activate coordinated response. |
| High | Suspected privileged account compromise or significant patient information exposure | Urgent coordinated investigation and management notification. |
| Moderate | A contained endpoint incident without known wider impact | IT-led investigation with escalation if scope increases. |
| Low | Suspicious message with no identified interaction or compromise | Review, record, and address through normal reporting procedures. |

Examples guide judgement. Severity depends on actual scope, exposure, and patient care impact.

These are proposed internal categories, not statutory reporting deadlines.

## 9. Containment

IT selects containment actions according to the incident and clinical impact.

Possible actions include:

- Isolating an affected endpoint from the network.
- Restricting a compromised account.
- Revoking active sessions and affected authenticators.
- Blocking confirmed malicious destinations or messages.
- Restricting access to an affected system.
- Protecting backups from further compromise.

For major clinical systems, coordinate disruptive actions with clinical leadership wherever feasible. Pre-authorised emergency actions should be documented.

Employees should avoid rebooting, wiping, or changing affected equipment unless instructed. Immediate safety and containment needs may take priority, and the reason must be recorded.

## 10. Evidence Preservation

Authorised responders should preserve relevant:

- Original emails and headers.
- Authentication and system logs.
- Alert records.
- Incident timelines.
- Relevant files or forensic copies.
- Records of containment and recovery actions.

For each evidence item, record:

- A unique identifier.
- Source and collection time.
- Collector.
- Collection method.
- Secure storage location.
- Transfers and access.
- Integrity checks, such as hashes, where appropriate.

Restrict access and avoid unnecessary changes to originals.

Never upload real incident evidence containing patient information, credentials, or sensitive infrastructure details to public GitHub.

## 11. Investigation and Remediation

Determine:

- How the incident began.
- Which accounts and systems were affected.
- Whether information was viewed, copied, altered, or lost.
- Whether unauthorised access remains.
- Which controls failed or were missing.

Remediation may include removing malware, rebuilding affected systems, fixing vulnerabilities, replacing exposed credentials, or correcting access permissions.

Use qualified external support where the clinic lacks the required capability.

Do not declare the cause confirmed without supporting evidence.

## 12. Recovery

Follow the backup and recovery plan where restoration is required.

Before returning to normal operation:

1. Address the known cause and remaining access paths.
2. Select and validate an appropriate recovery point.
3. Restore in a controlled environment.
4. Verify system operation and security controls.
5. Obtain clinical validation where patient records or workflows are affected.
6. Reconcile approved downtime records.
7. Obtain the required return-to-service authorisation.
8. Monitor for recurrence.

Recovery of a system does not establish whether information was previously stolen. Investigate confidentiality impacts separately.

## 13. Scenario Response Guides

### A. Phishing With Credentials Entered

- Record the employee’s report.
- Preserve the message.
- Protect the affected account through appropriate resets and session revocation.
- Review authentication activity and relevant account changes.
- Assess access to patient information and connected services.
- Support the employee and reinforce safe reporting.

### B. Suspected Ransomware

- Escalate urgently.
- Coordinate isolation and clinical downtime actions.
- Protect backups and preserve evidence.
- Assess the scope and possible information theft.
- Engage appropriate specialist support.
- Restore only after assessing and addressing the compromise.

Staff must not negotiate, promise payment, or communicate with attackers independently.

### C. Lost or Stolen Device

- Record the device, circumstances, and last known location.
- Assess encryption, stored information, and active sessions.
- Revoke access and use approved remote lock or wipe capabilities where appropriate.
- Consider evidence needs before destructive actions.
- Assess potential information exposure.

### D. Suspected Patient Record Alteration

- Notify clinical leadership immediately.
- Preserve relevant records and logs.
- Restrict affected access as appropriate.
- Have authorised clinical staff validate information using trusted sources.
- Correct records through an accountable process that preserves the audit trail.

## 14. Communication and Notifications

Use a trusted alternative channel if clinic email may be compromised.

Internal updates should state:

- Confirmed facts.
- Effects on services.
- Actions staff need to take.
- The next planned update.

Management must authorise external communications.

The designated privacy or legal adviser must promptly assess applicable notification requirements, recipients, thresholds, and deadlines. Record the decision and its basis.

This educational plan does not establish Nigerian legal notification deadlines or assume that HIPAA applies.

## 15. Incident Record

Maintain the following fields:

| Field | Details to record |
|---|---|
| Incident ID | Unique reference |
| Discovery and report times | Include timezone |
| Reporter | Restricted operational record |
| Description | Facts, symptoms, and uncertainties |
| Affected assets | Accounts, devices, services, and information |
| Severity | Rating and justification |
| Clinical impact | Disruption and safety concerns |
| Timeline | Actions, decisions, owners, and times |
| Evidence | References to protected evidence |
| Communications | Internal updates and notification decisions |
| Recovery | Validation and approval |
| Closure | Remaining actions and acceptance |

## 16. Review and Improvement

Propose a review within five working days of stabilisation, or an agreed alternative for a complex incident.

Discuss:

- What happened and what remains uncertain.
- Whether reporting and escalation worked.
- The effectiveness of containment and recovery.
- Effects on patient care.
- Control and training improvements.

Assign each corrective action an owner, deadline, and verification requirement.

Update the risk register and relevant plans.

## 17. Exercises and Measures

Propose a tabletop exercise every six months and after major changes.

Use fictional scenarios without disrupting production systems.

Track:

- Time from discovery to reporting.
- Time from reporting to assessment and escalation.
- Time to appropriate containment.
- Time to verified recovery.
- Exercise issues and completed corrective actions.

No response performance has yet been measured.

## 18. References

- NIST SP 800-61 Rev. 3:
  https://csrc.nist.gov/pubs/sp/800/61/r3/final

- CISA — #StopRansomware Guide:
  https://www.cisa.gov/stopransomware/ransomware-guide

- Project documents:
  - `backup-and-recovery-plan.md`
  - `mfa-implementation-plan.md`
  - `../assessment/risk-register.md`

## 19. Project Status

Proposed plan for a fictional educational scenario.

No response team has been appointed, no exercise has been conducted, and no real incident has been investigated.
