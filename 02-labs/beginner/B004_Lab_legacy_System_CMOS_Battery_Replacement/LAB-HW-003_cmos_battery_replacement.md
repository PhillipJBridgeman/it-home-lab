# IT Service Ticket – CMOS Battery Diagnosis & Replacement

**Ticket ID:** LAB-HW-003  
**Category:** Hardware → Motherboard → CMOS / RTC  
**Priority:** Low  
**Status:** Planned / Pending Replacement  
**Environment:** Home Lab / Legacy Desktop System  
**Requested By:** Client (Approved)  
**Technician:** Phillip Bridgeman  
**Date Opened:** 2025-12-24  
**Related Tickets:**  
- LAB-HW-001 – Memory Upgrade & Validation  
- LAB-OS-002 – Ubuntu 22.04 LTS Installation & Storage Reconfiguration  

---

## 📝 Summary

The system clock and date were observed to reset after power loss, indicating a failing or depleted CMOS (RTC) battery. This condition impacts system time accuracy, BIOS configuration persistence, and can affect OS time synchronization and security certificates.

---

## 🖥️ System Details

- **Motherboard:** ASRock N68C-S UCC  
- **BIOS Version:** P1.40  
- **Processor:** AMD Athlon II X2 255 (64-bit)  
- **Installed Memory:** 8 GB DDR3 (Dual Channel)  
- **Operating System:** Ubuntu 22.04.5 LTS  
- **System Type:** Legacy BIOS (Non-UEFI)

---

## 🔍 Issue Observed

- System date/time resets after power-off
- BIOS clock does not retain correct time
- Manual date/time correction required on boot
- Screenshot evidence confirms incorrect system date

---

## 📸 Evidence Collected

- BIOS System Overview screen showing incorrect date/time  
- Ubuntu OS date corrected only after network time sync  
- No BIOS setting changes persist across power cycles

*(Screenshots retained in `/evidence/LAB-HW-003/`)*

---

## 🧠 Root Cause Analysis

The CMOS (RTC) battery is no longer providing sufficient voltage to retain BIOS configuration data when the system is powered off.

This is consistent with:
- System age
- Legacy motherboard platform
- Typical CR2032 battery lifespan (3–7 years)

---

## 🛠️ Planned Resolution

1. Power down system and disconnect AC power
2. Discharge residual power
3. Open chassis and locate CMOS battery
4. Remove existing CR2032 battery
5. Install new CR2032 lithium coin cell
6. Boot system and re-enter BIOS
7. Set correct system date/time
8. Save BIOS configuration
9. Power off system for validation
10. Confirm date/time retention on subsequent boot

---

## ✅ Expected Outcome

- BIOS date/time retained across reboots
- No further clock resets after power loss
- Improved system stability and reliability
- Elimination of time-related OS warnings or sync issues

---

## ⚠️ Risk & Impact Assessment

- **Risk:** Minimal
- **Downtime:** < 10 minutes
- **Data Impact:** None
- **User Impact:** None

---

## 📚 Learning Outcomes (CompTIA A+ Alignment)

- CMOS battery purpose and failure symptoms
- BIOS/RTC time dependency
- Hardware maintenance best practices
- Preventative maintenance documentation
- Legacy system troubleshooting

---

## 📌 Notes

This task supports continued use of the system for:
- CompTIA A+ studies
- Linux administration practice
- Home lab experimentation

---

**Next Action:** Replace CMOS battery and update ticket status to *Resolved*
