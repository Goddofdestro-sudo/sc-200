---
title: Phishing Analysis
updated: 2026-05-11 10:34:06Z
created: 2026-04-14 12:33:04Z
---

Types of Phishing Emails.  
  
Reconnaissance (Recon) Emails

- Purpose: To verify if a mailbox is active and monitored, preparing for future phishing attacks.

- Types:

1. Spam Recon: Emails with random text (e.g., “adjdfkaweasda”) designed only to check for delivery success by triggering or avoiding bounce-back errors.
2. Social Engineering Recon: Emails impersonating known contacts or authority figures, using vague or urgent language to provoke a reply or engagement. Examples include messages like “Have you read the meeting notes yet?” or fake managerial requests.
3. Tracking Pixel Recon: Emails containing invisible HTML tracking pixels that load an external resource when opened, revealing if and when the email was viewed, the recipient’s device type, location (via IP), email client, and screen resolution. This helps attackers understand how actively the mailbox is monitored.

- Outcome: Confirmed active mailboxes can be sold or used for targeted phishing.

Credential Harvesters

- Goal: To steal usernames and passwords by tricking victims into submitting credentials into fake login portals.
- Characteristics:

- Often impersonate trusted services (e.g., Amazon, Microsoft Outlook, DHL).
- Use authentic branding, logos, and layouts copied from official websites to increase credibility.
- Use social engineering to create urgency or fear (“Your account will be locked!”).
- URLs may be suspicious: random domains, sub-domain impersonation (e.g., amazonupdates.sytes.net), or direct IP addresses instead of domain names.
- Stolen credentials are either saved on the phishing site or emailed to attacker-controlled accounts on free mail services.

- Risks: Stolen credentials can lead to account takeover, fraud, blackmail, or further internal compromise (business email compromise).
- Detection: Look for suspicious URLs, minor spelling errors, and unsolicited credential requests.

Social Engineering

- Definition: Using psychological manipulation rather than technical exploits to trick individuals into unsafe actions.
- Common Tactics in Phishing:

- Impersonation of trusted colleagues or high-ranking executives.
- Creating urgency, fear, or authority pressure to bypass critical thinking.
- Convincing users to reply, transfer funds, or disclose confidential info.

- Purpose: To exploit human trust and override normal security behavior, leading to actions that compromise security (sharing passwords, releasing sensitive data).
- Note: Nearly all phishing involves social engineering since it targets people, not just systems.

Vishing and Smishing

- Smishing: Phishing via SMS or text messages.

- Often sent in bulk with generic messages.
- Target sensitive personal info (PII) or financial data (PCI).
- Example: Fake PayPal alert with URL like paypal.verification-procedure[.]com instead of paypal.com.
- Defense: Awareness training, avoiding clicking unknown links, and using anti-bot SMS filters.

- Vishing: Phishing via phone calls (voice).

- Attackers impersonate executives or authority figures to obtain sensitive info or authorize actions like payments.
- Targets often mid-level employees with financial or system access.
- Defense: Security training, verifying callers, using internal codes, and blocking suspicious calls.

Whaling

- Definition: Highly targeted phishing attacks aimed at senior executives (CEO, CFO, COO).
- Characteristics:

- Use open-source intelligence (OSINT) to craft credible, personalized emails.
- May request confidential info, credentials, or to download malware.
- Sent in small volume to avoid detection by spam filters.

- Risks: Executives’ access to sensitive data or financial transactions makes this very damaging.
- Mitigation:

- Special training for executives and their assistants.
- Email markings to flag external messages.
- Strict policies like data loss prevention (DLP) and separation of duties.
- Assistants trained to filter and report suspicious emails.

Spam

- Definition: Bulk unsolicited emails, often non-malicious such as marketing, newsletters, or updates.
- Examples: Cryptocurrency ads, product promotions, adult content, and COVID-19 PPE offers.
- Key Points:

- Not inherently malicious but can clutter mailboxes.
- Can be abused as recon if unsubscribe links are clicked, confirming mailbox activity or leading to fingerprinting websites.
- Malicious spam (malspam) differs — it delivers malware or malicious payloads at scale.

- Advice:

- Avoid interacting with links or attachments in unsolicited spam.
- Forward suspicious emails to security teams for analysis and deletion.

Tacti's And Technique used.

Spear Phishing

- Definition: Targeted phishing where the attacker researches the victim to craft personalized, convincing emails.
- Method: Uses OSINT to gather info on the target’s websites, hobbies, colleagues, friends, etc.
- Goal: Increase likelihood of victim clicking links, opening malicious attachments, or divulging credentials.
- Techniques: Incorporates social engineering and impersonation for realism.
- Example: Attacker finds an employee on LinkedIn → collects data from Facebook → sends a tailored email with a malicious attachment to gain remote access.
- Impact: Highly effective, often leads to major data breaches.

Impersonation

- Definition: Pretending to be a trusted person (colleague, manager, CEO) to manipulate the target.
- Effectiveness: Exploits authority bias — victims comply quickly, fearing consequences.
- Example: Attacker poses as CEO, instructing finance to transfer funds to attacker’s account.
- Use: Often combined with spear phishing to increase trust and urgency.

Typosquatting & Homographs

- Typosquatting:

- Fake domains mimic legitimate ones by slight misspellings (e.g., securitybllue.team instead of securityblue.team).
- Used to create fake websites and emails to deceive users.
- Organizations may preemptively register similar domains to prevent abuse.

- Homographs:

- Use visually identical but different Unicode characters (e.g., Latin ‘o’ vs Cyrillic ‘о’) in domain names.
- Extremely hard for users to detect by sight.
- Used in internationalized domain names (IDN).
- Requires technical defenses beyond user awareness training.

- Example: Attackers register dicksonunted.co.uk to impersonate DicksonUnited.co.uk, then send phishing emails appearing to be from internal HR.

Sender Spoofing

- Definition: Faking the "From:" email address to appear as a trusted sender.
- How it works: SMTP protocol allows any "From:" address; no built-in verification.
- Common use: Credential harvesting by impersonating internal IT or known companies.
- Example 1: Email appears from ServiceDesk@DicksonUnited.co.uk, tricks employee into entering credentials.
- Example 2: Uses a fake Reply-to address so replies go to attacker-controlled mailbox, not the spoofed domain.
- Detection: Check sending IP address and Reply-to header for inconsistencies.
- Defenses: SPF, DKIM, and DMARC email authentication standards.

HTML Styling in Phishing Emails

- Use: Makes phishing emails look professional and brand-consistent using logos, buttons, colors, and tables.
- Effect: Increases trust and likelihood victim interacts with the email.
- Common elements:

- <a> for hyperlinks
- <table> for layout
- <b>, <i>, <u> for text formatting

- Email encoding: Often Base64 encoded to obfuscate content.
- Tools: Use CyberChef or similar to decode Base64 and analyze email content.
- Example: Amazon credential harvester email mimics official styling to trick victims.

Attachments in Phishing

Types of Attachments:

- Non-malicious files used for social engineering: Like fake invoices or forms, designed to trick recipients into providing info or taking action.
- Non-malicious files containing malicious hyperlinks: For example, PDFs or Word docs with embedded links that lead to malware or phishing sites.
- Malicious files: Often Microsoft Office documents with macros that execute malware if enabled.

Key tactics:

- Attackers use social engineering tactics like urgency or authority to pressure victims into opening attachments or enabling macros.
- Macros are often disabled by default; attackers try to convince users to “Enable Content.”

Hyperlinks

- Hyperlinks can redirect users to malicious sites for credential theft or malware download.
- Techniques include:

- Redirecting to typo-squatted domains.
- Using URL shortening services to obscure the real destination.

- Training users to hover over links to reveal real URLs helps, but attackers also obfuscate links in attachments.

URL-Shortening Services

- Attackers use services like Bitly to hide malicious URLs.
- Security teams can analyze shortened URLs without clicking, using tools like WannaBrowser or URL preview services.
- URL shorteners often use HTTP 301 redirects, revealing the final destination.

Use of Legitimate Services

- Attackers leverage trusted platforms (e.g., Gmail, Outlook, Dropbox, Google Drive) to bypass email filters.
- Hosting malicious documents on cloud services improves credibility.
- Using email marketing platforms (MailGun, MailChimp) can help mass send phishing emails that avoid blacklists.

Business Email Compromise (BEC)

- BEC attacks impersonate trusted business email accounts (usually executives).
- They often result in financial loss or sensitive data exposure.
- Very difficult to detect as they can bypass many email security controls.

Artifacts to collect:  
  
 

Phishing Email Investigation: Key Artifacts to Collect

1. Email Artifacts

- Sending Email Address:

- The address the email claims to be from
- Important even if spoofed for searching related emails

- Subject Line:

- Useful for searching/blocking similar phishing emails

- Recipient Email Addresses:

- Identify all targeted mailboxes (check BCC too)
- Warn affected users

- Sending Server IP & Reverse DNS:

- Identify sending server IP address
- Perform reverse DNS lookup to verify server legitimacy

- Reply-To Address:

- May differ from sending address
- Captures replies for attacker-controlled account

- Date & Time:

- Timestamp of email
- Helps identify timing patterns and campaign scope

2. File Artifacts

- Attachment Name:

- Filename and extension useful for blocking files

- SHA256 Hash:

- Unique cryptographic hash of the file
- Used for reputation checks (VirusTotal, Talos)
- Preferred over MD5/SHA1

3. Web Artifacts

- Full URLs:

- Copy exactly from email (right-click > Copy Link or from email source)
- Avoid mistakes during analysis

- Root Domain:

- Helps identify if domain is malicious or legitimate but compromised

Why Collect These Artifacts?

- Enables thorough investigation
- Helps block similar phishing emails and files
- Shares intelligence with other teams
- Tracks campaign reach and attacker infrastructure

Manual Collection - Email Artifacts (Phishing Investigation)

Why Manual Collection?

- To gather important info about phishing attacks.
- Used to search for other related emails and take defensive actions.
- Always analyze suspicious emails in a virtual machine (VM) or a “dirty” system to avoid risks.

Artifacts Easily Retrieved from Email Clients:

- Sending Address
- Subject Line
- Recipients (unless hidden in BCC)
- Date & Time Sent

Example: Using Outlook or Thunderbird

Retrieving Additional Artifacts Using a Text Editor:

- Download the email in .eml or .msg format.
- Open with a text editor like Sublime Text.
- Use search (CTRL+F) to find:

1. Sending Server IP (X-Sender-IP):

- Search for “IP” to locate X-Sender-IP.
- This shows the IP address of the mail server that sent the email.

3. Reverse DNS Lookup:

- Use tools like [Domain Tools](https://whois.domaintools.com/) to convert IP to hostname.
- Helps verify if the IP matches the sending domain or if spoofing occurred.

5. Reply-To Address:

- Search for “reply” to find where replies to the email will be sent.
- Often different from sending address in spoofed emails.

Summary: Artifacts You Can Manually Extract from Suspicious Emails

- Sending Address
- Subject Line
- Recipient(s)
- Date and Time
- Sending Server IP
- Reverse DNS lookup of Sending Server IP
- Reply-To Address (if present)  
      
     

Manual Collection - Web Artifacts (Phishing Investigation)

What Are Web Artifacts?

- Hyperlinks in phishing emails redirecting users to malicious sites.
- Can point to fake login pages or malware-hosting sites.
- Key artifacts to collect:

- Full URL (complete web address as sent in the email)
- Root Domain (main domain name without specific pages)

Collecting Web Artifacts from Email Clients (Outlook, Thunderbird)

- Hover over the hyperlink text to reveal the URL.
- Right-click the hyperlink and select “Copy Hyperlink” to copy the URL safely.
- Caution: Avoid clicking the link accidentally—always analyze emails in a VM or isolated system.

Collecting Web Artifacts from a Text Editor

- Open the email file (.eml or .msg) in a text editor (e.g., Sublime Text).
- Use CTRL+F to search for URLs by:

1. Searching for “http” to find all HTTP/HTTPS URLs.
2. Searching for <a> tags in the HTML code that define hyperlinks.
3. Searching for the hyperlink text visible in the email (e.g., "you can cancel it").

- Copy the full URL directly from the text editor without risk of accidental clicks.

Summary:

- Full URL and Root Domain are the critical web artifacts to extract.
- Use email clients for quick copying but be cautious.
- Use text editors for safer, more controlled extraction of URLs.
- Always perform analysis in a secure environment (VM or isolated system).

Manual Collection - File Artifacts (Phishing Investigation)

Why Collect File Hashes?

- File hashes uniquely represent a file’s content.
- Even a small change in the file changes the hash completely.
- Hashes are used to:

- Perform reputation checks online.
- Block or detect malicious files in security tools like Endpoint Detection and Response (EDR).

Common Hash Algorithms

- SHA256 (current security standard, preferred)
- SHA1 (older, less secure)
- MD5 (older, prone to collisions)

Generating File Hashes on Windows (PowerShell)

- Use the command:  
      
    powershell  
    CopyEdit  
    Get-FileHash <file>

- By default, returns SHA256 hash.

- To specify algorithm (MD5 or SHA1):  
      
    powershell  
    CopyEdit  
    Get-FileHash <file> -Algorithm MD5  
    Get-FileHash <file> -Algorithm SHA1
- To get all three hashes at once:  
      
    powershell  
    CopyEdit  
    Get-FileHash <file> -Algorithm MD5; Get-FileHash <file> -Algorithm SHA1; Get-FileHash <file> -Algorithm SHA256

Generating File Hashes on Linux (Command Line)

- SHA256:  
      
    bash  
    CopyEdit  
    sha256sum <file>
- SHA1:  
      
    bash  
    CopyEdit  
    sha1sum <file>
- MD5:  
      
    bash  
    CopyEdit  
    md5sum <file>

Key Points

- SHA256 is recommended for modern security tools and online reputation checks.
- Knowing how to generate all three hashes helps in using different tools and services.
- Always generate file hashes before further analysis or sharing indicators.

Report Writing:  
 

Email Header, Artifacts, and Body Content

- Collect artifacts (IOCs) from emails for linking attacks, identifying actors, and trend analysis.
- Include artifacts clearly in reports for easy lookup and sharing.
- Key Email Header Artifacts:

- Sending Email Address
- Reply-to Address
- Date Sent
- Sending Server IP + Reverse DNS
- Recipient(s)
- Subject Line

- URLs: Sanitize and list full URLs or root domains.
- Attachments: Filename + extension and file hashes (MD5, SHA256).
- Attach the full email file (.eml/.msg) to investigations, include brief description and screenshot in reports.
- Write 1–2 sentence descriptions about email appearance and intent (social engineering tactics, urgency, etc.).

Analysis Process, Tools, and Results

- Divide into URL Analysis and Attachment Analysis.
- Use tools: WHOIS, VirusTotal, URL2PNG, Talos File Reputation, sandbox detonations.
- WHOIS: Check domain age, registrar, owner info.
- VirusTotal/Talos: Check if artifacts flagged malicious.
- URL2PNG: Visualize fake login pages or malware hosting sites.
- Provide clear justification of risk and impact of artifacts.
- Document tools and methods used, results, and assessment of threat level.

Defensive Measures Taken

- Defensive measures block repeated attacks post-analysis:

- Email artifact blocking (sender, subject, IP)
- Web artifact blocking (URLs, domains, IPs)
- File artifact blocking (file names, hashes)

- Some analysts can apply blocks directly; others request it through escalation.
- Reports must state actions taken, reasons, and accountability (who, when).
- Examples include:

- Blocking suspicious subject lines if sender IP/domain can’t be blocked due to legitimate use.
- Blocking malicious domains hosting credential harvesters or malware downloads.
- Blocking sending addresses if no legitimate business impact expected.

Artifact Sanitization (Defanging)

- Sanitize URLs/IPs in reports to prevent accidental clicks or execution.
- Replace "." with "[.]" and "http" with "hxxp".
- Example:

- 8.8.8.8 → 8[.]8[.]8[.]8
- [https://example.com](https://example.com) → hxxp[://]example[.]com

- Tools like CyberChef can automate defanging.
- Essential for safe sharing and documentation within organizations.