# IT Service Ticket – Storage Diagnostic & RAID Evaluation

---

## Ticket Information

- **Ticket ID:** LAB-STOR-RAID-001  
- **Category:** Hardware → Storage → RAID / HDD  
- **Priority:** Medium  
- **Status:** Pending External Diagnostics  
- **Reported By:** Phillip Bridgeman  
- **Assigned Technician:** Phillip Bridgeman  
- **Date Opened:** December 12, 2025  
- **Last Updated:** December 12, 2025  

---

## Summary

An 8TB SATA hard disk drive previously configured as part of a RAID 1 (mirrored) dual-bay NAS was reported in a degraded state. This ticket documents the evaluation process used to determine whether the drive remains serviceable, should be restricted to non-critical use, or should be securely decommissioned.

---

## Environment Details

- **System Type:** Home lab / learning environment  
- **Primary OS:** Windows 7 (legacy, offline)  
- **Boot Drive:** 500GB PATA HDD  
- **Secondary Storage:**
  - 1TB SATA HDD (planned Linux installation)
  - 8TB SATA HDD (former RAID 1 member – degraded)
- **RAID Configuration:** RAID 1 (mirror)  
- **Device Origin:** Dual-bay NAS (SOHO class)  
- **Network Status:** System kept offline / air-gapped during diagnostics  

---

## Problem Description

The NAS reported one member of a RAID 1 mirror as degraded, prompting removal of the affected 8TB HDD. At the time of removal, it was unclear whether the degraded status resulted from:

- Physical disk failure  
- RAID metadata inconsistency  
- NAS controller behavior  
- Transient read/write errors  

An independent, standalone disk health assessment was required prior to reuse or disposal.

---

## Risk & Impact Assessment

| Risk Area | Assessment |
|---------|------------|
| Data Loss | Low (RAID 1 redundancy previously in place) |
| Hardware Failure | Unknown prior to diagnostics |
| Security Risk | Mitigated by offline testing |
| Improper Reuse | Mitigated by SMART analysis |
| Cost Impact | Evaluation preferred over immediate replacement |

---

## Scope of Work

1. Isolate the HDD from the RAID configuration  
2. Perform physical inspection  
3. Test drive independently (non-RAID)  
4. Collect SMART health data  
5. Determine serviceability and disposition  

---

## Actions Performed

### 1. Hardware Isolation
- System powered down and ESD precautions observed  
- 8TB SATA HDD removed from NAS / RAID environment  
- Drive labeled for identification and tracking  

### 2. Standalone Drive Configuration
- HDD connected directly via SATA to test system  
- BIOS inspection attempted  
- Verified system booted from existing PATA OS drive  

### 3. Diagnostic Methodology
- **Tool Selected:** CrystalDiskInfo (Portable Edition)  
- **Execution Method:** USB removable media  
- **Network Access:** None (offline testing only)  
- **Rationale:** Avoid exposure of unsupported Windows 7 system to network threats  

---

## Diagnostic Results

⚠️ **SMART diagnostics could not be completed internally**

- Legacy test system (circa 2010) was unable to reliably enumerate the modern NAS-grade 8TB HDD (Seagate IronWolf, ~2020)  
- Behavior consistent with known BIOS and SATA controller limitations on older platforms  
- No write, initialization, formatting, or partition changes were performed  
- Internal SATA testing was discontinued to avoid unreliable results or unintended disk modification  

---

## Assessment

The inability to detect the disk internally is consistent with hardware generation incompatibility rather than confirmed disk failure. RAID 1 rebuild completion confirms data integrity on the surviving mirror member but does not, by itself, indicate physical failure of the removed disk.

Further diagnostics require access to a **supported testing environment** capable of OS-level SMART analysis.

---

## Risk Considerations

- Disk will **not** be used for sensitive or production data  
- No active data loss risk (RAID already rebuilt successfully)  
- Secure handling maintained to prevent accidental damage or data exposure  

---

## Next Steps

One of the following actions will be performed:

### Option 1: External Evaluation
- External SMART health check at a local PC repair shop using a modern system  
- Health assessment only (no wipe)  
- Decision to retain vs decommission based on SMART results  

**OR**

### Option 2: Deferred Testing
- Testing postponed until access to a newer Windows 10 system with UEFI/NVMe is available  

Following SMART evaluation, a final determination will be made to:
- Retain the disk for non-production use  
- Or perform secure wipe and recycle/donate  

---

## Current Status

- Diagnostic phase paused pending access to supported testing resources  
- Drive stored safely in ESD-safe packaging  
- No further action required until external evaluation is completed  

---

## Technician Notes

This evaluation followed a structured troubleshooting methodology emphasizing isolation, evidence-based diagnostics, and risk-aware decision-making. Pausing diagnostics reflects appropriate tooling selection and avoids unsafe assumptions when working with legacy hardware and modern storage devices.

---

## Closure (Pending)

**Final disposition to be recorded following SMART evaluation and execution of recommended action.**
