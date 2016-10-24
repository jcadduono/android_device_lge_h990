## TWRP device tree for LG V20 (International H990)

Add to `.repo/local_manifests/h990.xml`:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<manifest>
	<project path="device/lge/h990" name="android_device_lge_h990" remote="TeamWin" revision="android-6.0" />
</manifest>
```

Then run `repo sync` to check it out.

To build:

```sh
. build/envsetup.sh
lunch omni_h990-eng
make -j5 recoveryimage
```

Kernel sources are available at: https://github.com/jcadduono/android_kernel_lge_msm8996/tree/twrp-7.0

