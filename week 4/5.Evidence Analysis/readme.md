#Evidence Analysis & Chain-of-Custody

## Overview
This task focuses on analyzing endpoint evidence using Velociraptor and maintaining a proper chain-of-custody record to ensure evidence integrity.

---

##  Objectives
- Analyze network connections from a Windows VM
- Identify suspicious activity
- Document evidence handling process

---

##  Tools Used
- Velociraptor
- FTK Imager

---

##  Evidence Collection

The following Velociraptor query was used to retrieve network connections:

```sql
SELECT * FROM netstat 

