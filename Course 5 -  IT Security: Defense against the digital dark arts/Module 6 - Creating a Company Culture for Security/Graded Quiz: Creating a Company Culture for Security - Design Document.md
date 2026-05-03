# Graded Quiz: Creating a Company Culture for Security - Design Document


1.

**Overview:** Now that you’re super knowledgeable about security, let's put your newfound know-how to the test. You may find yourself in a tech role someday, where you need to design and influence a culture of security within an organization. This project is your opportunity to practice these important skillsets.

**Assignment:** In this project, you’ll create a security infrastructure design document for a fictional organization. The security services and tools you describe in the document must be able to meet the needs of the organization. Your work will be evaluated according to how well you met the organization’s requirements.

**About the organization:** This fictional organization has a small, but growing, employee base, with 50 employees in one small office. The company is an online retailer of the world's finest artisanal, hand-crafted widgets. They've hired you on as a security consultant to help bring their operations into better shape.

**Organization requirements:** As the security consultant, the company needs you to add security measures to the following systems:

- An external website permitting users to browse and purchase widgets
- An internal intranet website for employees to use
- Secure remote access for engineering employees
- Reasonable, basic firewall rules
- Wireless coverage in the office
- Reasonably secure configurations for laptops
- Since this is a retail company that will be handling customer payment data, the organization would like to be extra cautious about privacy. They don't want customer information falling into the hands of an attacker due to malware infections or lost devices.

Engineers will require access to internal websites, along with remote, command line access to their workstations.

**Grading:** This is a required assignment for the module.

**What you'll do:** You’ll create a security infrastructure design document for a fictional organization. Your plan needs to meet the organization's requirements and the following elements should be incorporated into your plan:

- Authentication system
- External website security
- Internal website security
- Remote access solution
- Firewall and basic rules recommendations
- Wireless security
- VLAN configuration recommendations
- Laptop security configuration
- Application policy recommendations
- Security and privacy policy recommendations
- Intrusion detection or prevention for systems containing customer data


Security Infrastructure Design Document: Artisanal Widgets Inc.
1. Authentication System
To eliminate the risk of credential theft (the #1 attack vector), we will implement a Centralized Identity Provider (IdP) using a Single Sign-On (SSO) solution.

Method: All employees will use Multi-Factor Authentication (MFA).

Implementation: We will use FIDO2/WebAuthn (U2F tokens) for engineers and high-level admins, and TOTP (Authenticator Apps) for general staff. This ensures that even if a password is phished, the attacker cannot gain access.

2. External & Internal Website Security
External (Customer-Facing):

HTTPS/TLS: Mandatory encryption for all traffic using a Certificate Authority (CA) like Let’s Encrypt.

Web Application Firewall (WAF): To protect against SQL Injection and Cross-Site Scripting (XSS).

Internal (Intranet):

Accessible only via the corporate network or VPN.

Integration with SSO to ensure only active employees with valid MFA can view internal company news and resources.

3. Remote Access Solution
Engineers require command-line access to workstations.

Solution: A Client-to-Site VPN using OpenVPN or WireGuard.

Gateway: A Bastion Host (Jump Box). Engineers must SSH into the Bastion host first using SSH keys (not passwords). From there, they can jump to their specific internal workstations.

4. Firewall & Basic Rules
We will deploy a Stateful Inspection Firewall at the network perimeter.

Default Policy: Implicit Deny (Block everything not explicitly allowed).

Inbound Rules: Allow Port 443 (HTTPS) to the web server; allow VPN traffic.

Outbound Rules: Restrict outbound traffic to known update servers and essential web ports to prevent "command and control" communication if a device is infected.

5. Wireless Security & VLAN Configuration
We will segment the office network to limit the "blast radius" of an attack.

Wireless: Use WPA2/WPA3 Enterprise (802.1X). Employees log in with their unique SSO credentials, not a shared "office password."

VLAN Segmentation:

VLAN 10 (Sales/Admin): General office work.

VLAN 20 (Engineering): Access to workstations and dev environments.

VLAN 30 (Guest): Internet access only; completely isolated from internal servers.

VLAN 40 (PCI/Payments): Strictly isolated zone for handling customer data.

6. Laptop Security Configuration
Since the company is worried about lost devices:

Full-Disk Encryption (FDE): Mandatory (FileVault for Mac / BitLocker for Windows).

Endpoint Detection & Response (EDR): Modern antivirus that looks for suspicious behavior, not just known signatures.

Remote Wipe: Managed through an MDM (Mobile Device Management) solution.

7. Application & Privacy Policies
Application Whitelisting: Only pre-approved software can be installed on company laptops.

Data Handling: PCI DSS Compliance is mandatory. No credit card numbers should be stored on local laptops or in plain text in the database. Use Tokenization via the payment processor.

Privacy Policy: Implement a "Least Privilege" model—employees only have access to the customer data necessary for their specific job role.

8. Intrusion Detection & Prevention (IDS/IPS)
To protect customer data:

Deployment: A NIDS (Network Intrusion Detection System) will be placed at the edge of the PCI VLAN.

Action: Set to Prevention (IPS) mode to automatically drop packets that match known attack signatures (like brute force or database exploits).

Logging: Centralized logging to a secure server to ensure an audit trail exists if a breach occurs.



```
To secure Artisanal Widgets Inc., the infrastructure focuses on protecting customer payment
 data (PCI DSS compliance) while enabling engineering productivity.
 The strategy employs Defense in Depth, ensuring that if one security layer fails,
 others are in place to stop the threat.

Core Security Pillars
Identity & Access: All systems are gated by Multi-Factor Authentication (MFA) and
Single Sign-On (SSO). This ensures that compromised passwords alone aren't enough for an attacker to gain entry.

Network Defense: A stateful firewall enforces an "Implicit Deny" policy. The network is
segmented into VLANs to isolate sensitive payment data from general office traffic and the guest Wi-Fi.

Secure Engineering: Remote work is secured via a VPN and a Bastion Host, ensuring engineers
 can only access workstations through a single, highly monitored entry point.

Endpoint Protection: To prevent data loss from stolen hardware, all laptops utilize
 Full-Disk Encryption (FDE) and are managed via MDM for remote wiping capabilities.

Monitoring: A Network Intrusion Prevention System (IPS) specifically monitors the database
 environments to detect and block suspicious activity in real-time.
```

## Implementation Checklist

 | Requirement                  |        Solution|
|---------------------------------|--------------------------------------------|
|
|Customer Data	|PCI DSS compliance & Tokenization|
|
|Remote Access	|VPN + Bastion Host|
|
|Physical Loss	|BitLocker/FileVault Encryption|
|
|Phishing Defense	|FIDO2/U2F Security Keys|
|
|Internal Web	|SSO & Intranet Isolation|
|
