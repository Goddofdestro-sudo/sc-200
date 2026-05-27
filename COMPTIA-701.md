---
title: COMPTIA-701
updated: 2026-05-11 10:34:06Z
created: 2026-04-14 12:35:56Z
---

Section 4: Physical Security

1. Fencing:

-Bollards

-Fences

1. Brute Force:

Forcible entry

● Tampering with security devices

● Confronting security personnel

● Ramming a barrier with a vehicle

1. Surveillance Systems

Video

Security

Light

Sensor

1. Access control

Double door system: Open one door at a time

Piggybacking:

Involves two people working together with one person who has

legitimate access intentionally allows another person who doesn't have

proper authorization to enter a secure area with them

Tailgating:

Occurs whenever an unauthorized person closely follows someone

through the access control vestibule who has legitimate access into the secure space.

1. Bypassing Surveillance Systems  
    1. Visual Obstruction.
2. Blinding sensor and cameras
3. Interfering with Electromagnetic
4. Attacking the Physical Environment

Biometrics Challenge:

1. False Acceptance Rate: Giving access even though it should not have given.
2. False rejection Rate: Denise access to an authorized user.
3. Cross over Error Rate. Balance between FAR and FRR.

          Access Badge Cloning

4. Scan
5. Extract
6. Copy and clone
7. Use

Stop Access Cloning:

1. 2FA
2. Shield wallets
3. Update security protocol
4. Advance encryption tech

Section 5 : Social Engineering:

Manipulative strategy exploiting human psychology for unauthorized access to

systems, data, or physical spaces.

Motivational Trigger:

1. Authority
2. Urgency
3. Scarcity
4. Fear
5. Likability
6. Social Proof.

Impersonation:

1. Impersonation
2. Brand Impression
3. Typo Squatting: URL Hijacking ( Using similar domain name but some words are misplaced)
4. Water Hole Attack ( Attackers compromise a specific

website or service that their target is known to use)

Pre -Texting: Giving some info that seems true so that the victim will give the information.

Phishing Attack:

1. Phishing
2. Spear-Phishing
3. Whaling
4. Business Email Compromise
5. Vishing
6. Smishing

Preventing Phishing Attack:

1. Anti Phishing Campaign.
2. Security Awareness training.

Key Indicators for Phishing attack:

1. Urgency
2. Mismatched spelling or URL
3. Unusual request.
4. Strange email address.

Frauds and Scam:

1. Identity Fraud: Using a person's information without their consent.
2. Identity Theft: Using another person's identity and using as their own.

Scams: Fraudulent or deceptive act or operation

1. Invoice  scam
2. Scam Calls.

Influence Campaigns:

1. Misinformation
2. Disinformation  
     

Other Social Engineering tech:

1. Hoaxes
2. Shoulder surfing
3. Dumpster Diving
4. Baiting
5. Eaves dropping

Section 6 Malware:

Malicious software that infiltrate computer system and damage it without the users consent.

Malwares:

1. Virus: code/script that will execute when there is a user interaction but the user is unaware about the execution. It will infect the system and computer when executed.  
     
2. Worms: Malicious software  that can replicate without user interaction. It will self-replicate and spread throughout the system and network. Will take advantage of vulnerability.

3. Affect workstation and asset
4. Affect network.

5. Trojans: Malicious software that looks harmless but will exploit the system vul and perform data exfiltration. Will create backdoor to maintain access to the system.

6. Spyware: Unwanted software that is installed on the system without user consent and knowledge. It will infiltrate data from the system.  
    Bloatware: Any software that comes pre-installed on a new computer or smartphone that

         you, as the user, did not specifically request, want, or need.

7. Ransomware: Malicious software that blocks the access of the data or system by encrypting them and until the ransom is paid, they will no release it.

How to prevent from ransomware:

1. Regular backup
2. Regular security update.
3. 2MFA

4. Rootkits: Software that design to gain admin access on a system.  
    Ring 3: Outermost Ring- General user access

Ring 0: Inner ring- Admin access/Kernel mode

1. Spam
2. Zombie and Botnets: Network or system that has been compromised and is used as a pawn to conduct Malicious activities. Botnets are combination of numbers of Zombie systems.

Most common use of Botnets is to conduct DOS or DDOS.

1. Backdoors and Logics Bombs:  
    Backdoor: Used to bypass the normal security and authentication functions. Developers and designers often put this in the program or software.

Easter Eggs: Used as a GAG for the users. Sometimes this can be vulnerabilities.  
 

Logics Bomb:  Codes that has malicious intent, which will execute when certain conditions has met. It is also considered as evolved easter egg.

1. Key Loggers: Software or hardware that will record every single keystroke. Mostly used to gain information or credentials. Types,  
    1. Software Keyloggers:  
    2. Hardware Keyloggers:

Malware Techniques:

Most modern malware uses fileless techniques to avoid detection by

signature-based security software.

When user accidently clicks on a malicious, the process where the file gets installed is called Dropper or Downloader.

Dropper: Malware type design to initiate or run other malware forms within a payload on an infected host.

Downloader: Retrieves additional tools post the initial infection triggered.

2nd stage: Now it will download RAT which will give the attacker access to the system.

3rd: Concealment: Method to hiding their tracks like erasing log files.

1. Code Injection
2. Masquerading
3. DLL injection
4. DLL sideloading
5. Process Hollowing

Indications of Malware Attacks.

1. Account lockout.
2. Resource Inaccessibility.
3. Missing Logs
4. Impossible Travel.
5. Resource Consumptions.
6. Blocked Content.

Section:7 Data Protection

1. Data Classification.

2. Sensitive
3. Confidential
4. Critical
5. Public
6. Restricted
7. Private

Data Ownership:

1. Data owner : Maintains the CIA and P of the data.
2. Data controller: Entity responsible for determining data storage, collection, and usage purposes

and methods, as well as ensuring the legality of these processes

1. Data processor: Individual responsible for processing and collection of the information after extraction.
2. Data steward: Who works with the owner to maintain labels and appropriate criteria to be maintained. Works under data owner.
3. Data custodian:

Responsible for managing the systems on which data assets are stored, including

enforcing access controls, encryption, and backup measures

1. Privacy Officer:

Oversees privacy-related data, such as personally identifiable information (PII),

sensitive personal information (SPI), or protected health information (PHI),

Data Ownership Responsibility:

Owners should be individuals from the business side who understand the data's

content and can make informed decisions about classification.

Data States:

1. Data at rest: When data is being stored in storage, file system or any form of storage. When rested, data is usually encrypted.

Encryption method.

1. Full Enc
2. Partition Enc
3. Volume Enc
4. File Enc
5. Database Enc
6. Records Enc

7. Data at transit: Data actively moving.

Transport Encryption Methods.

1. SSL
2. VPN
3. IPsec: Secures IP communications by authenticating and encrypting IP

Packets

1. Data at use: Data actively being created, retrieved, updated, or deleted.

2. Encryption at application Level: Encrypt during processing.
3. Access Control:
4. Secure Enclaves: A isolated environment to process sensitive/critical data.
5. INTEL Software Guard: Encrypt data at memory to stop unauthorized access.

Data Types:

1. Regulated Data: Controlled by laws, regulation and industry standard. Compliance requirement.
2. Personal Identification Information.: Information used to identify and individual.
3. Personal Health Information:  Information about health status, healthcare provision, or payment linked to a

specific individual

1. Intellectual Property: Creations of the mind (e.g., inventions, literary works, designs).Protected by patents, copyrights, trademarks to encourage innovation
2. Legal Information: Data related to legal proceedings, contracts, regulatory compliance.
3. Financial Information: Data related to financial transactions (e.g., sales records, tax documents, bank

statements).

1. Human-Readable Data: Understandable directly by humans (e.g., text documents, spreadsheets).
2. Non-human Readable Data: Requires machine or software to interpret (e.g., binary code, machine language)

Data Sovereignty: Laws on how digital information are collected and processed. Each country or nation has their own law.

1. General Data protection Regulation: EU

Geographical Restriction: Data has to be stored and processed within the respective country. China and Russia has that law where data has to be within the country. Will bring headache to International organisation.

Securing Data: How data can be secured.

1. Geo Restriction: Virtual geo boundary created.
2. Encryption: Encrypting data or mask.
3. Hashing: Converts data into fixed-size hash values. Irreversible one-way function and mostly used for password storage.
4. Masking: Some or all data is concealed with X. Some data is revealed for data analysis.
5. Tokenization: Replace sensitive data with non-sensitive tokens. Original data stored securely in a separate database. Mostly used for payment processing.
6. Obfuscation: Making data unclear or unintelligible so that unauthorized personal will have hard time understanding it.

7. Segmentation: Divide network into separate segments with unique security controls .Prevent lateral movement in case of a breach. Limits potential damage.
8. Permission Restriction: Restriction based access control.

Data loss prevention (DLP): Aims to monitor data in use, in transit, or at rest to detect and prevent data theft.

Types of DLP system which are hardware or software based.

1. Endpoint DLP: Installed as software on workstations or laptops. Can prevent or alert on file transfers based on predefined rules.
2. Network DLP: Software or hardware placed at the network perimeter. Focuses on monitoring data entering and leaving the network.

|   |   |
|---|---|
|Mostly focused on data leaving the network.||

1. Storage DLP: Installed on a server in the data centre. Inspects data at rest, especially encrypted or watermarked data. Monitors data access patterns and flags policy violations.
2. Cloud based DLP: SAS and part of cloud service and storage need. Protects data stored in cloud services.

Section 9: Risk Management

Risk Management:  Fundamental process involving identification, analysis, treatment, monitoring,

and reporting of risks

Risk management lifecycle:

1. Risk Identification: Involves recognizing potential risks that could impact an organization.

Techniques.  
 

- Brainstorming
- Checklists
- Interviews
- Scenario Analysis

Business Impact Analyisis: Evaluates effects of disruptions on business functions. Assesses impact of risk on functions.

Key Metrics:  
1. RTO: Recovery time objective: Time till impact.

2.RPO: Recovery Point Objective: Acceptable amount of data loss

1. MTTR: Mean time to Repair: Time to repair the system
2. MTBF: Mean time between Failure: Time bewteen system and component failure.

3. Risk Analysis:
4. Risk Treatment
5. Risk Monitoring
6. Risk Reporting

Risk Assessment Frequency: Regularity at which risk assessment is conducted.

1. Ad-hoc: Conducted as needed, often in response to specific events or situations.
2. Recurring: Conducted at regular intervals (e.g., annually, quarterly, monthly).
3. One time: Conducted for specific projects or initiatives.
4. Continuous: Ongoing monitoring and evaluation of risks. Enabled by technology, involving real-time data collection and analysis.

Used for proactive threat and vulnerability monitoring, facilitating quick

Responses.

Risk Register: details of identified risk including their  descriptions, impact, likelihood , outcome and level of risk.

1. Risk Description.
2. Risk Impact
3. Risk Likelihood
4. Risk outcome
5. Risk Level.
6. Risk cost

Risk Tolerance and Risk Appetite:  An organization or individual’s willingness to deal with uncertainty in

pursuit of their goals. Maximum amount of risk they are willing to accept.

Key Risk Indicators: Predictive metrics signalling increasing risk exposure. Provide early warning of potential risks. Used to monitor risk changes and take proactive steps.

Risk Owners: Responsible for managing the risk. Monitors, implements mitigation actions, and updates Risk Register.

2 types of Risk analysis:

1. Qualitative Risk Analysis: Assesses risks based on potential impact and likelihood. Subjective and relies on expertise and experience. Categorizes risk as high, medium or low.

It is mostly based on the likelihood of the risk and the level of its impact.

1. Low Impact: Minor damage.
2. Medium Impact: Damage of assets.
3. High Impact. Disruption of function.

4. Quantitative Risk Analysis: Objective and numerical evaluation of risks. Used for financial, safety, and scheduling decisions.

Key Components:

Exposure Factor: Proportion of asset lost in an event (0% to 100%).

Single Loss Expectancy: Monetary value expected to be lost in a single event. Asset Value x Exposure Factor.

Annualized Rate of Occurrence (ARO): Estimated frequency of threat occurrence within a year.

Annualized Loss Expectancy (ALE): Expected annual loss from a risk. Calculated as SLE x ARO.

Risk Management and Strategies:

Four strategies:

1. Transferring: Example is Insurance.
2. Avoidance: Change plans or strategies to eliminate a specific risk. Chosen when the risk is too great to accept or transfer.
3. Acceptance: Accept the risk when the cost of managing the risk outweighs potential loss or risk.
4. Mitigation: Take steps to reduce likelihood or impact of risk.

Risk Monitoring and Reporting:

1. Tracking identified risks.
2. Monitoring residual risks.
3. Identifying new risks.
4. Evaluating risk response plans.

Risk Reporting:

Communicating information about risk management activities to stakeholders. Includes results of risk identification, assessment, response, and monitoring. Often presented in the form of a risk report.

They are important for,

1. Informed decision making
2. Risk mitigation
3. Stakeholder communication
4. Regulatory compliance

Third Party Vendor Risk: Potential security and operational challenges from external collaborators.

Threat Vectors

● Paths attackers use to gain access

Attack Surfaces

● Points where an unauthorized user can try to enter

Various Types of Vulnerabilities

Hardware Vulnerabilities

● Components with vulnerabilities

Software Vulnerabilities

● Applications with hidden backdoors

Operational Vulnerabilities

● Lack of cybersecurity protocols

Supply Chain Risk:

1. Hardware Manufactures:
2. After Market Sources.
3. Software Developers:
4. MSP: Security challenges with Software-as-a-Service (SaaS) providers.

5. Data confidentiality and integrity concerns

6. Assess provider's cybersecurity protocols and support for security

incidents

1.  Vendor selection should consider due diligence, historical performance,

and commitment to security

Supply Chain Attacks: An attack that targets a weaker link in the supply chain to gain access to a

primary target.

Safeguarding Against Supply Chain Attacks:

1. Vendor Due Diligence.
2. Regular Monitoring & Audits
3. Education and Collaboration
4. Incorporating Contractual Safeguards

Vendor Assessment: Process to evaluate the security, reliability, and performance of external entities. Crucial due to interconnectivity and potential impact on multiple businesses.

Vendors

Suppliers

MSP

1. Pen test on Suppliers
2. Right to Audit Clause
3. Internal Audit
4. Independent Assessment
5. Supply chain analysis

Vendor Selection and Monitoring:

Vendor Selection: A rigorous evaluation that goes beyond surface-level credentials. Check for conflicts of interest that could bias the selection process.

Vendor Questionnaires: Comprehensive documents filled out by potential vendors.

Rules of Engagement: Guidelines for interaction between organization and vendors. Cover communication protocols, data sharing, and negotiation boundaries.

Vendor Monitoring: Mechanism used to ensure that the chosen vendor still aligns with organizational

needs and standards.

Contracts and Agreement:  
 

1. Basic Contracts
2. Service Level Agreement
3. Memorandum of Agreement. Outline responsibilities of the involved parties.
4. Non-Disclosure Agreement:

Ensures confidentiality of sensitive information shared during

Negotiations.

1. Business Partnership Agreement (BPA) or Joint Venture Agreement (JV): Goes beyond basic contracts when two entities collaborate.

Outlines partnership nature, profit-sharing, decision-making, and exit

Strategies.

Governance and Compliance:

Governance: Overall management of IT infrastructure, policies, procedures, and operations

Crucial Aspect:

   Risk Management

○ Identify, assess, and manage potential risks

   Strategic Alignment

○ Ensure IT strategy aligns with business objectives

  Resource Management

○ Efficient and effective use of IT resources

●Performance Measurement

○ Mechanisms for measuring and monitoring the performance of IT

Processes

Compliance: Adherence to laws, regulations, standards, and policies.

    Legal Obligations

○ Non-compliance leads to penalties (fines, sanctions)

   Trust and Reputation

○ Compliance enhances reputation and fosters trust

   Data Protection

○ Prevents breaches and protects privacy

  Business Continuity

○ Ensures operation in disasters or disruptions

Governance Structure:

1. Boards and Committee.
2. Govt entities

Policies: High-level guidelines indicating organizational commitments.  
 

Acceptable Use Policies

● Information Security Policies

● Business Continuity

● Disaster Recovery

● Incident Response

● Change Management

● Software Development Lifecycle (SDLC

Standards: Specific, mandatory actions or rules adhering to policies.

   Password Standards

● Access Control Standards

● Physical Security Standards

● Encryption Standards

Procedures

■ Step-by-step instructions ensure consistency and compliance

■ Covered Procedures

● Change Management Procedures

● Onboarding and Offboarding Procedures

● Playbooks

Compliance Coverage

■ Monitoring and Reporting

● Concepts like due diligence, due care, attestation, and acknowledgment

■ Internal and External Compliance

● Differentiating factors

■ Automation in Compliance

● Utilizing automation in the compliance process

Governance Considerations:

1. Regulatory Considerations
2. Legal Considerations
3. Industry
4. Geographical.

Compliance: Ensures adherence to laws, regulations, guidelines, and specifications. Includes compliance reporting and compliance monitoring

Compliance Reporting:

1. Internal compliance reporting: conducted by internal audit team and adhering to internal policies, rules and guidelines.
2. External compliance Reporting: Conducted by an external auditors and bounded by law or contract.

Consequences of Non-compliance

■ Fines, Sanctions

● Legal penalties

■ Reputational Damage

   Loss of license

● Impact on trust and reputation

Asset and Change Management:

Assest Management:

Systematic process of developing, operating, maintaining, and selling assets

cost-effectively.

1. Tangible Assets: Office buildings/computers/machine
2. Non-Tangible Assets: IP, reputation

3. Assignment and accounting of assets
4. Classification and categorization
5. Monitoring and tracking

- Asset Monitoring
- Asset Tracking
- Enumeration

Mobile Device Management:  Centralizes management, enforces corporate policies, ensures software

uniformity, safeguards sensitive data.

Asset Disposal and Decommissioning: Necessity to manage the disposal of outdated assets.

-Destruction.

-Certification.

-Data Retention.

-Data Protection.

Change management:

Orchestrated strategy to transition teams, departments, and organizations from

existing state to a more desirable future state.

Change Approval and Assessment:

1. Changes must be approved and assessed.
2. Organizational processes and procedures for change approval.
3. Change Advisory Board (CAB).

4. Change Owner
5. Stakeholder
6. Impact Analysis

Change Management Process 5 steps:

1. Preparing Change.
2. Creating the vision.
3. Implementing the Change.
4. Verifying the Change.
5. Documenting the Change.

Key aspects:

1. Schedule a maintenance window.
2. Back out plan.
3. Testing the result.
4. SOP( Standard Operation Procedure) Step by step

Audit and Assesment:

Audit: Systematic evaluations of an organization's information systems, applications,

and security controls.

1. Internal audit.
2. External audit.

Significance of Audits:

Identifying gaps: Security policies, procedures, and controls

1. Security policies, procedures, and controls: GPR, HIPAA, PCI DSS.

Internal Audits: Systematic evaluations conducted by an organization's own audit team.

Focus areas may include ● Data protection ● Network security ● Access controls ● Incident response procedures

Process:

1. Review Policies and process
2. Exam access right
3. Testing effectiveness of controls.
4. Findings documented for recommendations and improvements.

Compliance: Ensuring adherence to established standards, regulations, and laws.

Audit Committee

Internal Assessment: Proactive evaluation of an organization's security posture.

Using a sample checklist: Organization's governance ● Risk ● Compliance practices

Minnesota Counties Intergovernmental Trust : Check list helps to minimize data and cybersecurity related exposures. And it consists of yes/no question with section for comments and action items.  To maximize the checklist's effectiveness, involve a diverse group of participants from across the organization. The checklist is broad and aims to provide a quick overview of the organization's current risk posture.

External Audit /Assessment: Essential tools for maintaining a robust security posture and ensuring regulatory compliance.

Regulatory Standard:

1. GDPR
2. HIPPA
3. PCI DSS  
     

May include testing of the following:

1. Key Personal
2. Certifications
3. Standardized Assessments.

Performing External Assessment:

Part of maintaining a robust security posture and ensuring compliance. Purpose is to validate compliance with specific regulations and minimize.

Penetration Testing: Simulated cyberattack to identify exploitable vulnerabilities in a computer system.

Various types include

● Physical

● Offensive: Red team and simulation an attack on the vulnerabilities.

● Defensive: Blue Team and simulation a defensive mechanism deployed against the attack.

● Integrate: Purple Team, includes both offensive and defensive team.

Reconnaissance in pen test: Initial phase where an attacker gathers information about the target system.  
 

Importance of Reconnaissance ■ Crucial step in penetration testing ■ Identifies potential vulnerabilities in the target system ■ Helps plan the attack to reduce the risk of detection and failure.

1. Active Reconnaissance: Direct engagement
2. Passive Reconnaissance: Indirect Engagement.

Attestation of findings: Involves formal validation or confirmation provided by an entity to assert the accuracy and authenticity of specific information. Crucial in internal and external audits to ensure the reliability and integrity of the following.

Types of Attestation

1. Software Attestation.
2. Hardware Attestation.
3. System Attestation.

Cyber Resilience and Redundancy

High Availability: Aims to keep services continuously available by minimizing downtime.

Achieved through load balancing, clustering, redundancy, and multi-cloud

Strategies.

Up time: The time a system remains online, typically expressed as a percentage

Five Nine: 99.999% Uptime.

Six nines: 99.9999% Uptime

1. Load Balancing: Distributes workloads across multiple resources. Prevents overloading of any single resource. Incoming requests are directed to capable servers.
2. Clustering: Uses multiple computers, storage devices, and network connections as a single

System. Ensures continuity of service even in case of hardware failure.

1. Redundancy: Involves duplicating critical components to increase system reliability.

Redundancy can be implemented by adding multiple

● Power supplies

● Network connections

● Servers

● Software services

1. Multi-Cloud Approach: Distributes data, applications, and services across multiple cloud providers. Offers flexibility for cost optimization. Requires proper data management, unified threat management, and consistent

policy enforcement for security and compliance.

1. Strategic Planning: Utilize load balancing, clustering, redundancy, and multi-cloud approaches. Safeguard organizational continuity and reliability in a competitive environment

Data Redundancy:

RAID (Redundant Array of Independent Disks):  Combines multiple physical storage devices into a single logical storage

device recognized by the operating system

Raid 0: Provides data striping across multiple disks. Used for improved performance but offers no data redundancy

Raid 1: Provides redundancy by mirroring data identically on two storage devices.

Suitable for critical applications and maintains a complete copy of data on both

devices

Raid 5: Utilizes striping with parity across at least three storage devices. Offers fault tolerance by distributing data and parity

Raid 6: Similar to RAID 5 but includes double parity data. Requires at least four storage devices.

Raid 10: Combines RAID 1 (mirroring) and RAID 0 (striping). Offers high performance, fault tolerance, and data redundancy. Requires an even number of storage device.

RAID Resilience Categories

1. Failure-Resistance: Raid 1
2. Fault-Resistance: Raid 1, Raid 5, Raid 6 and Raid 10.
3. Disaster -tolerant: Raid 1 and Raid 10

Capacity Planning: Critical strategic planning effort for organizations. Ensures an organization is prepared to meet future demands in a cost-effective manner.

4 main aspect:

People:  
Technology:

Infrastructure:

Process:

Powering Data Centres:  
Power Protection Components:

1. Line Conditioners
2. Uninterruptible Power Supplies
3. Generators
4. Power Distribution Centres

Data Backups: Creating duplicate copies of digital information to protect against data loss,

corruption, or unavailability

■ Safeguards data from accidental deletion or system failures

1. Onsite and Offsite Backups: Within the office ( HDD) and storing it on a different geo location.

Frequency:

Recovery Point Objective

1. Encryption: Data in rest, Transit, use
2. Snapshots: Point-in-time copies capturing a consistent state.

Valuable for systems where data consistency is critical, like databases and

file servers.

1. Data Recovery:
2. Data Replication:
3. Journaling: Maintaining a detailed record of data changes over time. Maintains an audit trail. Ensures data integrity and compliance.

Continuity of Operations Plan.

1. Business continuity plan
2. Disaster Recovery Plan

Redundant Site Considerations: Backup location or facility that can take over essential functions and operations

in case the primary site experiences a failure or disruption

1. Hot Site: Up and running continuously, enabling a quick switchover. Expensive, but provides instant availability
2. Warm Site: Not fully equipped, but fundamentals in place. Cheaper than hot sites but with a slight delay.
3. Cold Site: May be just an empty building, ready in 1-2 months. Cost-effective but adds more recovery time.
4. Mobile site: Can be hot, warm, or cold. Utilizes portable units like trailers or tents. Offers flexibility and quick deployment (e.g., military DJC2)

Virtual Site:

1. Virtual Hot site: Fully replicated
2. Virtual Warm site: Scaling up resource when needed.
3. Virtual cold site: Minimizes ongoing costs by activating resources only during disasters.

Geographic Dispersion: Spreading resources across different locations for higher redundancy. Mitigates the risk of localized outages.

Resilience and Recovery Testing:

1. Tabletop Exercises: Scenario based exercise
2. Simulation :Computer-generated representation of a real-world scenario. Computer-generated representation of a real-world scenario.
3. Failover Tests: Controlled experiment. Making sure that your backup plan works effectively.
4. Parallel Processing: Replicates data and system processes onto a secondary system. Assesses the system's ability to handle multiple failure scenarios simultaneously.

Security Architecture

Design, structure, and behaviour of an organization's information security

Environment.

On-Premise vs. Cloud Deployment

Cloud Dep:

Delivery of computing services over the internet, including servers, storage,

databases, networking, software, analytics, and intelligence

Responsibility matrix: Responsibility between CSP and customer.

Key Considerations:

1. Scability
2. Realibility
3. Cost
4. Resilence
5. Scability
6. Ease of recovery
7. Deployment
8. Patch availibility

 9. Cloud computing offers flexibility, scalability, and cost-effectiveness

 10. On-premise solutions provide control and security but can be expensive and

challenging to maintain

 3. Hybrid solutions offer flexibility and control but require considerations of

security, compliance, interoperability, and cost

Cloud Security

1. Shared physical server: if one gets compromised then through that the entire server can get affected.

Miti: hyper visor protector, multiple tenancy, regular scanning and patching.

1. Inadequate VE security:

Miti: regular scanning and patching, Monitor unusual activity, network segmentation.

1. User access management: Weak user access management can result in unauthorized access to sensitive

data and systems.

Miti: Access control, Password management, MFA

1. Lack of Up-to-date Security Measures: Cloud environments are dynamic and require up-to-date security measures.

Miti:

Regularly update and patch software and systems, Review and update security policies

1. Single point of failure: Cloud service relying on single resource and if one goes off, then overall system wide outage.

Miti: Implement redundancy and fail over procedure. Multiple servers and datacentres.

1. Weak Authentication and Encryption Practices: Weak authentication and encryption can expose cloud systems and data.

Miti: Use multi-factor authentication, Strong encryption algorithms.

1. Data Remnants: Residual data left behind after deletion or erasure processes.

Miti: Implement secure data deletion procedures, Data backup securely, Data removal verification.

Virtualization and Containerization:

2 types of Hyper visor

1. Bare metal: that runs on hardware directly.
2. Hosted: Operated with standard OS.

Securing VM

1. Regular update and patch
2. Strong security policies.
3. VM to be distributed to many servers
4. Files and data to be encrypted.
5. Limit of VM connection to physical device.

Serverless: Relies on cloud service providers to handle server management, databases, and

some application logic. Developers can build and run app without having to manage the server.

Benefit:

1. Reduced operational cost
2. Automated scaling
3. Faster time to market.

Drawbacks:

1. Vendor lock in
2. Not mature practise

Micro services:

Architectural style for breaking down large applications into small, independent

Services.

Contrasts with traditional monolithic architecture, where all components are

Interconnected

Network Infrastructure:

1. Physical separation: where a component is isolated from the entire network. Which is called Air Gapping.
2. Logical Separation: logical boundaries with access control. VLAN, Firewall.

Software define network:

SDN Architecture: Designed by separating the three planes.

1. Data plane: handles the packets and is responsible for sending and receiving data
2. Control Plane: Centralized decision maker of SDN. Dictates traffic flow over network.
3. Application Plane: Hosts all network applications that interact with the SDN

Controller. Applications instruct the controller on network management. Controller manipulates the network based on these instruction.

Infrastructure as code: Modern approach to IT infrastructure management. Automates provision and management through code.

High-level languages like YAML, JSON, or domain-specific languages (e.g., HCL)

Used

Benefits:

1. Speed and consistency
2. Scabiliwty
3. Cost
4. Standardization.

Challenge:

1. Learning Curve
2. Complexity
3. Security risk

Centralized and de centralized architecture:

Centralized for Data accuracy and resource management priorities.

De-Centralized for Resilience, flexibility, and rapid scaling needs

Internet of things: Network of physical devices with sensors, software, and connectivity that exchanges data among connected device.

1. Hub
2. Smart Device
3. Sensor
4. Wearables

IOT Risk  
1.       Security concerns

1. Poorly configured network settings.

Industry controlled system (ICS) and Supervisory controlled and data acquisition system (SCADA):

ICS: Systems used to monitor and control industrial processes, found in various

industries like electrical, water, oil, gas, and data.

1. Distributed Control Systems (DCS): Used in control production systems within a single location.
2. Programmable Logic Controllers (PLCs): control specific processes such as assembly lines and factories.

SCADA:

Type of ICS designed for monitoring and controlling geographically dispersed

industrial processes like

1. Electrical power generation, trans and distribution
2. Water treatment
3. Oil and pipeline monitoring and control.

Securing ICS and SCADA Systems:

1. Implement Strong Access Controls
2. Regularly Update and Patch Systems
3. Use Firewall and Intrusion Detection Systems

Embedded system: System designed for dedicated function within larger device.

RTOS (Real time operating system) : that works for real time application by minimising the time for data processing.

1. Flight navigation
2. Medical equip

Security Infrastructure:

Port and Protocols:  
Logical communication endpoints on a computer or server

1. Inbound – Listen for connection.
2. Outbound- Used to connect to a server.

3. Well Known Ports (0-1023)
4. Registered Port (1024-49151)

Port Number

Protocol Used

TCP/UDP

Basic Description

Firewalls:

Identity and Access Management (IAM) Solutions:

IAM: Critical component of enterprise security, focusing on managing access to

Information.

Ensures the right individuals have access to the right resources at the right times

for the right reasons.

4 main reasons for IAM:

1. Identification.
2. Authentication
3. Authorization
4. Auditing:

Key IAM Concepts:

1. Provisioning and de provisioning users
2. Identity proofing.
3. Interoperability
4. Attestation.

Multifactor authentication:

A security system requiring multiple methods of authentication from

independent categories of credentials.  
  
Five Categories of Authentication for MFA:

1. Something you have
2. Something you know
3. Something you are
4. Something you are
5. Something you do.

Authentication types:

1. Single factor
2. 2 factor authentication
3. Multi factor authentication
4. Knowledge based.
5. Passkey: Passkeys utilize public key cryptography.

Password Security:  
 

1. Measures the effectiveness of a password in resisting guessing and brute-force

Attacks.

1. Estimates the number of attempts needed to guess a password correctly.

Group Policy Editor for Password Policies:

1. Used to create password policies in Windows

■2.  Available for local machines, and global policy orchestrator can be used in

domain environments

5 characteristics of password policies:

1. Length
2. Complexity
3. Reuse
4. Age
5. Expiry.

Password less authentication methods:

1. Biometrics
2. Hardware token
3. OTP
4. Pass key
5. Magic Link.

Password attacks:

1. Brute force: Tries every possible character combination until the correct password is found.

Mitigation: Password length, Login limit, MFA

1. Dictionary: Most commonly used password. Variations of numbers and symbols.

Mitigation: Password length, MFA, employ captcha

1. Password spraying: A form of brute force attack that tries a few common passwords against many

usernames or accounts. Effective because it avoids account lockouts and targets weak passwords.

Mitigation: Use unique passwords and implement multi-factor authentication.

1. Hybrid: Combines elements of brute force and dictionary attacks.

Single Sign on: Authentication process allowing users to access multiple applications with one set of credentials. Simplifies the users experience and enhances productivity. Trusted relationship between applications and Identity providers (IdP).

How SSO Works:

1. User logs into primary identity provider.
2. Accesses a secondary application with the SSO configured.
3. 2nd application verifies the user's identity with the IdP's assertion.
4. Access is granted.

Protocols for SSO.

1. LDAP( Lightweight directory access protocol):

- Used to maintain and access distributed directory information across network resource.
- Central reprisitory fort authentication and authorization.

1.  Oauth(open authentication):

- Token based authorization and authentication. Allows 3rd party to access user info without accessing the pass.

SAML(Security Assertion Markup Language): For authenticating the users identity.

Federation:

Federation Process :

1. Login initiate.
2. Redirect to IDP
3. Authentication of user.
4. Generation of Assertion
5. Return to IDP
6. Verification and access
7. Login complete

Priviliged access management: Solution that restricts and monitors privileged access within an IT environment. The policies, procedures, and technical controls that are used to prevent malicious abuse of privileged accounts.

Components for PAM:

1. JIT permission
2. Password Vaulting
3. Temporal accounts.

  
Access control Models:

1. Mandatory access control.
2. Role based access control
3. Rule based access control
4. Discretionary access control
5. Attribute access control:

  
Access Control Extension:  
1. Time of Day restriction

2. Principle of Least privilege.

  
Vulnerability and Attacks:

Hardware Vulnerabilities: Security flaws or weaknesses in a device's physical components or design that can be exploited to compromise system integrity, confidentiality, or availability.  
 

1. Firmware Vulnerability:
2. Legacy, End of life and unsupported.
3. Unpatched Vulnerability:
4. Hardware Misconfigure:

Mitigation techniques to hardware Vulnerabilities:  
1.  Patching

1. Hardening
2. Configuration enforcement
3. Segmentation
4. Isolation
5. Decommission.

Bluetooth Vulnerability and attacks:

1. Vulnerabilities:

2. Unsecure Pairing.
3. Device Spoofing
4. On path attack.

Bluetooth attacks:

1. Blue jacking: Send unsolicited message.
2. Blue snarfing: Steal info from the device.
3. Blue bugging: Take control of the device.
4. Blue smacking: Denial of service attack and make the device unresponsive.
5. Blue Borne: without connection but spread through air.

Bet practise:

1. Turn Bluetooth off.
2. Make it undiscoverable.
3. Update firmware.
4. Pair with trusted device.
5. Use  encryption.

Mobile Vulnerabilities and attack:

1. Sideloading
2. Jailbreaking
3. Insecure connection method.

Mobile Device Management:

1. Patching
2. Configuration management
3. Best practise management.

Zero day Vulnerabilities:

- Zero Day Attack:
- Zero Day Vulnerability:
- Zero Day Exploit:
- Zero Day Malware:

Operating system Vulnerabilities:

1. Unpatched system.
2. Misconfiguration
3. Zero day vulnerabilities.
4. Data Exfiltration.
5. Malicious updates.

SQL and XML injection:   
  
Injection Attack: Involves sending malicious data to a system for unintended consequences.

SQL (Structured Query Language):

4 main SQL actions:

1. Select: Read from DB
2. Insert: Write on DB
3. Delete: Remove from DB
4. Update: Overwrite on DB

SQL Injection: Process of injecting malicious SQL codes into input field. Attackers use, URL parameters, Form field, cookies, HTTP headers.

Mitigation

1. Input Validation
2. Data Sanitization
3. Web application firewall

XML(Extensible markup language) injection:

XML is used during the data exchange in web application. It should use TLS for transfer.

XML attack:

1. XML Bomb (Billion laugh attack): Consumers memory, similar to DOS.
2. XXE (XML External entity attack): Attempts to read the local resource, like password hash in the shadow file.

Implementation:

-Proper input validation

Cross Site Scripting: Injects a malicious script in a website to compromise the visitor.

4 steps,

1. Identify input validation vulnerability in a website
2. Crafts URL to perform code injection in the site.
3. Trusted site will return the page containing the malicious code.
4. Malicious code then runs in the users browsers with permission level as trusted site.

Function:

1. Defacing the website.
2. Stealing users data
3. Intercepting communication.

Type of XSS:

1. Persistent XSS: Attackers are able to inject code in the website database.
2. Non persistent XSS: attack that only happens once when launched.
3. Data object Model XSS: Exploits the client’s web browser using client-side scripts to modify the content and layout of the web page. Client side attack

Session Management;

Cookie:

1. Non-persistent
2. Persistent

XSRF(Cross site request Forgery): Malicious script is used to exploit a session started on another site within the same web browser. It is also called, session riding or One click attack.

Prevention.

1. User specific token.
2. MFA
3. User need to enter their current password to change their password.

Buffer Overflow:

Buffer flow attack: Occurs when the process stores the data outside the memory allocated by the developer. 85% of data breach uses buffer flow as initial vector attack. Attackers exploit the excess data written beyond buffer boundaries to manipulate program execution.

Buffer: Temporary storage areas used by the programmer to hold data. Overflowing a buffer results in data spilling into adjacent memory locations, causing unintended consequences.

Technical aspect:

1. Stack
2. Smashing the stack.
3. NOP slide

Mitigation against Buffer attack:

Address space layout randomization (ASLR): prevent attackers from guessing return pointer addresses. Randomizes the memory used by well-known

apps, making it harder to predict the location of the attackers code.

Race conditions:  Software vulnerabilities related to the order and timing of events in concurrent processes. Race conditions occur when multiple threads or processes access and manipulate shared resources simultaneously.

Dereferencing: when the code tries to break off the relationship between the pointer and the thing it was pointing at the memory that allows the changes to be made.

Types of Race condition:

1. Time of check (TOC): Before the resource state is checked.
2. Time of use (TOU): Manipulate it after it is checked, but before used.
3. Time of Evaluation (TOE): When the system is making the evolution of the process.

Mitigating Race condition:

1. Mutuex: Acts as a gate keeper, where it makes sure that only 1 thread or process can access the code at the time.,
2. Deadlocks: Occurs when a lock remains in place because the process it’s waiting for is terminated, crashes, or doesn’t finish properly, despite the processing being complete.

Malicious Activity: Constantly evolving threats in the digital age.

Distributed denial of service attack: Used to describe an attack that attempts to make a computer or server’s resources unavailable.

1. Flood attack :Overload server with request.

2. Ping: Overloading a server with ICMP echo requests (pings). Often countered by blocking echo replies
3. SYN : Multiple TCP sessions but not completing the 3-way handshake.

Counter: Flood Guard, Timeout, IPS(Intrusion prevention system).

1. Permanent Denial of Service (PDOS) Attack: Exploits security flaws to break a networking device permanently by re-flashing its firmware. Requires a full firmware reload to bring the device back online.
2. Fork Bomb: Attack creates a large number of processes, consuming processing power. Self-replicating nature causes a denial of service condition. But it's not a worm.
3. DDOS: Malicious attempt to disrupt the normal functioning of a network, service, or website by overwhelming it with a flood of internet traffic. Involves multiple machines attacking a single server simultaneously.

DDOS Amplification: Generate high amount of packets and initiate DNS request from a spoof IP.

Surviving and Preventing DoS and DDoS Attacks :

1. Blackhole or Sinkhole: Routes attacking IP traffic to a non-existent server through a null interface.
2. Intrusion Prevention Systems: Can identify and respond to DoS attacks for small-scale incidents.
3. Elastic Cloud Infrastructure: Scaling cloud infrastructure when need to handle large attack.
4. Specialized Cloud Service Providers: Some specialized cloud provider like Cloudflare and Akamai provide DDOs.

DNS attacks: Types of DNS attacks:

1. DNS cache poisoning:  Corrupting DNS resolver's cache with false info, then redirecting the users to malicious website.

Network config and firewall and also using DNSSEC that is used to add digital signature to the DNS data.

1. DNS Amplification: Spoofed DNS queries sent to open DNS servers.

Limit the size of DNS response.

1. DNS Tunnelling: Encapsulates non-DNS traffic (e.g., HTTP, SSH) over port 53. Attempts to bypass firewall rules for command and control or data exfiltration  
    Monitor and Analyse DNS logs.
2. Domain Hijacking: Unauthorized change of domain registration. May lead to loss of website control and redirection to malicious sites  
    Regularly update and secure registration account information.  
     
3. DNS Zone Transfer Attack: Attempts to obtain an entire DNS zone data copy. Exposes sensitive information about a domain's network infrastructure

Directory Traversal Attack: Application attack that allows access to commands, files, and directories that may or may not be connected to the web document root directory. May be used to access any file on a system with the right permissions.

File Inclusion: Vulnerability that will allow the attacker to either download a file from that directory or create an executable file to create an backdoor.

Remote file inclusion: An attacker executes a script to inject a remote file into the web app or website.

Local file inclusion: An attacker adds a file to the web app or website that already exists on the hosting server

Execution and Escalation attack:

1. Arbitrary code execution: IF can access system and execute code.
2. Remote code execution: IF executing code remotely.
3. Privilege execution:  
    a. Vertical: Normal user to admin.  
    B. Horizontal: Accessing or modifying resources at the same level as the attacker. Occurs when a user attempts to access resources for which they don't have permissions at the same level
4. Rootkits: Class of malware that conceals its presence by modifying system files, often at the kernel level.

Ring 0: admin level

Ring 1-3: User level

Kernel Mode Rootkit: Has the maximum privileged by embedding the rootkit in ring 0.

User Mode Rootkit: Attached to user-level components (Rings 1 to 3).

Replay Attack: Type of network-based attack where valid data transmissions are maliciously or fraudulently re-broadcast, repeated, or delayed. Involves intercepting data, analysing it, and deciding whether to retransmit it later.

Different from a Session Hijack

● In a Session Hijack, the attacker alters real-time data transmission

● In a Replay Attack, the attacker intercepts the data and then can decide later whether to retransmit the data.

Credential Replay Attack: Specific type of replay attack that Involves capturing a user's login credentials during a session and reusing them for unauthorized access.

Preventing replay attack:

1. Session tokens to uniquely identify authentication sessions.
2. MFA.
3. Using WPA3 security protocols.

Session Hijacking: A type of spoofing attack where the attacker disconnects a host then replaces it with his or her own machine, spoofing the original host's IP address.

Session Management: Enables web applications to uniquely identify a user across a number of different actions and requests, while keeping the state of the data generated by the user and ensuring it is assigned to that user.

Cookie: Text file used to store information about a user when they visit a website.

Session Cookie: Non-Persistent, resides in memory and are deleted when the browser instance is closed.

Persistent cookie: Cookies that are stored in the browser cache until they are deleted by the user or pass a defined expiration date.

Session Prediction Attacks :

A type of spoofing attack where the attacker attempts to predict the session token to hijack a session.

Cookie Poisoning: Modifies the contents of a cookie after it has been generated and sent by the web service to the client's browser so that the newly modified cookie can be used to exploit vulnerabilities in the web app.

On-Path Attack: An attack where the attacker positions their workstation logically between two hosts during communication. The attacker transparently captures, monitors, and relays communications.

Methods:

1. ARP Poisoning
2. DNS Poisoning
3. Rouge AP
4. Rouge Switch

Relay Attack: The attacker becomes part of the conversation between two hosts. Serves as a proxy and can read or modify communications between the hosts.

Downgrade attack: An attacker forces a client or server to abandon a higher security mode in favour of a lower security mode.

Injection Attack: LDAP statement generated by user input is fabricated. Input Validation and Input Sanitization.  
  
Lightweight Directory Access Protocol (LDAP): An open, vendor-neutral, industry standard application protocol for accessing and maintaining distributed directory information services over an Internet Protocol network.

Command Injection: Occurs when a threat actor is able to execute arbitrary shell commands on a host via a vulnerable web application.

Process Injection: Method of executing arbitrary code in the address space of a separate live process.

Indicators of Compromise (IoC):

 Pieces of forensic data that identify potentially malicious activity on a network or system.

1. Account Lockouts
2. Blocked Contact
3. Resource Consumption.
4. Resource Inaccessibility.
5. Out of cycle logging
6. Missing log
7. Impossible travel.

  
Hardening:

Process of enhancing system, application, or network security.

-Apply security patches, configure access controls, disable unnecessary

Services

Changing default configurations:

1. Default passwords

- Should be complex.
- Must be changed 90 days.  
     

1. Unneeded ports and protocols.

- Close any ports that aren’t needed.
- Audit ports and protocols that are enabled.

1. Extra open ports

- Open by default
- Use the secure one and close the unsecure ones.

Restriction Application:

1. Least functionality
2. Managing Software.
3. Preventing unauthorized software.
4. Applications Allowlist
5. Application Blocklist
6. Centralized mgmt.

Trusted Operating System:  
 

An operating system that is designed to provide a secure computing environment

by enforcing stringent security policies that usually rely on mandatory access

Controls. Used where CIA is essential.

Evaluation Assurance Level (EAL):

security standard and certification from the Common Criteria for

Information Technology Security Evaluation

EAL 0 - Lowest level

EAL1 - Highest Level

Trusted OS includes  
1. MAC (Mandatory Access Control)

2. RBAC
3. Security Auditing.

Example:

1. SELinux:
2. Trusted Solaris:

Updated and Patches:

Patch Management can be:

1. Manual
2. Automated:

Hotfix: Once tested, it is applied immediately to resolve the security issue.

Update: Provides a system with additional functionality, but it doesn’t usually provide any patching of security related issues.

Service Pack: Include all the hotfix and update for the OS since the release.

Patch Management:

1. Assigning a team to hunt down the vendor security patch.
2. Automated system-wide patching.
3. Priotrizing the patches as urgent, not urgent or non-critical.
4. Create a testing environment for critical patches.
5. Test and deploy the firmware patch.
6. Maintain patch logs.
7. Assesing a non critical patches.

Patch Management:

Consists of 4 simple steps,

1. Planning
2. Testing
3. Implementing
4. Auditing.

Group Policies:

- A set of rules and policies that can be applied to users or computer accounts within an operating system
- To access group policy., launch gpedit.
- Group policy can act as a security template applying rules

1. Password complexity
2. Access control
3. Software Restriction
4. Application restriction

Security Template: group of security policy that can be implemented in one procedure.

Group policy objective: Hardening the OS and creating a security baseline.

Data encryption: Process of converting data into a secret code to prevent unauthorized access.

SELinux:

A security mechanism that provides an additional layer of security for

Linux distributions.

Enforced MAC. Enables information to be classified and protected.

Enhances file system and network security, preventing unauthorized access,

security breaches, and execution of untrustworthy programs

3 main context in SELinux are,

1. Userc context:

Defines which users can access an object.

1. Role Context:

Determines which roles can access an object, using 'object_r' for files and

Directories.

1. Type Context:

Essential for fine-grained access control, grouping objects with similar

security characteristics.

Selinux Mode:

1. Disabled: Where the MAC is disabled and DAC is enabled for access control.
2. Enforced: all security policies are enforced.
3. Permissive:

Enables SELinux but doesn't enforce policies, allowing processes to

bypass security policies

Policies:

1 .Targeted : only specific process.

1. Specific: Every subject and object operate under MAC

Secure Baselines: Standard set of security configurations and controls applied to systems, networks, or applications to ensure a minimum level of security. consistent security postures and mitigate common vulnerabilities

Establishing a secure Baseline: Overall analysis of the company's IT infra and Sec infra to create a baseline that is going to be out model.

Configuring a Secure Baseline: Configuring a baseline by using a device and allaying it for any vulnerabilities point  and creating an= image

Deployment : Deploye the baseline by config firewall, user permission, GPO.,

Maintenance: Regular audits, monitoring, and continuous assessment are required to keep the baseline up-to-date, Periodically review and update the secure baseline to adapt to changes in organizational infrastructure, business needs, and emerging threats.

Conduct training sessions to educate employees about the importance of adhering to secure baseline configurations

Employee Training and awareness:

Security Techniques:

Wireless Infrastructure Security: Crucial for securing wireless networks in organizations.

Wireless Access Point Placement: Network, Connectivity and Security.

Placement consideration: not near the wall to avoid leakage, central location.

External service set: Multiple WAPs work together to provide seamless network coverage.

WAP interface: There is a disturbance in the signal if all the WAP uses the same channel or overlapping frequencies.

Tools for ensuring WAP coverage:

1 Site survey

2 Heat wave : Graphical rep, troubleshooting, WAP placement infrastructure.

Wireless Security Settings:  
  
Wired Equivalent Privacy (WEP)

Using static encryption system

24 bit initialization vector made it unsecure

Wifi protected access : Uses the TKIP for key encryption. Due to TKIP vuln, it was considered prone to cryptographic attack, insufficent data integ due to TKIP implement.

Wifi protected access 2: Introuduced in 2004, and uses AES and CCMP.

Uses Message integrity code for integrity.

Wifi protected access-3: The most protected protocol using AES.

Extra feature:  Replaces 4 way hand shaking with

Diffie-Hellman key

Agreement.  
 

: Data encryption for open network  
: Cryptographic protocols

 : Provide integrity of network management.

AAA protocols

1. RADIUS (remote authentication dial in user services): provides AAA service, used to secure access to network resources.
2. TACACS+ (Terminal Access Controller Access-Control System Plus):

Separates Authentication, Authorization, and Accounting

Functions. More granular control.

Authentication Protocols:

1. Extensible authentication protocol:
2. Protected EAP
3. EAP-TTLS
4. EAP-FAST (flexible authentication via secure tunnelling)

Application Security: Focuses on building secure applications. Aims to prevent, detect, and remediate security vulnerabilities.

1. Input Validation: Ensures that applications process well-defined, secure data
2. Cookies: Stores vital user information. Transmitted over HTTPS.
3. Static code analysis:

A method of debugging an application by reviewing and examining its

source code before running the program. Identifies issues like buffer overflows, SQL injection, and XSS.

1. Dynamic code analysis: Debugging the application after the program has been executed. Fuzz testing, stress testing
2. Code signing: whether it is from a authorized vendor or not. Digital signature to verify the atheneite.
3. Sandboxing. Isolates running programs, limiting their access to resources. Used to execute untrusted or untested programs securely

Network Access Control:

Used to protect networks from both known and unknown devices by scanning

devices to assess their security status before granting network access. Can be applied to device connecting to both internal and through VPN.

NAC Process:

1. When being scanned, its placed in a virtual holding area.
2. Scanning checks various factors like antivirus, security patch and security threats.
3. If passed, it will allow
4. If failed, will be hold on a quarantine area.

NAC agents:  
1. Persistent Agent:

Installed on devices in a corporate environment where the organization

owns and controls device software

1. Non persistent agent: 

Common in environments with personal devices (e.g., college campuses);

users connect, access a web-based captive portal, download an agent for

802.1x Standard:  
 

Port-based Network Access Control mechanism based on the IEEE 802.1x

Standard. Modern NAC solutions build on 802.1x.

Rule based access control factors:

1. Time-based
2. Location based
3. Rule based
4. Role based.

Web filtering:

Web filtering or content filtering is used to control or restrict the content users

can access on the internet

1. Agent Based WF: Installing agent that monitors and enforces the policies:
2. Centralized proxy:

Uses a proxy server as an intermediary between an organization’s end

users and the Internet. Evaluates and controls web requests based on policies.

1. URL Scanning: Analyses website URLs to check for matches in a database of known malicious websites.
2. Content Categorization: Based on policies, Categorize the content that the user can access.
3. Block rule: Certain site and URL or links to be blocked as per the org guidelines.
4. Reputation based filtering: Reputation score analysis based on third party scoring.

DNS filtering:

DNS filtering (Domain Name System filtering) blocks access to specific websites

by preventing the translation of domain names to their IP addresses.

Users' devices request domain name translation from DNS servers; if the domain

is on the block list, the server withholds the IP address to prevent access.

Often employed by schools, universities, and organizations to ensure safe and

educational internet usage.

Email Security:

Encompasses techniques and protocols to protect email content, accounts, and

infrastructure from unauthorized access, loss, or compromise

1. DKIM: Domain Key Identify email where the receivers server validates the sender's email digital signature on a DNS record using the senders public cryptographic key.

2. SPF (Sender Policy Framework): Checking the senders IP and verifying it on the DNS records before accepting the email.

3. DMARC (Domain bases message authentication, reporting and conformance): 

detects and prevents email spoofing by setting policies for email

sending and handling failures. It can work with both DKIM , SPF and both. Helps to prevent  Phishing scams, email spoofing.

1. Email gateway config:

Email gateways serve as entry and exit points for emails, facilitating

secure and efficient email transmission. SMTP (Simple Mail Transfer Protocol) to send and receive emails.

1. On prem email gateway:
2. Cloud Email gateway:
3. Hybrid:

4. Spam Filtering:

Spam filtering detects and prevents unwanted and unsolicited emails from

reaching users' inboxes

1. Content filtering
2. Email filtering rule
3. DNS-based sinkhole list.
4. Keywords basis

Endpoint detection and response:  
 

Category of security tools that monitor endpoint and network events and record

the information in a central database. Continuously monitoring and response to advanced threats. Monitors endpoint and network events, providing data for the following,

1. Analysis
2. Detection
3. Investigation
4. Reporting
5. Alerting

How EDR works:

1. Data collection
2. Data consolidation
3. Threat Detection
4. Alert and Threat Response
5. Investigation
6. Remediation  
      
    File Integrity Monitoring (FIM):

Validates the integrity of operating system and application software files by

comparing their current state with a known, good baseline

Identifies changes to:

1. Binary Files
2. System and Application files
3. Configuration and parameter files.

Extended Detection and Response (XDR):

Security strategy that integrates multiple protection technologies into a single

Platform. Correlates data across multiple security layers to detect threats faster, including.

1. Email
2. Server
3. Endpoint
4. Cloud
5. Network

EDR focuses on endpoints for p[potential threats and XDR focuses on endpoint but also on multiple platforms like cloud,. Email, server and network.

User Behaviour Analytics:

Advanced cybersecurity strategy that uses big data and machine learning to

analyse user behaviours for detecting security threats.

Focuses on understanding user behaviour within systems and networks to identify

patterns and anomalies.

User and Entity Behaviour Analytics (UEBA):

Technology similar to UBA but extends the monitoring of entities like routers,

servers, and endpoints in addition to user accounts.  
 

UBA and UEBA systems process data from various sources

1. User device
2. Logs
3. Application logs
4. Network traffic

Benefit:

Early threat detection

Insider threat detection

Improved IR

Selecting secure protocols: Choosing a secure protocols to protect data in transit for unauthorized access:

1. HTTP VS HTTPS
2. FTP VS SFTP
3. Telnet VS SSH

Port Selection:

Well-known ports (0-1023)

● Registered ports (1024-49151)

● Dynamic/private ports (49152-65535)  
  
Additional security considerations

1. least privilege by opening only necessary ports to

minimize the attack surface.

1. Changing port numbers can add a layer of obscurity but should not

replace robust security measures

Transport Method:  
 

TCP (Transmission Control Protocol)

● Connection-oriented, ensuring data delivery without errors

● Ideal for applications where data accuracy is crucial, like web and email

servers

● Uses acknowledgments, retransmission, and sequencing for data integrity  
  
 

UDP (User Datagram Protocol)

● Connectionless and faster, but doesn't guarantee data delivery

● Suitable for applications prioritizing speed over accuracy, like streaming

video or gaming

Vulnerability Management:

Systematic process for identifying, evaluating, prioritizing, and mitigating

Vulnerabilities.  Maintain secure and resilient cybersecurity posture, minimize security

breaches, and manage risk effectively.

Identifying Vulnerabilities:  Process of recognizing and categorizing weakness in system, network and application. Important for preventing unauthorized breach and protecting orgn data and system integrity.

Methods:

1. Vuln Scanning: Nessus and OpenVAS
2. Application security
3. Pen test
4. System and process Audit.

4 process pf Identifying Vulnerabilities:

1. Planning
2. Testing
3. Implementation
4. Auditing

Threat Intelligence Feeds:

Provide valuable information about potential or current threats to an

organization's security. Continuous streams of data related to potential or current threats.

Collected, analysed, and disseminated by security researchers, organizations, or

automated tools.

Evolution of Threats:

Sources of Threat Intelligence:

1. Open Source Intelligence (OSINT): Collected from public sources like news, forms, blogs, articles and are available at no cost.
2. Third party: Provided by commercial vendors under a subscription model. Offer more refined, analysed, and timely information. Fire Eye, McAfee, Symantec
3. Information Sharing org: Formed to facilitate the sharing of threat intelligence among members.

Collaboration among businesses in specific industries (e.g., finance,

healthcare) to share industry-specific threat information.

1. Dark Web: Everything there is to know.

Responsible Disclosure Program:

Ethical practice for disclosing vulnerabilities in software, hardware, or online

Services.

The goal is to provide stakeholders time to address vulnerabilities before public

Disclosure.

1. Bug Bounty Programs
2. Pen Test

Analysing Vulnerabilities: 

Vulnerability confirmation

1. True Positive: Detected and Identified.
2. False Positive: Falsely Detected.
3. True Negative: Identified but not confirmed.
4. False Negative: Serious Finding but Vulnerability cannot be detected.

Priotrizing Vulnerabilities: Ranking identified vulnerabilities by severity and potential impact. Scoring system Common Vulnerability scoring system.

Classifying Vulnerabilities: Software flaws, Configuration errors, Security policy gaps.

CVE (Common Vulnerabilities and Exposures): System that uniquely identifies vulnerability, plus providing solutions and mitigation and assess/ priories vuln fix.

Org Impact: Assessing potential impact on confidentiality, integrity, and availability.

Exposure Factor (EF): A quantifiable metric to estimate the percentage of asset damage.  
Risk Tolerance:

Vulnerabilities Response and Remediations:

1. Remediation: Involve installing patches, reconfiguring devices, or other actions
2. Rescanning Device:
3. Auditing Device: Configuration audit and patch auditing.

Vulnerability Reporting:

Process of documenting and communicating security weaknesses in software or

systems to individuals and organizations responsible for addressing the issues

1. Internal Reporting
2. External Reporting
3. Responsible disclosure
4. Importance of confidence.

Alert and Monitoring: Observing computer systems performance.

Monitoring System:

1. CPU.
2. Memory.
3. Disk Usage.

4. Network Performance.

Baseline: A reference point representing normal system behavior under typical operating conditions. Deviations from the baseline can indicate potential issues, prompting proactive troubleshooting and maintenance. Deviations from the baseline can indicate potential issues, prompting proactive troubleshooting and maintenance.

Application Monitoring: Managing and monitoring software application performance and availability. Tracks errors, bottlenecks, and issues that may affect an application's performance or user experience.

Infrastructure Monitoring: Observes physical and virtual infrastructure, including servers, networks, virtual machines, containers, and cloud services.  
Provides insights into network traffic, bandwidth usage, and device status. Overloaded network switches can signal the need for additional capacity or configuration issues.

Alerting and Monitoring activities:

1. Log Aggregation: Collection of logs from various sources.
2. Alerting: Setting up automated alerts for any events or conditions. Based on threshold or Anomalies.
3. Scanning: Regularly examines systems, networks, or applications to identify vulnerabilities, misconfigurations. Vul, config and code scanning.
4. Reporting: Generates summaries or detailed reports based on collected and analyzed data.
5. Archiving: Ensures data is retained for future reference, analysis, auditing, or compliance
6. Alert Response and Remediation: Managing and resolving identified issues based on alerts or scans. Begin by taking appropriate actions such as,

Investigating ○ Escalating ○ Initiating

Quarantine: Isolates a system, network, or application suspected of being compromise. Prevents the spread of threats and limits potential impact.

Alert Tuning: Adjusts alert parameters to reduce errors, false positives, and improve alert relevance. changing alert thresholds, conditions, or delivery methods.

SNMP: Simple network Management Protocol: Collecting information from managed devices on IP network and changing their behavior.  
  
Managed devices include the following ● Routers ● Switches ● Firewalls ● Printers ● Servers ● Client devices

SNMP Manager ;Central hub that collects information from the devices. It is setup as a server. Sends and receives SNMP messages to and from Agent.

SNMP Agent: Networked devices that send information about themselves to the manager. Transmit data at regular intervals or when requested by the manager.

SNMP message types:

1. Set: Manager-to-agent request to change variable values
2. Get: Manager-to-agent request to change variable values
3. Trap: Async message from agent to manager about various events about uptime, config change and network downtime.

It can be granular or Verbose.

1. Granular: Sent a trap message get a UOID to distinguish each message as a unique message received.

2. Verbose: SNMP traps may be configured to contain all of the  event info about as a payload.

SNMP 1&2: Use plain-text community strings for access, making them less secure.

SNMP 3: Security Enhancements in SNMP Version 3.

C: Enforcing advance encryption.

I: Hashsing the messgae.

A: AUTHenticing source of messgae.  
  
Security Information and Event Management (SIEM):  A solution for real-time or near-real-time analysis of security alerts generated by network hardware and applications. SIEM helps correlate various events and incidents from system logs.

SIEM Functionality:

1. Consolidates data from various systems into a centralized DB.
2. Correlates and analyzes log data.
3. Detect patterns indicating security threats.
4. Generates alerts for security teams to investigate.

Agent VS Agent less SIEM:

Agent: software is installed on each system to collect and send log data. Provide real time data.

Agent less: Collects logs through a set policy but may not be able to  collect real time or detailed data.

SIEM solutions:

1. SPLUNK
2. ELK (Elastic Stack)
3. Arcsight

Data from security tool:

1. Antivirus: Application and system scans, logs etc.
2. DLP: data on endpoints, network and cloud stored.
3. Firewall: allowed and blocked traffic logs, rule change, policies, potential threat.
4. NIDS/NIPS: Network anomalies, network traffic, detected threats.
5. Vuln Scanner: Generate data on identified vulnerabilities, severity, and remediation recommendations.

Network flow analysis:

Full Packet Capture (FPC): Captures entire packets, including headers and payloads.

Flow Analysis: Focuses on recording metadata and statistics about network traffic, saving storage space. Doesn’t include the actual content, just the metadata.

Flow Collector: Records meta data and statistics about network traffic. Allows for efficient data storage and reduces processing overhead.

Net Flow: Cisco-developed protocol for reporting network flow information. (Zeke)

IPFIX( IP flow information export) : Defines traffic flows based on shared characteristics (e.g., source and destination IP).

Data collected by NetFlow:

1.Network protocol interface

1. Ip version and type
2. Source and destination.
3. IP address
4. Source and destination ports
5. Types of service used.da

Security Content Automation and Protocol (SCAP): List of open standards that enhances automation for vuln management, measurement and policy compliance of the system in the organization. Developed by the National Institute of Standards and Technology (NIST).

SCAP Languages:

1. OVAL( Open vulnerability and assessment language): XML schema for describing system security states and querying vulnerability reports.
2. XCCDF(Extensible configuration checklist description format): XML schema for developing and auditing best-practice configuration checklists and rules.
3. ARF(Asset reporting format):XML schema for expressing information about assets and their relationships.

Enumeration Methods in SCAP

Common configuration enumerations: Scheme for provisioning secure configuration checks across multiple sources. Provides unique identifiers for different system configuration issues.

Common platform enumerations CPE: Identifies hardware devices, operating systems, and application.  
Common Vulnerability and exposure CVE: Describes publicly known vulnerabilities with unique identifier

Single Pane of Glass: Central point of access for security teams. Provides access to information, tools, and systems for monitoring, managing, and securing an organization's IT environment. Offers a unified view of the security posture and facilitates informed.

Benefits:

1. Simplified management and unified security posture view.
2. Monitor environment.
3. Track progress of incident response.
4. Automate repetitive task.
5. Improves collaboration and communication within security team.

Implementing: Can be implemented as hardware or software.

Steps:

1. Defining Requirement
2. Identifying and integrating data source.
3. Customize interface.
4. Standard operation procedure and documentation.
5. Continuous monitoring and maintenance.

INCIDENT RESPONSE:

Phases of Incident Response

1. Preparation: Make the organization system resilient against attacks.
2. Detection: Determines if a security incident has occurred.
3. Analysis: Thoroughly examines and evaluates the incident.
4. Contamination: Limits the incident's scope by securing data and minimizing business

Impact.

1. Eradication:Focuses on removing malicious activity from systems or networks
2. Recovery: Restores affected systems and services to their secure state

● Includes restoring from backups, patching, and updating configurations

1. Post-Incident Activity: Identifies the initial incident source and improvements to prevent future.

Includes:

1. Root cause analysis
2. Lesson learned
3. After action report.

Threat Hunting:

Proactive cybersecurity technique to detect threats that haven't been discovered

by normal security monitoring. Involves actively seeking out potential threats within your network, as opposed

to waiting for them to trigger alerts

Steps in Threat Hunting.

1. Establish a hypothesis: Create a specific model to identify threats with high impact.
2. Profile the threat actors: Profiling actors who might pose threat toy your organisation.
3. Threat hunting process.

4. Utilizes security monitoring and incident response tools
5. Analyse logs and system and alerts.
6. New tactics, techniques, and procedures used by threat actors

Root Cause Analysis:

Systematic process to identify the initial source of an incident and prevent it from

Recurring.

Steps in RCA:

1. Define and Scope the Incident: Define the cause and identify what has been affected.
2. Determine Causal Relationships: How it happened. How did it occur
3. Identify Effective Solutions: Find solutions to prevent the incident from recurring. Solutions may be various security measure.
4. Implement and Track Solutions: Execute and see if the solution worked and has fully resolved the situation. change management processes to update systems and configurations.

Benefits.

1. Helps to identify weak links that might be vulnerable.
2. Helps to create more secure environment.
3. Encourage no blame focusing on solution and improvement.

Incident Response Training and Testing:

1. Training
2. Testing
3. Table Top Exercise
4. Pen test
5. Simulation

Digital Forensic Procedure:

Digital Forensics:

Systematic process of investigating and analysing digital devices and data to

uncover evidence for legal purposes.

4 phase:

1. Identification: Secure the scene, preserve evidence, and document the scene.

Identify where relevant data might be stored (e.g., tablets, smartphones,

servers).

1. Collection: Requires proper authorization (e.g., warrant, executive authorization). Following order of volatility minimizes data loss.

5 steps:

1. Collect data from the system’s memory
2. Capture data from the system state.
3. Collect data from storage device.
4. Collect data from remotely stored.
5. Collect Network traffic and logs.  
     

Evidence Collect technique:

1. Disk Imaging:

Involves creating a bit-by-bit or logical copy of a storage

device, preserving its entire content, including deleted files

and unallocated space.

1. File craving:

Focuses on extracting files and data fragments from

storage media without relying on the file system.

1. Analysis:

Systematically scrutinize data for relevant information, timestamps, user

interactions, and signs of criminal activity

1. Reporting:

The report serves as crucial evidence in legal proceedings, and the

forensic analyst may need to testify

Ethical Considerations  
a. Avoiding Bias

1. Repeatable actions
2. Evidence preservation.

Data Collection procedure:

Data Collection involves the following:

1. Capturing and hashing system image.
2. Analyse data with forensic tools:
3. Capturing machine screenshot
4. Reviewing network logs
5. Collecting cctv video

Order of volatility.

1. Collect data from system mem
2. Collect data from system state
3. Collect data from storage
4. Collect data from network logs
5. Collect data from Remote stored data.

Investigating an Incident:

SIEM (Security Information and Event Monitoring System):

1. Real-time analysis of security alerts from applications and network hardware
2.  Combination of different data sources into one tool
3.  Provides a consolidated view of network activity
4.  Allows for trend analysis, alert creation, and correlation of data

5. Log files
6. Sys logs: commonly used to feed logs into SIEM.
7. Netflow:
8. Sflow: alternative to sflow
9. IPFIX: Universal standard for exporting IP flow information
10. Meta data: Describe other data.

Use Cases for Metadata

● Email

○ Analyse metadata for phishing campaigns

● Mobile

○ Review data transfer, call duration, and contacts

● Web

○ Determine website visits and user behaviour

● File

○ Examine file details, such as creation time and viewer statistics

1. Dashboard

2. Single glass of pane:
3. Splunk:
4. Dashboards help analyse trends over time and inform actions.

5. Automated reports:

6. Report ID
7. Generation date
8. Report Period
9. Prepared by
10. Executive Summary
11. Incident Alert
12. Incident Detail
13. Incident Analysis
14. Security Recommendation
15. Conclusion
16. Appendices.

17. Vulnerability Sacn:  
    Vulnerability Scan reports:
18. Packet Capture:

19. Captures data going to or from a network device
20.  Can be set up on a span port to capture all data going to and from devices on the

Network.

Packet Capture Columns

1. Number
2. Time
3. Source/Dest IP
4. Protocol
5. Length
6. Info

7. Metadata: Information about a file, application, or other data.  
    a. MD5/SHA256 Checksum:

Serves as unique digital fingerprint for file identification, including potential

Malware

Automation and Orchestration:

When to automate and Orchestration:

Automation and Orchestration:

-Effective automation and orchestration are for repeatable and stable tasks and

Workflows.

-Identify consistent processes in your organization for automation and

Orchestration.

Decision factors for implementing automation and orchestration:

1. Complexity
2. Cost
3. SPOF(Single point of failure)
4. Technical Debt
5. Ongoing supportability.

Benefits of automation and Orchestration:

1. Time saving
2. Enforcement of baseline.
3. Standardized configuration
4. Quicker response
5. Secure sailing
6. Workforce Multiplier

Automation Support Tickets:

Automation support Tickets process:

1. User submit
2. Ticket generation
3. Capture info
4. Categorize ticket
5. Assign to relevant
6. Automated notification on status.

Automation Ticket escalation:

Ticket Escalation Automation:

1. Define escalation criteria based on issue nature, urgency, and service.
2. Create automation rules to monitor ticket attributes and trigger

Escalation

1. Perform predefined escalation actions (e.g., notification, reassignment,

change in priority)

1. Monitor and track the escalated ticket's progress.
2. Resolve and close the ticket, triggering notification to the user.

Automation Onboarding:

Streamlining onboarding ensures new hires are integrated quickly and efficiently

into their roles and the organization's culture.

1. Eliminates manual task and errors.
2. Reduces admin burden on IT and HR

Areas to automate:

1. Documentation of records.
2. Provisioning equipment.
3. Access manage
4. Feedbacks.

User Provisioning:

Involves creating and managing user accounts and access rights

Ensures new employees have necessary access to systems, applications, and

Resources.

Resource Provisioning:

Ensures timely allocation of physical and digital resources needed by new

Employees.

1. Workstation
2. Communication tools
3. Licenses.

Automation Security:

Helps prevent security vulnerabilities, respond to threats swiftly, and maintain

consistent security policies.

It involves using technology to perform crucial but repetitive security tasks to

maintain updated defences and swift response to security threats.

Automating Security:

1. Implementing guardrails:
2. Managing security groups
3. E/D services and access.
4. Automating Permission Management:

Automating application Development:

Automating application development: Enhances efficiency, consistency, and the quality of software products.  
 

Continuous Integration and Continuous Deployment (CI/CD) significantly improve

software efficiency, consistency, and quality.

Continuous Integration:

1. Merge codes in a central repository.
2. Build process verifies each check-in and detects problem.
3. Tool manages code integ and provide notification on error.
4. Automate test ensure quality of the software after integ.

Continuous Deployment:

Takes CI/CD further by automatically deploying code changes to testing

and production environments.

Automation ensures consistent deployments, faster releases, and offers

rollback capabilities.

Requires a paradigm shift, more developer involvement in the

deployment process

● Promotes increased communication and collaboration within teams for

collective responsibility

Integrations and APIs: Combining subsystems or components into a single, functioning system

API(Application Program Interface):  
- Set of rules and protocols used for building and integrating application software.

Enable software developers to access functions or features of another

application programmatically

API Communication:  
 

1. APIs facilitate communication between different parts of a microservice or

service-oriented architecture

1.  Allows automation of administration, management, and monitoring of services

and cloud-based infrastructures

Common communication styles

1. REST( Representational state transfer):

REST uses standard HTTP methods, status codes, URIs, and MIME

types for interactions

○ Primarily uses JSON for data transfer

1. SOAP(Simple Object Access Protocol)):

2. SOAP has a structured message format in XML.

3. Known for robustness, additional security features, and

transaction compliance

1. Suitable for enterprise-level web services with complex

transactions and regulatory compliance requirements

  
  
Benefits of API Integrations:  
 

1. Improved efficiency and consistency
2.  Allows direct integration of third-party applications into web applications
3.  Reduces the need to build entire services from scratch

Security Awareness:  
  
Recognizing Insider Threats:

Behaviours:

1. Altered State or Substance Abuse.
2. Emotional Distress
3. Lifestyle Incongruences
4. Financial Struggles.

Password Managers:  
 

Specialized tool, plugin, or extension used with web browsers

■ Helps users securely store and manage various usernames and passwords for

different websites  
 

Password Reuse Risks

■ Reusing passwords across multiple websites is dangerous

■ Breaches of one website can expose reused passwords

■ Attackers use known credentials to compromise other sites

■ Most usernames are email addresses, further increasing risk

Built-In vs. Third-Party Password Managers

■ Many web browsers offer built-in password functionality

■ Third-party password managers like Bit warden, Dashlane, LastPass, or OnePass

are often preferred for enhanced security

Avoiding Social Engineering:

1. Social Engineering: Involves deception to manipulate individuals into breaching security procedures
2. Maintaining Situational Awareness.
3. Piggybacking and Tailgating
4. Dumpster diving.
5. Operational Security (OPSEC).
6. Technological Social Engineering Attacks
7. Pressure Tactics
8. Proactive Culture of Security

Policy and Handbook:

Remote and Hybrid work:

Creating a culture of security: Technical security solutions are ineffective if employees do not value security.

Involves integrating cybersecurity into the organization's ethos, behaviours, and

decisions

Requirments:  
 

- Organizational change management
- Strategic planning
- Execution
- Monitoring
- Reportin

CRYPTOGRAPHIC SOLUTIONS

Encryption:

1. Symmetric Encryption: Single key used for both encrypt and decrypt. Same key is shared by both sender and receiver. Offers confidentiality but lacks non-repudiation.
2. Asymmetric Encryption: Uses two separate keys 1. Public key for encryption and private key for decryption. Often called “Public Key Cryptography”. Slower compared to symmetric encryption but solves key distribution challenges.
3. Hybrid: Asymmetric encryption used to encrypt and share a secret key ■ Symmetric encryption used for bulk data transfer, leveraging the shared secret key.
4. Stream Cipher: Encrypts data bit-by-bit or byte-by-byte in a continuous stream. Suitable for real-time communication data streams like audio and video.
5. Block Cipher: Breaks input data into fixed-size blocks before encryption.

Symmetric Algo:

1. DES: Uses a 64-bit key (56 effective bits due to parity. Encrypts data in 64 bit blocks through 16 rounds of transposition and sub.
2. Triple DES: Encrypts data with 3 56 bit keys. 1st to encrypt, 2nd to decrypt, 3rd to encrypt.
3. IDEA( International data encryption algorithm): Uses a 128-bit key, faster and more secure than DES. Not widely used as AES.
4. AES Advance encryption standard: Supports, 128 bit, 192 bit and 256 bit key for encryption and considered to be the best for encrypting sensitive information.
5. Blowfish: Support key from 32 bit to 448 bit. Was develop for replacing DES.
6. Two fish: A block cipher supporting 128-bit block size and key sizes of 128, 192, or 256 bits
7. RC Cipher suite (RC4,5,6): RC4 is stream cipher with key size ranging from 40 to 2048 bit. RC5 is a block cipher with the variable ranging upto 2048 bit. Rc6 based on RC5 and was considered DES replacement.

Note: When working with encryption, identify if it's symmetric or asymmetric and whether it's a block or stream cipher.  
  
 

Asymmetric Algo:

Public Key cryptography: No shared secret key required. Uses a public key for encryption and private key for decryption.

Common Asymmetric Algorithms:

1. Diffie-Hellman: Used for key exchange and secure key distribution. Commonly used in VPN tunnel establishment (IPSec)
2. RSA: Used for key exchange, encryption, and digital signatures. Supports key sizes from 1024 to 4096 bit. Widely used in organisation and M.FA.
3. Elliptic Curve Cryptography(ECC): Uses algebraic structure of elliptical curves. Commonly used in mobile devices and low-power computing. Six times more efficient than RSA for equivalent security.

Hashing: One-way cryptographic function that produces a unique message digest from an input.

Common Hashing algorithm:

1. MD5 (Message Digest Algorithm 5):  Creates a 128-bit hash value .Limited unique value that might result in collision. It is not suitable for security-critical application.
2. SHA(Secure Hash Algorithm Family):

3. SHA-1 :produces a 160 bit hash value.
4. SHA-2: offers a longer hash digest( SHA-224, SHA-256)
5. SHA-3: Uses 224 to 512 bit hash digest.

6. RIPEMD (RACE Integrity Primitive Evaluation Message Digest):Versions available ○ 160-bit (Most common) ○ 256-bit ○ 320-bit.
7. HMAC (Hash-based Message Authentication Code): Checks message integrity and authenticity. Utilizes other hashing algorithms (e.g., HMAC-MD5, HMAC-SHA1, HMAC-SHA256).

Digital Signature:

1.  Hash digest encrypted with a private key.
2. Sender hashes' the message and encrypts the hash with their private key, receiver decrypts using the sender's public key.\

Common DIgital signature algo:

1. Digital signature Algorithm(DSA): Uses a 160-bit message digest created by DSS (Digital Security Standard)
2. Rivest-shamir-adelman(RSA): Used for key exchange, encryption, and digital signatures. Supports key sizes from 1024 to 4096 bit. Widely used in organisation and M.FA.

Increasing Hash Security:

Common Hash Attacks:

1. Pass the Hash: Attackers authenticate to the remote server using the hash of the users password.

Mitigation : Patching, MFA, least privileged.

1. Birthday Attack: Occurs when there is a collision in the hash digest. Use longer has output to avoid collision.

Increasing Hash Security:

1. Key Stretching: using longer secure keys at least 128 bit. Used in WAP and WPA-2
2. Salting: Adds random data to the password before hashing. Ensure distinct hash output for the same password due to salt.
3. Nonces:

Adds unique, often random numbers to password-based authentication

Processes. Prevents attackers from reusing stolen authentication data.

1. Limiting Failed attempts: Restricts the number of incorrect login attempts a user can make.

Public Key Infrastructure.

PKI components: An entire system involving hardware, software, policies, procedures and people.  
 

Facilitates secure data transfer, authentication, and encrypted communications.

Benefit:

1. Confidentiality
2. Authentication

Public Key Infrastructure vs. Public Key Cryptography

PKI:

Involves generating, validating, and managing public and private key pairs

that are used in the encryption and decryption process. Ensures the security and trustworthiness of keys.

PCE:

Refers to the encryption and decryption process using public and private

Keys. Only a part of PKI architecture.

Key Escrow: Storage of cryptographic keys in a secure, third-party location (escrow). Enables key retrieval in cases of key loss or for legal investigations.  
  
 

Digital Certificate: Digitally signed electronic documents. Used for individuals, servers, workstations, or devices. X.509 Standard.

Types of Digital Certificate.

1. Wild Card Cert: Allows multiple subdomains to use the same certificate
2. SAN (Subject Alternate Name) Field:

Certificate that specifies what additional domains and IP addresses are

going to be supported

1. Single side and Dual Side: Only requires the server to be validated. Both server and user validate each other
2. Self-Signed:

Digital certificate that is signed by the same entity whose identity it it

certifies

1. Third Party: Digital certificate issued and signed by trusted certificate authorities (CAs).Trusted by browsers and systems

Block Chain:

Is essentially a really long series of information with each block containing

information in it. Each block has the hash for the block before it.

Chain of Block contains:

1. Previous block's hash
2. Time Stamp
3. Root transactions (hashes of individual transactions)
4. Blocks are linked together in a chronological order.

Public Ledger:

1. Secure and anonymous record-keeping system.
2. Maintain participant records
3. Tracks crypto balance.
4. Records all genuine transactions in a network.

Block Chain Apps:

1. Smart Contract
2. Commercial use
3. Supply chain management.

Broad Implications

1. Versatility
2. Decentralization
3. Immutable ledger
4. Digital Evo.

Encryption Tool:

1. Trusted platform module: Dedicated microcontroller for hardware-level security. Used in BitLocker drive encryption for Windows devices.
2. Hardware security Module: Physical device for safeguarding and managing digital keys. Ideal for mission-critical scenarios like financial transactions. Performs encryption operations in a tamper-proof environment.
3. Key management system: Manages, stores, distributes, and retires cryptographic keys. Centralized mechanism for key lifecycle management. Crucial for securing data and preventing unauthorized access.
4. Secure Enclaves: Isolated from the main processor for secure data processing and storage. Safeguards sensitive data like biometric information.

Obfuscation:

1. Steganography: Conceals a message within another to hide its very existence. Involves altering image or data elements to embed hidden information.
2. Tokenization: Substitutes sensitive data with non-sensitive tokens. Original data securely stored elsewhere.
3. Data Masking: Disguises original data to protect sensitive information. Common in industries handling personal data.

Masks portions of sensitive data for privacy, e.g., credit card digits, social

security numbers.

Cryptographic Attack:

Techniques and strategies that adversaries employ to exploit vulnerabilities in

cryptographic systems with the intent to compromise the confidentiality,

integrity, or authenticity of data.

Downgrade attack: Forces the system to use a weaker or older cryptographic protocol. Exploit known vulnerabilities or weaknesses in outdated versions.

Countermeasures include phasing out support for insecure protocols and

version-intolerant checks.

Collision attack:  Find two different inputs producing the same hash output. Vulnerabilities in hashing algorithms, e.g., MD5, can lead to collisions. Birthday Paradox or Birthday Attack.

Quantum computing threats:

computer that uses quantum mechanics to generate and manipulate

quantum bits in order to access enormous processing powers. Uses quantum bits (qubits) instead of using ones and zeros.

NIST selected four post-quantum cryptography standards:

1. CRYSTALS-Kyber - general encryption needs.
2. Digital signatures

CRYSTAL-Dilithium

FALCON

SPHINCS_

Security Architecture:

Ports : Logical communication endpoints on a computer or server.

Inbound and Outbound

Port Classification: 0-1023 ( Well Known Ports)

1024-49151 (Registered Ports IANA)

49152-65535 (Dynamic and Private Ports)

Protocols: Rules governing device communication and data exchange. HTTPs, SMTP, TCP, UDP.

Firewalls:

A network security device or software that monitors and controls network traffic

based on security rules. Protects networks from unauthorized access and potential threats.

  
Screened Subnet (Dual-homed Host):

Acts as a security barrier between external untrusted networks and internal

trusted networks using a protected host with security measures like a

packet-filtering firewall.

Types of Firewall:

1. Packet Filtering Firewall: Inspect packet headers for IP addresses and port numbers. Operates at layer 4 transport layer.
2. Stateful Firewall: Track connections and requests, allowing return traffic for outbound. Operates at layer 4 transport layer.

Requests.

1. Proxy Firewall: Make connections on behalf of endpoints, enhancing security. 2 types a. Circuit level and Application Level
2. Kernel Proxy Firewall:  Minimal impact on network performance, full inspection of packets at

every layer.

Fire wall Evolution:

1. Next Generation Firewall:

- distinguish between different types of traffic
- Conduct deep packet inspection
- Operate fast within minimal network performance impact
- Can integrate with other security products.

1. Unified threat management firewall:

- Combines multiple security functions in a single device.
- Functions include firewall, intrusion prevention, antivirus, and more
- Reduces Number of Devices.
- single point of failure

1. Web application firewall: Focuses on inspecting HTTP traffic.

Prevents common web application attacks like cross-site scripting and SQL

Injections.

Layer Based Firewall:

Layer 4: Operates at transport layer and Filters traffic based on port numbers and protocol data.

Layer 7: Operates at application layer. Filters based on content and data.

Configuring Firewall:

Dedicated devices for using Access Control Lists (ACLs) to protect

Networks.

Access Control List: Consist of permit and deny statements, often based on port numbers. Used by the firewall to secure network from unwanted traffic. Control the flow of traffic into and out of networks.

May define quality of service levels inside networks but are primarily

used for network security in firewalls.

Configuring ACL's:

1. Web based or command line based interface can be used.
2. Order of the ACL rule specifies the order of the action.
3. First matching rule is executed and no other ACL are checked.
4. Specific rules at the top and generic rule at the bottom.

ACL Rules:

1. Type of traffic.
2. Source of traffic
3. Destination of traffic.
4. Action to be taken against the traffic.

Firewall types:

1. Hardware Based:

A dedicated network security device that filters and controls network

traffic at the hardware level

1. Software Based:

A firewall that runs as a software application on individual devices, such

as workstations

Intrusion detection and intrusion prevention:

IDS: Intrusion detection systems: Logs or alerts that it found something suspicious or malicious.

3 types of IDS

1. Network Based: Monitors the traffic coming in and out of a network.
2. Host Based: Monitors the traffic coming in and out of a single endpoint.
3. Wireless IDS: Detects attempt to cause DOS in wireless network.  
    All the IDS function on basis of

4. Signature based
5. Anomalies based

IDP: Intrusion prevention system: Logs, alerts, and takes action when it finds something suspicious or malicious. Scans traffic to look for malicious activity and takes action to stop it.

Network Appliances:

A dedicated hardware device with pre-installed software for specific networking

Services.

1. Load Balancer: Distribute network/application traffic across multiple servers. Enhance server efficiency and prevent overload. Essential for high-demand environments and high-traffic websites.
2. Proxy Server: Act as intermediaries between clients and servers. Enhance request speed and reduce bandwidth usage. Protect against DDoS attacks.
3. Sensors: Monitor, detect, and analyse network traffic and data flow. Identify unusual activities, security breaches, and performance issues.
4. Jump Servers/Jump Box:

Secure gateways for system administrators to access devices in different

security zones. Control access and reduce the attack surface area. Offer protection against downtime and data breaches.

Port Security:

A network switch feature that restricts device access to specific ports based on

MAC addresses.

EAP(Extensible authentication protocol) Frame work for authentication.

1. EAP-MD5:

Uses simple passwords and the challenge handshake

authentication process to provide remote access authentication

1. EAP-TLS:

Uses public key infrastructure with a digital certificate which is

installed on both the client and the server

1. EAP-TTLS: Digital cert is on the server but the client just uses their password.
2. EAP-FAST: Uses protected access credential, instead of a certificate,
3. PEAP: Uses digital cert and AD database to confirm the users pass.
4. EAP- LEAP: Cisco proprietary and limited to cisco device.

Securing Network Communications:  
 

Allow remote users to securely connect to an organization's network

VPN's can be configured,

- Site to Site: Connects two sites cost-effectively. Utilizes a VPN tunnel over the public internet. Slower, but more secure.
- Client to Site: Connects a single host (e.g., laptop) to the central office. Ideal for remote user access to the central network.
- Client less VPN: Uses a web browser to establish secure, remote-access VPN. Utilizes HTTPS and TLS protocols for secure connections to Websites.

1. Full Tunnel: Encrypts and routes all network requests through the VPN. Provides high security, clients fully part of central network. Suitable for remote access to central resources.
2. Split Tunnel: Divides traffic, routing some through the VPN, some directly to

the internet. Less secure; potential exposure to attackers

Transport layer Security: provides encryption and security. Used for secure connection in web browsers. Uses TCP for secure connection.

DTLS( Datagram Transport layer security): Alternate to TLS but this uses UDP. Ensures CIA.

IPSEC( Internet protocol security) A secure protocol suite for IP communication. Provides CIA and anti replay protection. Used for both client to site and site to site VPN.

5 steps in establishing IPSEC

1. Request IKE process
2. Authenticate IKE-1
3. Negotiate IKE-2
4. Data transfer
5. Tunnel Termination.

SD-WAN and SASE:

SD-WAN( Software defined wide network area):

A virtualized approach to managing and optimizing wide area network

Connections.

Software-based architecture with control extracted from underlying

Hardware.  
Ideal for enterprises with multiple branch offices moving towards

cloud-based services.

SASE(Secure Access Service Edge) :

A network architecture combining network security and WAN capabilities in a

single cloud-based service.

Purpose:

Addresses challenges of securing and connecting users and data across

distributed locations.

Key Tech:

Utilizes software-defined networking (SDN) for security and networking

services from the cloud.

Components

● Firewalls

● VPNs

● Zero-trust network access

● Cloud Access Security Brokers (CASBs)

Cloud Providers:

1. AWS VPC
2. Azure Virtual WAN
3. Google cloud Interconnect

Infrastructure Consideration:

1. Device Placement.
2. Security Zone and Screened Subnets.
3. Attack Surface
4. Connectivity Methods
5. Device Attributes
6. Failure Mode: Fail Open and Fail close.

Selecting Infrastructure Controls:  
  
1. Least privilege

2. Défense in depth
3. Risk-based Approach
4. Lifecycle Management.

5. Asses current State.
6. Risk assessment.
7. Baselining
8. Create a frame work
9. Align with a frame work
10. Training.