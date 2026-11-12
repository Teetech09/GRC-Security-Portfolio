NIST CSF 2.0 and ISO/IEC 27001:2022 Control Mapping

1. Overview

This document maps the eight cybersecurity risks identified in the simulated assessment of **NorthBridge Financial Services Ltd.** to relevant cybersecurity framework outcomes and security controls.

The mapping uses:

- NIST Cybersecurity Framework (CSF) 2.0.
- ISO/IEC 27001:2022 Annex A.

The purpose is to demonstrate how identified organisational risks relate to recognised cybersecurity practices and control requirements.

2. Framework Mapping

| Risk ID | Identified Risk | NIST CSF 2.0 Reference | ISO/IEC 27001:2022 Annex A Reference |
|---|---|---|---|
| R001 | Former employees retain active system accounts | PR.AA-01, PR.AA-05 | A.5.18, A.6.5 |
| R002 | Employees fall victim to phishing attacks | PR.AT-01 | A.6.3 |
| R003 | Sensitive customer data exposed through AWS S3 misconfiguration | PR.DS-01, PR.AA-05 | A.5.15, A.5.23, A.8.3 |
| R004 | Ransomware disrupts banking operations | PR.PS-05, RS.MA-01 | A.8.7, A.5.24 |
| R005 | Security incidents go undetected due to inadequate monitoring | DE.CM-01, DE.AE-02 | A.8.15, A.8.16 |
| R006 | Third-party payment processor exposes customer information | GV.SC | A.5.19, A.5.20, A.5.22 |
| R007 | Backups are unavailable or unusable during recovery | PR.DS-11, RC.RP-01 | A.8.13, A.5.30 |
| R008 | Unpatched vulnerabilities allow attackers to compromise systems | ID.RA-01 | A.8.8 |

3. Mapping Rationale

R001 – Identity and Access Management

- NIST PR.AA-01: Addresses the management of user identities and credentials.
- NIST PR.AA-05: Addresses access permissions, reviews and removal of unnecessary privileges.
- ISO A.5.18:Access rights.
- ISO A.6.5: Responsibilities after termination or change of employment.

These references support effective account lifecycle management and timely removal of access when employees leave.

R002 – Phishing and Security Awareness

- NIST PR.AT-01: General cybersecurity awareness and training for personnel.
- ISO A.6.3: Information security awareness, education and training.

These controls support employee awareness of phishing, social engineering, and safe security practices.

R003 – AWS S3 Data Exposure

- NIST PR.DS-01: Protection of data at rest.
- NIST PR.AA-05: Management and review of access permissions.
- ISO A.5.15:Access control.
- ISO A.5.23: Information security for use of cloud services.
- ISO A.8.3:Information access restriction.

These references support the protection of stored customer information and the restriction of unauthorised access to cloud resources.

R004 – Ransomware

- NIST PR.PS-05: Protection against unauthorised software installation and execution.
- NIST RS.MA-01: Execution of the incident management plan.
- ISO A.8.7:Protection against malware.
- ISO A.5.24: Information security incident management planning and preparation.

These references support malware prevention and organisational readiness to respond to ransomware incidents.

R005 – Security Monitoring and Logging

- NIST DE.CM-01: Monitoring of networks and network services.
- NIST DE.AE-02 Analysis of potentially adverse events to understand associated activities.

- ISO A.8.15:Logging.
- ISO A.8.16: Monitoring activities.

These controls support security event visibility, detection and investigation.

R006 – Third-Party and Vendor Security

- NIST GV.SC: Cybersecurity supply chain risk management.
- ISO A.5.19: Information security in supplier relationships.
- ISO A.5.20: Addressing information security within supplier agreements.
- ISO A.5.22 Monitoring, review and change management of supplier services.

These references support vendor due diligence, contractual security requirements and ongoing supplier monitoring.

R007 – Backup and Disaster Recovery

- NIST PR.DS-11: Creation, protection, maintenance and testing of backups.
- NIST RC.RP-01: Execution of the recovery plan.

- ISO A.8.13: Information backup.
- ISO A.5.30: ICT readiness for business continuity.

These references support backup protection, restoration testing and recovery preparedness.

R008 – Vulnerability and Patch Management

- NIST ID.RA-01: Identification, validation and recording of vulnerabilities in assets.
- ISO A.8.8: Management of technical vulnerabilities.

These references support vulnerability identification, prioritisation, remediation and tracking.

4. Mapping Limitations

The mappings are indicative and intended for portfolio demonstration.

A framework reference does not automatically mean that an organisation has implemented or complied with the corresponding control.

Actual applicability should be determined through organisational scope, risk assessment, control selection, implementation evidence and, where relevant, the ISO/IEC 27001 Statement of Applicability (SoA).

The mapping should also be reviewed against the official framework and standard before being used in a real audit or compliance assessment.

5. Disclaimer

NorthBridge Financial Services Ltd. is a fictional organisation. All risks and mappings in this document are simulated for educational and professional portfolio purposes.

This document does not represent an actual certification, compliance assessment or independent audit.
