# Jan 28, 2026
- Improved scheduler and memory management (Again)
- Fix multiple memory leaks from latest build
- Another cleanup of debug/unused drivers in kernel
- Fixed battery indicator issue in maxim
- Show LTE icon instead of 4G
- Kernel builded with full LLVM and the latest AOSP clang 22.0.1

# Dec 27, 2025
- Kernel fully reworked, based on the qcom_8250 and Antennae kernel
- Improved overall system stability, scheduler efficiency, memory management, and power consumption
- Disable high performance transitions
- Restrict 60fps video recording to SD and HD on camera 0 (Aperture only)
- Fix wakeups denials
- Fine-tune foreground cpuset
- December security patch 
- Clone apps added
- Enable AOD wallppaper

# Dec 14, 2025
- Enable 60 fps video record suporte in Aperture
- Switch to common QCOM AIDL bootctrl HAL
- Switch to Lineage Power hal
- Tune F2FS and dirty writeout policy
- Some issues in the PixelOS source have been fixed, like the lock screen pattern and custom ROM detection by some apps.

# Dec 07, 2025
- Android QPR1 update
- Use LZ4 for EROFS compression for improved decompression speed
- Set readahead_size_kb=128 for relevant partitions to reduce memory pressure
- Disabled some hwui/sf debug properties
- Downscale task snapshots to 70% for better performance.
- Fixed sound/ringtone when using headphones
- Updated all Xiaomi drivers to the latest Antennae HEAD, resolving multiple issues including thermal and fast charging.
- Improved Simple LMK memory management

# Nov 25, 2025 (HotFix)
- Fix battery indicator in the syv variant.

# Nov 24, 2025
- Backport fuse-bpf, afs and nfs from k5.10
- Update xiaomi drivers from Antennae kernel (power, custom_project, usb, audio)
- Add Kcompressd for accelerated memory compression
- Switch main partitions to EROFS
- Introduce per-app reflesh rate
- Fix sunlight and anti-flicker mode not working
- Some minor changes to the XiaomiParts UI

# Out 31, 2025
- Fixed charging control
- Fixed codecs-related issues (like video and screen recording lags, etc)
- Fixed doze-related issues (like offline charging and AOD)
- Fixed palm sensor and other sepolicy denials
- Update Xiaomi drivers from Antennae kernel (power supply, usb and pstore)
- Several new upstream/backports on the kernel side (tbl, zram, bpf, sched, IncrementalFS, etc)
- Fixes issues with memory management and scheduler (Like black screen during deepsleep and extreme lags due to memory pressure)
- Bring SurfaceFlinger offsets from google redbull and latch all buffers 
