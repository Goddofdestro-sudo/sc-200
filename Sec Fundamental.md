---
title: Sec Fundamental
updated: 2026-05-11 10:34:06Z
created: 2026-04-14 12:32:48Z
---

Physical Security

Overview

- Prevents unauthorized physical access to buildings/areas.
- Main controls: Deterrents, Monitoring Controls, Access Controls.
- Important in cybersecurity investigations.

Why Important?

- Physical access often means full system compromise.
- Risks: direct system access, data theft, physical damage.

Controls

Access Controls

- Prevent unauthorized area access.
- Examples:

- Mantraps: Holding room between two doors, inspection before access.
- Turnstiles/Gates: ID badge required to enter.
- Electronic Doors: Role-based access (e.g., HR can't enter server room).

Monitoring Controls

- Detect and respond to intruders.
- Examples:

- CCTV: Real-time and recorded video surveillance.
- Security Guards: Trained personnel to operate and respond.
- Intrusion Detection Systems: Detect heat, sound (e.g., glass breaking), movement.

Deterrents

- Discourage potential intruders.
- Examples:

- Warning signs (“Do Not Enter,” “Trespassing”).
- Fences with barbed/razor wire.
- Guard dogs.
- Security lighting.
- CCTV presence (even fake cameras can deter).

Endpoint Security

Overview

- Protects endpoints like desktops, laptops, servers from attacks.

Key Controls

Host Intrusion Detection System (HIDS)

- Software on endpoints detects suspicious activity.
- Generates alerts for investigation.

Host Intrusion Prevention System (HIPS)

- Similar to HIDS but can autonomously block threats or remove malicious files.

Anti-Virus (AV)

- Detects/removes malware.
- Types:

- Signature-based: Detects known malware patterns.
- Behavior-based: Detects anomalies from normal behavior.

Log Monitoring

- Endpoints send logs to centralized SIEM for analysis and alerting.

Endpoint Detection and Response (EDR)

- Monitors activity, allows deep investigations, and helps detect insider threats.

Vulnerability Scanning

- Regular scans to find security flaws.
- Internal and external scans; credentialed and non-credentialed.
- Helps prioritize fixes.

Compliance Scanning

- Checks endpoint security against compliance standards.

Email Security

Overview

- Phishing is the top attack vector; email security is critical.
- Humans are targeted, so training is essential.

Key Controls

Spam Filter

- Blocks spam and malicious emails before delivery.

Data Loss Prevention (DLP)

- Prevents sensitive data from leaving via email.
- Scans email body, headers, attachments for sensitive info.
- Blocks or alerts on suspicious emails.

Email Scanning

- Detects malicious URLs and attachments.
- Uses signatures, blacklists.
- Suspicious emails quarantined and alerts generated.

Security Awareness Training

- Mandatory training on spotting and reporting phishing.
- Includes simulated phishing tests.

Network Security

Overview

- Protects networks and systems from attacks.

Key Controls

Network Intrusion Detection System (NIDS)

- Monitors network traffic and alerts analysts.
- Deployment types:

- Inline (can block traffic, acts like NIPS)
- Network Tap
- Passive (via SPAN port)

Network Intrusion Prevention System (NIPS)

- Like NIDS but can block malicious activity automatically.

Firewalls

- Restrict traffic to create secure network zones.
- Types:

- Hardware firewalls (dedicated)
- Software firewalls (on endpoints)
- Web Application Firewalls (on web servers)

Log Monitoring

- Network device logs sent to SIEM for alerts.
- Examples: Web proxy logs, perimeter firewall logs.

Network Access Control (NAC)

- Prevents rogue or non-compliant devices from accessing network.
- Enforces patching, AV status.
- Used for BYOD and guest networks.
- Examples: WiFi signups at public venues.

AAA: Authentication, Authorization, Accountability

1. Authentication

- Confirms identity.
- Types:

- Something you know (passwords, PINs)
- Something you have (ID badges, keys)
- Something you are (biometrics like fingerprints, face scans)

- Strong security means combining at least two factors = Multi-factor Authentication (MFA).

2. Authorization

- Determines what an authenticated user can do or access.
- Principle of Least Privilege: give users only the access they need, no more.
- Limits damage if accounts are compromised.

3. Accountability

- Tracks user actions for audit and incident investigation.
- Logs show who did what and when.
- Helps determine if an action was legitimate or malicious, and can identify if credentials were stolen or misused.

Why is AAA important?

- Protects sensitive data and systems.
- Limits damage from insider threats or attackers with stolen credentials.
- Enables investigation and response to security incidents.

Networking 101

Networking Fundamentals Overview

Key Protocols:

- TCP (Transmission Control Protocol)

- Connection-oriented protocol at the Transport layer (OSI Layer 4).
- Ensures reliable two-way data transmission with error correction.
- Uses a "three-way handshake" (SYN, SYN-ACK, ACK) to establish connections.
- Works with IP (Internet Protocol), forming the TCP/IP stack foundational for internet communication.
- IP addresses identify devices; ports identify specific applications/processes.
- RFC references: RFC 793 (original), RFC 7323 (latest).

- UDP (User Datagram Protocol)

- Connectionless protocol; sends datagrams without establishing a connection.
- Faster than TCP due to no handshake and no retransmission.
- Uses ports to direct traffic to applications.
- Does not guarantee delivery, order, or data integrity — suitable for applications that can tolerate some loss (e.g., streaming).
- RFC reference: RFC 768.

- ICMP (Internet Control Message Protocol)

- Used for network diagnostics (e.g., ping).
- Helps determine if data reaches the destination timely.
- Operates at the Internet Layer (OSI Layer 3).

Addresses:

- IP Addresses

- Unique identifiers for devices on a network.
- DNS translates domain names (e.g., [www.lifewire.com](http://www.lifewire.com)) into IP addresses.
- Types:

- Private IPs: Used within local networks (ranges: 192.168.x.x, 172.16.x.x–172.31.x.x, 10.x.x.x).
- Public IPs: Assigned by ISPs, used to communicate on the internet.

- Can be Static (manually assigned) or Dynamic (assigned by DHCP).

- MAC Address (Media Access Control)

- Hardware identifier assigned to network interfaces.
- Permanent, unique, represented as six pairs of hexadecimal digits (e.g., 00:0d:83:b1:c0:8e).
- Used at the Data Link Layer (Layer 2) to deliver data within local networks.
- Can be viewed on systems and spoofed by attackers.

OSI Model — The 7 Layers

- Developed by ISO in 1984 to standardize network communication processes.
- Each layer performs specific roles and communicates with the layer above and below it.
- Mnemonics to remember layers:

- Top to Bottom: All People Seem To Need Data Processing
- Bottom to Top: Please Do Not Throw Sausage Pizza Away

|   |   |   |   |
|---|---|---|---|
|Layer No.|Name|Function Summary|User Interaction?|
|7|Application|Interfaces with user apps (browsers, email)|Yes|
|6|Presentation|Data translation, encryption, decryption|No|
|5|Session|Manages sessions (open, close, reset connections)|No|
|4|Transport|Ensures reliable data transfer (error, flow control)|No|
|3|Network|Routes data across networks (IP routing)|No|
|2|Data Link|Frames data, handles physical addressing (MAC)|No|
|1|Physical|Transmits raw bits over physical media (cables)|Yes|

Network Devices

- Router

- Forwards data between networks based on IP addresses.
- Connects home or office networks to the internet.
- Handles domain name resolution via DNS.

- Hub

- Connects devices in a LAN.
- Broadcasts all incoming data to all ports — inefficient and insecure.
- Known as a "dumb" device.

- Switch

- Smarter than a hub; forwards data only to intended device using MAC addresses.
- Uses ARP (Address Resolution Protocol) to map IPs to MACs.
- Reduces unnecessary traffic.

- Bridge

- Connects two separate networks to create one larger network.
- Operates at Data Link Layer (Layer 2).
- Different from routers which keep networks independent.

- Firewall

- Provides network security by filtering incoming/outgoing traffic.
- Can be hardware or software.
- Controls traffic based on set rules.
- Creates private networks by blocking unauthorized access.
- Example: PfSense firewall activity for practical learning.

Network Tools (Basics & Cybersecurity Use Cases)

- IP / ipconfig: Check your device’s IP, gateway, DNS, and routing info. Great for diagnosing network issues.

- Examples:

- ip a — show IP addresses
- ip r list — routing table
- ip link set dev eth0 up — enable interface

- Traceroute / tracert: View the path packets take to a destination, helpful for spotting routing issues.

- Example: traceroute example.com

- Dig / Nslookup: Query DNS records to find IPs or mail servers.

- Examples:

- dig example.com
- dig example.com MX

- Netstat: Monitor active TCP/UDP connections and ports. Good for spotting suspicious connections.

- Examples:

- netstat -a — all connections & listening ports
- netstat -a -b — same + executable names

- Nmap: Powerful network scanner to discover devices, open ports, running services, and even OS info.

- Example for a TCP connect scan with version detection:  
      
    nginx  
    CopyEdit  
    nmap -v -sT -sV scanme.nmap.org
- Use NSE scripts for advanced tasks (network discovery, vulnerability checks) — but that’s more advanced.

- Ethical reminder: Always get permission before scanning networks or hosts! scanme.nmap.org is a safe public target.

Protocols and Ports (Common Services & Their Ports)

- Ports are like doors on a machine that network traffic uses to communicate with services.
- Ranges:

- Well-known: 0-1023 (common services)
- Registered: 1024-49151
- Private/Dynamic: 49152-65535 (client ephemeral ports)

Common Ports & Protocols:

|   |   |   |
|---|---|---|
|Port|Protocol / Service|Notes / Security|
|20, 21|FTP|File transfer, but insecure (cleartext credentials)|
|22|SSH|Secure remote shell, encrypted|
|23|Telnet|Like SSH but insecure, don’t use|
|25|SMTP|Sending email|
|53|DNS|Domain name resolution, TCP/UDP 53|
|67, 68|DHCP|Automatic IP assignment (UDP)|
|80|HTTP|Web traffic, unencrypted|
|443|HTTPS|Secure web traffic with TLS encryption|
|514|Syslog (UDP)|Logs sent to SIEM or monitoring|
|3389|RDP|Windows remote desktop|

Management Principles

Risk

- Risk: Possibility of negative impact (business, financial, security).
- Vulnerability: Weakness that can be exploited.
- Risk Management: Applying controls to reduce risk to an acceptable level.
- Risk Assessments: Identify hazards, who might be harmed, evaluate severity & likelihood, implement controls, review regularly.
- Risk Management Strategies:

- Mitigate (reduce risk)
- Transfer (e.g., insurance)
- Accept (live with it)
- Avoid (eliminate risk)

Policies and Procedures

- Policy: High-level plan or intent guiding actions, outlining roles and responsibilities.
- Examples:

- Acceptable Use Policy (AUP) — defines what users can/cannot do on network.
- Service Level Agreement (SLA) — commitment between service provider and customer.
- Bring Your Own Device (BYOD) — rules for personal device usage.
- Memorandum of Understanding (MOU) — non-binding agreement between parties.

- Standard Operating Procedures (SOP): Step-by-step instructions for routine tasks ensuring consistency and compliance.

Compliance and Frameworks

- Compliance: Following rules, laws, and standards.
- Important because: Legal requirement, reduces risk, builds trust.
- Key frameworks:

- GDPR (EU data protection law)
- ISO 27001 (information security management system)
- PCI DSS (payment card data security)
- HIPAA (healthcare data protection in US)

Change and Patch Management (Not in your test scope but good to know)

- Change Management: Controlled process to document and approve changes in an organization.
- Patch Management: Deploying updates and fixes to software to close security vulnerabilities.
- Tools:

- WSUS (Windows Server Update Services)
- SCCM (System Center Configuration Manager)
- Commercial tools like ManageEngine Patch Manager Plus (multi-OS patching)

Active Directory

What is Active Directory?

- A directory service by Microsoft providing network services for Windows environments.
- Manages authentication, authorization, and resource management.
- Controls who can access files, tools, systems, and settings.
- Supports businesses of all sizes.

Why Use AD?

- Prevents chaos by restricting access based on roles.
- Example: Salespeople get Office, Developers get coding tools.
- Ensures users see only what they need.

Key Features of Active Directory

1. Authentication

- Users log in with accounts provisioned by the organization.
- Supports security features like account lockout on failed logins.

3. Authorization

- Controls access to resources based on permissions and group membership.

5. Centralized Management

- Manage user accounts, computers, printers, and security policies across domains.

7. Group Policy

- Allows centralized setting of security, software installations, desktop configs.

AD Objects & Organizational Units (OUs)

- Object: A digital representation of resources (users, computers, groups, printers, etc.).
- Each object has:

- A GUID: unique, constant ID.
- A Distinguished Name (DN): shows location in AD.
- A class: defines what attributes it can have (e.g., User, Computer).

Common Object Types:

- User Objects: Store usernames, passwords, personal info, group memberships.

- Have a unique Security Identifier (SID).

- Computer Objects: Represent domain-joined computers, have unique SIDs.
- Group Objects: Collections of users/computers.

- Security Groups: Assign permissions.
- Distribution Groups: Email lists, no security permissions.

- Organizational Units (OUs): Containers organizing users, groups, computers, and other OUs.

- Enable delegated admin and apply Group Policies.

- Printer Objects: Network printers with config and permissions.
- Shared Folder Objects: Manage shared resources and permissions.

Security Identifiers (SID)

- Every object has a SID:

- Domain SID: Same for all objects in a domain.
- Relative Identifier (RID): Unique to each object.

- Example:

- Domain SID: S-1-5-21-123456789-987654321-123456789
- User SID: S-1-5-21-123456789-987654321-123456789-1000
- Computer SID: S-1-5-21-123456789-987654321-123456789-1001

Searching AD Objects

- PowerShell:

- Command: Get-ADUser -Identity "NameHere" -Properties * (all properties)
- Can specify particular properties like LastLogonDate, LockedOut, MemberOf, etc.

- LDAP:

- Protocol to access/manage directory services.
- Tools like Softerra LDAP Browser provide GUI to browse/search objects.

Domain Controllers (DCs)

- Servers hosting Active Directory Domain Services (AD DS).
- Responsibilities:

- Authenticate users logging into the domain.
- Authorize access based on permissions/groups.
- Store and provide access to the AD database.
- Apply Group Policies.
- Replicate changes between multiple DCs.

Types of Domain Controllers:

- Primary Domain Controller (PDC):

- Manages password changes, backward compatibility.

- Backup Domain Controller (BDC): (legacy)

- Read-only copies in old Windows NT.

- Read-Only Domain Controller (RODC):

- Read-only AD copy for less secure sites. Can authenticate but not modify.

Active Directory Structures

Single Domain

- One domain with OUs for departments (e.g., HR, Finance, Corporate).

Multi-Domain (Tree/Forest)

- Multiple subdomains (e.g., finance.company.com, engineering.company.com).
- All part of one AD forest.

Multi-Root Domain (Forest)

- Multiple independent domains linked by trust relationships.
- Example: Two companies merged, maintaining separate domains but sharing access.

Security Groups

- Purpose:  
    Group users or other AD objects (like computers) to assign permissions collectively rather than individually.
- Difference from OUs:

- Security Groups: Control access (permissions).
- Organizational Units (OUs): Used for administration (grouping objects, applying Group Policy).

- Naming Conventions (example):

- Prefix: SG- (indicates Security Group)
- Department: IT, HR, Marketing
- Permission Level: ReadOnly, Write, FullAccess
- Location: London, NewYork, etc.

- Example Groups:

- SG-IT-FullAccess-London
- SG-Marketing-ReadOnly-Singapore
- SG-Security-FullAccess-Global

- Use Case:  
    Provide access control to file server folders.  
    Example:

- Create groups: SG-Design-FileServer, SG-HR-FileServer
- Assign users to groups.
- Set folder permissions so only respective groups can access their folders.

Group Policy (GPO)

- Problem solved:  
    Managing security and configuration across many computers and users manually is hard and error-prone.
- What is Group Policy?  
    A collection of rules/settings (in a Group Policy Object - GPO) applied to users/computers to enforce security and configuration centrally.
- Types of GPOs:

1. Local GPO: Applies to a single computer, good for standalone or testing.
2. Non-local GPO: Stored in AD, applied across many users/computers in a domain.
3. Starter GPO: Templates with basic recommended settings, used to create new GPOs faster.

- GPO Processing Order (LSDOU):

1. Local GPO (first)
2. Site-level GPO
3. Domain-level GPO
4. OU-level GPO (from outer to nested OU)

- Conflicts are resolved by last applied wins (lowest-level OU GPO overrides domain-level if conflicting).
- Enforced GPOs override all conflicts regardless of position.

- Creating and Linking GPOs:

- Use Group Policy Management Console (GPMC).
- Create GPO, give it a descriptive name (e.g., CommandLine Logging Enable).
- Edit GPO to configure specific settings.
- Link GPO to domain, OU, or group.
- GPOs refresh every ~90 minutes automatically.

Authentication & Security in AD

Authentication Protocols

1. Kerberos

- Secure, ticket-based authentication system.
- User logs in → requests Ticket Granting Ticket (TGT) from KDC.
- Uses TGT to request service tickets for apps/services without re-entering password.
- Prevents password transmission on the network.

3. NTLM (NT LAN Manager)

- Older challenge-response authentication protocol.
- Server sends a challenge; client encrypts challenge with password hash and returns response.
- Server verifies and grants access if valid.
- Less secure than Kerberos, still used in some legacy systems.

5. LDAP (Lightweight Directory Access Protocol)

- Used for querying and authenticating against AD directory.
- Client sends credentials via bind request.
- Server validates and grants/denies access to resources.

Best Practices for AD Security

- Regular Auditing & Monitoring:  
    Track login attempts, permission changes, unusual activities via event logs.
- Least Privilege Principle:  
    Users only get access necessary for their job, minimizing damage if accounts are compromised.
- Segregation of Duties:  
    Split responsibilities among different people to prevent abuse of power (e.g., one creates accounts, another approves).
- Patch Management:  
    Keep AD servers and related software up-to-date with security patches.