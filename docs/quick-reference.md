# Quick Reference

## Essential Commands

### View Alerts
\`\`\`bash
sudo tail -f /var/ossec/logs/alerts/alerts.log
sudo grep "syscheck" /var/ossec/logs/alerts/alerts.log
\`\`\`

### Check Agents
\`\`\`bash
sudo /var/ossec/bin/agent_control -l
\`\`\`

### Active Response
\`\`\`bash
sudo iptables -L INPUT -n | grep DROP
sudo tail /var/ossec/logs/active-responses.log
\`\`\`

### Dashboard
- URL: https://192.168.23.132
- User: admin
