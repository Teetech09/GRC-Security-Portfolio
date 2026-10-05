
# MediHealth Clinic — Sample Phishing Email

## 1. Purpose

This fictional email illustrates how an attacker could impersonate an insurance provider to steal healthcare employees’ credentials.

It is an educational example. All names and addresses are fictional, and the link uses the reserved `.example` domain.

## 2. Intended Audience

- Reception and administrative staff.
- Insurance and billing personnel.
- Medical personnel who handle patient-related messages.

## 3. Fictional Phishing Email

**From:** Claims Support <claims@medicover-updates.example>  
**To:** MediHealth Clinic Billing Team  
**Subject:** Urgent: Verify Your Account to Prevent Patient Claim Suspension

Dear MediHealth Team,

We have identified a verification issue affecting your clinic’s insurance claims account.

To avoid delays in processing patient claims, all billing staff must verify their accounts within two hours. Accounts that remain unverified will be temporarily suspended.

Open the portal below and sign in using your clinic username and password:

https://medicover-verification.example/login

If you receive a verification code, enter it on the portal to complete the process.

Please do not contact your usual account representative, as this update is being managed by our technical verification team.

Regards,  
Daniel Reed  
Claims Support Officer  
MediCover Insurance Services

## 4. Warning Signs

| Warning sign | Where it appears | Why it matters |
|---|---|---|
| Unexpected account verification | The message claims there is a verification issue. | Staff should confirm unexpected requests through an established contact or trusted portal. |
| Time pressure | “Within two hours.” | Urgency can discourage careful checking. |
| Threat of disruption | Patient claims will allegedly be suspended. | The message uses concern about clinic operations to pressure the recipient. |
| Unverified sender and website | The sender and login address use different domains. | Staff must check both against known legitimate addresses. A mismatch is a warning sign, although it is not conclusive proof by itself. |
| Request for clinic credentials | The email asks staff to use their clinic username and password. | An unexpected external portal requesting internal credentials needs independent verification. |
| Request for a verification code | The portal allegedly needs a code. | An attacker could capture a code and attempt to use it during a live login. |
| Discourages verification | “Please do not contact your usual account representative.” | The message attempts to prevent staff from checking through a trusted channel. |

Professional wording, a familiar name, a logo, or HTTPS does not establish that an email is trustworthy.
## Additional Check: View the Email’s Technical Details

Sometimes an email displays a familiar name, but the address behind it is unfamiliar. You can inspect the full sender address and, in some email applications, check how the message was authenticated.

### How to Check in Gmail on a Computer

1. Open the email without clicking any links or attachments.
2. Click the three dots beside the Reply button at the top-right of the message.
3. Select **Show original**.
4. Look for the sender details and the results labelled **SPF**, **DKIM**, and **DMARC**.

Other email applications may use options such as “View message source” or “View headers.” Ask IT for help if you cannot find them.

### What Do These Checks Mean?

| Check | Friendly explanation |
|---|---|
| SPF | Checks whether the sending server is authorised to send email for the domain used in the technical sending address. |
| DKIM | Checks a digital signature to help confirm that signed parts of the message have not changed since signing. |
| DMARC | Checks whether a passing SPF or DKIM result matches the domain shown in the visible From address. |

### What Should You Do With the Results?

- **PASS:** The message passed that authentication check. Continue checking the sender address, request, and links.
- **FAIL:** Something may be wrong. Report the message for IT to review. Legitimate messages can sometimes fail because of forwarding or configuration problems.
- **Missing or unclear results:** Ask IT for help rather than trying to interpret the technical details yourself.

### Remember: PASS Does Not Mean Safe

An attacker can send a message from their own domain that passes all three checks. A compromised legitimate account can also send harmful messages.

These checks do not prove who the person behind the email is or whether their request is trustworthy.

**Pause, check, verify through a trusted channel, and report anything suspicious. You do not need to understand email headers before reporting a message.**




## 5. Expected Employee Response

1. Pause before clicking or replying.
2. Inspect the full sender address and link destination.
3. Verify the request using a known contact number or an independently opened, trusted portal.
4. Report the message through the clinic’s approved reporting channel.
5. Follow IT instructions for preserving or removing the message.

The clinic’s reporting channel must be defined before training is delivered.

On a computer, hovering over a link may reveal its destination. On mobile devices, use a safe preview method where available without opening the link. If uncertain, report the message.

## 6. If an Employee Already Interacted

### Clicked the link

Report the interaction promptly and describe what happened. Clicking alone does not establish that the account or device was compromised.

### Entered a password or verification code

Contact IT immediately through a trusted channel. IT should assess the incident and arrange appropriate account protection, such as a password reset, session revocation, and review of authentication activity.

### Downloaded or opened a file

Stop interacting with the file and contact IT promptly. Follow the clinic’s incident response instructions.

Employees should report mistakes without fear of blame. Early reporting can reduce the impact of an incident.

## 7. Learning Objectives

After reviewing this example, employees should be able to:

- Recognise urgency and operational pressure as possible phishing tactics.
- Inspect sender addresses and website destinations.
- Verify requests through independent, trusted channels.
- Avoid entering credentials into unexpected websites.
- Report suspicious messages and accidental interactions promptly.

## 8. Suggested Discussion Questions

1. Which detail would make you pause first?
2. How would you verify the insurance request?
3. Why should you avoid using contact details supplied in the suspicious email?
4. What should you do if you already entered your password?

## 9. Success Criteria

During a training exercise, staff should be able to:

- Identify at least three warning signs.
- Explain a safe verification method.
- Describe the approved reporting process.
- Explain what to do after an accidental interaction.

These are proposed learning outcomes, not measured results.

## 10. Project Status

Sample developed for the educational portfolio.

No email has been sent, no simulation has been conducted, and no credentials have been collected.
