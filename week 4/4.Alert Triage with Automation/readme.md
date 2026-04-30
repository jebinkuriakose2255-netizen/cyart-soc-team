Alert Triage with Automation Report

Objective

The objective of this task is to perform alert triage using Wazuh and automate threat validation through integration with VirusTotal and TheHive. This ensures faster identification of malicious activity and reduces manual effort in the SOC workflow.

Tools Used

Wazuh (SIEM for alert detection)

VirusTotal (Threat intelligence platform)

TheHive (Incident response & case management)

Triage Simulation (Wazuh)

Alert Details

Alert ID	Description	Source IP	Priority	Status

005	File Download	192.168.1.102	High	Open

Analysis

A high-priority alert was triggered due to a suspicious file download

The activity originated from 192.168.1.102

The alert indicates potential malware delivery or unauthorized download

Immediate validation is required to determine the file’s legitimacy

Automated Validation (TheHive + VirusTotal)

Workflow

Alert generated in Wazuh

Alert forwarded to TheHive

File hash extracted from the alert

TheHive automatically queries VirusTotal

Results attached to the case for analyst review

Validation Summary (50 words)


The suspicious file’s hash was automatically analyzed using VirusTotal through TheHive integration. Multiple antivirus engines flagged the file as malicious, confirming a potential threat. Automation enabled rapid validation without manual lookup, improving triage efficiency and allowing the SOC team to quickly initiate containment and remediation actions.

Outcome

Threat successfully validated using automation

Reduced manual workload for SOC analysts

Faster decision-making and response time

Improved accuracy in identifying malicious files

✅ Conclusion

The integration of Wazuh, TheHive, and VirusTotal enabled efficient alert triage and automated threat validation. This workflow enhances SOC capabilities by reducing response time and ensuring consistent handling of security alerts.
