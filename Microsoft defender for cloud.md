---
title: Microsoft defender for cloud.
updated: 2026-05-22 22:33:15Z
created: 2026-04-14 12:28:54Z
---

CSPM: Cloud Security Posture Management

Cloud workload protection:

```
1. Servers
2. App services
3. Storages
4. Database
5. Containers
6. Key Vault
7. Resource Manager
8. API's
9. SQL Servers
```

Not only limiting to that, MDC can defend your hybrid environment too.

```
1. Non-azure servers
2. Multi cloud machines.
```

Defender for Cloud is a tool for security posture management and threat protection. It strengthens the security posture of your cloud resources, and with its integrated Microsoft Defender plans, Defender for Cloud protects workloads running in Azure, hybrid, and other cloud platforms.

It fills the 3 vital needs.

```
1. Continuously Asses
2. Secure
3. Defend
```

Tools MDC provides,  
1.Secure Score  
2\. Security Reco  
3\. Security Alerts.

For MDC to secure your Paas. You will simply need to turn on the defender for cloud plan and then it will automatically start covering the cloud infra. Note: When onboarding no LAW is required as MS has native visibility.

Except for Azure VM, servers and non-azure VM, we will need to on board it via Azure Ark.  
Note: When onboarding we will need to create a LAW as it needs logs to be feed.

\*Connect Azure assets to Microsoft Defender for Cloud

Asset Inventory:

Auto Provisioning:

Data collection is only needed for compute resources (VMs, virtual machine scale sets, IaaS containers, and non-Azure computers).

Data collection using:

```
1. Azure monitor agent
2. MDE
3. Log analytics agent
4. Security extension


5. Auto provisioning :Defender for Endpoint integration is enabled by default when you enable a Defender for Servers plan
```

In Defender for Cloud, select Environment settings and select the subscription containing the machines on which you want to deploy the Defender for Endpoint integration.  
In Settings and monitoring > Endpoint protection, toggle the Status column settings to On.  
Select Continue and Save to save your settings.  
The Defender for Endpoint sensor is deployed to all Windows and Linux machines in the selected subscription.

```
2. Direct onboarding: using Microsoft defnender for endpoint agent

To enable direct onboarding:
In Defender for Cloud, go to Environment Settings > Direct onboarding.
Switch the Direct onboarding toggle to On.
Select the subscription you want to use for servers onboarded directly with Defender for Endpoint.
Select Save.
```

Manual Agent provisioning

Azure Monitor Agent: Azure Monitor Agent (AMA) is the recommended modern agent for collecting data from virtual machines. Unlike the legacy Log Analytics agent, AMA uses Data Collection Rules (DCRs) to specify what data to collect and where to send it.

==Onboarding VM/server and enabling AMA and ingesting it to LAW==  
==• Create Azure VM or install Azure Arc agent (for non‑Azure server)==  
==• Server becomes visible in Defender for Cloud (onboarded)==  
==• Create or select Log Analytics Workspace (LAW)==  
==• Create Data Collection Rule (DCR)==  
==• Associate DCR to VM / Arc server==  
==• Azure Monitor Agent (AMA) auto‑installs==  
==• Logs start flowing to LAW==  
==• Create Log Analytics / Sentinel analytics rules for alerts==  
==• (Optional) Enable Defender for Servers (P1/P2) for built‑in security alerts==

Simply enabling Defender for Cloud plans at the subscription level will protect native Azure services.  
You do not have to manually onboard those resources or create a workspace first for that coverage.  
Only for extended telemetry, advanced security logs, and server-level insights do workspaces and agents matter — but that’s separate from basic resource coverage.

\*Connecting Non-azure resource using MDC

Azure arc allows to manage following resource  
1\. Servers  
2\. Kubernetes Clusters  
3\. Azure Data services  
4\. SQL servers

Azure Arc enabled servers: To deliver this experience with your hybrid machines hosted outside of Azure, the Azure Connected Machine agent needs to be installed on each machine that you plan on connecting to Azure. This agent doesn't replace the Azure Monitor Agent  
Supported Cloud operation.  
1\. Govern  
2\. Protect  
3\. Configure  
4\. Monitor

\*Managing Your Cloud Security Posture Management

Security Policy: An Azure Policy definition, created in Azure Policy, is a rule about specific security conditions that you want controlled. Built in definitions include things like controlling what type of resources can be deployed or enforcing the use of tags on all resources. You can also create your own custom policy definitions.

Security Initative: An Azure Policy initiative is a collection of Azure Policy definitions, or rules that are grouped together towards a specific goal or purpose. Azure initiatives simplify management of your policies by grouping a set of policies together, logically, as a single item.

Security Recommendation: Defender for Cloud makes its security recommendations based on your chosen initiatives. When a policy from your initiative is compared against your resources and finds one or more that aren't compliant, it's presented as a recommendation in Defender for Cloud.

Secure Score:

\*Cloud Workload Protection:

```
1. Defender for App Services:
```

Microsoft Defender for App Service uses the scale of the cloud to identify attacks targeting applications running over App Service  
• Detects attacks like:  
• SQL injection  
• Command injection  
• Watches app behaviour  
2\. Defender for Storage: Protects Blob storage and file shares.  
Detects:  
• Malware uploaded  
• Data exfiltration  
• Anonymous access abuse  
Also, it doesn't scan the files but scans the file has of the newly uploaded file and match with the known hash of virus, torjan, spyware and ransomeware.

3.  Defender for SQL: Azure SQL DB and SQL servers  
    • Detects:  
    • SQL injection  
    • Brute-force logins  
    • Abnormal queries  
    • Flags misconfigurations  
    2 main benefit  
    Vuln assesment and advance threat protection
    
4.  Defender for Open-Source Databases: MySQL, PostgreSQL, MariaDB  
    • Suspicious logins  
    • Abnormal queries  
    • Misconfigurations
    
5.  Microsoft Defender for Key Vault: Secret, Keys and Certificates  
    • Unusual secret access  
    • Access from risky locations  
    • Credential misuse
    
6.  Microsoft Defender for Resource Manager: Azure control plane (ARM)  
    • Suspicious deployments  
    • Privilege escalation  
    • Risky template changes
    
7.  Microsoft Defender for DNS: DNS queries  
    • Communication with malicious domains  
    • Command-and-control traffic
    
8.  Microsoft Defender for Containers: Kubernetes and Container Images  
    • Scans container images  
    • Detects runtime attacks  
    • Flags risky configs
    
9.  Defender for Additional Protection  
    • Threat protection for Azrue Cosmos DB  
    • WAF alerts  
    • DDOs proetection
    

• Remediate security Alerts using MDC  
How threats are detected:

1.  Threat Intelligence
2.  Behavioural analytics
3.  Anamoly detection