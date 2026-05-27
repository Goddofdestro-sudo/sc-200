---
title: Configuring sentinel Environment
updated: 2026-05-11 10:34:06Z
created: 2026-04-14 12:29:28Z
---

Microsoft Sentinel: SIEM tool to collect, analyse logs to perform operations.

	1. Log Management
	2. Alerting
	3. Visualization
	4. Incident mgmt
	5. Data query
	
How Sentinel works.

1. Data ingestion9Using Data Connectors): Content Hub Solution
	2. Log retention:  After data is ingested, the logs are stored in LAW where we can run KQL.
	3. Workbooks: Data visualization or dashboard
	4. Analytics alert: Using those logs, we can now setup Analytics rule that alerts when suspicious events occur.
- Threat Hunting using KQL
- Incident and Investigation
- Playbooks
	
	
Managing multiple Sentinel workspace or workspace in not in your tenant:

	1. Azure light house :Directory plus subscription selector

	2. 
	3. Sentinel Workspace Manager: Centrally Manage sentinel workspace within one or more tenants.

	4. 
Sentinel Roles: Managed via RBAC
	5. Sentinel Reader: view data, incidents, workbooks, and other Microsoft Sentinel resources.
	6. Sentinel Responder: Above and manage incident
	7. Sentinel Contributor: Above and create and edit analytic rules.
	8. Sentinel automation contributor : Playbooks and Automation rules

Configuring Logs:

Data are in 2 states:
	1. Analytics state :90 days free
	2. Long term retention state: upto 12 yrs

3 Plans for LAW
	1. Analytics Plan: suited for continuous monitoring, real-time detection, and performance analytic
	2. Basic: plan is suited for troubleshooting and incident response
	3. Auxiliary: Low touched data used for auditing and compliance.

Data Tiers

	1. Analytics Tier: Hot state, used for real time analytics
	2. Data Lake : cold state, needed mostly KQL jobs, Analyze over time.
	3. XDR default tire: Retains threat hunting data in XDR by default.
	
	Tables
	4.  Sentinel Tables- security alerts, security incident, watchlist
	5. Common tables: Securityalerts, securityinfo, auditlogs, syslogs
	6. XDR: Device Events, Devicinfo,Emailurlinfo, Emailevents
 

Watchlist in Sentinel:

Data collection from external source for correlation with events in your workspace.
It can be used in search, detection, threat hunting and playbook.
Defender>Configuration>watchlist

Note:
Using KQL in defender and sentinel is different.
Sentinel is like global view, will give you everything
Defender give you logs of XDR and endpoints.

Threat Intelligence in MS sentinel
Integrate Threat intelligence:
	1. Data Connectors
	2. Analytics rule template
	3. Threat intelligence logs 

Integrating sentinel with XDR

	1. Ingesting service data to sentinel
	2. Integrating both into a single portal: using XDR connector in sentinel and onboardings sentinel to XDR.




