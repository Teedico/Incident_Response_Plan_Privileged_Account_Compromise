# Incident_Response_Plan_Privileged_Account_Compromise

# Sample Incident Response Plan for Fictional Company "Apex Capital"

**Project Overview:**

This repository contains a sample Incident Response Plan (IRP) created as a personal project. "Apex Capital" is a fictional financial institution used for demonstration purposes.

The primary goal of this project is to showcase the structure, components, and procedures involved in creating a formal IRP, with a specific focus on scenarios related to **privileged account compromise**. It includes defining CSIRT roles, outlining detection and analysis steps, detailing containment/eradication/recovery processes, and establishing post-incident activities.

# Incident Response Plan For Apex Capital: Privileged Account Compromise Scenarios

## OVERVIEW

Maintaining trust and meeting regulatory requirements is crucial to protect confidential information and systems against cyber-attacks. Apex Capital's incident response plan aims to quickly and effectively contain cyber threats while ensuring normal business operations. This involves protecting privileged accounts and requires the collaboration of various departments. The plan will be updated regularly to reflect organizational changes, compliance culture, and new technologies, and regular testing will be conducted to ensure preparedness.

## PURPOSE

This plan provides a comprehensive approach to respond to a privileged account compromise, addressing different methods of attack, and ensuring thorough detection, containment, and remediation processes.



## PREPARATION

These preparation steps are crucial to establishing an effective Cybersecurity Incident Response Team and ensuring that Apex Capital is ready to respond promptly and effectively to security incidents. Preparation must be completed *before* an incident.

### 1. Determine the Members of the Cybersecurity Incident Response Team (CSIRT)

**a. Core CSIRT Member Composition:**

The core CSIRT includes members from Information Technology roles and a few roles from various departments for support. This helps maintain confidentiality and efficiency.

**CSIRT Roles, Responsibilities, and Contacts:**

#### Information Security

| ROLES | RESPONSIBILITY | CONTACT DETAILS |
|---|---|---|
| **Chief Information Security Officer** | Develops operational, financial, and technical, risk ranking criteria used to prioritize incident response plans. Authorizes when and how incident details are reported. A primary point of contact for the executive team and Board of Directors. | Seun Matthew <br> 09051120975 <br> Seunmatthew@apex-capital.org |
| **Incident Response Team Lead and Team Members** | A central team that oversees and coordinates incident response across multiple teams and functions through all stages of a cyber incident. <br><br> Maintains incident response plan, documentation, and catalog of incidents. <br><br> Conducts random security checks to ensure readiness to respond to a cyber attack. Responsible for identifying, confirming, and evaluating the extent of incidents. | Ese Brume <br> 08054768572 <br> brumeese@apex-capital.org |
| **Identity and Access Team Lead and Team Members** | Responsible for privilege management, enterprise password protection, and role-based access control. <br><br> Conducts random checks to audit privileged accounts, validate whether they are required, and re-authenticate those that are. <br><br> Monitors privileged account uses and proactively checks for indicators of compromise, such as excessive logins, or other unusual behavior. <br><br> Informs incident response team of potential attacks that compromise privileged accounts, validates and reports on the extent of attacks. <br><br> Takes action to prevent the spread of a breach by updating privileges. | Paul Ike <br> 08143304076 <br> paulike@apex-capital.org |

#### IT Operations and Support

| ROLES | RESPONSIBILITY | CONTACT DETAILS |
|---|---|---|
| **IT Operations and Support (Internal)** | Manages access to systems and applications for internal staff and partners. <br><br> Centrally manages patches, hardware and software updates, and other system upgrades to prevent and contain a cyber incident. | Micheal Nwokeke <br> 08036713523 <br> michealnwokeke@apex-capital.org |

#### Legal, Compliance, HR, Regulatory

| ROLES | RESPONSIBILITY | CONTACT DETAILS |
|---|---|---|
| **Legal Counsel** | Confirms requirements for informing employees, customers, and the public about cyber breaches. <br><br> Responsible for checking in with local law enforcement. <br><br> Ensures the IT team has legal authority for privilege account monitoring. | Kemi Oshinowo <br> 07074696452 <br> kemioshinowo@apex-capital.org |
| **Audit & Compliance** | Communicates with regulatory bodies, following mandated reporting requirements. | Sydney Biose <br> 08067534219 <br> sydneybiose@apex-capital.org |
| **Human Resources** | Coordinates internal employee communications regarding breaches of personal information and responds to questions from employees. | Adenike Ola <br> 08185697166 <br> adenikeola@apex-capital.org |
| **Regulatory Contacts** | Receives information about a breach according to the timeline and format mandated by regulatory requirements. | Chioma Aniekwe <br> 08156723489 <br> chiomaaniekwe@apex-capital.org |

#### Communications

| ROLES | RESPONSIBILITY | CONTACT DETAILS |
|---|---|---|
| **Marketing & Public Relations Lead** | Communicates externally with customers, partners, and the media. <br><br> Coordinates all communications and requests for interviews with internal subject matter experts and security team. <br><br> Maintains draft crisis communications plans and statements which can be customized and distributed quickly in case of a breach. | Chukwuemeka Anthony <br> 07056432134 <br> anthonyemeka@apex-capital.org |
| **Web & Social Media Lead** | Posts information on the company website, email, and social media channels regarding the breach, including our response and recommendations for users. <br><br> Sets up monitoring across social media channels to ensure we receive feedback or questions sent by customers through social media. | sodiq Isah <br> 08045792236 <br> sodiqisah@apex-capital.com |
| **Technical Support Lead (Internal)** | Provides security bulletins and technical guidance to employees in case of a breach, including required software updates, password changes, or other system changes. | Amos Oghenetega <br> 09024657688 <br> amosoghenetega@apex-capital.org |
| **Technical Support Lead (External)** | Provides security bulletins and technical guidance to external users in case of a breach. | Akpan Okon <br> 08123567890 <br> akpanokon@gmail.com |

### 2. Define Escalation Paths

Establish clear escalation paths to ensure incidents are handled efficiently and appropriately. Incidents may begin as low-impact events and escalate as more information is gathered. Clear guidelines should define when and how incidents should be escalated within the organization.

### 3. Ensure Appropriate Logging Levels

**a. Account Login System Components:**
Ensure logging levels for account login systems (such as Active Directory, VPN, and Remote Access) are set to appropriate levels to capture necessary data. A minimum of 90 days of log retention is recommended.

**b. Secure Logging Storage:**
Logs should be stored in secure locations, ideally on a secondary system such as a Security Information and Event Management (SIEM) system. This ensures logs are protected from tampering and can be reliably used during incident investigations.



## DETECTION AND ANALYSIS

1.  Outline how the team initially discovered the attack.
2.  Analyze Security logs for unusual/suspicious account activity to identify potential attacks and confirm if an attack has occurred.
3.  Identify the access point and the source of the attack (e.g., endpoint, application, downloaded malware) as well as the responsible party. Also, search for malware and credential harvesting links, keyloggers, etc.
4.  Apply the information from the method of compromise to identify the sensitive data that the attacker could have accessed. If logs are unavailable, assume the attacker accessed all accessible data.
5.  Describe potential attackers, including their known or expected capabilities, and motivations.
6.  Evaluate Apex Capital's information assets list to identify any potentially compromised assets, and make note of their integrity and any gathered evidence.



## INCIDENT SCENARIOS (Privileged Account Compromise)

### Incident 1

*   **Evidence:** Observed notification of several failed login attempts and the same account repeatedly logging in with different passwords from various IP addresses in the organization's system.
*   **Method of Compromise:** Brute force, credential harvesting phishing, credential scraping from local systems, brute-forced passwords.

| SAMPLE CYBER INCIDENT                                                                 | CIA CATEGORY | PRIVILEGED ACCOUNT BREACH | BUSINESS IMPACT | RISK LEVEL |
| :------------------------------------------------------------------------------------ | :----------- | :------------------------ | :-------------- | :--------- |
| Multiple failed login attempts and logins from various IP addresses with diff passwords. | C, I         | Yes                       | High            | High       |

### Incident 2

*   **Evidence:** Abnormal employee behavior in the workplace and online.
*   **Method of Compromise:** Insider Threat, employee accessing unauthorized/malicious sites, copying large files to external storage, divulging organization confidential information.

| SAMPLE CYBER INCIDENT                                                                                        | CIA CATEGORY | PRIVILEGED ACCOUNT BREACH | BUSINESS IMPACT | RISK LEVEL |
| :----------------------------------------------------------------------------------------------------------- | :----------- | :------------------------ | :-------------- | :--------- |
| Abnormal employee behavior, accessing unauthorized/malicious sites, copying large files, divulging conf info. | C, I         | Yes                       | Medium          | Medium     |

### Incident 3

*   **Evidence:** An email with a phishing link attached to it, spelling errors, inconsistency in email address.
*   **Method of Compromise:** Social engineering, phishing emails, etc.

| SAMPLE CYBER INCIDENT                                                | CIA CATEGORY | PRIVILEGED ACCOUNT BREACH | BUSINESS IMPACT | RISK LEVEL |
| :------------------------------------------------------------------- | :----------- | :------------------------ | :-------------- | :--------- |
| Phishing emails with links, spelling errors, inconsistent addresses. | C            | Yes                       | Medium          | High       |

### Post-Detection Investigation Steps

After finding out how an attacker got in (initial method of compromise), it's essential to:

a.  Apply various tools and methods to monitor the network and system activity, such as intrusion detection systems (IDS), log analysis, firewall rules, and alerts.
b.  Look for signs of unusual or excessive login attempts, failed authentication, or abnormal traffic patterns.
c.  Analyze Apex Capital's employees' behaviors at the workplace and unusual work habits.
d.  Query Apex Capital's email system, consider inputting details such as the email subject name, document name, document hash, URL from the email, and other relevant information logs in account login systems searching for anomalies.
e.  Assess Apex Capital's employees' and victims' accounts thoroughly to determine the presence of sensitive information or their access to sensitive data stored on centralized storage including but not limited to OneDrive, Google Drive, SharePoint, shared mailboxes, and fileservers. This is to comprehensively evaluate the potential exposure of sensitive information. If sensitive information is a possibility, consult Apex Capital's legal counsel for the next steps.



## CONTAINMENT, ERADICATION, AND RECOVERY

### Containment

These steps in containment should be followed cautiously and carried out based on the kind of attack and the response that best handles the compromise.

**IMMEDIATE RESPONSE**

1.  Lock out the compromised account from all systems and applications.
    *   Ensure password resets and multi-factor authentication re-enrollment.
2.  Block any identified phishing URLs, IP addresses, or domains. Implement email filters to detect and block similar phishing attempts.
3.  Restrict account access for privileged user.
4.  Disable or delete any unauthorized accounts, and revoke any access tokens or sessions.
    *   Also, disconnect any devices or services that are not essential for your operations or recovery.
5.  Analyze the attack on the compromised privilege accounts and determine its impact and origin.
    *   This should be done by collecting and preserving evidence, such as logs, files, screenshots, and network packets.

**LONG TERM RESPONSE**

6.  Use forensic tools and techniques to identify the attacker's methods, tools, and goals.
7.  Monitor systems continually to collect data and use artificial intelligence to detect the activities in the compromised account accurately.
8.  If malware is discovered:
    *   I. Save a sample.
    *   II. Analyze using available tools.
    *   III. Get the file hash from compromised system depending on the operating system.
    *   IV. Submit hash to VirusTotal, Hybrid-Analysis, etc.
    *   V. Note malware characteristics.

### Eradication

**Eradication Actions:**

*   Identify the root cause of the malware; phishing, etc.
*   Remove the malicious files and processes identified on the infected systems.
*   Use antivirus and anti-malware tools to scan and clean the affected endpoints.
*   Update all software and apply necessary patches to address vulnerabilities exploited by the attackers.
*   Ensure the latest security updates are installed on all systems.

**Credential Reset:**

*   Reset passwords for compromised accounts and ensure multi-factor authentication (MFA) is enforced.
*   Monitor for any suspicious account activities post-incident.
*   Disable the compromised account and isolate affected systems.
*   Scan and clean affected systems using antivirus and anti-malware tools.
*   Close firewall ports and network connections that were used during the attack.

### Recovery

*   Apply the latest security patches and software updates to address vulnerabilities exploited by the attackers.
*   Return any systems that were taken offline to production. Close network access previously used by the attackers and reset passwords for affected accounts.
*   Download and apply the latest security patches to address any vulnerabilities exploited during the incident.
*   Conduct a vulnerability analysis to ensure that all identified issues have been resolved.
*   Inform employees about the recovery process and any changes made.
*   Share recovery information externally through appropriate channels.
*   Continue to monitor for any signs of malicious activity related to the incident to ensure that the threat has been fully eradicated.



## POST-INCIDENT

1.  Evaluate the cost of the incident.
2.  Discuss the following questions and document the information for future reference.
    *   a. Discuss what went well during the investigation.
    *   b. Identify areas that did not go well during the investigation.
    *   c. Determine any vulnerabilities or gaps in the organization's security and how to address them.
    *   d. Explore additional steps or actions that could have helped prevent the incident.
    *   e. Consider whether modifications must be made to existing protocols or procedures.
3.  Update the incident response plan.
4.  Maintain robust application security Operating System and Application patching procedures.
5.  Conduct Employee, IT, or CSIRT Training.
6.  Create and distribute an incident report to relevant parties.
7.  Document all information and more technical reports for the CSIRT.
8.  Document and present an executive summary of the incident to the management team.
