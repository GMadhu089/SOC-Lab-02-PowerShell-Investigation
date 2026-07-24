# SOC-Lab-02-PowerShell-Investigation
## Overview

This project demonstrates how to investigate PowerShell execution using Microsoft Sysmon logs collected in Splunk. The objective is to understand normal and suspicious PowerShell behavior, perform threat hunting, create detection rules, and document the findings like a SOC Analyst.

---

## Objectives

- Monitor PowerShell execution
- Investigate parent-child process relationships
- Detect hidden PowerShell execution
- Detect Base64 encoded commands
- Detect PowerShell download activity
- Perform threat hunting using Splunk SPL
- Create detection rules
- Map activities to MITRE ATT&CK

---

## Lab Environment

| Component | Technology |
|-----------|------------|
| SIEM | Splunk Enterprise |
| Endpoint Logging | Sysmon |
| Operating System | Windows 11 |
| Investigation Tool | Splunk Search |
| Attack Simulation | PowerShell |

---

## Skills Demonstrated

- Log Analysis
- Threat Hunting
- Detection Engineering
- Windows Internals
- PowerShell Investigation
- MITRE ATT&CK Mapping
- Incident Response

---

## Project Structure

```
SOC-Lab-02-PowerShell-Investigation/

README.md

Attack-Simulation.md

Investigation.md

Detection.md

MITRE.md

Incident_Report.md

Lessons_Learned.md

Queries/
```

---

## MITRE ATT&CK Techniques

- T1059.001 – PowerShell
- T1027 – Obfuscated/Encoded Files
- T1105 – Ingress Tool Transfer

---

## Author
Gampanapalli Madhu
