# Project Radiant #

### Sync ###

```bash

# Initialize local repository
repo init -u https://github.com/ProjectRadiant/manifest -b eleven

# Sync
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
```

### Build ###

```bash

# Set up environment
$ . build/envsetup.sh

# Choose a target
$ lunch radiant_$device-userdebug

# Build the code
$ mka bacon -jX
```

# Flags #

### Gapps ###
By default the ROM builds with GApps, if you wish to do a vanilla build. Set the flag `TARGET_INCLUDE_GAPPS` to false.

Optionally you may also configure `TARGET_INCLUDE_STOCK_ARCORE` and `TARGET_INCLUDE_GOOGLE_RECORDER` according to your device if you ship a gapps build. (These 2 flags default to false.)

<br>

# Apply for Official # 
If you would like to apply for official, then feel free to take a look [here](https://github.com/ProjectRadiant/official_devices).
