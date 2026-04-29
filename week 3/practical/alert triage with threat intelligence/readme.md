Alert Triage with Threat Intelligence
Overview

This project demonstrates the process of alert triage and IOC validation in a Security Operations Center (SOC). A high-priority alert involving suspicious PowerShell execution was analyzed using Wazuh and validated against external threat intelligence platforms.
Alert Details
Alert ID	Description	Source IP	Priority	Status
004	Suspicious PowerShell Execution	192.168.1.101	High	Open
Analysis

The alert was triggered due to abnormal PowerShell activity, which is commonly associated with malicious scripting and post-exploitation techniques. Given its high severity, the alert was prioritized for immediate investigation.

IOC Validation

The source IP was cross-referenced using:

VirusTotal
AlienVault OTX

Summary:
The IP address did not show strong malicious indicators in threat intelligence databases, suggesting it may belong to a controlled lab environment. However, the suspicious behavior still warrants further investigation.

Triage Decision
Status: Under Investigation
Reason: Suspicious behavior detected despite low external threat intelligence hits
Next Steps:
Analyze endpoint activity
Correlate logs
Monitor for persistence mechanisms
Screenshots
Tool	Description
Wazuh	Alert dashboard showing PowerShell execution
Wazuh	Detailed alert logs
