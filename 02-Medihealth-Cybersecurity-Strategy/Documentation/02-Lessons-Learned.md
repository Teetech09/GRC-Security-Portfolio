# MediHealth Clinic — Lessons Learned

## 1. Project Overview

In this project, I developed a proposed cybersecurity strategy for a fictional healthcare clinic with 50 employees.

The work covered asset identification, threat assessment, risk prioritisation, phishing awareness, password security, MFA, backup and recovery, and incident response.

## 2. Connecting Security to Patient Care

I learned to explain cybersecurity risks in terms of their effects on clinic operations and patient care.

For example, an unavailable EHR can delay access to medical histories, while unauthorised record changes can affect the reliability of information used for clinical decisions.

This helped me look beyond data theft and consider confidentiality, integrity, and availability together.

## 3. Separating Facts From Assumptions

One important lesson was that missing documentation does not prove a control is absent.

The scenario states that the clinic has no backup and recovery policy, but it does not establish whether backups exist. Similarly, repeated phishing attempts do not prove that an account was compromised.

I therefore documented unknowns and verification requirements instead of presenting assumptions as confirmed findings.

## 4. Understanding Assets, Vulnerabilities, Threats, and Risks

The assessment helped me distinguish these concepts.

The EHR server is an asset. Outdated software is a vulnerability. An attacker exploiting a software flaw is a threat scenario. The resulting possibility of information compromise or service disruption is a risk.

Making these connections helped me propose controls that address specific weaknesses.

## 5. Using Risk Scores With Judgement

I used likelihood and impact scores to organise the risks, but learned that a score should not determine priorities on its own.

Although outdated software received the highest initial score, backup verification remained an immediate action because an EHR outage had already occurred.

Risk prioritisation should also consider patient care, uncertainty, dependencies, and the effort needed to implement controls.

## 6. Designing Friendly Awareness Materials

Preparing the phishing campaign showed me the importance of language that employees can understand and use.

Healthcare examples, such as insurance updates and patient notifications, made the material relevant to staff responsibilities.

I also included a supportive reporting message. Employees should feel comfortable reporting accidental interactions promptly rather than hiding them out of fear.

## 7. Explaining Email Authentication Carefully

I learned to present SPF, DKIM, and DMARC as supporting checks rather than proof that an email is safe.

A message can pass authentication while still containing a harmful request. Staff should continue checking the address, context, and links and verify unexpected requests independently.

Technical checks should support reporting without making employees feel they must understand email headers before asking for help.

## 8. Updating Password Recommendations

The project brief requested password complexity and regular rotation. Reviewing current guidance helped me understand why a policy can instead emphasise length, unique passwords, compromised-password screening, and changes after suspected compromise.

I documented the reason for this departure rather than following the older requirement without explanation.

This reinforced the importance of checking the currency of guidance before writing a policy.

## 9. Planning MFA Around Real Workflows

I learned that selecting an authentication method is only part of an MFA plan.

Successful implementation also requires compatibility checks, individual accounts, staff enrolment, recovery procedures, and testing for bypass routes.

For a clinic, shared workstations and urgent access needs must be considered without relying on informal credential sharing.

## 10. Treating Recovery as Something to Test

A successful backup job does not prove that a system can be restored.

The recovery plan therefore includes restoration testing, application checks, clinical validation, and reconciliation of records created during downtime.

I also learned to distinguish RTO, the restoration time target, from RPO, the acceptable data loss measured in time. The proposed targets remain assumptions until approved and tested.

## 11. Defining Ownership and Response Authority

Writing the incident response plan highlighted the need for clear responsibilities.

Technical staff, clinical leadership, and management may need to make different decisions during the same incident. Disruptive containment actions require agreed authority and consideration of clinical effects.

Recovery also does not resolve every question. A restored system may still require investigation into whether information was previously accessed or stolen.

## 12. Handling Regulatory References Responsibly

I learned not to assume that a regulation applies merely because it concerns healthcare.

The strategy identifies Nigerian data protection requirements for further assessment and treats HIPAA applicability as a separate question.

Technical guidance can inform recommendations, but it does not establish legal compliance or certification.

## 13. Documenting the Project on GitHub

Organising the project into assessment, awareness, policies, plans, report, and presentation folders helped make the work easier to navigate.

Clear filenames, relative links, and descriptive commit messages support review.

I also kept the distinction between completed documentation and proposed operational activities visible throughout the project.

## 14. Skills Practised

- Defining assessment scope.
- Identifying assets and security weaknesses.
- Developing threat scenarios.
- Scoring and prioritising risks.
- Writing security policies and implementation plans.
- Preparing staff awareness materials.
- Communicating recommendations to management.
- Recording assumptions and limitations.
- Organising portfolio documentation.

## 15. What I Would Improve in a Real Assessment

With access to a real clinic, I would:

1. Interview clinical staff, management, and IT personnel.
2. Verify architecture, software versions, permissions, and existing controls.
3. Review authentication and backup records.
4. Perform authorised restoration and workflow tests.
5. Complete a business impact assessment with clinical leadership.
6. Obtain vendor compatibility information and cost estimates.
7. Validate regulatory obligations with qualified support.
8. Reassess risks using the evidence collected.

## 16. Project Limitations

This was a fictional, scenario-based documentation project.

I did not conduct a live audit, deploy controls, deliver staff training, run a phishing simulation, or perform recovery or incident response exercises.

The project demonstrates assessment and planning skills. It does not demonstrate verified operational improvements.

## 17. Personal Reflection

This project helped me move from identifying individual weaknesses to developing a connected cybersecurity strategy.

I learned to explain why a control matters, who should own it, how it could be introduced, and what evidence would show that it works.

My main takeaway is that a useful security recommendation must protect information while fitting the organisation’s operational needs.
