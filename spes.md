# Jun 14, 2025 
## This update requires you to install your keybox manually in order to have Play Integrity working, I will make keyboxes available in my telegram group.
+ Checkout binder to d53a061 from android13-5.10
+ Revert phase offsets as duration
   - This caused out-of-order buffer errors and jank at 90Hz due to lack of matching high-fps timing.
+ Switch to new XiaomiParts
   - Automatic hbm and dc dimming added
   - New automatic dynamic thermal profiles added
+ Switch to AIDL ST NFC HAL
+ Shim some NFC blobs with libbase_shim
   - Fixes missing symbol crash in some nfc blobs
+ Switch to new AIDL IR service
+ Update CarrierConfig, brightness overlays and blobs from spesn TKQ1.221114.001-V816.0.11.0.TGKMIXM
+ Enable client composition cache
   - Keeping this disabled did not show any improvement.
+ Create a new uclamp.boosted tunable
+ Some changes in display drivers on kernel side
+ Switch to simple lmk
   - Much better multitasking on 4gb
+ More kernel cleanup
+ Now fleshable by pixelos recovery
