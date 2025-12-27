# Installation Guides

* **[Clean Installation](#clean-flash-guide-pixelos-spes)**
    * *Required when coming from stock firmware or another ROM.*

* **[Update / Dirty Flash](#dirty-flashupdate-guide-pixelos-spes)**
    * *Used for OTA or manual updates without wiping data*

* **[KernelSU Installation](#kernelsu-guide-pixelos-spes)**
    * *Instructions for flashing the KernelSU patched boot image.*

------------

# Clean flash Guide: PixelOS (spes)

This guide details the clean installation process of **PixelOS 16.1** for the **Redmi Note 11 (spes)**.

> [!WARNING]
> **Important:**
> * Backup your data before proceeding. This process will wipe your internal storage.
> * Ensure your battery is charged above 50%.
> * You are responsible for your device. Follow the steps carefully.

---

## Required Files

Ensure you have downloaded the following files:

1.  **ROM:** `PixelOS_spes-XXX.zip`
2.  **Recovery:** `RECOVERY-PixelOS_spes-XXX.zip`

### File Preparation
Before starting, extract the **RECOVERY** zip file. Locate and copy the following files to your ADB/Fastboot folder:
* `boot.img`
* `vendor_boot.img`
* `dtbo.img`

---

## Installation Instructions

### 1. Boot into Fastboot
Power off the device. Turn it on by holding **Volume Down** + **Power Button** until the Fastboot screen appears.

### 2. Flash Boot Images
Open a terminal (CMD/PowerShell) in the folder where your files are located and run the following commands:

```bash
fastboot flash vendor_boot vendor_boot.img
fastboot flash dtbo dtbo.img
fastboot flash boot boot.img
```

### 3. Reboot to Recovery
While still in Fastboot mode, run:

```bash
fastboot reboot recovery
```

### 4. Factory Reset
Once in Recovery mode, use the Volume buttons to navigate and the Power button to select:

1. Select **Factory Reset**.
2. Select **Format Data / Factory Reset**.

### 6. Apply Update
1.  From the main menu, select **Apply Update**.
2.  Select **Apply from ADB**.

Note: If installing via SDCard, select **Apply from SDCard**, navigate to the file, and skip to step 8.

### 7. Flash ROM
On your computer, run the command below to sideload the ROM file.

```bash
adb sideload PixelOS_spes-XXX.zip
```

Note: The process may stop at 47% on the computer terminal with a success message or "Total xfer: 1.00x". This is normal and indicates the installation is complete.

------------

# Dirty flash/Update Guide: PixelOS (spes)

This guide details how to update **PixelOS** without wiping your personal data.

> [!WARNING]
> **Important:**
> * Although this process preserves data, it is highly recommended to **backup important files** before proceeding.
> * Ensure your battery is charged above 50%.

---

## Method 1: OTA (Automatic)

The easiest way to update is via the system settings.

1.  On your device, navigate to:
    **Settings > System > System Updater**
2.  Tap **Check for updates**.
3.  If an update is available, download and install it following the on-screen prompts.

---

## Method 2: Recovery (Manual via ADB)

Use this method if the OTA fails or if you prefer manual installation.

### 1. Boot into Recovery
Reboot your device into recovery mode (hold **Volume Up** + **Power** during boot, or use the Advanced Restart menu).

### 2. Apply Update
1.  From the main menu, select **Apply Update**.
2.  Select **Apply from ADB**.

### 3. Flash ROM
On your computer, run the command below to sideload the ROM file.

```bash
adb sideload PixelOS_spes-XXX.zip
```

------------

# KernelSU Guide: PixelOS (spes)

This guide details how to flash the KernelSU-patched boot image for **PixelOS 16.1**.

> [!WARNING]
> **Important:**
> * Modifying the boot image carries risks. Ensure you have the original `boot.img` available in case you need to restore it.

---

## Required File

Download the following file:
* **Boot Image:** `KSU-BootImage-PixelOS_spes-XXX.img`

---

## Installation Instructions

### 1. Boot into Fastboot
Power off the device. Turn it on by holding **Volume Down** + **Power Button** until the Fastboot screen appears.

### 2. Flash Boot Image
Open a terminal (CMD/PowerShell) in the folder where the file is located and run:

```bash
fastboot flash boot KSU-BootImage-PixelOS_spes-XXX.img
```

### 3. Reboot
Reboot your device to the system:

```Bash
fastboot reboot
```
