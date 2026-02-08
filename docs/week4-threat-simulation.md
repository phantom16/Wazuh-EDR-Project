# Week 4: Ransomware Detection

## Sysmon Integration
- Version: 15.15
- Events: Process Creation (ID 1)

## Simulation
\`\`\`powershell
1..50 | ForEach-Object {
    "ENCRYPTED_$_" | Out-File "file_$_.encrypted"
}
\`\`\`

## Results
- FIM Alerts: 50+ 
- Detection: Rapid file encryption
- Sysmon: PowerShell execution logged

## MITRE ATT&CK
- T1486: Data Encrypted for Impact
- T1485: Data Destruction  
- T1059.001: PowerShell

**Gate Check**: ✅ PASSED
