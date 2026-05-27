---
title: Microsoft Defender XDR
updated: 2026-05-11 10:34:06Z
created: 2026-04-14 12:27:32Z
---

Defender XDR: Unified threat protection solution.



Microsoft Graph:
Microsoft Graph exposes REST APIs and client libraries to access data(read and Write) on the following Microsoft cloud services: (One for all).
	Microsoft 365 core services: Bookings, Calendar, Delve, Excel, Microsoft Purview eDiscovery, Microsoft Search, OneDrive, OneNote, Outlook/Exchange, People (Outlook contacts), Planner, SharePoint, Teams, To Do, Viva Insights
	Enterprise Mobility + Security services: Advanced Threat Analytics, Advanced Threat Protection, Microsoft Entra ID, Identity Manager, and Intune
	Windows services: activities, devices, notifications, Universal Print
	Dynamics 365 Business Central services

MS Graph Security API: 

Primary ingestion (bulk logs)
	This is Sentinel’s main diet 🍽️
• Entra ID sign-in logs
• Audit logs
• Defender logs
• O365 logs
➡️ Via native connectors → Log Analytics → KQL
🔹 Secondary ingestion (security objects)
This is where Graph fits 🎯
• Incidents
• Alerts
• Threat indicators
• Investigation metadata
➡️ Via Microsoft Graph Security API
These are not raw logs, but security conclusions made by Microsoft products.
Q: Why not just use primary ingestion and leave secondary ingestion.

- Primary ingestion contains raw logs and telemetry, while Microsoft Graph Security API provides processed, correlated security information that is used to speed up investigation and response.
	
Blast Radius Analysis:

Blast radius analysis extends the incident graph with an advanced, interactive view of both the current impact of a breach (post‑breach) and the potential future impact (pre‑breach) in one consolidated graph.

Utilizes sentinel graph and requires onboarding  of sentinel data lake.

Automated Investigation and Response (AIR):The technology in automated investigation uses various inspection algorithms and is based on processes that are used by security analysts. AIR capabilities are designed to examine alerts and take immediate action to resolve breaches. AIR capabilities significantly reduce alert volume, allowing security operations to focus on more sophisticated threats and other high-value initiatives

	1. Full
	2. Semi
	3. No AR (Manual)

Threat Analytics:

Threat analytics is a threat intelligence solution from expert Microsoft security researchers. It's designed to assist security teams to be as efficient as possible while facing emerging threats, such as:
	Active threat actors and their campaigns
	Popular and new attack techniques
	Critical vulnerabilities
	Common attack surfaces
	Prevalent malware
	
Email Notification XDR Alerts and Incident,



Microsoft Defender for O365

Automated Rules:
They automate the assignment of tags, grouping, or incident handling rules, based on predefined logic you create.
Playbook(AIR): 
Playbooks perform actions, often including remediation tasks.
	1. AIR
	2. Sentinel/Logic Playbooks

a. Anti Phishing Policy:
		○ Phishing Threshold
		○  Domain Impersonation
		○ Trusteed impersonation sender and Domain
		○ Mailbox Intelligence 
		○ Spoof Intelligence
	
	1. Anti-Spam Email
	• Bulk email Threshold
	• SPF hard fail
	• Allowed sender and domain list.

	2. Anti-malware
	• Custom file types
	• Zero auto Purge
	• Custom notification

	a. Safe attachment
	• For Safe attachment detection response
	Off, Block, Monitor, Replace, Dynamic Delivery
	• Redirect the email.

	a. Safe Links
	• Rewrite the link on the email or message
	• Real time URL scanning
	• Options to bypass the email.
	• Track user click

*Manage Microsoft Entra Identity Protection


Risk detection type	Description
Anonymous IP address	Sign in from an anonymous IP address (for example: Tor browser, anonymizer VPNs).
Atypical travel	Sign in from an atypical location based on the user's recent sign ins.
Malware-linked IP address	Sign in from a malware-linked IP address.
Unfamiliar sign in properties	Sign in with properties we've not seen recently for the given user.
Leaked credentials	Indicates that the user's valid credentials have been leaked.
Password spray	Indicates that multiple usernames are being attacked using common passwords in a unified brute-force manner.
Microsoft Entra threat intelligence	Microsoft's internal and external threat intelligence sources have identified a known attack pattern.
New country	This detection is discovered by Microsoft Defender for Cloud Apps (MDCA).
Activity from anonymous IP address	This detection is discovered by MDCA.
Suspicious inbox forwarding	This detection is discovered by MDCA.

	Sign in risk Policy : The sign-in risk policy detects suspicious actions that come along with the sign-in.
	User risk policy: The user risk policy detects the probability that a user account has been compromised by detecting risk events that are atypical of a user's behavior.

	
	

User risk policy threshold to High and the sign-in risk policy to Medium and higher.
	
	*Self-remediation with risk policy: If you allow users to self-remediate, with multifactor authentication (MFA) and self-service password reset (SSPR) in your risk policies, they can unblock themselves when risk is detected. These detections are then considered closed. Users must have previously registered for MFA and SSPR in order to use when risk is detected.
	
	A workload identity is an identity that allows an application or service principal access to resources, sometimes in the context of a user. These workload identities differ from traditional user accounts as they:
		Can’t perform multifactor authentication.
		Often have no formal lifecycle process.
		Need to store their credentials or secrets somewhere.
		
	MS defender for Identity:

	
	1. M365 Defender: Cloud service running on Azure. Signals from Endpoint, O365 and cloud apps.
	2. Defender for Identity sensor: Installed on DC or ADFS
	3. Defender for Identity portal: Identity instance, data received from Defender for identity sensors, manage, monitor and investigate threats.

*Defender for Identity: For hybrid 
*Microsoft Entra ID Protection: For cloud native only.

Note: About Radius Server
Intune → provisions device + cert
CA     → issues cert
RADIUS → validates cert & enforces access
AD / Entra ID → identity authority

Device (certificate / credentials)
   │
Network Access Device (Wi-Fi AP / VPN)
   │
RADIUS Server (NPS / cloud RADIUS)
   │
Identity Store (AD / Entra ID / CA)
   │
Network access granted / denied

-Securing cloud apps and services with Microsoft defender for cloud apps
Microsoft Defender for Cloud Apps is a CASB that helps you identify and combat cyberthreats across Microsoft and third-party cloud services. Microsoft Defender for Cloud Apps integrates with Microsoft solutions, providing simple deployment, centralized management, and innovative automation capabilities


4 elements of MDCA
1 .Discover and control the use of shadow IT
	2. Protect anywhere in the cloud
	3. Protect against cyber threats and anomalies
	4. Access compliance of your cloud.

Conditional Access App control:
Conditional Access App Control lets you monitor and control user app access and sessions in real time. By integrating with Microsoft Entra Conditional Access, it's easy to configure apps to work with Conditional Access App Control. It lets you selectively enforce access and session controls on your organization's apps based on any condition in Conditional Access. 



DATA Loss Prevention: Preventing data exfiltration
Data Label: Public, Internal, Confidential, Highly confidential
DLP can enforce policies based on these labels
- DLP policies  will provide you low and high volume option to manage.
	1. Using Labels (Classification based DLP)
	2. Sensitive Info types (Content based DLP)

Insider risk management:
Pain Points:
	1. Leak of data
	2. Confidentiality violation
	3. IP theft
	4. Fraud 
	5. Insider trading
	6. Compliance violation.

Principle: Transparency, Configurable, Integrated, Actionable






DEFENDER FOR CLOUD APPS: MCASB (Cloud apps security broker): log connect, API connector, Reverse Proxy.

What can it do: 
	1. Discover cloud apps, Iaas and Paas services.
	2. Classify and protect information
	3. Detect unusual behavior in apps
	4. Asses compliance of cloud apps.

	5. 
	
Apps discover:
• Automatic detection → via traffic logs (Cloud Discovery)
•  Manual connection → for advanced monitoring and control (API connectors)


	
	




	

