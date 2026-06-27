# Troubleshooting Notes

## Issue

Quick Scan button unavailable.

### Resolution

Verify Microsoft Defender Antivirus is enabled.

---

## Issue

No Defender Operational logs generated.

### Resolution

Run a new Quick Scan.

Refresh Event Viewer.

---

## Issue

Operational Log empty.

### Resolution

Navigate to:

Applications and Services Logs

→ Microsoft

→ Windows

→ Windows Defender

→ Operational

Ensure the correct log is selected.

---

## Issue

Protection History empty.

### Resolution

Complete at least one Defender scan.

Refresh Windows Security.

---

## Issue

No Event ID 1001 present.

### Resolution

Allow the scan to finish completely before reviewing logs.

---

## Issue

Event Viewer not updating.

### Resolution

Press Refresh (F5).

Or reopen Event Viewer.

---

## Lessons Learned

- Defender scans generate useful operational telemetry.
- Event Viewer provides deeper visibility than the Windows Security dashboard.
- Operational Logs are valuable for SOC investigations.
- Protection History and Event Viewer complement each other during incident validation.
