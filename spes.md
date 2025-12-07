# Dec 07, 2025
- Android QPR1 update
- Switch to LZ4 for EROFS compression for improved decompression speed
- Set readahead_size_kb=128 for the relevant partitions to avoid memory pressure
- Disables some hwui/sf debug props
- Downscale task snapshots to 70% for better performance.
- Fixed sound/ringtone when using headphones
- Updated all Xiaomi drivers to the latest antenna HEAD, resolving multiple issues including thermal and fast charging.
- Improve Simple LMK memory management

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
