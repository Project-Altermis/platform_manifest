# <img src="https://github.com/Project-Altermis/platform_manifest/blob/Sanitize/Project-Altermis.png" width="290"> #

### 做好编译前的准备工作先，拉取源码与初始化（To Sync） ###

```bash
# 先初始化本地存储库一下（Initialize local repository）
repo init -u https://github.com/Project-Altermis/platform_manifest -b Sanitize

# 拉取源码DA🌟ZE（sync）
repo sync -c -j$(nproc --all) --force-sync --no-clone-bundle --no-tags --fail-fast
```

### 准备工作完成，开始编译（To Build） ###

```bash
# 先设置好环境（Set up environment）
$ . build/envsetup.sh

# 选择好模式（Choose a target）
$ lunch altermis_$device-userdebug

# 开始享受编译的过程吧（To build）【可以考虑喝杯奶茶】
$ make bacon -j$(nproc --all)

#欢迎一起完善
