# Mai 28, 2025 
# Clean flash required if on builds before 05/20
- Uprev audio HAL to V7.0
- Optimize SF durations: Significantly reduces visual stutter and lag 
- Bring back some Android Go configs
- Bring back omx avc for encoding only: Improve screen recording performance
- Add "can-swap-width-height" for video codecs | Raise c2.android.avc/hevec decoding limits: fixes thumbnail generation of some videos
