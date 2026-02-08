<div align="center">

# 🛡️ Wazuh EDR Project
### Enterprise Security Operations Center

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Wazuh](https://img.shields.io/badge/Wazuh-4.7.5-blue)](https://wazuh.com/)
[![Platform](https://img.shields.io/badge/Platform-Ubuntu%20%7C%20Windows%20%7C%20Kali-orange)](https://github.com)
[![Status](https://img.shields.io/badge/Status-Complete-success)](https://github.com/phantom16/wazuh-edr-project)

**Enterprise-grade Endpoint Detection & Response system with real-time threat detection**

[Features](#-features) • [Architecture](#-architecture) • [Installation](#-installation) • [Results](#-results)

---

![Week 1](https://img.shields.io/badge/Week%201-Infrastructure-success?style=for-the-badge)
![Week 2](https://img.shields.io/badge/Week%202-FIM-success?style=for-the-badge)
![Week 3](https://img.shields.io/badge/Week%203-Active%20Response-success?style=for-the-badge)
![Week 4](https://img.shields.io/badge/Week%204-Threat%20Detection-success?style=for-the-badge)

</div>

---

## 🌟 Overview

Production-grade **Security Operations Center** built with **Wazuh SIEM**. This 4-week project demonstrates enterprise security monitoring, real-time threat detection, and automated incident response.

### 🎯 Key Achievements

✅ Real-time Security Monitoring  
✅ File Integrity Monitoring (FIM)  
✅ Automated Threat Response  
✅ Ransomware Detection  
✅ MITRE ATT&CK Mapping  
✅ Zero False Positives

---

## ✨ Features

### 🔍 Detection
- **File Integrity Monitoring** - Real-time alerts (< 5s latency)
- **Process Monitoring** - Sysmon integration
- **Authentication Monitoring** - SSH brute force detection

### ⚡ Response
- **Automated IP Blocking** - Response in < 15 seconds
- **Custom Scripts** - Flexible automation
- **Threat Intelligence** - MITRE ATT&CK mapping

### 🛡️ Compliance
PCI DSS • HIPAA • NIST 800-53 • GDPR

---

## 🏗️ Architecture

\`\`\`
           ┌──────────────────────┐
           │  Wazuh Manager       │
           │  192.168.23.132      │
           └──────┬───────────────┘
                  │
       ┌──────────┼──────────┐
       │          │          │
  ┌────▼────┐ ┌──▼───┐ ┌────▼────┐
  │Windows  │ │ Kali │ │ Future  │
  │Agent +  │ │Agent │ │ Agents  │
  │Sysmon   │ │      │ │         │
  └─────────┘ └──────┘ └─────────┘
\`\`\`

---

## 🚀 Quick Start

### Install Manager
\`\`\`bash
curl -sO https://packages.wazuh.com/4.7/wazuh-install.sh
sudo bash ./wazuh-install.sh -a
\`\`\`

### Install Windows Agent
\`\`\`powershell
msiexec.exe /i wazuh-agent.msi /q WAZUH_MANAGER='<IP>'
NET START WazuhSvc
\`\`\`

---

## 📊 Results

| Metric | Target | Achieved | Status |
|:-------|:------:|:--------:|:------:|
| FIM Latency | < 10s | **< 5s** | ✅ |
| Response Time | < 30s | **< 15s** | ✅ |
| False Positives | < 5% | **0%** | ✅ |
| Uptime | > 95% | **100%** | ✅ |

### Stats
📊 Events: **800+** | 👥 Agents: **3/3** | 🚨 Alerts: **50+** | 🛡️ Blocked: **24** | ⚡ Response: **12s**

---

## 🎯 MITRE ATT&CK

| ID | Technique | Detection | Status |
|:---|:----------|:----------|:------:|
| T1110.001 | Brute Force | Auth correlation | ✅ |
| T1059.001 | PowerShell | Sysmon ID 1 | ✅ |
| T1486 | Data Encrypted | FIM mass changes | ✅ |
| T1485 | Data Destruction | FIM deletions | ✅ |

---

## 📚 Documentation

- [Complete Summary](docs/Project2_Complete_Summary.md)
- [Active Response Guide](docs/Week3_Active_Response_Guide.md)
- [Quick Commands](docs/Week3_Quick_Commands.md)

---

## 📄 License

MIT License - Copyright (c) 2026 Phantom16

---

## 👤 Author

<div align="center">

### **Phantom16**

[![GitHub](https://img.shields.io/badge/GitHub-phantom16-181717?style=for-the-badge&logo=github)](https://github.com/phantom16)

**Cybersecurity Professional | SIEM Specialist**

</div>

---

<div align="center">

### ⭐ Star this repository if it helped you!

**Built with ❤️ for Cybersecurity**

**[⬆ Back to Top](#-wazuh-edr-project)**

</div>
