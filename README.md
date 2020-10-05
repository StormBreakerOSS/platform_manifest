# StormBreaker
Keeping it simple here bois, Performance? Battery? yes.

### Requirements
- Around 200G disk space.
- A computer with at least 32G RAM running Linux.
- Some brain cells.

### Instructions
1. Make sure you have a build environment setup.

### Sync ###
```bash
        repo init -u https://github.com/StormBreakerOSS/android_manifest -b reikon
        repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
```

### Build ###
```bash
        source build/envsetup.sh
        lunch stormbreaker_$device-userdebug
        make storm-prod -j$(nproc --all)
```

### Reporting compilation issues
- For common porting related errors, visit [**Android Building Help**](https://t.me/AndroidBuildingHelp)

Credits
-------
 * [**AOSP**](https://android.googlesource.com)
 * [**LineageOS**](https://github.com/LineageOS)
 * [**HentaiOS**](https://github.com/hentaios)
