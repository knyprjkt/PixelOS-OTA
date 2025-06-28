# Jun 28, 2025
+ simple_lmk: Lower pressure threshold
  - Reduce lag during heavy multitasking
+ sched/walt: Fix negative count of sched_asym_cpucapacity static key
+ cpufreq: schedutil: Ignore rate limit when scaling up with FIE present
+ cpufreq/sched: Fix the usage of CPUFREQ_NEED_UPDATE_LIMITS
+ cpufreq: schedutil: Fix superfluous updates caused by need_freq_update
+ cpufreq: schedutil: Clean up
+ cpufreq: schedutil: Reduce DVFS headroom boost
+ Merge branch 'lineage-20' of @LineageOS/android_kernel_qcom_sm8250
  - Reapply new patch from upstream kernel
+ spes: sepolicy: Label remaining wakeups nodes
+ spes: Import systemui preopt otimizations from hw pixel
+ spes: Enable R8 optimizations for system_server and SystemUI
+ spes: Remove default dexpreopt compiler filter override
  - 'speed-profile' is the default
  - 'everything' consumes significantly more storage and RAM
+ spes: props: Enable adpf cpu hint session for SurfaceFlinger and HWUI
+ spes: Build sendhint
+ spes: init: Increase zram size
  - Our new kernel allows us to use more zram
+ spes: audio: Load mixer_paths configs properly
