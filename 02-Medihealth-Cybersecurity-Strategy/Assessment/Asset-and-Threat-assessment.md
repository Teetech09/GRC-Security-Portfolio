# MediHealth Clinic — Asset and Threat Assessment

## 1. Purpose

This assessment identifies important assets, connects the weaknesses described in the project brief to plausible threats, and explains their potential effects on patient information and clinical services.

This is a scenario-based assessment. No systems have been inspected or tested.

## 2. Key Assets

| ID | Asset | Value to the clinic | Protection priorities |
|---|---|---|---|
| A01 | Patient information | Supports identification, diagnosis, treatment, and insurance processing. | Confidentiality, integrity, and availability |
| A02 | EHR application | Allows staff to manage and access patient records. | Confidentiality, integrity, and availability |
| A03 | EHR server | Supports the operation of the EHR system. | Integrity and availability |
| A04 | Staff accounts and credentials | Control access to systems and information. | Confidentiality and integrity |
| A05 | Staff laptops and portable devices | Allow medical personnel to perform their work and access information. | Confidentiality, integrity, and availability |
| A06 | EHR communications | Carry information between users and the EHR system. | Confidentiality and integrity |
| A07 | Clinic premises and equipment | Provide the physical environment for care and information processing. | Confidentiality, integrity, and availability |

The exact architecture, asset quantities, system owners, and data locations require verification.

## 3. Threat and Vulnerability Assessment

### T01 — Account Compromise Through Phishing

**Affected assets:** Staff accounts, patient information, and the EHR application.

**Observed vulnerabilities:** Basic awareness training without a recurring programme; no MFA.

**Threat scenario:** An employee receives a convincing fake patient notification or insurance message and enters their login details into a fraudulent website. An attacker attempts to use those credentials to access clinic systems.

**Potential impact:**
- Confidentiality: Patient information could be viewed or copied.
- Integrity: Records could be changed if the compromised account has editing permissions.
- Availability: An attacker could disrupt access, depending on the account’s privileges.
- Patient care: Unavailable or altered information could interfere with clinical work.

**Proposed controls:**
- Provide recurring healthcare-focused phishing training.
- Establish a simple reporting process.
- Implement MFA on supported systems.
- Apply least privilege to staff accounts.
- Monitor suspicious authentication activity.

**Evidence limitation:** The brief describes phishing attempts but does not establish a successful account compromise.

### T02 — Unauthorised Activity Using Shared or Weak Credentials

**Affected assets:** Staff accounts, patient information, and the EHR application.

**Observed vulnerabilities:** Weak passwords and shared login details.

**Threat scenario:** Someone guesses a weak password or uses credentials shared by a colleague to access records beyond their responsibilities.

**Potential impact:**
- Confidentiality: Patient information could be accessed without a legitimate need.
- Integrity: Unauthorised changes could affect the accuracy of patient records.
- Accountability: Shared accounts make it difficult to identify who performed an action.
- Patient care: Incorrect records could affect clinical decisions.

**Proposed controls:**
- Assign individual accounts to staff.
- Prohibit credential sharing.
- Define suitable password requirements.
- Review access according to job responsibilities.
- Record user activity and promptly revoke unnecessary access.

**Evidence limitation:** Account permissions and audit logging capabilities are unknown.

### T03 — Exploitation of Outdated Software

**Affected assets:** EHR application, server, staff devices, and patient information.

**Observed vulnerability:** The EHR system and software on staff devices are described as outdated.

**Threat scenario:** An attacker exploits an unpatched vulnerability to gain access, steal information, or deploy malware.

**Potential impact:**
- Confidentiality: Patient information could be stolen.
- Integrity: Systems or records could be altered.
- Availability: Malware or ransomware could interrupt clinical services.
- Patient care: Staff could lose timely access to medical histories and other essential information.

**Proposed controls:**
- Create a software and device inventory.
- Verify versions and vendor support status.
- Prioritise security updates based on risk.
- Test updates before deployment to critical systems.
- Replace unsupported software.
- Apply endpoint protection and restrict unnecessary network access.

**Evidence limitation:** No software versions or specific exploitable vulnerabilities have been verified.

### T04 — Interception of Unencrypted EHR Communications

**Affected assets:** EHR communications, patient information, and potentially credentials.

**Observed vulnerability:** The brief states that EHR communications lack encryption.

**Threat scenario:** An attacker with access to a relevant network path intercepts unencrypted traffic. Depending on the protocol and other controls, the attacker may also attempt to alter communications.

**Potential impact:**
- Confidentiality: Sensitive information transmitted over the connection could be exposed.
- Integrity: Information could potentially be modified in transit.
- Patient care: Altered information could affect decisions if accepted by the system.

**Proposed controls:**
- Verify the protocols and connections used by the EHR.
- Enable supported transport encryption.
- Manage certificates securely.
- Disable insecure connections where feasible.
- Protect and segment relevant networks.

**Evidence limitation:** The brief does not identify the protocols or exact information transmitted.

### T05 — EHR Outage and Delayed Recovery

**Affected assets:** EHR server, application, and access to patient information.

**Observed conditions:** A server hardware failure disrupted EHR access, and no backup and recovery policy is documented.

**Threat scenario:** Another hardware failure or disruptive event causes an outage. Unclear recovery procedures or ineffective backups prolong the disruption.

**Potential impact:**
- Availability: Staff cannot access the EHR when needed.
- Integrity: Records could be lost or restored incompletely if recovery arrangements are inadequate.
- Patient care: Treatment, documentation, and other services could be delayed.

**Proposed controls:**
- Verify whether backups exist and whether they can be restored.
- Define recovery responsibilities and procedures.
- Agree recovery time and recovery point targets with clinical management.
- Protect backups and test restoration.
- Establish procedures for clinical work during an EHR outage.
- Review hardware maintenance and resilience requirements.

**Evidence limitation:** Backup existence, restoration capability, and the duration of the previous outage are unknown.

### T06 — Unauthorised Physical Access

**Affected assets:** Clinic equipment, staff devices, EHR server, and patient information.

**Observed vulnerabilities:** No staff identification cards and no physical security are described in the brief.

**Threat scenario:** An unauthorised person enters a sensitive area and accesses an unattended device, steals equipment, or interferes with the server.

**Potential impact:**
- Confidentiality: Patient information could be exposed.
- Integrity: Equipment or information could be tampered with.
- Availability: Theft or damage could interrupt services.

**Proposed controls:**
- Introduce staff identification and visitor procedures.
- Restrict entry to server and records areas.
- Secure devices and enable automatic screen locking.
- Assign responsibility for physical access.
- Review appropriate monitoring arrangements.

**Evidence limitation:** The building layout and existing entry procedures have not been inspected.

## 4. Cross-Cutting Weakness: Incident Response

The absence of a documented incident response plan could worsen the consequences of any of the scenarios above.

Recommended improvements include:

- A clear incident reporting channel.
- Defined response roles and escalation contacts.
- Procedures for containment and evidence preservation.
- Recovery and communication arrangements.
- Post-incident review and corrective actions.

## 5. Next Step

Assess the likelihood and impact of each scenario in the risk register.

Threat numbering does not represent priority. Priorities will be established using a defined scoring method and documented reasoning.
