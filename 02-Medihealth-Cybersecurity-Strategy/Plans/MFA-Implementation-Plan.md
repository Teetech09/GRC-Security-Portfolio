# MediHealth Clinic — MFA Implementation Plan

## 1. Purpose

Reduce the risk of account takeover by introducing multi-factor authentication (MFA) while maintaining reliable access to clinical systems.

The project brief states that MFA is not implemented across clinic systems. This plan proposes a staged rollout for the clinic’s 50 employees.

## 2. What MFA Means

MFA requires different types of evidence to authenticate a user, such as:

- Something you know: a password.
- Something you have: a registered security key or authenticator.
- Something you are: a biometric used to activate an authenticator.

Two passwords do not constitute MFA because they belong to the same factor category.

## 3. Systems and Priorities

| Priority | System or account | Reason | Verification needed |
|---|---|---|---|
| 1 | Privileged and administrative accounts | Compromise could permit widespread changes or access. | Inventory accounts and supported authentication methods. |
| 1 | Staff email | Email can expose information and support account recovery for other services. | Confirm the email platform and MFA features. |
| 1 | Remote access, if present | External access can provide an entry point into clinic systems. | Establish whether remote access exists and how it operates. |
| 2 | EHR access | Accounts can provide access to sensitive patient records. | Confirm vendor support, integration options, and clinical workflows. |
| 2 | Password manager, if adopted | The vault protects access credentials. | Confirm the selected product and plan capabilities. |
| 3 | Other sensitive applications | Protection depends on information, privileges, and exposure. | Identify applications and assess their risks. |

Remote access and a password manager are proposed assessment items, not confirmed existing systems.

## 4. Proposed Authentication Methods

### Preferred Method

Use FIDO2/WebAuthn authentication with user verification, such as a security key protected by a PIN or a supported passkey requiring device unlock.

Verify that the selected configuration provides the required authentication factors. Possession of a key alone should not automatically be described as MFA.

Prioritise this approach for administrators and other high-risk accounts.

### Interim Methods

Where the preferred method is unavailable:

- Use an authenticator app generating time-based codes.
- Alternatively, use push authentication with number matching where supported.
- Document the remaining phishing risk and a migration plan.

SMS or voice codes should require a documented exception when stronger supported methods are unavailable.

Do not use simple approve-or-deny push prompts as the preferred configuration.

## 5. Discovery and Preparation

Before rollout, IT must:

1. Identify systems, account owners, and authentication methods.
2. Replace shared staff accounts with individual accounts where feasible.
3. Check vendor documentation, licensing, and compatibility.
4. Identify legacy sign-in paths that could bypass MFA.
5. Assess shared workstations and device availability.
6. Agree recovery and emergency access procedures.
7. Record costs and obtain management approval.

No product, licence cost, or compatibility is assumed in this plan.

## 6. Pilot

Propose a pilot involving 5–8 employees representing IT, clinical, reception, and billing workflows.

The pilot should test:

- Enrolment and normal sign-in.
- Shared workstation use without sharing authenticators.
- Lost or unavailable authenticators.
- Recovery and replacement.
- Clinical access during busy periods.
- Authentication logs and failed attempts.
- Whether alternative sign-in routes bypass enforcement.

Use test accounts and synthetic data where possible.

## 7. Rollout Schedule

| Stage | Proposed timing | Activities |
|---|---|---|
| Discovery | Week 1 | Inventory systems, assess compatibility, and confirm responsibilities. |
| Preparation | Week 2 | Select methods, configure recovery, and prepare staff guidance. |
| Pilot | Week 3 | Test representative workflows and resolve issues. |
| Priority rollout | Week 4 | Protect administrators, email, and remote access where present. |
| Wider rollout | Weeks 5–6 | Extend coverage to supported EHR and other sensitive applications. |
| Review | After rollout | Verify enforcement, review exceptions, and assess support needs. |

These are planning estimates. Vendor dependencies, resources, and clinical requirements may change the schedule.

## 8. Staff Enrolment and Training

- Verify the employee’s identity before enrolment.
- Guide staff through an approved registration process.
- Explain normal authentication prompts and suspicious requests.
- Provide a clinic-issued alternative when staff cannot use personal devices.
- Explain how to report a lost device or key.
- Confirm that each employee can authenticate before enforcement begins.

Staff must never share authenticators, codes, or recovery information.

## 9. Recovery and Replacement

IT must establish an approved process for:

- Verifying the person requesting recovery.
- Registering a replacement authenticator.
- Revoking a lost or compromised authenticator.
- Protecting backup recovery information.
- Notifying the account owner of significant changes.
- Recording the action without exposing authentication secrets.

Use a second registered authenticator where supported and appropriate.

Do not disable MFA indefinitely as a routine response to a lost device.

## 10. Clinical Continuity and Emergency Access

Clinical management and IT must define emergency access before rollout.

The procedure must specify:

- When emergency access is permitted.
- Who can authorise and use it.
- How credentials or authenticators are secured.
- What activity is logged and alerted.
- When access expires or returns to normal.
- Who reviews each use.

Test the procedure with the EHR vendor and clinical representatives.

If systems remain unavailable, follow the clinic’s approved downtime procedures.

## 11. Legacy Systems

If the EHR cannot support MFA directly:

- Ask the vendor about supported upgrades or identity integration.
- Assess whether a protected access gateway can enforce MFA.
- Verify that users cannot bypass the gateway through direct access.
- Restrict exposure and privileges.
- Increase monitoring.
- Document residual risk and a replacement or upgrade plan.

Gateway MFA does not automatically protect every application sign-in path.

## 12. Challenges and Responses

| Challenge | Proposed response |
|---|---|
| Staff concern about extra steps | Demonstrate the process and explain its relevance to patient information. |
| Staff lack suitable devices | Provide supported clinic-issued keys or authenticators. |
| Lost device or key | Use the verified recovery and revocation process. |
| Older applications | Assess supported integration and document time-limited exceptions. |
| Internet or service outage | Test dependency failures and establish downtime procedures. |
| Clinical workflow disruption | Pilot with clinical staff and adjust the rollout before wider enforcement. |
| Limited budget | Prioritise high-risk accounts and prepare a costed phased proposal. |

## 13. Verification and Success Measures

Record:

- Accounts requiring MFA.
- Accounts with MFA enforced.
- Accounts protected by phishing-resistant authentication.
- Exceptions, owners, and expiry dates.
- Recovery test results.
- Support requests and workflow issues.

MFA coverage = accounts with MFA enforced ÷ accounts requiring MFA × 100.

Enrolment alone does not prove enforcement.

Before approving each rollout stage, confirm that:

- Protected sign-in requires the intended authentication.
- Relevant bypass routes are blocked or documented.
- Recovery works.
- Logging records authentication activity.
- Clinical representatives accept the workflow.

Do not publish user identifiers, secrets, QR codes, or recovery codes on GitHub.

## 14. Responsibilities

| Proposed role | Responsibility |
|---|---|
| Clinic management | Approve funding, priorities, and residual risks. |
| IT lead | Configure, test, monitor, and support authentication. |
| Clinical operations lead | Assess care workflows and emergency access. |
| Department managers | Coordinate staff enrolment and training. |
| Employees | Protect authenticators and report unexpected prompts or loss. |
| EHR vendor | Confirm supported integration and assist with testing. |

## 15. References

- CISA — Implementing Phishing-Resistant MFA:
  https://www.cisa.gov/sites/default/files/publications/fact-sheet-implementing-phishing-resistant-mfa-508c.pdf

- NIST SP 800-63B-4 — Authentication and Authenticator Management:
  https://pages.nist.gov/800-63-4/sp800-63b.html

## 16. Project Status

Proposed implementation plan for a fictional educational scenario.

No MFA configuration, enrolment, pilot, or effectiveness testing has been performed.
