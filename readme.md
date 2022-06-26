# <img src="https://github.com/Project-Altermis/platform_manifest/blob/Sanitize/Project-Altermis.png" width="512"> #

### 同步我们的源码/To Sync ###

```bash
# Initialize local repository
repo init -u https://github.com/Project-Altermis/platform_manifest -b Sanitize

# Sync
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags --fail-fast
```

### 开始编译吧/To Build ###

```bash
# Set up environment(设置好环境˃ʍ˂)
$ . build/envsetup.sh

# Choose a target(选择目标(●'◡'●))
$ lunch altermis_$device-userdebug

# Start(激动⊙∀⊙！)
$ make bacon -j$(nproc --all)
