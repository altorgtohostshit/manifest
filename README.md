# NezukoOS #

### Sync ###

```bash

# Initialize local repository
repo init -u https://github.com/NezukoOS/manifest -b eleven

# Sync
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags
```

### Build ###

```bash

# Set up environment
$ . build/envsetup.sh

# Choose a target
$ lunch nezuko_$device-userdebug

# Build the code
$ mka bacon -jX
```

### Apply for Official ###
If you would like to apply for official, then feel free to take a look [here](https://github.com/NezukoOS/Docs/blob/main/official_requirements.md).