# Detection Engineering

## Detection Logic
Alert when PowerShell executes:

- Hidden
- Encoded Commands
- Invoke-WebRequest
- ExecutionPolicy Bypass

---

## Detection Query
```spl
index=sysmon Image="*powershell.exe"

(CommandLine="*-enc*"

OR CommandLine="*Hidden*"

OR CommandLine="*Invoke-WebRequest*"

OR CommandLine="*ExecutionPolicy Bypass*")
```

---

## Severity
High

---

## Alert Schedule
Every 5 Minutes

---

## Possible False Positives

- System Administrators
- Automation Scripts
- Configuration Management Tools

---

## Recommendations

Investigate:

- Parent Process
- User
- Host
- Command Line
- Network Connections
