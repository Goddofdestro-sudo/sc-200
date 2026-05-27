---
title: Detection and Threat Investigation using Sentinel
updated: 2026-05-11 10:34:06Z
created: 2026-04-14 12:29:42Z
---

Threat detection with Microsoft Sentinel analytics 

Sentinel Analytics: Microsoft Sentinel Analytics provides several functionalities that you can use to implement security for the data and resources at Contoso.

	• Identification of compromised accounts
	• User behavior analysis to detect potentially suspicious patterns
	• Network traffic analysis to locate trends indicating potential attacks
	• Detection of data exfiltration by attackers
	• Detection of insider threats
	• Investigation of incidents
	• Threat hunting

	Types of Analytics rule:
	
	• Anomaly
	• Fusion: Fusion engine co-relates with ML to detect multistage attacks

	• Microsoft security
	• Machine learning (ML) behavior analytics
	• Scheduled alerts : Custom rules
	• NRT (Near Real Time) rules: Rules created for high fidelity and priority alerts. Rather than looking at all logs, I looks at the latest logs to trigger alerts for incident and alert happening in real time.
	• Threat Intelligence


Automation in MS Sentinel:

	1. Automation Rule
	2. Playbook: 
Can be attached to a analytics rule and also an existing incident.

Data Normalization:

ASIM: Advance Security information Model. Normalizes the logs from various sources.

Data collection rule:
	1. Standard: Modern and cirrently being used.
	2. Workspace transformation: Typically when a legacy data connector cannot talk with the new DCR, it acts as a bridge.
	3. 


