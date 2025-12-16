# Legacy System Intake & Hardware Assessment

## Overview
This lab documents the intake and initial assessment of a legacy desktop system being repurposed for use in a personal IT home lab. The objective was to inventory hardware, verify system condition, and determine suitability for future lab use (Linux, troubleshooting practice, or controlled legacy scenarios).

This task mirrors real-world IT asset intake performed during:
- New device onboarding
- Hardware refresh projects
- Legacy system migrations
- Lab or training environment preparation

---

## Objectives
- Perform a structured intake of legacy hardware
- Document BIOS configuration and system specifications
- Identify constraints and risks associated with legacy components
- Determine appropriate next steps for integration into the home lab

---

## Environment
- **System Type:** Legacy Desktop PC
- **Use Case:** Home lab / learning environment
- **Status:** Non-production

---

## Hardware Summary
| Component | Details |
|--------|--------|
| Motherboard | ASRock N68C-S UCC |
| CPU | AMD Athlon II X2 255 (64-bit) |
| Memory | 4 GB DDR3 (2 × 2 GB, dual-channel) |
| Storage | 500 GB WD SATA HDD + 500 GB Hitachi SATA HDD |
| Optical | DVD Writer |
| BIOS | American Megatrends v02.67C |
| Expansion | PCIe + legacy PCI slots |

---

## Evidence & Documentation
Photos captured during intake are stored under the `assets/` directory:

- BIOS system overview
- BIOS boot configuration
- Internal case layout
- Motherboard and chipset
- RAM modules
- Installed storage devices

These images provide visual verification of configuration and condition.

---

## Findings & Observations
- System uses legacy BIOS (non-UEFI)
- Hardware supports both DDR2 and DDR3 memory (board-specific feature)
- CPU and chipset suitable for lightweight Linux distributions
- No Secure Boot or modern firmware security features
- Mechanical drives show age and should be treated as non-critical

---

## Risks & Limitations
- Hardware is not suitable for modern Windows versions
- No TPM or UEFI support
- Aging storage increases failure risk
- Limited performance headroom

---

## Outcome
The system was accepted into the home lab inventory as a **legacy training asset**. No immediate remediation was required. The device is suitable for:
- Linux installation
- Hardware troubleshooting practice
- BIOS/boot diagnostics labs
- Legacy OS experimentation (isolated)

---

## Next Steps
- Perform SMART diagnostics on storage
- Decide on target OS (Linux distribution)
- Wipe and re-partition disks
- Document OS installation as a follow-up lab

---

## Related Documentation
- `ticket-legacy-system-intake.md` — Detailed intake ticket and step-by-step actions
