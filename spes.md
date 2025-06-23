# Jun 23, 2025
+ Powerhint and init uclamp tunning completely redone based on google komodo and redbull
+ Backported zsmalloc from mainline.
+ Backported zram from mainline.
+ Backport usb uvc from mainline
+ zstd: Update zstd to facebook/zstd@c5926fb
  - Merge optimizations from Samsung
+ sched: Implement tapered dvfs_headroom
  - Optimize quadratic headroom calculation
  - Apply quadratic tapering to dvfs headroom
  - Make DVFS headroom capacity-aware and add low-util suppression
+ mm/vmscan: reclaim more pages to find free pages in compaction
  - add a new member reclaim_state in struct shrink_control
  - calculate reclaimed slab caches in all reclaim paths
  - add checks for incorrect handling of current->reclaim_state
  - do not set reclaim_state on soft limit reclaim
+ zram: allow zram to allocate CMA pages
+ Revert "qcacld-3.0: Do not allow any wakelocks to be held"
  - Avoid problems with wifi
