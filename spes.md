# Mai 01, 2025
- Import lmkd props from fogona for less overhead
- Increase offroad audio buffer size to 256kb for fix audio stuttering
- Rebase in device tree kernel, removing unwanted overlays, problematic commits...
- Align cpusets with crosshatch
- Align default rate limit values ​​with Google devices
- Restrict max CPU freq to critical hints
- Merge latest 'lineage-20' of https://github.com/LineageOS/android_kernel_qcom_sm8250
- Demote unwanted logging to debug
- Fixes and updates for binder drivers
- Switch to aidl health hal

# April 17, 2025
- Optimize and checkout binder to android14-5.15
- Merge latest 'android-4.19-lts' of https://github.com/frstprjkt/kernel-lts (4.19.331)
- Merge latest 'lineage-20' of https://github.com/LineageOS/android_kernel_qcom_sm8250
- Kernel device tree completely rebased, fixing issues and deleting unwanted commits
- Add timeout for power supply wakelocks, prevent them from crashing and breaking idle
- Return to default lmkd configs

# Apr 01, 2025
- Recalculate dynamic power coefficients and update dmips for big.LITTLE cores
- Undervolt GPU
- Fixed Kernel panic when using gadget functions, like MTP, USB Thethering...
- Pick power supply driver updates/fixes from the most up-to-date Antennae source
- Dont force LTE+, now works without hacks
- Optimize powerhal for better performance and efficiency
- Merged PixelOS release source

# March 28, 2025
- Import most updated Carrier Config from vauxite
- Set Zstd as the default compression algorithm for ZRAM
- Updated Zstd to upstream release 1.5.7 
- Some fixes/optimizations in the scheduler (EEVDF, delayed dequeue, wakeup-preempt...)
- LTE+ working fine
- Update Certification/Play integrity Overlay
