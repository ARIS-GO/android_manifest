Aris Go
=======

What is Aris Go?
----------------

Aris Go is an [AOSP](http://android.googlesource.com/) & [LineageOS](https://github.com/LineageOS) based project.

> ~~A noob starts a new project~~


How to start?
-------------

To get started with Aris, you'll need to get familiar with [Source Control Tools](https://source.android.com/setup/develop).

To initialize your local repository, use this command:
```bash
repo init -u https://github.com/Aris-Go/android_manifest.git -b vinah --depth=1 --git-lfs
```

Then to sync up:
```bash
repo sync
# You can also set a higher job value by using `-jN`(default N=4) to speed up the sync.
```

Building
--------

Initialize the ROM environment with the envsetup.sh script.
```bash
. build/envsetup.sh
```

To lunch your device after cloning all device sources.
```bash
lunch aris_<codename>-ap3a-<buildtype>
```

Then start building.
```bash
mka bacon
```
