## TWRP device tree for HTC Desire 620G dual sim (htc_a31mg_dug)

Add to `.repo/local_manifests/htc_a31mg_dug.xml`:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<manifest>
	<project path="device/htc/htc_a31mg_dug" name="android_device_htc_htc_a31mg_dug" remote="liquidporting" revision="android-5.1" />
</manifest>
```

Then run `repo sync` to check it out.

To build:

```sh
. build/envsetup.sh
lunch omni_htc_a31mg_dug-eng
make -j5 recoveryimage
```
