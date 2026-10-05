# MediHealth Clinic — Password Security Policy

## 1. Document Control

| Item | Details |
|---|---|
| Policy ID | MHC-POL-001 |
| Version | 1.0 |
| Status | Proposed — educational portfolio |
| Author | Titilayo Yusuf |
| Proposed owner | IT lead |
| Approval authority | Clinic management |
| Effective date | To be assigned after approval |
| Review | Annually and after significant incidents or changes |

## 2. Purpose

Protect patient information and clinic systems by establishing requirements for creating, using, storing, and recovering passwords.

This policy addresses the weak passwords and shared login details described in the MediHealth Clinic scenario.

## 3. Scope

This policy applies to employees, contractors, and other authorised users of clinic systems.

It covers EHR accounts, email, workstations, remote access, administrative accounts, and other password-protected clinic services.

Device unlock PINs and machine credentials require separate technical standards.

## 4. Individual Accounts

- Each employee must use an individually assigned account.
- Employees must not share passwords or use another person’s account.
- Managers must request access appropriate to each employee’s duties.
- IT must remove or adjust access when employment or responsibilities change.
- Administrators must use separate accounts for administrative work.

Where a system requires a shared technical account, management must approve a documented exception with restricted access and activity monitoring.

## 5. Password Requirements

- User account passwords must contain at least 15 characters.
- Systems should support passwords of at least 64 characters.
- Staff may use long passphrases or password manager-generated passwords.
- Systems must reject common, expected, and known compromised passwords where supported.
- Do not impose mandatory mixtures of uppercase letters, numbers, and symbols.
- Use a different password for each account.
- Do not use patient information, personal details, or predictable clinic-related phrases.

The 15-character minimum is the clinic’s proposed standard, including accounts protected by MFA.

## 6. Password Changes and Expiration

Do not require routine password changes solely because a fixed period has elapsed.

Require a change when compromise is suspected or confirmed, including disclosure through phishing.

Replace default credentials before operational use. Temporary credentials must expire and require replacement at first use where supported.

### Alignment With the Project Brief

The brief requests regular password rotation. This policy instead adopts event-driven changes in line with current NIST guidance.

Any verified legal, contractual, or technical requirement for scheduled changes must be documented and reviewed.

## 7. Password Manager

Proposed product for evaluation: **Bitwarden Business Password Manager**.

Before adoption, IT and management must assess:

- Device and application compatibility.
- Administration, recovery, and offboarding capabilities.
- Subscription features and total cost.
- Vendor security and data handling arrangements.
- Staff training and clinical workflow requirements.

Required operating practices:

- Use an approved organisational account.
- Protect the vault with a unique master passphrase and MFA.
- Enable automatic vault locking.
- Restrict access to stored credentials according to responsibilities.
- Protect recovery information through an approved process.
- Install software only from verified official sources.
- Do not store patient records in the password vault.

The password manager must not become a way to share individual EHR credentials.

## 8. Password Handling

Employees must not:

- Send passwords through email, chat, or ordinary support tickets.
- Leave passwords visible on desks or equipment.
- Save passwords in unprotected documents.
- Enter credentials through unexpected email links.
- provide passwords or verification codes to someone claiming to be IT.

IT must never ask employees to disclose their existing passwords.

## 9. Multi-Factor Authentication

Deploy MFA according to the clinic’s MFA implementation plan.

Prioritise privileged accounts, email, remote access, and EHR access where supported.

Employees must reject and report unexpected authentication prompts.

IT must establish recovery arrangements that support clinical continuity without informal credential sharing.

## 10. Account Recovery and Suspected Compromise

- Verify identity through an approved process before resetting access.
- Do not rely solely on an unexpected email or telephone request.
- Record resets without recording passwords.
- Deliver temporary access through an approved secure method.
- After suspected compromise, assess active sessions, account activity, and recovery settings.
- Escalate suspected misuse through the incident response process.

Clinical urgency must be handled through approved emergency access procedures.

## 11. Technical Enforcement

IT must assess whether each system supports the policy and document gaps.

Proposed technical controls include:

- Secure transport for authentication.
- Appropriate salted password hashing.
- Rate limiting against repeated guessing.
- Support for password managers and paste functionality.
- Logging of authentication and administrative activity.

For vendor-managed systems, obtain evidence of supported controls rather than assuming they exist.

## 12. Legacy System Exceptions

An exception must record:

- The affected system and limitation.
- The associated risk.
- Compensating controls.
- The responsible owner.
- Management approval.
- An expiry date and remediation plan.

Possible controls include restricted network access, MFA through a supported access gateway, closer monitoring, and replacement planning.

IT must test changes to critical clinical systems before rollout.

## 13. Responsibilities

### Employees

Follow the policy, protect credentials, and report suspected exposure promptly.

### IT Lead

Configure controls, support recovery, maintain exceptions, and verify implementation.

### Department Managers

Confirm access needs and support staff training.

### Clinic Management

Approve the policy, allocate resources, and decide whether to accept documented residual risks.

## 14. Verification and Review

Evidence of implementation should include:

- Password configuration records.
- Individual account and access reviews.
- MFA enrolment records.
- Password manager configuration.
- Approved exceptions.
- Training records.

Do not collect actual employee passwords as assessment evidence.

Address violations through investigation, support, and applicable clinic procedures.

## 15. Regulatory Applicability

This policy supports the protection of sensitive healthcare information.

Applicable Nigerian obligations and contractual requirements require separate verification. This document does not claim HIPAA compliance or regulatory certification.

## 16. References

- NIST SP 800-63B-4, Authentication and Authenticator Management:
  https://pages.nist.gov/800-63-4/sp800-63b/authenticators/

- Bitwarden Business Password Manager:
  https://bitwarden.com/products/business/

- Bitwarden Two-Step Login Methods:
  https://bitwarden.com/help/setup-two-step-login/

## 17. Implementation Status

Policy drafted for a fictional educational scenario.

Management has not approved it, and no technical implementation or effectiveness testing has taken place.
