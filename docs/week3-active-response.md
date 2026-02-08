# Week 3: Active Response

## Attack Simulation
- Type: SSH Brute Force
- MITRE ATT&CK: T1110.001
- Tool: Hydra

## Configuration
\`\`\`xml
<active-response>
  <command>firewall-drop</command>
  <rules_id>2502,5710,5711,5712</rules_id>
  <timeout>3600</timeout>
</active-response>
\`\`\`

## Results
- Detection: < 15 seconds
- Response: < 5 seconds
- Effectiveness: 100% (IP blocked)

**Gate Check**: ✅ PASSED
