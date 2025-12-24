# IT Service Ticket – OS Migration & Storage Reconfiguration

## Ticket Information
- **Ticket ID:** LAB-OS-STOR-002
- **Category:** Operating Systems → Linux | Storage → Disk Management
- **Priority:** Medium
- **Status:** Closed – Successful
- **Client:** Phillip Bridgeman
- **Technician:** Phillip Bridgeman
- **Environment:** Home Lab / Learning System
- **Date Opened:** 2025-12-21
- **Date Closed:** 2025-12-21

---

## Summary
At the client’s request and with formal approval, the system operating system was migrated to **Ubuntu 22.04 LTS** on a **500 GB PATA hard disk**, and the existing **1 TB SATA hard disk** was fully wiped and repurposed as a **dedicated data volume** for the operating system.

This change improves system security, supports ongoing CompTIA A+ studies, and modernizes the platform for safe internet connectivity.

---

## Business / Technical Justification
The change was approved to:
- Replace unsupported **Windows 7** with a supported, secure OS
- Enable safe network and internet access with current security updates
- Separate **operating system and data storage**, following best practices
- Reuse existing hardware efficiently in a learning environment
- Provide hands-on experience with Linux installation and disk management

---

## Pre-Change System State
- **Primary OS:** Windows 7 (Unsupported)
- **Boot Configuration:** Mixed / inconsistent boot behavior
- **Primary Disk (PATA):** 500 GB – Previously underutilized
- **Secondary Disk (SATA):** 1 TB – Contained legacy Windows 7 NTFS partitions
- **Security Risk:** High (end-of-life OS)

---

## Approved Change
- Install **Ubuntu 22.04 LTS (64-bit)** on 500 GB PATA HDD
- Remove all legacy Windows partitions from 1 TB SATA HDD
- Reformat 1 TB SATA HDD as a Linux-compatible data volume
- Configure system to boot exclusively into Ubuntu

---

## Change Implementation

### Operating System Installation
- Created Ubuntu 22.04 LTS bootable USB
- Installed OS to **500 GB PATA HDD**
- Verified successful installation and system boot
- Confirmed network connectivity and package updates

### Storage Reconfiguration
- Identified disks using `lsblk` and GNOME Disks
- Wiped all NTFS partitions from **1 TB SATA HDD**
- Repartitioned and formatted disk for Linux use
- Mounted disk as a dedicated data volume

---

## Post-Change Validation

### OS Validation
- Ubuntu 22.04 LTS boots successfully
- System receives security and software updates
- Network connectivity verified via LAN
- No dual-boot or legacy Windows entries detected

### Storage Validation
- 1 TB SATA HDD visible to OS
- Disk mounted and accessible
- Confirmed writable data volume
- No legacy Windows data remains

---

## Issues Encountered
- **Legacy Hardware Constraint:** PATA disk results in slower boot times  
  - *Resolution:* Accepted as a hardware limitation; system remains stable and functional
- **Mixed Boot Behavior (Pre-change):** System intermittently attempted to boot Windows  
  - *Resolution:* Removed all Windows partitions and boot records

---

## Outcome & Benefits
- System now runs a **fully supported Linux OS**
- Improved security posture for internet usage
- Clear separation between OS and data storage
- Reduced risk of boot conflicts
- Improved learning environment for Linux and CompTIA A+ studies

---

## CompTIA A+ Alignment
This ticket demonstrates skills aligned with:
- **Core 1 – 2.5:** Storage types and interfaces (PATA vs SATA)
- **Core 1 – 5.2:** Disk partitioning and formatting
- **Core 2 – 1.1:** Operating system installation and configuration
- **Core 2 – 2.2:** Security best practices (removal of unsupported OS)

---

## Change Approval
- **Approved By:** Phillip Bridgeman (Client)
- **Change Type:** Planned
- **Approval Date:** 2025-12-21

---

## Closure Notes
The system is now operating on Ubuntu 22.04 LTS with a clean storage layout. This configuration supports continued learning, safe network access, and future lab expansion.

**Ticket Status:** Closed
