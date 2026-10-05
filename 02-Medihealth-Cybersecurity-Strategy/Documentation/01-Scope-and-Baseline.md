
# MediHealth Clinic — Assessment Scope and Security Baseline

## 1. Purpose

This document defines the scope of the cybersecurity assessment and records MediHealth Clinic’s security posture as described in the project brief.

The baseline will guide the identification of risks and the development of practical recommendations to protect patient information and maintain clinical services.

## 2. Organisation Profile

| Item | Description |
|---|---|
| Organisation | MediHealth Clinic |
| Industry | Healthcare |
| Location | Suburban area in Nigeria |
| Size | 50 employees |
| Services | Primary healthcare |
| Key system | Electronic health record (EHR) system |
| Sensitive information | Patient identification details, medical histories, and insurance information |

MediHealth Clinic depends on its EHR system to manage patient information. A recent server hardware failure prevented access to the system, demonstrating the importance of service availability and recovery planning.

The brief also describes repeated phishing attempts. It does not provide enough information to establish whether those attempts resulted in a confirmed compromise.

## 3. Assessment Objectives

The assessment aims to:

- Identify weaknesses affecting patient information and clinical systems.
- Evaluate potential impacts on confidentiality, integrity, availability, and patient safety.
- Prioritise risks using a documented scoring method.
- Recommend controls suitable for a clinic with 50 employees.
- Develop awareness materials, policies, and implementation plans.
- Identify information that would require verification during a real assessment.

## 4. Assessment Scope

### Included

- EHR system security and availability.
- Staff accounts, passwords, and shared credentials.
- Multi-factor authentication.
- Staff laptops and portable devices.
- Protection of EHR communications.
- Storage and access control arrangements.
- Phishing awareness and reporting.
- Physical access controls and staff identification.
- Backup and recovery planning.
- Incident response planning.

### Excluded

- Live vulnerability scanning or penetration testing.
- Access to real patient records.
- Deployment or configuration changes.
- Actual phishing simulations.
- Detailed assessment of medical devices not described in the brief.
- Formal regulatory compliance certification.

These exclusions reflect the educational nature of the project.

## 5. Baseline Security Observations

The observations below come from the supplied scenario. They have not been independently verified.

| ID | Area | Observation from the brief | Potential security concern |
|---|---|---|---|
| B01 | EHR availability | Server hardware failure prevented access to the EHR system. | Disruption could delay access to information needed for patient care. |
| B02 | Password security | Weak passwords are common, and no complexity or rotation policies are enforced. | Easily guessed or compromised passwords could enable account takeover. Password requirements will be evaluated against current guidance. |
| B03 | Authentication | MFA is not implemented across clinic systems. | A stolen password could be sufficient to access an account. |
| B04 | User accountability | Medical personnel share login details. | Shared credentials reduce accountability and make individual access revocation difficult. |
| B05 | Software maintenance | The EHR system and software on laptops and portable devices are outdated. | Unpatched or unsupported software could expose systems to exploitation. |
| B06 | Communication security | EHR communications lack encryption. | Patient information could be exposed or altered if communications are intercepted. |
| B07 | Storage and access control | The brief describes no centralised storage system with access control policies. | Storage arrangements and access permissions require assessment to determine how patient information is protected. |
| B08 | Phishing awareness | Employees have received basic training, but there is no recurring awareness programme. | Employees may fail to recognise or report convincing phishing messages. |
| B09 | Physical security | The brief describes no staff identification cards and no physical security at the premises. | Unauthorised people could potentially access sensitive areas or equipment. |
| B10 | Backup and recovery governance | No backup and recovery policy is documented. | Recovery responsibilities, procedures, and testing may be undefined. The existence of backups is unknown. |
| B11 | Incident response governance | No incident response plan is documented. | Staff may respond inconsistently or delay escalation during an incident. |

## 6. Security and Patient Care Priorities

### Confidentiality

Patient information should be accessible only to authorised people with a legitimate need to use it.

### Integrity

Patient records should remain accurate and protected against unauthorised changes. Incorrect information could affect clinical decisions.

### Availability

Authorised staff should be able to access essential systems and records when needed, including during disruptions.

### Patient Safety

Risk assessment will consider how loss of access, incorrect records, or disrupted services could affect care. The scenario does not establish that any patient has already suffered harm.

## 7. Assumptions and Unknowns

| Item | Status | How it would be verified in a real assessment |
|---|---|---|
| EHR hosting arrangement | Unknown; server hardware is mentioned, but the architecture is not specified. | Review architecture documents and interview the system administrator. |
| Existing backups | Unknown; absence of a policy does not prove backups are absent. | Inspect backup configurations, logs, and restoration test records. |
| MFA compatibility | Unknown for individual systems. | Review vendor documentation and test supported authentication methods. |
| Current access permissions | Unknown. | Review user accounts, roles, and permission assignments. |
| Software versions and support status | Unknown; software is described as outdated. | Review the asset inventory and vendor support information. |
| Existing endpoint and network controls | Not specified. | Review security configurations, subscriptions, and monitoring records. |
| Available security budget | Not specified. | Discuss priorities and resources with management. |
| Regulatory obligations | Require verification. | Review applicable Nigerian requirements and any contractual or international obligations. |

Proposed controls and risk ratings will be labelled as recommendations or scenario-based estimates.

## 8. Assessment Method

The project will use the following process:

1. Identify assets and the information they process.
2. Connect observed vulnerabilities to plausible threats or disruptive events.
3. Describe the potential business, security, and patient care impacts.
4. Score likelihood and impact using a defined 1–5 scale.
5. Calculate risk scores and prioritise treatment.
6. Recommend controls, proposed owners, and implementation timeframes.
7. Document limitations and matters requiring further evidence.

Risk scoring definitions will be documented in the risk register before risks are rated.

## 9. Planned Outputs

- Asset and threat assessment.
- Risk register.
- Phishing awareness campaign and proposed simulation plan.
- Password security policy.
- MFA implementation plan.
- Backup and recovery plan.
- Incident response plan.
- Final cybersecurity strategy report.
- Presentation and lessons learned.

## 10. Assessment Limitations

This assessment is based entirely on a fictional project brief.

No interviews, system inspections, technical tests, or recovery exercises have been performed. Therefore, this document establishes a scenario baseline rather than verified audit findings.

Recommendations will require validation against the clinic’s actual systems, resources, and obligations before implementation.

## 11. Source

Mama CyberShield Cohort 2.0 Project Work — Project Topic 1:
Developing a Comprehensive Cybersecurity Strategy for a Health Sector.
