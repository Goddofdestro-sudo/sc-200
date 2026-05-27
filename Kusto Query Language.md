---
title: Kusto Query Language
updated: 2026-05-11 10:34:06Z
created: 2026-04-14 12:29:10Z
---

	1. Search Operator:
	Multi table/column search experience.
	2. Where Operator:
	Filters a table to the subset of rows that satisfy a predicate



	What you want to investigate	Table category
	Sign-ins, MFA, Conditional Access	Entra ID (Azure AD) tables
	Security events from Windows	SecurityEvent
	Device telemetry (Defender for Endpoint)	Device* tables
	Emails, phishing, mailflow	Email* tables
	SaaS app activity	CloudAppEvents
	Office 365 logs	OfficeActivity
	Alerts and Incidents	SecurityAlert, Incidents
	Network logs	CommonSecurityLog, AzureDiagnostics
	Anything connected via Syslog	Syslog
	Anything connected via CEF	CommonSecurityLog
	
	Username, hostname	string
	Event ID, count	int
	Big number / size	long
	Percentage / score	real
	List / JSON / Entities	dynamic
	
	
	Operators:
	1. Where : queries a tables and only keeps rows that satisfy the condition.
	SecurityAlert
	| where AlertSeverity contains "high"
	|where Entities contains "hostname"
	
	2. Let: you define something beforehand and then use it.
let TimeRange = 10d;
SecurityAlert
|where TimeGenerated > ago(TimeRange)
|where AlertSeverity == "High"

	3. Extend operator
The extend operator will create calculated columns and append the new columns to the result set.

	4. Order by: result in the way you want to order.

	let TimeRange = 10d;
	SecurityAlert
	|where TimeGenerated > ago(TimeRange)
	|where AlertSeverity == "High"
	|order by AlertName asc 
	
	5. Summarize
arg_max function & arg_min function : Return top and bottom row.
	
	Make_function return a dynamixc array.
	
	Make_list()
	Make_set()
	
	



