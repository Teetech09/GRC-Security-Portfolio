
# MediHealth Clinic — Backup and Recovery Plan

## 1. Document Control

| Item | Details |
|---|---|
| Plan ID | MHC-PLAN-002 |
| Version | 1.0 |
| Status | Proposed — educational portfolio |
| Author | Titilayo Yusuf |
| Proposed owner | IT lead |
| Approval authority | Clinic management |
| Review | Annually and after major changes or incidents |

## 2. Purpose

Protect essential clinic information and restore clinical systems following hardware failure, accidental deletion, malicious activity, or another disruption.

The plan addresses the EHR outage described in the project brief.

## 3. Current Position

The scenario confirms:

- A server hardware failure prevented access to the EHR.
- No backup and recovery policy is documented.

The following remain unknown:

- Whether backups exist.
- Their frequency, coverage, and protection.
- Whether restoration has been tested.
- The previous outage’s duration.
- Available replacement equipment and vendor support.

Absence of a policy does not prove absence of backups.

## 4. Initial Verification

IT should:

1. Identify existing backup jobs and storage locations.
2. Review recent success and failure logs.
3. Confirm what information and system components are included.
4. Identify who can access, change, or delete backups.
5. Verify access to encryption keys and recovery credentials.
6. Perform a controlled restoration test.
7. Record gaps and agree corrective actions with management.

A successful backup job alone does not demonstrate successful recovery.

## 5. Backup Scope

| Item | Proposed coverage | Verification required |
|---|---|---|
| EHR database | Patient records and related database components | Vendor-supported backup and restoration method |
| EHR attachments | Documents or images stored outside the database | Locations and links to patient records |
| Application configuration | Settings needed to restore operation | Vendor requirements and dependencies |
| Server recovery resources | Required configuration, installation resources, and licensing information | Available rebuild or recovery method |
| Essential clinic documents | Operational documents needed during recovery | Approved storage locations and owners |
| Recovery documentation | Procedures, contacts, and dependency information | Accessible protected copies during an outage |

Inventory additional dependencies before approving the scope.

## 6. Recovery Objectives

### Recovery Time Objective (RTO)

The target time for restoring a system after disruption.

### Recovery Point Objective (RPO)

The maximum acceptable data loss measured in time.

For example, a four-hour RPO means the recovery design aims to lose no more than four hours of changes.

### Proposed Starting Targets

| Service | Proposed RTO | Proposed RPO |
|---|---|---|
| EHR service, including essential records and attachments | 4 hours | 1 hour |
| Essential administrative documents | 1 working day | 24 hours |

These are discussion targets, not verified capabilities or clinical safety thresholds.

Clinical management must complete a business impact assessment and approve targets based on patient care, cost, dependencies, and tested recovery capability.

The total tolerable disruption must also account for clinical validation and reconciliation after technical restoration.

## 7. Proposed Backup Schedule

| Item | Proposed schedule |
|---|---|
| EHR database | Vendor-supported incremental or transaction-log protection at least hourly |
| EHR database full backup | Daily, or an equivalent vendor-supported recovery chain |
| EHR attachments | At least hourly where needed to meet the agreed EHR RPO |
| Essential administrative documents | Daily |
| Configuration | After approved changes and through a regular scheduled backup |

Confirm that the schedule is technically feasible and does not disrupt clinical services.

Database and attachment backups must support a consistent recovery point. A simple file copy of a running database may not provide a usable backup.

## 8. Backup Protection

Proposed controls:

- Maintain multiple recoverable copies.
- Keep a protected copy away from the primary server’s location.
- Maintain an offline or appropriately isolated immutable copy.
- Encrypt backups during transfer and storage.
- Restrict administration to authorised personnel.
- Use separate backup administration credentials and MFA where supported.
- Monitor failures and unusual deletion activity.
- Protect encryption keys and test their availability during recovery.

Synchronisation alone is insufficient because deletion or corruption may propagate.

## 9. Retention and Disposal

Before deployment, agree retention periods based on:

- Recovery needs.
- Storage capacity.
- Applicable obligations.
- Vendor capabilities.
- The possibility of discovering an incident after a delay.

As an initial planning assumption, assess retaining daily recovery points for 30 days and weekly recovery points for 12 weeks.

These periods are not statutory requirements and require approval.

Backup retention is separate from the clinic’s patient record retention policy. Securely dispose of expired backups unless an investigation or preservation requirement applies.

## 10. Monitoring and Responsibilities

| Proposed role | Responsibility |
|---|---|
| IT lead | Configure backups, review jobs, test restoration, and maintain procedures |
| Clinical operations lead | Define care priorities and validate restored clinical workflows |
| Clinic management | Approve resources, recovery targets, and residual risks |
| EHR vendor | Confirm supported procedures and assist with application recovery |
| Designated privacy lead | Review protection, retention, and handling of sensitive information |

Assign a deputy for each essential recovery responsibility.

Review backup job results daily and escalate failures that threaten the agreed RPO.

## 11. Recovery Procedure

### Step 1 — Assess the Disruption

Record the affected systems, discovery time, symptoms, and effects on care.

Determine whether the event appears to be hardware failure, accidental loss, or a possible security incident.

### Step 2 — Activate the Appropriate Plans

Notify IT, clinical leadership, and management.

Activate approved clinical downtime procedures. If malicious activity is suspected, coordinate with the incident response plan before restoring systems.

### Step 3 — Prepare a Safe Recovery Environment

Repair or replace failed equipment.

For suspected compromise, investigate and address the cause before returning systems to operation.

Preserve relevant evidence and avoid restoring into an environment that remains compromised.

### Step 4 — Select the Recovery Point

Identify a usable backup and verify its consistency, integrity, and suitability.

Document expected data loss and seek the required authorisation.

### Step 5 — Restore Dependencies and Data

Follow the vendor-approved sequence for infrastructure, application components, database, attachments, and configuration.

Protect credentials used during recovery.

### Step 6 — Validate

IT verifies technical operation.

Authorised clinical representatives check record accessibility, application functions, and a controlled sample of record relationships and completeness.

Use approved handling procedures for any real patient information.

### Step 7 — Reconcile Downtime Records

Identify information created or changed during the outage.

Reconcile it through an approved clinical process, preserving timestamps and accountability and avoiding duplicate entries.

### Step 8 — Return to Service

Obtain the agreed technical and clinical approval.

Notify staff, monitor stability, and confirm that backups resume successfully.

## 12. Clinical Downtime Arrangements

Clinical leadership must define safe procedures for working without the EHR.

The procedures should address:

- Patient identification.
- Access to essential information through approved alternatives.
- Secure temporary documentation.
- Escalation when safe care cannot continue.
- Reconciliation after restoration.
- Secure storage and disposal of temporary records according to approved requirements.

Staff must not improvise by placing patient information in personal email, messaging applications, or unapproved storage.

## 13. Restoration Testing

| Test | Proposed frequency |
|---|---|
| Controlled restoration of selected information | Monthly |
| EHR recovery in an isolated environment | Quarterly |
| Downtime and recovery tabletop exercise | Every six months |
| Additional test | After significant system or backup changes |

Record:

- Backup and recovery point used.
- Test environment and participants.
- Start and completion times.
- Restoration and validation results.
- Whether RTO and RPO targets were met.
- Failures, owners, and corrective actions.

A test must not overwrite production information.

## 14. Measures of Effectiveness

Track:

- Backup job success and failure.
- Age of the latest verified usable recovery point.
- Coverage of essential assets.
- Restoration test success.
- Time taken to restore and validate services.
- Unresolved failures and corrective actions.

Do not claim success rates or recovery performance until evidence exists.

## 15. Implementation Evidence

Planned evidence includes:

- Backup inventory.
- Approved configuration and access records.
- Monitoring summaries.
- Restoration test reports.
- Approved recovery targets.
- Clinical downtime exercise records.

Public GitHub evidence must exclude patient information, credentials, encryption keys, and sensitive infrastructure details.

## 16. References

- CISA — #StopRansomware Guide:
  https://www.cisa.gov/stopransomware/ransomware-guide

- NIST SP 800-34 Rev. 1 — Contingency Planning Guide:
  https://csrc.nist.gov/pubs/sp/800/34/r1/upd1/final

NIST guidance informs the planning approach; it is not presented as a Nigerian legal requirement.

## 17. Project Status

Proposed plan for a fictional educational scenario.

No backups have been configured or inspected, no restoration test has been performed, and no recovery targets have been approved.
