## Attack 1 – Normal PowerShell

```powershell
powershell
```

Purpose

Generate a normal PowerShell process creation event.

---

## Attack 2 – Hidden PowerShell

```powershell
powershell -WindowStyle Hidden
```

Purpose

Simulate attackers hiding PowerShell from users.

---

## Attack 3 – Encoded Command

Generate Base64

```powershell
$Text="whoami"

$Bytes=[System.Text.Encoding]::Unicode.GetBytes($Text)

[Convert]::ToBase64String($Bytes)
```

Execute

```powershell
powershell -enc dwBoAG8AYQBtAGkA
```

Purpose

Simulate encoded PowerShell execution.

---

## Attack 4 – Explorer → PowerShell

Win + R

```
powershell
```

Purpose

Observe Explorer launching PowerShell.

---

## Attack 5 – Download Cradle

```powershell
powershell -Command "Invoke-WebRequest https://example.com -UseBasicParsing"
```

Purpose

Generate download-related telemetry without downloading malware.
