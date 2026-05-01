# Graded Quiz: Module 6 challenge: System Administration Consultation

<img width="610" height="690" alt="image" src="https://github.com/user-attachments/assets/5bd81d73-c122-42d1-9f00-371417ebd77b" />


<img width="633" height="746" alt="image" src="https://github.com/user-attachments/assets/4663f234-47d7-4895-b6bc-cb98b890e877" />


<img width="641" height="751" alt="image" src="https://github.com/user-attachments/assets/70bce0c1-8d02-4693-8b7f-9bad0180029d" />


<img width="570" height="738" alt="image" src="https://github.com/user-attachments/assets/51e84be5-19f0-4191-aa0c-12d53603974d" />


<img width="636" height="747" alt="image" src="https://github.com/user-attachments/assets/92aba5fd-af01-4bdf-825a-2b682c968a4a" />


1. Process Review: Network Funtime Company
Network Funtime Company currently suffers from "reactive" IT management, leading to security vulnerabilities and operational delays. As the sole System Administrator, I recommend the following five improvements to stabilize the infrastructure:

Standardized Hardware Profiles: I will establish two standard laptop configurations—one high-performance for engineers and one mid-range for Sales/HR. Standardizing allows for a predictable budget and enables IT to maintain a "buffer stock," ensuring new hires have equipment on day one.

Centralized Identity Management: Implementing a Directory Service (like Google Workspace or Azure AD) with Single Sign-On (SSO) will replace manual logins. This allows for enforced password policies and remote password resets, ending the need to reimage machines for forgotten credentials.

Automated OS Deployment: Instead of manual USB installs, I will implement Mobile Device Management (MDM). This automates the deployment of Linux and Windows configurations, ensuring all devices meet security baselines immediately upon unboxing.

Asset Tagging and Inventory: Every device will receive a physical Asset Tag linked to a digital inventory system. This creates an audit trail for lost or stolen hardware and tracks the fleet’s physical health.

Ticketing System Implementation: Moving requests from HR’s email to a dedicated Helpdesk Ticket System ensures technical issues are tracked, prioritized, and resolved without bottlenecking HR personnel.

Rationale
These changes shift the burden of technical setup from HR to a scalable, automated system. By centralizing identity and standardizing hardware, we minimize downtime and significantly harden the company's security posture, which is essential for a growing open-source software firm.


2. Process Review: W.D. Widgets
W.D. Widgets is facing a "scaling wall." While the use of Active Directory is a strong start, the reliance on manual setups and on-premise single points of failure will lead to a total collapse as the company hires hundreds more. I recommend these five improvements:

Automated Software Deployment: I will implement Group Policy Objects (GPO) or Microsoft Endpoint Configuration Manager to push sales applications automatically. This eliminates the "few hours" spent manually installing software per machine, allowing me to scale with the hiring surge.

Migration to Cloud Productivity: Transitioning email and instant messaging to a cloud suite (like Microsoft 365) removes the burden of maintaining in-house servers. This ensures high availability and offloads hardware maintenance, which is critical for a sole administrator.

Redundant Backup System: The single file server is a catastrophic risk. I will implement a 3-2-1 backup strategy—three copies of data, on two different media, with one off-site—to ensure customer data is never permanently lost.

Permission Structure Overhaul: I will replace "creator-owner" permissions with a Role-Based Access Control (RBAC) model. This prevents accidental deletions and ensures data security as the sales team grows.

Helpdesk Ticketing System: Moving from direct emails to a formal ticketing system allows for request prioritization and creates a knowledge base, preventing me from becoming a bottleneck during rapid expansion.

Rationale
These changes shift W.D. Widgets from a fragile, manual environment to a resilient, automated infrastructure. By removing the risk of data loss and automating repetitive tasks, the IT department can support a 300% growth rate without a linear increase in workload.


3. Process Review: Dewgood
Dewgood’s infrastructure relies on high-risk manual processes and "single points of failure." To protect this non-profit’s mission while staying budget-conscious, I recommend these five improvements:

Cloud Migration for Public Web and Email: I will move the website to a low-cost host and migrate email to a suite like Google Workspace for Nonprofits. This ensures the website stays online even if the local server fails and reduces the maintenance burden on a sole administrator.

Automated Account Deactivation: I will implement a strict offboarding protocol to disable Active Directory accounts immediately when an employee departs. This closes critical security gaps created by dormant, authorized accounts.

Modernized Backup Strategy: Taking disks home is a liability. I will implement an encrypted cloud backup for the file server to ensure data is recoverable in case of theft, transit loss, or site-wide disaster.

Knowledge Base Integration: To fix the "confusing" ticketing system, I will build a Self-Service Wiki. Documenting common fixes allows staff to solve minor issues independently, reducing direct interruptions.

Non-Profit Vendor Accounts: Establishing a business account with a hardware vendor allows for standardized laptop orders. This eliminates time-consuming retail trips and ensures hardware consistency across the 50-person team.

Rationale
These steps move Dewgood from a "fragile" state to a "resilient" one. By leveraging non-profit cloud discounts and automating security, we protect sensitive data and ensure the organization can continue its mission without catastrophic technical interruptions.
