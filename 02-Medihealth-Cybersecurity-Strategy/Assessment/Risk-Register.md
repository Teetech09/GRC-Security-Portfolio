# MediHealth Clinic — Risk Register

## 1. Purpose

This register prioritises the risks identified in the asset and threat assessment.

Ratings are scenario-based estimates, not verified audit findings. They should be reviewed after interviews, system inspections, and technical checks.

## 2. Scoring Method

Risk score = Likelihood × Impact.

### Likelihood

| Score | Rating | Meaning |
|---|---|---|
| 1 | Rare | Requires exceptional circumstances; strong preventive controls are verified. |
| 2 | Unlikely | Possible, but exposure is limited and relevant controls are effective. |
| 3 | Possible | A credible scenario; exposure or control effectiveness is uncertain. |
| 4 | Likely | Significant weaknesses or repeated threat activity make occurrence plausible. |
| 5 | Almost certain | Strong evidence indicates the event is recurring or imminent. |

### Impact

Use the highest credible impact across patient safety, confidentiality, integrity, availability, and clinic operations.

| Score | Rating | Meaning |
|---|---|---|
| 1 | Negligible | Minimal disruption with no meaningful effect on sensitive information or care. |
| 2 | Minor | Limited disruption or exposure that can be managed through routine procedures. |
| 3 | Moderate | Meaningful disruption, limited sensitive data exposure, or delays requiring workarounds. |
| 4 | Major | Substantial sensitive data exposure or alteration, or serious service disruption. |
| 5 | Severe | Prolonged loss of essential services, extensive data compromise, or potential serious patient harm. |

### Priority Bands

| Score | Priority |
|---|---|
| 1–4 | Low |
| 5–9 | Moderate |
| 10–16 | High |
| 17–25 | Critical |

These bands are project conventions. Equal scores require further judgement about urgency, patient care, dependencies, and implementation effort.

## 3. Risk Summary

| ID | Related threat | Risk | Likelihood | Impact | Score | Priority |
|---|---|---|---|---|---|---|
| R01 | T01 | Phishing leads to account compromise and unauthorised access to patient information. | 4 | 4 | 16 | High |
| R02 | T02 | Weak or shared credentials enable unauthorised activity and reduce accountability. | 4 | 4 | 16 | High |
| R03 | T03 | Outdated software is exploited, causing data compromise or major service disruption. | 4 | 5 | 20 | Critical |
| R04 | T04 | Unencrypted EHR communications expose information to interception or possible alteration. | 3 | 4 | 12 | High |
| R05 | T05 | EHR server failure causes an extended outage because recovery arrangements are ineffective or unclear. | 3 | 5 | 15 | High |
| R06 | T06 | Unauthorised physical access leads to information exposure, equipment theft, or disruption. | 3 | 4 | 12 | High |

No risk is treated as already mitigated. Control effectiveness has not been verified.

## 4. Rating Justifications

### R01 — Phishing and Account Compromise

**Likelihood: 4.** The brief describes repeated phishing attempts, limited recurring training, and no MFA.

**Impact: 4.** Compromise of an account with access to patient records could expose sensitive information or permit unauthorised changes.

**Uncertainty:** Actual account privileges and the effectiveness of email filtering are unknown.

### R02 — Weak and Shared Credentials

**Likelihood: 4.** Weak passwords and credential sharing are explicitly described, creating opportunities for misuse.

**Impact: 4.** Unauthorised access could compromise patient records. Shared credentials also weaken accountability.

**Uncertainty:** The number of affected accounts, access permissions, and logging capabilities are unknown.

### R03 — Exploitation of Outdated Software

**Likelihood: 4.** Outdated software is reported across the EHR and staff devices. This is a conservative initial rating pending verification of versions and exposure.

**Impact: 5.** A widespread compromise or ransomware incident could prevent access to essential clinical information and seriously disrupt care.

**Uncertainty:** Specific vulnerabilities, network exposure, endpoint controls, and recovery capability are unknown. Reduce or increase the rating when evidence becomes available.

### R04 — Interception of EHR Communications

**Likelihood: 3.** Unencrypted communications create a credible risk, but exploitation depends on an attacker accessing a relevant network path.

**Impact: 4.** Interception could expose sensitive patient information; alteration may also be possible depending on the protocol.

**Uncertainty:** The protocols, transmitted data, and network protections are unknown.

### R05 — EHR Outage and Recovery Failure

**Likelihood: 3.** A hardware failure has already occurred, but its cause and the likelihood of recurrence are unknown. Recovery arrangements require verification.

**Impact: 5.** An extended outage could seriously disrupt access to information needed for care. This is a potential consequence, not evidence of actual patient harm.

**Uncertainty:** Backup capability, outage duration, hardware condition, and clinical workarounds are unknown.

### R06 — Unauthorised Physical Access

**Likelihood: 3.** Weak physical security makes unauthorised access plausible, but actual access opportunities have not been assessed.

**Impact: 4.** Access to sensitive equipment or records could cause data exposure, tampering, theft, or service disruption.

**Uncertainty:** The premises layout, device protections, and existing entry arrangements are unknown.

## 5. Proposed Risk Treatment

All owners and timeframes below are proposals requiring management agreement. Timeframes begin when the project recommendations are approved.

| Risk | Proposed actions | Proposed owner | Target timeframe | Status |
|---|---|---|---|---|
| R01 | Establish phishing reporting; deliver initial awareness training; pilot MFA on email and privileged accounts. | IT lead and designated training coordinator | Start within 7 days; initial rollout within 30 days | Proposed |
| R02 | Identify shared accounts; introduce individual accounts; review privileges; implement the password policy. | IT lead and department managers | Start within 7 days; initial remediation within 30 days | Proposed |
| R03 | Verify software versions and exposure; prioritise exploitable weaknesses; test and deploy updates; plan replacement of unsupported systems. | IT lead and EHR vendor | Triage within 7 days; remediation plan within 30 days | Proposed |
| R04 | Identify insecure EHR connections; confirm vendor support; enable and test transport encryption. | IT lead and EHR vendor | Assess within 14 days; implementation target within 30 days where feasible | Proposed |
| R05 | Verify backups immediately; perform a controlled restoration test; document outage procedures and recovery targets. | IT lead and clinical operations lead | Verification within 7 days; initial recovery plan within 30 days | Proposed |
| R06 | Restrict sensitive areas; establish visitor procedures and staff identification; review device locking and equipment security. | Clinic administrator and facilities lead | Initial measures within 14 days; broader improvements within 60 days | Proposed |

Implementation must account for clinical continuity. Changes to critical systems should be tested and scheduled with clinical staff.

## 6. Immediate Verification Priorities

Before relying on the scores or finalising treatment:

1. Confirm that usable backups exist and test restoration safely.
2. Identify EHR and device software versions, support status, and exposure.
3. Review shared accounts, privileged access, and MFA compatibility.
4. Confirm which EHR connections lack encryption.
5. Review physical access to servers, devices, and patient information.

These checks may change the ratings and implementation order.

## 7. Residual Risk and Review

Residual risk is the risk remaining after controls have been implemented.

Residual scores are not assigned yet because the proposed controls have not been deployed or tested.

For each completed action, record:

- Implementation evidence.
- Verification results.
- Updated likelihood and impact.
- Remaining weaknesses.
- Management approval of any accepted risk.

Review this register after significant changes, incidents, or new evidence, and periodically according to an agreed schedule.

## 8. Assessment Limitations

This register is based on a fictional project scenario. It does not establish that an attack occurred, that a specific software vulnerability exists, or that backups are absent.

Risk scores support prioritisation; they do not represent measured probabilities.
