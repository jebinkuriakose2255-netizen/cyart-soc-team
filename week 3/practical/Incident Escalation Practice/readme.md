1. Escalation Simulation (TheHive)

A high-priority security alert was simulated involving unauthorized access to a system.

Case Details
Title: Unauthorized Access on Server-Y
Severity: High
TLP: Amber
Status: In Progress
Assigned To: Tier 1 Analyst → Escalated to Tier 2
100-Word Escalation Summary

A high-priority security incident involving unauthorized access to Server-Y was detected at 13:00 on 2025-08-18. The activity originated from IP address 192.168.1.200 and is associated with MITRE ATT&CK technique T1078 (Valid Accounts). Initial analysis confirmed suspicious login behavior indicating potential credential misuse. Immediate containment actions were taken by isolating the affected server to prevent further compromise. No lateral movement has been observed at this stage. The case has been escalated to Tier 2 for deeper investigation, including log correlation, credential auditing, and validation of system integrity to ensure no persistence mechanisms remain active.

📸 Screenshot Recommendation (VERY IMPORTANT)
✅ Screenshot 1: TheHive Case Overview

Include:

Case title
Severity = High
Status = In Progress
Description (your summary visible)
/screenshots/thehive_case_overview.png
✅ Screenshot 2: Tasks / Escalation

Include:

Task: "Escalate to Tier 2"
Status: Pending or Completed
/screenshots/thehive_tasks.png
📄 2. SITREP (Situation Report)
Title

Unauthorized Access on Server-Y

Summary

A security incident involving unauthorized access was detected on Server-Y at 13:00 on 2025-08-18. The activity originated from IP address 192.168.1.200 and is associated with MITRE ATT&CK technique T1078 (Valid Accounts), indicating possible credential compromise.

Actions Taken
Server-Y isolated from the network
Incident escalated to Tier 2
Monitoring initiated for suspicious activity
📸 Screenshot Recommendation
✅ Screenshot 4: Google Docs SITREP

Include:

Title visible
Summary section
Actions section
/screenshots/sitrep_doc.png
⚙️ 3. Workflow Automation (Splunk Phantom)

A simple SOAR playbook was created to automate escalation.

Playbook Logic
Trigger: High-priority alert
Condition: Severity = High
Action: Assign case to Tier 2
Example Flow
If Severity == High → Assign to Tier 2 Analyst
Test Result
Mock alert triggered
Automatically assigned to Tier 2
Workflow executed successfully
