
Deliverable 4: Physical Security Measures and Asset Protection Plan

 Ebeano Supermarket Cybersecurity Consulting Project

Category: Governance, Risk and Compliance (GRC) / Physical Security  
Business: Ebeano Supermarket — Simulated Case Study  
Workforce: 28 Employees  
Deliverable: 4 of 5  
Status: Proposed — Not Implemented



1. Executive Summary

Ebeano Supermarket relies on Point-of-Sale (POS) terminals, employee tablets, kitchen devices, inventory equipment, and network infrastructure to support daily business operations.

Although cybersecurity controls such as MFA, network segmentation, and access restrictions are essential, physical security weaknesses can undermine these protections.

For example, an unattended tablet may allow unauthorized access to a logged-in business application. Similarly, a criminal may substitute a legitimate POS terminal with an unauthorized device to divert customer payments.

This proposed Physical Security Plan recommends affordable, practical safeguards suitable for a growing supermarket with 28 employees.

The plan focuses on protecting equipment, controlling access to sensitive areas, preventing POS substitution, improving employee accountability, and supporting incident response.

2. Physical Security Objectives

The objectives are to:

1. Prevent unauthorized access to business devices.
2. Reduce the risk of POS terminal substitution and payment fraud.
3. Protect unattended tablets and workstations.
4. Restrict access to sensitive operational areas.
5. Establish asset ownership and accountability.
6. Improve visitor and contractor management.
7. Support incident detection through CCTV and supervision.
8. Reduce theft, tampering, and business disruption.
9. Integrate physical security with IAM and network security controls.

 3. Physical Security Risk Assessment

| Threat | Vulnerability | Potential Impact | Proposed Control |
|---|---|---|---|
| Unauthorized POS substitution | Unverified payment terminals | Payment diversion and financial loss | POS asset register and daily verification |
| Unattended staff tablets | Devices left unlocked | Unauthorized system access | Automatic locking and secure storage |
| Equipment theft | Poor device supervision | Financial loss and operational disruption | Asset tracking and controlled storage |
| Unauthorized visitors | Unrestricted staff-only areas | Theft or tampering | Visitor management and access restrictions |
| Network device tampering | Exposed routers and switches | Network compromise or service interruption | Locked network cabinet |
| Insider misuse | Inadequate accountability | Fraud or unauthorized changes | Individual accounts, supervision, and dual control |
| Tailgating | Uncontrolled staff entrances | Unauthorized physical access | Staff awareness and controlled entry |
| CCTV blind spots | Poor surveillance coverage | Delayed detection of incidents | Risk-based camera placement |

These are scenario-based risks, not findings from an actual site inspection.

 4. POS Terminal Security and Payment Fraud Prevention

 4.1 Approved POS Device Register

All POS terminals should be recorded in an approved asset register.

Each record should include:

- Asset identification number.
- Device manufacturer and model.
- Serial number.
- Authorized merchant identifier.
- Assigned supermarket outlet.
- Assigned cashier or custodian.
- Installation date.
- Device status.
- Last verification date.

4.2 POS Verification Before Transactions

At the beginning of each shift, authorized staff should:

1. Confirm the POS terminal matches the approved asset register.
2. Inspect the device for unusual attachments or signs of tampering.
3. Verify that the merchant identity matches the supermarket's approved payment account using the payment provider's supported verification method.
4. Confirm that the device is located at its assigned workstation.
5. Report any suspicious or unfamiliar terminal.

A suspicious terminal should not be used until verified by authorized personnel.

 4.3 Dual Control for POS Replacement

POS device replacement must involve at least two authorized employees.

Proposed process:

1. The IT Administrator or authorized technician requests or performs the replacement.
2. The Store Manager or Assistant Manager independently verifies the new device.
3. The device details and merchant information are checked.
4. The asset register is updated.
5. Both employees record their approval.

This control reduces the opportunity for unauthorized device substitution.

4.4 Secure POS Storage

Unused POS devices should be stored in a locked cabinet or designated secure area.

Access should be limited to authorized personnel.

5. Staff Tablet and Workstation Security

5.1 Automatic Screen Lock

Company-managed tablets and workstations should automatically lock after a short period of inactivity.

A proposed maximum inactivity period is five minutes, subject to operational requirements and device capabilities.

5.2 Secure Authentication

Employees should use individual accounts, strong passwords or PINs, and MFA where supported.

Shared credentials should be avoided.

5.3 Device Handling

Employees must:

- Never leave active business applications unattended.
- Lock devices when stepping away.
- Avoid sharing assigned devices without authorization.
- Report missing or damaged equipment.
- Avoid installing unapproved applications.
- Return devices to secure storage after use.

5.4 Mobile Device Management

Where affordable and supported, the supermarket should consider Mobile Device Management (MDM) to:

- Enforce screen-lock settings.
- Apply security updates.
- Restrict unapproved applications.
- Support remote locking or wiping of lost devices.
- Maintain a device inventory.

Remote wiping should be restricted to authorized personnel and used according to an approved procedure.

6. Physical Access Control

The supermarket should classify areas according to their sensitivity.

| Area | Access Level | Authorized Personnel |
|---|---|---|
| Customer Shopping Area | Public | Customers and employees |
| Checkout Area | Controlled | Cashiers and authorized supervisors |
| Kitchen and Food Preparation Area | Restricted | Kitchen staff and authorized supervisors |
| Inventory / Stockroom | Restricted | Inventory staff and authorized managers |
| Management Office | Restricted | Store Manager and authorized supervisors |
| Network Equipment Area | Highly Restricted | IT Administrator and approved maintenance personnel |
| POS Storage Area | Restricted | Authorized custodians and supervisors |

Recommended Controls

- Lock staff-only rooms when unattended.
- Restrict keys or access credentials to authorized employees.
- Maintain records of issued keys.
- Review access after staff departures.
- Require visitors to be escorted in restricted areas.
- Report lost keys or access cards promptly.

7. CCTV and Surveillance

CCTV can support incident investigation, theft deterrence, and the protection of critical business areas.

Recommended Camera Locations

- Main entrances and exits.
- Checkout areas.
- Stockroom entrances.
- POS storage areas.
- Corridors leading to sensitive rooms.
- Network equipment access points, where appropriate.

CCTV Security Requirements

1. Restrict footage access to authorized personnel.
2. Protect recordings from unauthorized deletion or alteration.
3. Use unique administrator credentials.
4. Keep recording equipment updated.
5. Maintain reliable date and time settings.
6. Establish a documented retention period consistent with applicable law.
7. Display appropriate surveillance notices.
8. Avoid camera placement in private areas.

CCTV should not be used to capture customer payment PIN entry or other unnecessarily sensitive information.

8. Visitor and Contractor Management

Visitors, vendors, and external technicians may require access to supermarket facilities.

The proposed visitor procedure includes:

1. Confirm the visitor's identity and purpose.
2. Record arrival and departure where appropriate.
3. Obtain approval before entering restricted areas.
4. Provide an employee escort when required.
5. Prohibit unauthorized handling of POS and network equipment.
6. Verify completed maintenance work.
7. Record any equipment replacement or configuration changes.

External technicians should not receive unrestricted physical or digital access.

9. Asset Inventory and Accountability

The supermarket should maintain a central asset register covering:

- POS terminals.
- Staff tablets.
- Kitchen terminals.
- Inventory devices.
- Routers and firewalls.
- Network switches.
- Wireless access points.
- CCTV equipment.
- Other business-critical devices.

Example Asset Register

| Asset ID | Device Type | Assigned Area | Custodian | Verification Status |
|---|---|---|---|---|
| EBS-POS-001 | POS Terminal | Checkout 1 | Assigned Cashier | Pending |
| EBS-POS-002 | POS Terminal | Checkout 2 | Assigned Cashier | Pending |
| EBS-TAB-001 | Staff Tablet | Sales Floor | Assigned Supervisor | Pending |
| EBS-KIT-001 | Kitchen Terminal | Kitchen | Kitchen Supervisor | Pending |
| EBS-NET-001 | Firewall / Router | Network Cabinet | IT Administrator | Pending |

The entries above are fictional examples, not verified business assets.

10. Job Rotation, Dual Control, and Mandatory Leave

Physical security should reinforce the internal controls established in the IAM Policy.

Dual Control

- Require two authorized individuals for POS device replacement.
- Independently verify high-risk inventory movements.
- Require approval before removing critical equipment from the premises.

Job Rotation

- Rotate suitable cashier and stock verification duties.
- Ensure temporary employees receive only necessary access.
- Review asset custody records when duties change.

Mandatory Leave

- Arrange trained replacements for employees handling sensitive responsibilities.
- Review outstanding financial and inventory records during handovers.
- Recover or temporarily reassign company equipment as appropriate.

These controls should support accountability without compromising business operations or applicable employment requirements.

11. Physical Security Incident Response

Employees must immediately report:

- Missing or substituted POS devices.
- Lost or stolen tablets.
- Unauthorized entry into restricted areas.
- Evidence of equipment tampering.
- Missing stock or unexplained inventory discrepancies.
- Suspicious visitor behavior.
- Damaged locks or security equipment.

 Proposed Response Procedure

1. Report the incident to the Store Manager or designated supervisor.
2. Stop using any suspicious payment terminal.
3. Secure the affected area or equipment without unnecessary disturbance.
4. Notify IT if business systems or credentials may be affected.
5. Preserve relevant CCTV footage, device records, and incident details.
6. Contact the payment provider or appropriate authorities when required.
7. Investigate and document findings.
8. Implement corrective actions.

12. Physical Security Inspection Checklist

| Inspection Item | Proposed Frequency | Responsible Role |
|---|---|---|
| Verify approved POS terminals | Each shift | Cashier / Supervisor |
| Check tablet locking and storage | Daily | Assigned Custodian |
| Inspect restricted-area doors | Daily | Supervisor |
| Review CCTV operation | Weekly | Authorized Manager |
| Reconcile POS asset register | Weekly | Manager / IT Administrator |
| Inspect network cabinet security | Monthly | IT Administrator |
| Review issued keys and access credentials | Monthly | Manager |
| Review asset inventory | Quarterly | Manager / IT Administrator |
| Review physical security procedures | Annually | Store Manager |

13. Budget-Conscious Implementation Plan

| Priority | Recommended Measure | Cost Consideration |
|---|---|---|
| Critical | POS asset identification and verification | Low-cost administrative control |
| Critical | Automatic screen locks | Usually available in device settings |
| High | Secure storage for unused POS devices | Low to moderate |
| High | Lock network equipment cabinets | Low to moderate |
| High | Visitor and contractor procedures | Low-cost administrative control |
| High | Staff awareness and reporting | Low-cost training |
| Medium | Improved CCTV coverage | Depends on existing equipment |
| Medium | Mobile Device Management | Depends on vendor and licensing |
| Medium | Electronic access control | Higher cost; consider as business grows |

The supermarket should prioritize low-cost controls that address the highest risks before investing in more expensive technology.

14. Expected Business Benefits

If implemented effectively, these measures could:

- Reduce POS substitution and payment diversion risks.
- Improve protection of staff tablets.
- Reduce equipment theft and unauthorized access.
- Strengthen employee accountability.
- Improve incident detection and investigation.
- Support business continuity.
- Complement IAM and network security controls.

15. Implementation Status and Disclaimer

Status: Proposed — Not Implemented

This document was prepared as part of an educational cybersecurity consulting portfolio project.

The asset examples, risk assessment, inspection procedures, and physical security recommendations are based on a simulated 28-employee supermarket scenario.

No physical site assessment, CCTV inspection, POS verification, or live implementation has been conducted.



Project: Ebeano Supermarket Cybersecurity Consulting  
Category: GRC / Physical Security and Asset Protection  
Deliverable: 4 of 5
