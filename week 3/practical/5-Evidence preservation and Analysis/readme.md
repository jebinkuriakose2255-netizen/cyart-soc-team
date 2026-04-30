Evidence Preservation and Analysis Report

 Objective

The objective of this task is to collect and preserve volatile and non-volatile evidence from a Windows virtual machine using Velociraptor and ensure integrity through hashing. Proper chain-of-custody procedures are followed.

Tools Used

Velociraptor (DFIR tool for endpoint visibility)
FTK Imager (optional for forensic imaging)
SHA256 hashing utility (sha256sum)
Windows Virtual Machine

Volatile Data Collection

Network Connections Collection

Volatile network connection data was collected using Velociraptor with the following VQL query:

SELECT * FROM netstat()

Output

Data was exported in CSV format
Contains:
Local Address
Remote Address
Ports
Process IDs
Connection State

Purpose

This helps identify:

Suspicious outbound connections
Unknown remote IPs
Potential attacker communication

Memory Acquisition

Artifact Used
Artifact.Windows.Memory.Acquisition

Output

Full memory dump of the Windows VM
Stored securely for forensic analysis

Purpose

Memory dumps help detect:

Malware in memory
Injected processes
Credential artifacts
Suspicious DLLs

Evidence Integrity (Hashing)

The collected memory dump was hashed using:

sha256sum memory_dump.raw

Why Hashing?

Ensures data integrity
Detects any tampering
Required for legal and forensic validation

Chain of Custody

Item	Description	Collected By	Date	Hash Value
Memory Dump	Server-Y Dump	SOC Analyst	2025-08-18	3f5c2a8d9e7b1c4d6a8f0b1234567890abcdef1234567890abcdef1234567890

Replace the hash value with your actual output from sha256sum


Evidence Handling Procedure

Evidence collected from live system using Velociraptor
Data exported and stored in a secure directory
Memory dump generated and preserved
SHA256 hash calculated immediately after collection
Evidence documented in chain-of-custody table
Files stored in read-only format to prevent tampering

Key Observations (Example)

Multiple active connections observed on the system
No suspicious external IPs detected (modify based on your findings)
Memory dump successfully acquired without errors

Conclusion

The evidence collection process was successfully completed following forensic best practices. All collected data has been preserved with integrity and is ready for further analysis such as malware detection or incident investigation.
