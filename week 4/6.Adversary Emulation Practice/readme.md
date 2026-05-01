#  Adversary Emulation Practice

##  Overview
This task simulates real-world adversary behavior using MITRE Caldera and evaluates detection capabilities using Wazuh.

---

##  Objective
- Simulate spearphishing attack (MITRE ATT&CK T1566)
- Test SOC detection and alerting
- Identify detection gaps

---

##  Tools Used
- MITRE Caldera
- Wazuh

---

##  Emulation Details

The adversary emulation was conducted using MITRE Caldera to simulate a spearphishing attack (T1566). The attack involved delivering a malicious payload through a phishing scenario and monitoring endpoint behavior.

---

##  Detection Log

| Timestamp           | TTP   | Detection Status | Notes                  |
|---------------------|------|------------------|------------------------|
| 2026-04-30 17:00:00 | T1566 | Detected         | Phishing email blocked |

---

##  Analysis

- Wazuh successfully detected the phishing attempt
- Alert triggered based on suspicious activity patterns
- Endpoint protection prevented payload execution

---


##  Conclusion

The emulation demonstrated that Wazuh can detect basic spearphishing attempts. However, improvements are needed in log correlation, threat intelligence integration, and deeper visibility into email-based attacks to enhance detection accuracy and response effectiveness.
