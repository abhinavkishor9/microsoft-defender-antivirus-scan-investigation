# microsoft-defender-antivirus-scan-investigation

## Overview

This project demonstrates how Microsoft Defender Antivirus generates security telemetry during a Quick Scan and how those events can be investigated using Windows Event Viewer.

The lab focuses on understanding Defender Operational Logs, Event IDs, scan results, and protection history from a SOC analyst perspective.

---

## Objectives

- Perform a Microsoft Defender Quick Scan
- Monitor scan progress
- Review Protection History
- Investigate Windows Defender Operational logs
- Analyze Defender Event IDs
- Understand Defender security telemetry

---

## Lab Environment

| Component | Value |
|-----------|-------|
| Operating System | Windows 10 x64 |
| Security Product | Microsoft Defender Antivirus |
| Log Source | Windows Defender Operational |
| Investigation Tool | Event Viewer |
| Hypervisor | VMware Workstation |

---

# MITRE ATT&CK Mapping

| Technique | ID |
|-----------|----|
| Indicator Removal (Monitoring Security Events) | T1070 |
| System Information Discovery | T1082 |
| Security Software Discovery | T1518.001 |

---

# Investigation Workflow

1. Launch Windows Security
2. Open Virus & Threat Protection
3. Start a Quick Scan
4. Observe scan progress
5. Wait for scan completion
6. Review Protection History
7. Open Event Viewer
8. Navigate to:

Applications and Services Logs

→ Microsoft

→ Windows

→ Windows Defender

→ Operational

9. Review generated Defender events
10. Document findings

---

# Event IDs Observed

| Event ID | Meaning |
|----------|---------|
| 1000 | Scan Started |
| 1001 | Scan Completed |
| 1002 | Threat Detected (if applicable) |
| 2000 | Signature Update |
| 5007 | Defender Configuration Changed |

---

# Key Findings

- Defender successfully completed a Quick Scan.
- No threats were detected.
- Scan events were successfully logged.
- Protection History matched Operational Log entries.
- Event Viewer provides detailed scan metadata including Scan ID, Scan Type, Scan Time, and User.

---

# Skills Demonstrated

- Microsoft Defender Antivirus
- Windows Security
- Windows Event Viewer
- Defender Operational Logs
- Event Log Analysis
- Threat Investigation
- Security Monitoring
- SOC Investigation Workflow

---



## Learning Outcome

This lab demonstrates how a SOC Analyst validates Microsoft Defender activity using native Windows security telemetry and operational logs without requiring Microsoft Defender for Endpoint or Microsoft Sentinel.
