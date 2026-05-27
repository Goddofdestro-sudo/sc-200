---
title: Manage Incident using Defender.
updated: 2026-05-11 10:34:06Z
created: 2026-04-14 12:27:52Z
---

Microsoft Defender for Endpoint includes automated investigation and remediation (AIR) capabilities that can help your security operations team address threats more efficiently and effectively.

How the automated investigation starts
When an alert is triggered, a security playbook goes into effect. Depending on the security playbook, an automated investigation can start. For example, suppose a malicious file resides on a device. When that file is detected, an alert is triggered, and the automated investigation process begins. Microsoft Defender for Endpoint checks to see if the malicious file is present on any other devices in the organization. Details from the investigation, including verdicts (Malicious, Suspicious, and No threats found) are available during and after the automated investigation. To learn more about what happens after a verdict is reached, see Automated investigation results and remediation actions.

 Examples of remediation actions include sending a file to quarantine, stopping a service, removing a scheduled task, and more. (See Remediation actions.)
Automation levels in automated investigation
	1. Fully automated
	2. Semi-automated
	3. No-automation.

Action Center and Submission.

Action Center:
	1. Pending: Pending list of ongoing investigation which needs to be approved or rejected.
	2. History: History as an audit log for all the remediation action taken by the AIR.



Advance Hunting: 
	• Query Based Hunt
	• 30 days of Raw Data.
Advanced hunting capability supports queries that check a broader data set from:
	• Microsoft Defender for Endpoint
	• Microsoft Defender for Office 365
	• Microsoft Defender for Cloud Apps
	• Microsoft Defender for Identity
To use advanced hunting, turn on Microsoft Defender XDR.
2 Category.
	1. Event or activity Data: populates tables about alerts, security events, system events, and routine assessments.
	2. Entity Data: populates tables with information about users and devices. This data comes from both relatively static data sources and dynamic sources, such as Active Directory entries and event logs. 

Secure Score: Cloud security posture of the organization
Types of Defender Portal Email:
	1. Incidents 
	2. Threat Analytics
Setting up and Email
Defender>Setting>XDR>Email Notification>(Incident, Action<Threat Analytics)


