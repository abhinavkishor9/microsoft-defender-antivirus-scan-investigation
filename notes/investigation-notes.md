# Investigation Notes

## Objective

Validate Microsoft Defender Antivirus scan activity through Windows Security and Windows Event Viewer.

---

## Scan Details

Scan Type:
Quick Scan

Status:
Completed Successfully

Threats Found:
0

Protection History:
Reviewed Successfully

---

## Event Viewer Location

Applications and Services Logs

→ Microsoft

→ Windows

→ Windows Defender

→ Operational

---

## Important Event IDs

### Event ID 1000

Quick Scan Started

---

### Event ID 1001

Quick Scan Finished Successfully

Observed Information:

- Scan ID
- Scan Type
- Scan Parameters
- Scan Time
- User

---

### Event ID 5007

Windows Defender configuration changed.

Usually generated when Defender settings are modified.

---

### Event ID 2000

Security intelligence update.

---

## Investigation Findings

No malware detected.

Quick Scan completed successfully.

Protection History matched Operational Logs.

Operational logs contained detailed scan metadata.

Windows Defender logging was functioning correctly.

---

## Analyst Conclusion

The endpoint successfully completed a Microsoft Defender Quick Scan.

No indicators of malware were observed.

Windows Defender Operational logs provided sufficient telemetry to validate scan execution and completion.

The endpoint remained in a healthy security state throughout the investigation.
