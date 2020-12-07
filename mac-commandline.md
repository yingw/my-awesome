# 命令行

- 开启第三方软件运行权限 - `sudo spctl --master-disable`
- `sudo diskutil mount disk0s1`

scutil - 修改系统环境变量

```sh
# 设置计算机名称
scutil --get ComputerName
sudo scutil --set ComputerName "Guowei's iMac"

# 设置hostname（不能有空格）
sudo scutil --set HostName "GuoweiMac" && \
sudo scutil --set LocalHostName "GuoweiMac" && \
sudo defaults write /Library/Preferences/SystemConfiguration/com.apple.smb.server NetBIOSName -string "GuoweiMac"
```

显示已加载的 kext（Kernel Extensions）

```sh
sudo kextstat -l
```

加载和卸载 kext

```sh
sudo kextload -b com.apple.driver.ExampleBundle
Unload Kernel Extensions
sudo kextunload -b com.apple.driver.ExampleBundle
```

设置登入屏幕的文字

```sh
sudo defaults write /Library/Preferences/com.apple.loginwindow LoginwindowText "Yin Guo Wei's iMac, tel: 18918558295"
```

清理内存缓存

```sh
sudo purge
```

显示内存状态

```sh
vm_stat

# Table of data, repeat 10 times total, 1 second wait between each poll
vm_stat -c 10 1
```

安装 pkg 文件软件

```sh
installer -pkg /path/to/installer.pkg -target /
```

安装 dmg

更新

```sh

# 显示可用更新
softwareupdate --list
# 安装所有更新
sudo softwareupdate -ia
```

显示系统信息

```sh
sw_vers -productVersion
system_profiler SPSoftwareDataType
defaults read loginwindow SystemVersionStampAsString
```

重启 - `reboot`

时区

```sh
sudo systemsetup -gettimezone
sudo systemsetup -settimezone <timezone>
sudo systemsetup -listtimezones
```

[一些参考](https://github.com/herrbischoff/awesome-macos-command-line)
