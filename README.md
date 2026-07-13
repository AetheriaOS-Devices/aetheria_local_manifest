
Aetheria Devices Manifests
=======================

Getting Started
---------------

To get started with AetheriaOS, you'll need to get familiar with [Source Control Tools](https://source.android.com/setup/develop).

To initialize your local repository using the AetheriaOS trees, use a command like this:
```bash
repo init -u https://github.com/AetheriaOS/aetheria_manifest.git -b aetheria-1.0 --depth=1 --config-name
```
Clone this repository in `.repo/local_manifests`:
```bash
git clone --single-branch -b laurel_sprout_aetheria-1.0 https://github.com/AetheriaOS-Devices/aetheria_local_manifest.git .repo/local_manifests/laurel_sprout.xml
```
Then to sync up:
```bash
repo sync -c --no-clone-bundle --no-tags --optimized-fetch --prune --force-sync -j8
```
