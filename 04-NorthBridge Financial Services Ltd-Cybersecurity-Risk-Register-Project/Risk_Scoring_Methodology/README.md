Risk Scoring Methodology

1. Purpose

This document defines the methodology used to identify, assess, score, and prioritise cybersecurity risks at **NorthBridge Financial Services Ltd.**, a fictional Canadian financial services organisation.

The methodology provides a consistent approach for evaluating potential threats to the organisation's information assets, technology infrastructure and business operations.

2. Risk Assessment Approach

This project uses a qualitative risk assessment approach based on two factors:

- Likelihood: The probability that a risk event may occur.
- Impact: The potential consequences if the risk event occurs.

The risk score is calculated using the following formula:

**Risk Score = Likelihood × Impact**

Both factors are rated on a scale of 1 to 5.

3. Likelihood Rating

| Score | Rating | Description |
|---|---|---|
| 1 | Rare | The event is highly unlikely to occur. |
| 2 | Unlikely | The event could occur but is not expected under normal circumstances. |
| 3 | Possible | The event may occur under certain circumstances. |
| 4 | Likely | The event is expected to occur in many circumstances. |
| 5 | Almost Certain | The event is highly expected or may occur frequently. |

4. Impact Rating

| Score | Rating | Description |
|---|---|---|
| 1 | Negligible | Minimal disruption with little or no business impact. |
| 2 | Minor | Limited disruption requiring minimal corrective action. |
| 3 | Moderate | Noticeable operational impact or limited data exposure. |
| 4 | Major | Significant financial, operational, regulatory or reputational consequences. |
| 5 | Severe | Extensive business disruption, major data compromise or serious regulatory consequences. |

5. Risk Rating Classification

The calculated risk score determines the risk category.

| Risk Score | Risk Rating | Priority |
|---|---|---|
| 1–4 | Low | Routine monitoring |
| 5–9 | Medium | Planned risk treatment |
| 10–16 | High | Priority treatment and management attention |
| 17–25 | Critical | Urgent management attention and treatment |

These thresholds are illustrative and are specific to this simulated project. They are not universal industry thresholds.

6. Inherent Risk

Inherent risk is the level of risk that exists before considering the effect of security controls.

It represents the potential exposure associated with a threat exploiting a vulnerability.

Example:

A former employee retains an active account after leaving the organisation.

- Likelihood: 4 (Likely)
- Impact: 5 (Severe)
- Inherent Risk Score: 4 × 5 = 20
- Inherent Risk Rating: Critical

7. Existing Security Controls

Existing controls are safeguards already in place to reduce the likelihood or impact of identified risks.

Examples include:

- Multi-factor authentication (MFA).
- Identity and access management procedures.
- Endpoint protection.
- Security awareness training.
- Cloud security configurations.
- Security monitoring and logging.
- Backup and recovery procedures.
- Vendor security reviews.

Controls must be evaluated based on their design, implementation and available evidence. The existence of a policy or technical setting alone does not establish that a control is operating effectively.

8. Residual Risk

Residual risk is the level of risk remaining after considering existing security controls.

Residual risk is assessed using the same likelihood and impact scales.

Important: A residual risk score should only be lower than the inherent risk score where existing controls provide a reasonable and documented basis for reducing the likelihood or impact.

Proposed remediation actions must not automatically reduce the current residual risk score. The risk should be reassessed after remediation has been implemented and its effectiveness verified.

9. Risk Treatment Options

The project uses four recognised risk treatment approaches:

| Treatment | Description |
|---|---|
| Mitigate | Implement controls to reduce the likelihood or impact of the risk. |
| Avoid | Stop or change the activity that creates the risk. |
| Transfer | Transfer some financial or contractual consequences to another party, such as through insurance or contractual arrangements. |
| Accept | Formally acknowledge and approve the remaining risk by an authorised risk owner. |

Risk acceptance should be documented, approved by the appropriate authority and reviewed periodically.

10. Risk Assessment and Review

Each identified risk should include:

- Unique risk identification number.
- Risk description.
- Affected asset or business process.
- Threat and vulnerability.
- Potential business impact.
- Inherent likelihood, impact and score.
- Existing security controls.
- Residual likelihood, impact and score.
- Risk owner.
- Recommended treatment.
- Remediation action and target date.
- Relevant framework references.
- Review status and supporting evidence.

Risk assessments should be reviewed periodically and whenever significant changes occur in the organisation's technology, business operations, threat environment or regulatory obligations.

11. Framework References

The project uses the following frameworks as reference points:

- NIST Cybersecurity Framework (CSF) 2.0.
- ISO/IEC 27001:2022.
- CIS Critical Security Controls v8.1.

Framework mappings are indicative and should be validated against the actual control requirements, organisational scope and applicability before being treated as compliance evidence.

12. Project Disclaimer

This methodology was developed for a simulated GRC portfolio project. NorthBridge Financial Services Ltd. is fictional, and all risk scenarios, ratings, controls and recommendations are illustrative. This document does not represent an actual organisational risk assessment or independent audit.
