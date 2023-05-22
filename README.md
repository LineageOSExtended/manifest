## Repo Init ##
```bash
repo init --depth=1 --no-repo-verify -u https://github.com/LineageOSExtended/manifest -b lineage-20.0 -g default,-mips,-darwin,-notdefault --git-lfs
```
## Sync Source ##
```bash
repo sync -c --no-clone-bundle --optimized-fetch --prune --force-sync
```
## Build Time ##
```bash
. build/envsetup.sh
lunch lineage_device-userdebug
mka bacon
```