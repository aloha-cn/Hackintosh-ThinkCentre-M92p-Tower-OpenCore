# Hackintosh Big Sur Guide for ThinkCentre M92p Tower (OpenCore 0.6.3)

![Snapshot](images/snapshot.png)

### Hardware

Type|Item
:----|:----
**HDD** | SATA SSD
**GPU** | NVIDIA GT 720 1GB (Kepler core)
**WiFi + BT Combo** | BCM943602CS + PCIe Adaptor

### Current Driver Versions and Links
https://github.com/acidanthera/OpenCorePkg/releases/download/0.6.3/OpenCore-0.6.3-RELEASE.zip
https://github.com/acidanthera/Lilu/releases/download/1.4.9/Lilu-1.4.9-RELEASE.zip
https://github.com/acidanthera/WhateverGreen/releases/download/1.4.4/WhateverGreen-1.4.4-RELEASE.zip
https://github.com/acidanthera/AppleALC/releases/download/1.5.4/AppleALC-1.5.4-RELEASE.zip
https://github.com/acidanthera/IntelMausi/releases/download/1.0.4/IntelMausi-1.0.4-RELEASE.zip
https://github.com/acidanthera/VirtualSMC/releases/download/1.1.8/VirtualSMC-1.1.8-RELEASE.zip
(For HfsPlus.efi)
https://github.com/acidanthera/AppleSupportPkg/releases/download/2.1.7/AppleSupport-2.1.7-RELEASE.zip

## Instructions
### 1. BIOS Settings
* Enable UEFI boot and disable CSM mode
* Disable secure boot
* Enable VTx and disable VTd
### 2. Prepare installation media 
https://dortania.github.io/OpenCore-Install-Guide/extras/big-sur/
### 3. Modify 'config.plist' for your own serial number, UUID, MLB, ROM, etc.
### 4. Copy 'BOOT' and 'OC' directories to the EFI partition.  
### 5. Optional Settings
* Enable SSDT.aml for CPU PM according to your own CPU
[See the Guide](https://github.com/Piker-Alpha/ssdtPRGen.sh)
* Configure IGPU if you don't use dGPU
* Configure NVMe drive if you don't use SATA

### Notice
##### BIOS can't do UEFI boot from HDD. My solution is plugging an extra usb stick for booting.

