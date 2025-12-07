# Phillip's Home Lab

## Day 01 – Initial Inspection & Hardware Baseline

**Device Name**: HomeLab-01  
**Host Name**: desktop01-homelab  
**Purpose**: CompTIA A+ Core 1 & Core 2 hardware and operating system practice

### 1. Initial Inspection & Safety Procedures

The system was removed from a cold storage environment and required inspection prior to power-on. Visible dust and debris were present internally, indicating that cleaning and preventive maintenance would be required before continued use.

All work was performed using proper ESD-safe handling procedures, including:
- Working on an ESD mat
- Regularly grounding by touching the power supply chassis
- Avoiding contact with exposed circuitry where possible

The device was reported by the client to have previously functioned as a home office PC running Windows 7. At the time of inspection, it was unknown which storage device contained the operating system.

#### Security & Risk Considerations

Because the system previously ran an unsupported operating system (Windows 7), this poses:
- A security risk if connected to any active network
- A contamination risk for home lab or testing environments

A fresh operating system installation and/or network isolation will be required before further use.

### 2. System Specifications (Hardware Baseline)

#### Motherboard
- **Model**: ASRock N68C-S UCC
- **Firmware Type**: Legacy BIOS (AMI)
- **BIOS Version**: P1.40
- **Era**: ~2009–2011

**Notes:**
- No UEFI support
- No Secure Boot
- SATA II (3.0 Gb/s) support
- DDR3 memory support only

#### CPU (Processor)
- **Manufacturer**: AMD
- **Model**: Athlon II X2 255
- **Cores / Threads**: 2 cores / 2 threads
- **Architecture**: 64-bit
- **Clock Speed**: 3.1 GHz
- **Cache**:
    - L1: 256 KB
    - L2: 2048 KB

**Notes:** This CPU supports basic 64-bit operating systems but is unsuitable for modern virtualization or high-performance workloads.

#### Memory (RAM)
- **Total Installed**: 4 GB
- **Configuration**: Dual-channel
- **Type**: DDR3 DIMM (desktop)
- **Speed**: DDR3-1333 (667 MHz ×2)
- **Voltage**: 1.5 V

**Per Module**
- **Brand**: Kingston ValueRAM (KVR)
- **Model**: KVR1333D3N9/2G
- **Capacity**: 2 GB × 2
- **CAS Latency**: CL9

**Slots Used**
- DDR3_A1 – 2 GB
- DDR3_B1 – 2 GB

### 3. Storage Devices Identified

#### PATA (IDE) Hard Disk Drive
- **Manufacturer**: Western Digital
- **Series**: Caviar Blue
- **Model**: WD5000AAKB
- **Capacity**: 500 GB
- **Interface**: PATA / IDE
- **Cache**: 16 MB
- **Power Connector**: Molex

**Use Case:** Legacy storage identification, cabling practice, and A+ exam reference.

#### SATA Hard Disk Drive
- **Manufacturer**: Hitachi (HGST)
- **Model**: HDS721010CLA332
- **Capacity**: 1 TB
- **Form Factor**: 3.5-inch
- **Type**: Mechanical HDD
- **Interface**: SATA II (3.0 Gb/s)
- **Speed**: 7200 RPM
- **Cache**: 16 MB
- **Power Connector**: SATA power
- **Manufacture Date**: May 2010

**Use Case:** Primary lab storage device for OS installation and SATA troubleshooting.

### 4. Optical Drive
- **Type**: CD/DVD Drive
- **Manufacturer**: TSSTcorp (Samsung / Toshiba joint venture)
- **Interface**: SATA
- **BIOS Status**: Detected as first boot device

**Use Case:** Legacy OS installation and boot-order configuration practice.

### 5. Integrated Components

#### Graphics
- **Type**: Integrated chipset-based graphics
- **Shared Memory**: 256 MB (system RAM)
- **Output**: VGA

**Use Case:** Basic display output for BIOS and OS installation.

#### Audio
- **Type**: Integrated onboard audio
- **Typical Codec**: Realtek HD Audio

#### Networking
- **Type**: Integrated Ethernet NIC
- **Interface**: RJ-45
- **Speed**: Likely 10/100 or Gigabit Ethernet

### 6. Power & Cooling

#### Power Supply Unit (PSU)
- **Form Factor**: ATX
- **Connectors Observed**:
    - 24-pin ATX motherboard power
    - 4-pin CPU power
    - SATA power
    - Molex power

**Notes:** Exact wattage and model not yet verified.

#### Cooling
- **CPU Cooling**: Stock AMD air cooler
- **Case Cooling**: Standard chassis fan(s)

### 7. Other Observations & System Notes
- **CMOS Battery**: CR2032 (likely depleted or near end-of-life)
- **Boot Mode**: Legacy BIOS
- **Disk Partition Style**: MBR (not GPT)
- **USB Support**: USB 2.0

### 8. Learning Outcomes – Day 01

This lab session reinforced several essential fundamentals:
- Proper ESD-safe workstation preparation
- Importance of validating unknown or legacy systems
- Identifying hardware limitations before OS selection
- Understanding BIOS constraints (Legacy BIOS vs UEFI)
- Recognizing security risks associated with unsupported operating systems

This process emphasized the importance of planning, documentation, and risk assessment before performing upgrades or configuration changes.

### 9. Upgrade & Future Planning Considerations

To meet the requirements of CompTIA A+ Core 1 & Core 2 training:
- An SSD upgrade is recommended for performance and OS reliability
- Dual-boot configurations are technically possible but limited by hardware
- Virtual machines are not practical on this system due to CPU and RAM limitations

For more advanced learning (Network+ or CCNA), this system would need to be supplemented with:
- Additional PCs or laptops
- A managed switch and router
- Network isolation from production systems

### 10. Next Steps
- Replace CMOS battery (CR2032)
- Perform full interior cleaning
- Set BIOS date/time correctly
- Change boot order for USB installations
- Decide between SSD replacement or dedicated lab OS install
