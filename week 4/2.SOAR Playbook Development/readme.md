SOAR Playbook Development Report

Objective

The objective of this task is to design and validate an automated incident response playbook using SOAR principles. The playbook focuses on detecting phishing-related threats and automatically blocking malicious IPs while creating incident tickets for further investigation.

Tools Used

Splunk Phantom (SOAR automation)
TheHive (case management)
Wazuh (alert generation)
CrowdSec (IP blocking)
Google Docs (documentation)
Playbook Overview

Use Case

Automated response to phishing alerts involving suspicious or malicious IP addresses.

🧩 Playbook Workflow
Receive phishing alert from Wazuh
Extract source IP from alert
Check IP reputation (threat intelligence)
If malicious → Block IP via CrowdSec
Create incident ticket in TheHive
Log actions for audit and review

Playbook Test

 Simulation

A phishing alert was simulated in Wazuh with a malicious IP: 10.0.2.12
📑 Execution Results
Playbook Step	Status	Notes
Check IP	Success	IP flagged as malicious
Block IP	Success	CrowdSec blocked 10.0.2.12
Create Ticket	Success	Case created in TheHive

Analysis

The playbook successfully automated the full response workflow
Threat intelligence validation ensured accurate decision-making
No manual intervention was required during execution
Incident response time was significantly reduced

Playbook Summary (50 words)

The SOAR playbook automates response to phishing alerts by validating IP reputation and blocking malicious sources using CrowdSec. It also creates incident cases in TheHive for tracking and investigation. This automation reduces response time, ensures consistency, and enhances overall security operations efficiency with minimal manual intervention.

Conclusion

The SOAR playbook was successfully developed and tested, demonstrating effective automation of phishing incident response. Integration between tools ensured seamless detection, response, and case management, improving SOC efficiency and reducing potential impact.
