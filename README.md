## Overview

This document provides instructions for installing, updating, and modifying the ROM.

- **Clean Flash**: required when coming from stock firmware or another ROM.
- **Dirty Flash**: used for OTA or manual updates without wiping data.
- 
Always read the instructions carefully and back up your data before proceeding.

## Requirements
- Unlocked bootloader
- ADB & Fastboot
- ROM package
- Recovery packages (`boot.img`...)

## Clean Flash

Required when flashing from **stock firmware** or **another ROM**.

### Steps
1. Boot into **fastboot**
2. Flash recovery images:
```bash
fastboot flash vendor_boot vendor_boot.img
fastboot flash boot boot.img
```
3. Reboot to recovery:
```bash
fastboot reboot recovery
```
4. Factory reset:
```
Main Menu > Factory Reset > Format Data / Factory Reset > Format Data
```
5. Reboot to recovery
6. Apply update:
```
Apply Update > Apply from ADB
```
7. Flash ROM from sdcard or adb:
```bash
adb sideload rom.zip
```
8. Reboot

---

## Dirty Flash / Update

For updates **without wiping data**. Backups recommended.

### OTA

1. On your device, navigate to:
```
Settings > System > System Updater > Check for updates
```
2. If an update is available, download and install it.

### Recovery
1. Boot into recovery
2. Apply update:
```
Apply Update > Apply from ADB
```
3. Flash ROM from sdcard or adb:
```bash
adb sideload rom.zip
```
4. Reboot
