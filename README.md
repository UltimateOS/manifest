![banner](https://github.com/UltimateOS/.github/raw/main/banner1.jpg)
# UltimateOS | Android Open Source Software
An Android Operating System Based On AOSP.

### Requirements
- Around 500GB disk space.
- Around 32GB RAM running Linux.

### Sync our source ###
```bash
repo init -u https://github.com/UltimateOS/manifest.git -b 15 --depth=1
```
```bash
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
```

### Build our source ###

- Set up the build environment
```bash
source build/envsetup.sh
```

- Lunch a target
```bash
lunch ultimate_$devicecodename-userdebug
```

- To start compiling
```bash
mka ultimate -j$(nproc --all)
```