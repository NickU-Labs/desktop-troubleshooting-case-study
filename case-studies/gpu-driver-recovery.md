# Case Study: GPU Driver Failure and Recovery

## Summary

This case study documents a Windows desktop system where the GPU was detected by the BIOS
but failed to function correctly within Windows due to driver loading errors.

The issue presented as severe system lag, missing GPU metrics, and display instability.

---

## Initial Symptoms

- Extremely choppy system performance
- GPU graphs missing from Task Manager
- Display adapters showing driver errors
- Secondary monitor no longer detected
- Error Code 31: Windows cannot load the required drivers

---

## Environment

- GPU: AMD Radeon RX 6800
- OS: Windows 10/11
- Display: HDMI primary monitor
- Recent hardware troubleshooting performed (RAM isolation)

---

## Troubleshooting Process

### 1. Verification in Device Manager
- Confirmed GPU listed under Display adapters
- Observed driver error (Code 31)
- Verified system was not using Microsoft Basic Display Adapter

### 2. Performance Confirmation
- Confirmed severe lag inconsistent with normal GPU operation
- Verified missing GPU utilization metrics in Task Manager

### 3. Driver Recovery
- Downloaded latest AMD GPU drivers
- Reinstalled drivers cleanly
- Rebooted system after installation

---

## Outcome

- GPU fully detected and functional
- Normal system responsiveness restored
- GPU metrics returned in Task Manager
- Display stability restored on primary monitor

---

## Key Takeaway

Hardware instability and driver failures can overlap.
Resolving underlying hardware issues first allows accurate diagnosis
of GPU driver-related problems.
