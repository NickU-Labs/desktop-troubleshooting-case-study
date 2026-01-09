# Case Study: Windows Event Viewer – Kernel-Power Event 41

## Summary

This case study documents the use of Windows Event Viewer to investigate
unexpected system shutdowns and restarts.

Critical Kernel-Power Event ID 41 errors were identified and correlated
with underlying hardware instability rather than power delivery issues.

---

## Initial Symptoms

- Unexpected system shutdowns
- System restarts without warning
- No blue screen or error message
- Errors occurred intermittently (1–2 times per month)

---

## Investigation

### 1. Event Viewer Analysis
- Opened Windows Event Viewer
- Navigated to:
  - Windows Logs → System
- Filtered for **Critical** and **Error** events

### 2. Findings
- Identified repeated **Kernel-Power Event ID 41**
- Event indicated system rebooted without a clean shutdown
- No direct driver or OS fault listed

---

## Correlation and Root Cause Analysis

- Kernel-Power Event 41 indicates **unexpected loss of system stability**
- Event does **not** specify root cause
- Correlated timing with:
  - RAM instability
  - Boot failures in specific RAM slot configurations
  - GPU driver crashes following system instability

---

## Outcome

- Determined Kernel-Power events were **symptoms**, not the cause
- Focus shifted to hardware isolation and memory testing
- Prevented misdiagnosis of PSU or motherboard failure

---

## Key Takeaway

Event Viewer is a diagnostic tool that provides context, not conclusions.
Kernel-Power Event 41 requires correlation with hardware and system behavior
to identify true root causes.
