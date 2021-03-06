LG Optimus F3 KitKat device tree
=============

CM11 Device tree for LG Optimus F3

####Functionality status:
- [x] Calls/texts (GSM/GPRS/EDGE/HSPA)
- [x] Mobile Data
- [x] Wifi
- [ ] Bluetooth
- [x] Framebuffer/3D Acceleration
- [x] GLES 1/2/3
- [x] GPS
- [x] Accelerometer/Rotation
- [x] Compass
- [ ] Auto brightness
- [x] Proximity sensor
- [x] Vibrator

####Instructions:
Copy the contents of this folder to: device/lge/fx3t

Or, alternatively, you can add this to your .repo/local_manifests/ with this template:
```xml
<?xml version="1.0" encoding="UTF-8"?>
<manifest>
	<remote name="fx3t" fetch="https://github.com/" />
	<project path="device/lge/fx3t" name="daemon32/android_lge_fx3t.git" remote="fx3t" revision="master" />
	<project path="kernel/lge/fx3t" name="daemon32/android_kernel_lge_fx3t.git" remote="fx3t" revision="master" />
</manifest>
```

To build:
```
source build/envsetup.sh && brunch fx3t
```
