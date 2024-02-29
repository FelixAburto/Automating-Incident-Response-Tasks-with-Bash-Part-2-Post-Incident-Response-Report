<h1>Post Incident Response Report</h1>



<h2>Description</h2>

A post-incident response report is a comprehensive document compiled after an incident, like a security breach or technical failure, to analyze and understand the event. Here we will create an incident response report based on the previous project


<h2>Attempted Access of Confidential File Report</h2>

- **Date of the Report:** 02-25-2023
- **Incident Name/Number**: Incident #812
- **Report Author**: Felix Aburto

<h2>Executive Summary</h2>

This report presents a detailed analysis of a recent security incident that involved unauthorized access to a confidential file within our organization's network. The incident was contained and mitigated with minimal impact, showcasing the effectiveness of the preparation and automated response measures. The incident in question was initiated by a phishing attack, leading to the employee downloading a malicious PDF. This resulted in the unauthorized installation of a backdoor on the employee's system. The attacker gained access to the system via OpenSSH and attempted to compromise a confidential file. However, due to security measures and efficient automated response mechanisms, the attack was quickly detected and effectively contained. This report outlines how the incident was managed, highlighting the rapid activation of our automated Bash scripts designed for incident response. These scripts played a pivotal role in restricting the attacker's access and preserving the integrity of our systems and data. The containment was achieved with minimal disruption to our operations and without any significant data loss or compromise. The lessons learned and recommendations derived from this incident will further strengthen our security posture and resilience against future threats.

<h2>Incident Description</h2>

- **Date and Time of Incident**: 02-24-2023 03:35 PM CT
- **Location**: Financial Office of XYZ Company
- **Description**: An employee inadvertently downloaded a malicious PDF file, leading to the installation of a backdoor on their system. A malicious actor gained access via OpenSSH and attempted to access a confidential file.
- **Parties Involved**: Employee, Security Analyst, Malicious Actor
- **Assets Affected**: Employee's system, Confidential file

<h2>Timeline of Events</h2>

- **02-24-2023 03:35 PM CT**: Employee downloads and opens malicious PDF.
- **02-24-2023 03:38 PM CT**: Trojan installed and backdoor opened.
- **02-24-2023 10:18 PM CT**: Malicious actor accesses the system via OpenSSH.
- **02-24-2023 10:32 PM CT**: Actor attempts to access and copy the confidential file.
- **02-24-2023 10:33 PM CT**: File integrity monitor script triggered.
- **02-24-2023 10:34 PM CT**: Malicious actor's further access attempts failed.

<h2>Impact Assessment</h2>

- **Operations**: Minimal disruption due to Immediate detection and response.
- **Financial Implications**: Negligible, due to effective containment.
- **Data Integrity**: No evidence of data compromise or loss. Hash value of confidential file remains the same.

<h2>Response Actions</h2>

- **Immediate Actions**: Automated script initiated password change and network shutdown on the affected system. It also immediately collected necessary data for further analysis.
- **Incident Response Team Actions**: Analysis of automated logs and system forensics. Analysis of phishing email, restored system from known good backup, corrected user account privileges, blocked ssh traffic to the system, removed Openssh from the system, secured root access to system, blocked sender email address of the phishing email.
- **Stakeholder Communication**: Incident reported to management and IT security.

<h2>Root Cause Analysis</h2>

- **Cause**: Download of a malicious PDF from a phishing email.
- **Vulnerabilities**: Employee's lack of awareness about phishing, inadequate restrictions on administrator privileges, and unprotected root access.

<h2>Lessons Learned and Recommendations</h2>

- **Employee Training**: Enhance awareness programs on phishing and cybersecurity threats.
- **Privilege Restrictions**: Limit administrator privileges and secure root account access.
- **Monitoring and Response**: Continue improvement of monitoring tools and automate more response actions.

<h2>Appendices</h2>

- **Audit Logs**: Details of unauthorized access attempts.
- **System Logs**: Bash history, IP connection logs, and Hash values of confidential file.
- **Incident Response Scripts**: Automated response Bash scripts.

<h2>Approval and Distribution List</h2>

- **Reviewed and Approved By**: SOC Manager, CFO, and Stakeholders
- **Distributed To**: IT Security Team, Management, and Others

