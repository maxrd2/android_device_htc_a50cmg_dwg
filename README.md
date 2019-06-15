## TWRP device tree for HTC Desire 728G Dual Sim (a50cmg_dwg)

For building TWRP for MT6753 models only.


### Manifest
Add to `.repo/local_manifests/a50cmg_dwg.xml`:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<manifest>
	<project name="maxrd2/android_device_htc_a50cmg_dwg" path="device/htc/a50cmg_dwg" remote="github" revision="android-5.1" />
</manifest>
```

Then run `repo sync` to check it out.

### Build
To build:

```sh
. build/envsetup.sh
lunch omni_a50cmg_dwg-eng
make -j4 recoveryimage
```

Detailed build instructions can be found on [wiki page](https://github.com/maxrd2/android_device_htc_a50cmg_dwg/wiki/TWRP-Build-Instructions)
