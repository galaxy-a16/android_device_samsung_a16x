# Android device tree for samsung SM-A166E (a16x)

# How-to compile it:

- twrp-12.1 Manifest
```
    repo init --depth=1 -u https://github.com/minimal-manifest-twrp/platform_manifest_twrp_aosp.git -b twrp-12.1
```
 - Sync
```
    repo sync
```
 - Clone TheNoobDevs-Staging twrp tree
```
    git clone https://github.com/TND-STAGING/android_device_samsung_a16x.git -b android-14 device/samsung/a16x
```
 - Build
```
    export ALLOW_MISSING_DEPENDENCIES=true; . build/envsetup.sh; lunch twrp_a16x-eng; mka recoveryimage
```
## Multidisabler
once in twrp go to advanced, terminal and type "multidisabler" to stop restoration of stock recovery
