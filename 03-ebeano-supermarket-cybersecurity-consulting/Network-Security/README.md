
 Deliverable 2: Network Security Plan

 Ebeano Supermarket Cybersecurity Consulting Project

Category: GRC / Network Security Architecture  
Business: Ebeano Supermarket — Simulated Case Study  
Workforce: 28 Employees  
Deliverable: 2 of 5  
Status: Proposed — Not Implemented

---

1. Executive Summary

Ebeano Supermarket provides free Wi-Fi to customers while using cloud-based POS systems, staff tablets, kitchen terminals, inventory systems, and administrative devices.

Without adequate network separation, a compromised customer device or employee tablet could potentially expose sensitive business systems to unauthorized access, malware, or ransomware.

This proposed network security plan introduces network segmentation, firewall restrictions, secure Wi-Fi configuration, and monitoring to reduce these risks.

2. Network Security Objectives

- Separate customer Wi-Fi from internal business systems.
- Protect POS devices and payment-related communications.
- Restrict access to kitchen, inventory, and administrative devices.
- Reduce opportunities for malware to spread between networks.
- Protect router and firewall administration.
- Support secure business operations across multiple outlets.

3. Proposed Network Segmentation

Network segmentation divides one large network into smaller security zones.

For Ebeano Supermarket, the recommended zones are:

| Network Zone | Example VLAN | Devices | Access Restrictions |
|---|---|---|---|
| Guest Wi-Fi | VLAN 10 | Customer phones and laptops | Internet only; no internal access |
| POS / Payments | VLAN 20 | POS terminals and approved payment tablets | Approved payment services only |
| Staff Operations | VLAN 30 | Kitchen terminals and inventory devices | Approved business applications |
| Administration | VLAN 40 | Manager and authorized administrative devices | Approved business services |
| IT Management | VLAN 50 | Network management workstation | Restricted infrastructure administration |

VLAN identifiers are illustrative. Actual deployment requires compatible network equipment and configuration.

4. Proposed Network Architecture

<img width="2784" height="884" alt="mermaid-diagram" src="https://github.com/user-attachments/assets/3f497ba3-fa9a-4677-b435-a76d7db79e29" />





The diagram represents logical network zones. In deployment, each zone would connect through appropriately configured switching, wireless access points, and firewall interfaces.

 5. Guest Wi-Fi Security

Customer Wi-Fi should be isolated from all operational networks.

Recommended controls:

- Use a separate guest SSID.
- Enable client isolation where supported.
- Block access to internal IP ranges.
- Prevent guest access to router administration.
- Apply bandwidth limits to reduce service disruption.
- Use WPA2-AES or WPA3 where supported.
- Keep wireless equipment updated.

Business explanation: Customers can use the internet without gaining access to payment terminals, staff tablets, or internal business systems.

6. POS and Payment Network Protection

The POS network should be treated as a high-security zone.

Recommended controls:

1. Connect only authorized POS devices.
2. Allow outbound traffic only to required payment services and supporting infrastructure.
3. Block guest-to-POS communication.
4. Restrict POS-to-staff and POS-to-administration communication.
5. Disable unnecessary services and remote access.
6. Keep POS devices and payment applications updated.
7. Monitor payment connectivity and suspicious activity.
8. Maintain an approved POS device inventory.

Where payment provider endpoints are dynamic, use vendor-supported firewall rules rather than assuming fixed IP addresses.

7. Staff Operations Network

Kitchen terminals and inventory devices should operate on a separate staff network.

Recommended controls:

- Allow access only to required order and inventory applications.
- Restrict communication with the POS zone.
- Disable unnecessary file sharing.
- Require authenticated staff access.
- Apply device updates and endpoint protection where supported.
- Prevent unmanaged personal devices from joining this network.

8. Administration and IT Management

Manager devices should be separated from customer and general staff networks.

IT management access should be restricted further.

Recommended controls:

- Use unique administrator credentials.
- Require MFA where supported.
- Disable remote administration from the public internet unless specifically needed and securely configured.
- Permit management access only from authorized devices.
- Log administrative changes.
- Back up network configurations securely.
- Review network administrator access monthly.

9. Proposed Firewall Rules

| Source | Destination | Proposed Rule | Reason |
|---|---|---|---|
| Guest Wi-Fi | Internet | Allow approved outbound traffic | Customer connectivity |
| Guest Wi-Fi | Internal networks | Deny | Prevent unauthorized access |
| POS Network | Approved payment services | Allow required traffic | Process payments |
| POS Network | Guest Wi-Fi | Deny | Protect payment environment |
| Staff Operations | Approved cloud applications | Allow required traffic | Business operations |
| Staff Operations | IT Management | Deny | Protect administration |
| Administration | Approved business services | Allow required traffic | Management operations |
| IT Management | Authorized infrastructure interfaces | Allow restricted management traffic | Technical maintenance |
| All zones | Unnecessary inter-zone traffic | Deny by default | Limit lateral movement |

Firewall rules should be tested to confirm that required business applications continue to work.

10. Ransomware and Malware Risk Reduction

Segmentation can reduce the ability of malware to move between systems, but it cannot prevent all ransomware attacks.

Additional recommendations include:

- Enable automatic security updates.
- Deploy endpoint protection where supported.
- Maintain tested, protected backups of important business data.
- Restrict administrative privileges.
- Train staff to recognize phishing.
- Disable unnecessary services.
- Monitor unusual device and network activity.
- Maintain a basic incident response procedure.

Cloud-based systems should also be reviewed for available backup, recovery, and audit features.

11. Multi-Outlet Security Considerations

For multiple supermarket outlets:

- Apply a consistent network segmentation standard.
- Use separate authorized administrative credentials.
- Maintain an inventory of routers, switches, and access points.
- Secure any connections between outlets using approved encrypted methods.
- Avoid exposing management interfaces directly to the internet.
- Review security settings after new outlet installations.

Each outlet should have an approved network diagram and configuration record.

12. Implementation Roadmap

| Phase | Recommended Activity | Priority |
|---|---|---|
| Phase 1 | Inventory existing network devices and connected systems | Critical |
| Phase 2 | Separate guest Wi-Fi from internal business networks | Critical |
| Phase 3 | Isolate POS and payment devices | Critical |
| Phase 4 | Configure firewall rules and restrict administrative access | High |
| Phase 5 | Separate staff, administration, and IT management networks | High |
| Phase 6 | Test connectivity, logging, and business applications | High |
| Phase 7 | Establish ongoing monitoring and configuration reviews | Medium |

13. Validation and Testing Plan

Before considering the network secure, the following tests should be performed:

1. Confirm guest devices can reach the internet.
2. Confirm guest devices cannot access internal systems.
3. Confirm POS devices can reach approved payment services.
4. Confirm unauthorized devices cannot access POS administration.
5. Confirm staff devices cannot access network management interfaces.
6. Confirm firewall logs capture blocked connection attempts.
7. Confirm business applications continue to operate after segmentation.
8. Confirm network configuration backups can be restored.

These are proposed validation activities, not completed tests.

 14. Expected Business Benefits

If implemented correctly, this network security plan could:

- Reduce exposure of POS systems to customer devices.
- Limit opportunities for unauthorized internal access.
- Reduce the potential spread of ransomware.
- Improve protection of sensitive business operations.
- Strengthen administrative accountability.
- Support consistent security practices across outlets.

15. Limitations and Assumptions

- The existing router, switch, and access point capabilities are unknown.
- VLAN support may require additional equipment.
- Actual cloud POS connectivity requirements must be confirmed with the vendor.
- The number of outlets and existing network topology are not specified.
- Segmentation does not replace endpoint security, backups, or staff training.

16. Implementation Status

Status: Proposed — Not Implemented

This plan is part of a simulated cybersecurity consulting engagement. The architecture, VLANs, firewall rules, and validation steps are recommendations and have not been deployed or tested in a live supermarket environment.



Project: Ebeano Supermarket Cybersecurity Consulting  
Deliverable: 2 of 5 — Network Security Plan
  
