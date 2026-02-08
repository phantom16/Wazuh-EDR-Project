# Week 2: File Integrity Monitoring

## Configuration

**Monitored Paths**:
- Windows: `C:\test-fim`
- Linux: `/tmp/test-fim`

## Results
- Detection time: < 5 seconds
- Alerts: File creation, modification, deletion
- False positives: 0%

## Test Commands
\`\`\`bash
echo "test" > /tmp/test-fim/test.txt
echo "modified" >> /tmp/test-fim/test.txt
rm /tmp/test-fim/test.txt
\`\`\`

**Gate Check**: ✅ PASSED
