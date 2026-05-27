---
title: Microsoft defender for Endpoint
updated: 2026-05-20 11:14:31Z
created: 2026-04-14 12:28:38Z
---

What combination of tech is used:  
1\. Endpoint behavioral sensors.  
2\. Cloud security analytics.  
3\. Threat intelligence

Advance Hunting:  
where. Filter a table to the subset of rows that satisfy a predicate.  
summarize. Produce a table that aggregates the content of the input table.  
join Merge the rows of two tables to form a new table by matching values of the specified column(s) from each table.  
count. Return the number of records in the input record set.  
top. Return the first N records sorted by the specified columns.  
limit. Return up to the specified number of rows.  
project. Select the columns to include, rename or drop, and insert new computed columns.  
extend. Create calculated columns and append them to the result set.  
makeset(). Return a dynamic (JSON) array of the set of distinct values that Expr takes in the group.  
find. Find rows that match a predicate across a set of tables.

Deploying Endpoint Environment:

Microsoft Defender for Endpoint is available on the following Operating Systems:

Windows  
macOS  
Linux  
Android  
iOS

Onboarding device to defender:

Different ways:  
1\. Group Policy  
2\. Endpoint config manager  
3\. MDM (Intune)  
4\. Local Script  
5\. VDI onboarding  
6\. SCCM

Managing Access:

Using Defender for Endpoint RBAC, we can manage access control over system.

The best practice is create role groups and assign those role grps access to the device groups.

Note: the remediation level is just for AIR's actions and nothing to do with the device group.  
\-Defender AV mode ≠ Defender for Endpoint  
You can have:  
• Defender AV in Passive mode  
• Defender for Endpoint fully active

Windows Security enhancement with MDE

Attack Surface Reduction:

Attack Surface Reduction rules currently support the rules below:

Block executable content from email client and webmail  
Block all Office applications from creating child processes  
Block Office applications from creating executable content  
Block Office applications from injecting code into other processes  
Block JavaScript or VBScript from launching downloaded executable content  
Block execution of potentially obfuscated scripts  
Block Win32 API calls from Office macro  
Use advanced protection against ransomware  
Block credential stealing from the Windows local security authority subsystem (lsass.exe)  
Block process creations originating from PSExec and WMI commands  
Block untrusted and unsigned processes that run from USB  
Block executable files from running unless they meet a prevalence, age, or trusted list criteria  
Block Office communication applications from creating child processes  
Block Adobe Reader from creating child processes  
Block persistence through WMI event subscriptio

Note: If it's an windows platform then use ASR blade  
If its non-windows platform and other platform then use the configuration profiles in Intune.

Performing device Investigation in MDE:

Investigating the device: Go to alert>asset>device and open the device on the device page, you will see all the information needed of the device.

As a response action, you can take the following actions:

BBCC: Behavioral blocking and containment capabilities can help identify and stop threats based on their behaviors and process trees even when the threat has already started. ==Next-generation protection, EDR, and Defender for Endpoint components and features work together in behavioral blocking and containment capabilities.==

Client Behavioral Blocking: Client behavioral blocking is a component of behavioral blocking and containment capabilities in Defender for Endpoint. ==As suspicious behaviors are detected on devices, referred to as clients or endpoints, artifacts, like files or applications are blocked, checked, and remediated automatically.==

Feedback Loop Blocking: When a suspicious behavior or file is detected, such as by Microsoft Defender Antivirus, information about that artifact is sent to multiple classifiers. ==The rapid protection loop engine inspects and correlates the information with other signals to arrive at a decision as to whether to block a file.==

Endpoint detection and response in block mode  
When endpoint detection and response (EDR) in block mode is turned on, Defender for Endpoint blocks malicious artifacts or behaviors that are observed through post-breach protection. EDR in block mode works behind the scenes to remediate malicious artifacts that are detected post-breach.

When EDR in block mode is turned on and a malicious artifact is detected, blocking and remediation actions are taken. You'll see detection status as Blocked or Prevented as completed actions in the Action Center.

Discovery Methods: Discover your onboarded device.  
1.Basic : Passive collection events on network.  
2\. Standard: Active collection of events on network.

```
To onboard device from intune
    a. Make user the intune onboarding is enabled.
    b. 

    a. Once done navigate to Intune>Setup>MDE you should see the connection status to enabled.


    b. 

    a. Now create and EDR policy navigating to EDR blade and "new policy"
    b. 

    a. Followed by Next Gen antivirus policy and then ASR policy for the devices.
```

\*Performing Action on Device using MDE

When investigating a device, we can perform following contamination actions,

Isolate Device

Restrict app execution

Run antivirus scan

And also perform following actions,

Initiate Automated Investigation

Collect investigation package:  
• Autoruns  
• Installed apps  
• Network connections  
• Prefetch files  
• Processes  
• Scheduled task  
• Security event logs  
• Services  
• SMB sessions  
• System info  
• Temp directories  
• Users and Grps  
• WD support logs  
• Summary report

Initiate Live Response Session:  
In order to get the live response following needs to be activasted

1.  Live response must be turned on from advance feature  
    2\. Device must be in a device grp with auto remediation enabled.

\*Performing Evidence and Entity investigation:

```
1. Investigating file
2. Investigating User
3. Investigating IP and Domain
```

\*Configuration and Manage Automation

Configurating Advance Features

# ==Manage Automation Upload: Enable the File Content Analysis capability so that certain files and email attachments can automatically be uploaded to the cloud for more inspection in Automated investigation.==  
==We can manage automation upload of the following==  
==1\. Files==  
==2\. Folder==  
==3\. Extension==  
\==4. File name  
<br/><img src="../../_resources/a49e1c23ca0c63e49770a31dcd48f465.png" alt="a49e1c23ca0c63e49770a31dcd48f465.png" width="462" height="283" class="jop-noMdConv">

Also, we can add an exclusion of the folder we want the AI to exclude.

Automated Investigation and Response

1.  Turn on the Automatically Resolve Alerts option  
    As discussed previously, in order for this feature to work on device, the endpoints should be under device grps and full remediation should be enabled.

Block at risk device:  
Contain a threat by not letting risky devices access your corporate resources through Conditional Access.  
1\. Turn on Intune connection in MDE

```
2. Turn on defender in Intune portal

3. Create a device compliance policy in Intune.
```

Machine Risk score.  
• Clear  
• Low  
• Med  
• High.  
Overall device with high, med and low threats are considers compliant.  
4\. Creating and CAP.  
Need to be sure that when setting the Grant access, we need to select access based only given to device that are compliant.

\*Configure alert and detection MDE

Configure Alert and vuln email notification:

Alerts tuning:

Manage Indicators: Managing IOC.

```
• Vulnerability Management in MDE
```

Real time discover:  
1\. Real time device inventory  
2\. Visibility in software and vuln  
3\. Application runtime context  
4\. Config posture

Intelligence Driven Priotirzation

1.  Exposing emerging attack  
    2\. Pinpoint active breach  
    3\. Protect high value asset

Seamless remediation

1.  Remediation sent to IT  
    2\. Alternate Mitigation  
    3\. Real time remediation status

Vulnerability Management:

&nbsp;

**Summary:**

- **Protect against threat**
- **Deploying MDE**
- **Implement Win 10 : Attack Surface Reduction Rule**
- **Investigation on device**
- **Action on device: Isolate, live remediation, block app from execution, Lice response using advance feature**
- **Investigation evidence Investigation**
- **File investigation: File exclusion in IOC, file page, quarantine file, Submit for analysis.**
- **Automatic device remediation using roles and device groups**
- **Block Device risky device: Connecting to MDE, Device compliance, Conditional access, alert and email notification.**
- **Threat and Vulnerability management: Remediation, Critical path attack, Vuln managment**

&nbsp;