
Aetheria Devices Manifests
=======================

Getting Started
---------------

To get started with AetheriaOS, you'll need to get familiar with [Source Control Tools](https://source.android.com/setup/develop).

To initialize your local repository using the AetheriaOS trees, use a command like this:
```bash
repo init -u https://github.com/AetheriaOS/aetheria_manifest.git -b aetheria-<use the existing version> --depth=1 --config-name
```
Clone this repository in `.repo/local_manifests`:
```bash
git clone --single-branch -b <branches in this repository> https://github.com/AetheriaOS-Devices/local_manifest.git .repo/local_manifests
```
Then to sync up:
```bash
repo sync -c --no-clone-bundle --no-tags --optimized-fetch --prune --force-sync -j8
```
