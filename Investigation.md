### User

Identifies the account that executed PowerShell.

---

### ParentImage

Shows which process launched PowerShell.

Examples

- explorer.exe
- cmd.exe
- winword.exe
- excel.exe
- outlook.exe
- mshta.exe

---

### CommandLine

Shows the complete PowerShell command.

Examples

- Hidden
- -enc
- Invoke-WebRequest
- ExecutionPolicy Bypass

---

### Timeline

Helps reconstruct attacker activity.

---

## Investigation Workflow

1. Search events
2. Verify User
3. Verify Host
4. Verify Parent Process
5. Analyze CommandLine
6. Determine if activity is expected
7. Escalate if suspicious
