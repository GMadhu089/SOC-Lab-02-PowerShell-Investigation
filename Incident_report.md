# Incident Report

## Executive Summary

A PowerShell investigation was conducted using Sysmon logs collected in Splunk. Multiple PowerShell executions were analyzed to differentiate normal administrative activity from suspicious behavior.

---

## Timeline

PowerShell Process Created

↓

User Executed Command

↓

Sysmon Logged Event

↓

Splunk Indexed Event

↓

SOC Investigation

---

## Evidence

Collected

- User
- Host
- Parent Process
- Command Line
- Timestamp

---

## Findings

Observed:

- Normal PowerShell execution
- Hidden PowerShell
- Encoded Commands
- Invoke-WebRequest activity

---

## MITRE ATT&CK

- T1059.001
- T1027
- T1105

---

## Analyst Verdict

No malicious payload was executed.

The activities were intentionally generated to simulate attacker behavior and validate detection capabilities.

---

## Recommendations

- Enable Script Block Logging
- Enable Module Logging
- Monitor Parent Processes
- Alert on Encoded Commands
