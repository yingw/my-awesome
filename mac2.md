# MacOS 命令

Apple 官方文档：

- [Mac 笔记本电脑支持](https://support.apple.com/zh-cn/mac/laptops)

## 1.3. MacOS 恢复功能

- [重置 Mac 的 SMC](https://support.apple.com/zh-cn/102605)
- [以安全模式启动 Mac](https://support.apple.com/zh-cn/116946) - Intel 芯片：按住 Shift 开机；Apple 芯片：安装开机键看到启动选项，再按住 Shift 按“继续以安全模式运行”按
- [如何从“macOS 恢复”启动](https://support.apple.com/zh-cn/102518) - “按下再松开电源按钮以将 Mac 开机，然后立即按住键盘上的 Command (⌘) 和 R 这两个按键。”（Intel芯片），进入恢复，可以：
- [重置 Mac 上的 NVRAM](https://support.apple.com/zh-cn/102539) (Apple CPU 不需要)
- 电池问题：[如果你在 MacBook Air 或 MacBook Pro 上看到“建议维修”](https://support.apple.com/zh-cn/108376)
- [识别 Mac 电源适配器](https://support.apple.com/zh-cn/109509)
- 关于充电：[为 MacBook Air 或 MacBook Pro 充电](https://support.apple.com/zh-cn/102397)
- 关于快充：[为 MacBook Air 或 MacBook Pro 快速充电](https://support.apple.com/zh-cn/102378) - 没有提到 PD 协议充电器，但是应该也支持
- [苹果历代充电器](https://post.smzdm.com/p/a90r70wo/)
- [笔记本电脑按键](https://support.apple.com/zh-cn/101268)

1. Restore From Time Machine Backup
2. Reinstall Mac OS X
3. Disk Utility （分区）

注：重装需要联网下载整个 OS 镜像

或者 [制作使用引导安装器](https://support.apple.com/zh-cn/HT201372)

## 降级 / 重新安装 macOS

- [如何重新安装 macOS](https://support.apple.com/zh-cn/102655)
- [如何下载和安装 macOS](https://support.apple.com/zh-cn/102662)
- [创建可引导的 macOS 安装器](https://support.apple.com/zh-cn/101578)

## 1.4. 初始化

在安全和隐私里显示允许第三方来源应用的选项： `sudo spctl --master-disable`

## 1.5. 安装 Windows

用 Mac 做 Windows 启动盘，需要 ISO 文件，[官方文档](https://support.apple.com/zh-cn/HT205016)
[在 Mac 上通过 “启动转换助理” 安装 Windows 10](https://support.apple.com/zh-cn/HT201468)

[参考](https://www.cnblogs.com/zhengxu/articles/6145651.html)

要用 Mac 的 Bootcamp 制作启动盘；（不需要）
重装后要在 U 盘里面执行

安装过程下周 2G 左右的驱动

切换：开机按着 Optional

[OmniGraffle 破解版](https://www.zhinin.com/omnigraffle_pro-mac.html)

如何卸载内置不用的应用：如股票 / 消息

### JDK

查看当前 JDK 版本：`/usr/libexec/java_home -V`

配置：`.bash_profile`

```bash
JAVA_HOME=/Library/Java/JavaVirtualMachines/jdk1.8.0_181.jdk/Contents/Home
PATH=$JAVA_HOME/bin:$PATH:.
CLASSPATH=$JAVA_HOME/lib/tools.jar:$JAVA_HOME/lib/dt.jar:.
export JAVA_HOME
export PATH
export CLASSPATH
```

把应用命令行加入 PATH，比如 VSCode

```bash
export PATH=/Applications/Visual\ Studio\ Code.app/Contents/Resources/app/bin:$PATH
```

设置别名
`alias  web="code ~/work/web"`

### 环境变量

给 Mac 设置环境变量，有很多配置可以，用户环境变量推荐 `.bash_profile`，如果是 zsh 修改 `.zshrc`, 或者推荐在. zshrc 文件加一行 source .bash_profile

[参考](https://blog.csdn.net/lilang66/article/details/81415990)

- `/etc/profile`
- `/etc/paths`
- `~/.bash_profile`
- `~/.bash_login`
- `~/.profile`
- `~/.bashrc`

```bash
HOMEBREW_NO_AUTO_UPDATE=1
export HOMEBREW_NO_AUTO_UPDATE
# 或者
export HOMEBREW_NO_AUTO_UPDATE=true

export PATH=$PATH:<PATH 1>:<PATH 2>
```

brew 加入 .zshrc 的 PATH

```sh
cd /opt/homebrew/bin/

PATH=$PATH:/opt/homebrew/bin

echo export PATH=$PATH:/opt/homebrew/bin >> ~/.zshrc
```

然后 `source .bash_profile`

curl 连不上，设置代理
(之前可以写 socket5： ，但是现在不支持了)

```s
export http_proxy=http://127.0.0.1:20090
export https_proxy=http://127.0.0.1:20090
```

curl 可能不直接使用系统设置的代理，可以在命令上加参数 `-x`，或者写 alias

```sh
alias curl="curl -x <proxy_host>:<proxy_port>"
```

或者在  ~/.curlrc 中添加：

```sh
proxy = <proxy_host>:<proxy_port>
```

pip 也可以临时加：

```sh
pip install xxx --proxy=https://xx.xx.xx.xx:xxxx
```

禁用 MacOS 的系统升级提示
hosts 增加

```hosts
127.0.0.1 swscan.apple.com
127.0.0.1 swdist.apple.com
127.0.0.1 swcdn.apple.com
127.0.0.1 swquery.apple.com
127.0.0.1 swdownload.apple.com
```

执行

```s
defaults write com.apple.systempreferences AttentionPrefBundleIDs 0
Killall Dock
```

## 给 iterm 终端设置代理

设置代理

使用 curl，wget，brew 等 http 应用程序会调用 http_proxy 和 https_proxy 这两环境变量进行代理，通过下面方式设置：

方式 1

```sh
export http_proxy=http://127.0.0.1:20091
export https_proxy=$http_proxy
```

方法 2

```sh
export http_proxy=http://127.0.0.1:20091 https_proxy=http://127.0.0.1:20091
```

取消设置代理

```sh
unset http_proxy https_proxy
```

快速切换代理

可以在 ~/.zshrc 或者 ~/.bash_profile 中添加这样的 alias：

```sh
alias goproxy='export http_proxy=http://127.0.0.1:20091 https_proxy=http://127.0.0.1:20091'
alias disproxy='unset http_proxy https_proxy'
```

后续通过 goproxy / disproxy 进行切换

### 设置PATH

有时候需要手动设置新应用的 PATH，在 ~/.bash_profile 或 ~/.zshrc 中添加：

```sh
export PATH=/usr/local/bin:$PATH
export PATH=/opt/homebrew/bin:$PATH
```

## 快捷键

[Mac 键盘快捷键](https://support.apple.com/zh-cn/102650)

修饰键：

- Fn (Function) 或地球仪
- Control（或 Ctrl）⌃
- Option（或 Alt）⌥
- Shift ⇧
- Command（或 Cmd）⌘

常用快捷键：

- Command-X：剪切
- Command-C：拷贝
- Command-V：粘贴
- Finder 里文件剪切需要：拷贝（Command-C）后，再“移动” (Option-Command-V)
- Command-Z：撤销上一个命令。Shift-Command-Z 来重做
- Command-A：选择所有
- Command-F：查找
- Command-H：隐藏最前方 App 的窗口。要查看最前方的 App 但隐藏所有其他 App，请按 Option-Command-H。
- Command-M：将最前方的窗口最小化至程序坞。要最小化最前方 App 的所有窗口，请按 Option-Command-M。
- Command-O：打开所选项目，或打开一个对话框以选择要打开的文件。
- Command-S：存储当前文稿。
- Command-T：打开新标签页。
- Command-W：关闭最前方的窗口。要关闭 App 的所有窗口，请按下 Option-Command-W。

文本编辑：

- Backspace：删除光标前的字符
- Fn + Backspace：删除光标后的单词（相当于 Windows 的 Delete）

系统桌面

- Command-空格键：显示或隐藏“聚焦”搜索栏
- Option-Command-Esc：强制退出 App
- Shift + Ctrl + Opt + 关机: 瞬间关机
- Ctrl + Opt + 关机: 正常关机
- F11
- Ctrl + Command + F 全屏
- Optional + Command + D 隐藏任务栏
- Shift + Option + Command + Esc 关闭窗口（关闭一些没有 APP、没有菜单的弹出告警窗口，如 “自动任务” 的 wine 运行报错）
- Command-重音符 (`)：在你当前所用 App 的各个窗口之间切换
- Command-逗号 (,)：打开最前方 App 的设置（偏好设置）。

访达（Finder，文件管理器）：

- Shift-Command-C：打开“电脑”窗口
- Shift-Command-D：打开“桌面”文件夹
- Shift-Command-F：打开“最近使用”窗口
- Shift-Command-G：打开“前往文件夹”窗口
- Shift-Command-H：打开当前 macOS 用户账户的个人文件夹
- Option-Command-L：打开“下载”文件夹
- Shift-Command-N：新建文件夹。
- Shift-Command-T：显示或隐藏“访达”窗口中的标签页栏。
- Command-Delete：将所选项目移到废纸篓。
- Fn-Shift-A：显示或隐藏启动台。

## Macbook Pro

耗电问题：

睡眠一晚上耗电 50%，官方宣传的是一天 1~2%

可能的问题或解决设置：

- DHCP 租约更新太短（在路由器上设置）
- 关闭屏幕时间
- 关闭 Siri
- 在休眠时关闭蓝牙和 WIFI，可以使用工具：`brew install --cask bluesnooze`
- 其他各种可能在睡眠中唤醒的服务，可以在活动监视器里面打开“阻止睡眠”查看
- Chrome 会在休眠时多次唤醒，尽量在休眠前退出 Chrome，在 Chrome 的 设置 - 节能模式 - 在拔下电源线时开启
- 用命令 pmset 设置休眠模式。参考这两篇帖子：[Macbook battery drain while in sleep (actually) SOLVED!](https://www.reddit.com/r/apple/comments/11nhs8a/macbook_battery_drain_while_in_sleep_actually/)
- 禁用电源小睡以及TCP keep alive:

```sh
sudo pmset -a hibernatemode 25
sudo pmset -b tcpkeepalive 0
sudo pmset -a powernap 0

恢复
sudo pmset -a hibernatemode 3
sudo pmset -b tcpkeepalive 1

```

其他命令

```sh
pmset -g log|grep -e " Sleep " -e " Wake " # 查看睡眠和唤醒的日志，注意到 TCPKeepAlive=Active
pmset -g log | grep -i "wake from"
pmset -g log | grep -w Charge | more
pmset -g  # 查看当前电源设置
pmset -g assertions
pmset -g log | grep "Wake Requests"
sudo pmset -a standbydelayhigh 10
sudo pmset -a autopoweroffdelay 60
sudo pmset -a standbydelaylow 10
sudo pmset -a standby 1
sudo pmset -a hibernatemode 3
sudo pmset -a tcpkeepalive 0
# 浅休眠模式
sudo pmset -b hibernatemode 3
# 深度休眠模式
sudo pmset -b hibernatemode 25
```

Rosetta - 在 Arm 架构的 Mac CPU 上模拟 X86 环境运行 APP
安装（新版本默认安装了）：
`/usr/sbin/softwareupdate --install-rosetta --agree-to-license`
选择有bug或闪退的软件右键——显示简介——勾选使用Rosetta打开

## Parallels Desktop

使用宿主机的代理服务

查看宿主机 IP

```sh
ifconfig | grep inet
```

一般是这个：10.211.55.2

然后在客户机里面设置代理

## 自动操作

场景1: [将脚本封装为 App](https://blog.csdn.net/qq_37164975/article/details/109519155)

新建 文稿类型：应用程序
资源库里选：运行shell脚本
测试运行无误后，存储为 APP

```sh
/opt/homebrew/bin/wine notepad++
# 或者用绝对路径
/opt/homebrew/bin/wine /Users/yinguowei/Tools/BeyondCompare-v4.1.4/BCompare.exe
# 或者用
/usr/local/bin/wine notepad++

```

## 替换 APP 图标

在 APP 显示简介 上，点中图标，直接复制图标，或者拖拽图标文件上去。

## Wine

运行 .exe 程序： `wine program.exe`
运行 .msi 安装程序： `msiexec /i program.msi`
设置 wine： `winecfg`
查看程序兼容性： `appdb Program Name`，其实是链接到 appdb.winehq.org 进行查询

中文乱码方块，[参考](https://app.techweb.com.cn/ios/2017-05-05/2520364.shtml)

```regedit
REGEDIT4
[HKEY_LOCAL_MACHINE\Software\Microsoft\Windows NT\CurrentVersion\FontLink\SystemLink]
"Arial"="Lantinghei.ttc"
"Lucida Sans Unicode"="Lantinghei.ttc"
"Microsoft Sans Serif"="Lantinghei.ttc"
"MS Sans Serif"="Lantinghei.ttc"
"SimSun"="Lantinghei.ttc"
"Tahoma"="Lantinghei.ttc
"Tahoma Bold"="Lantinghei.ttc"
```

导入注册表：

还没完全解决，部分界面上的字体还是方块，参考：

https://blog.csdn.net/u011233383/article/details/105454632

Mac 字体文件目录：
'/System/Library/Fonts/'
Wine Windows 字体目录：
/Users/yinguowei/.wine/drive_c/windows/Fonts/

自动生成的 .desktop 桌面快捷方式文件似乎没用，只要去 exe 创建一个替身就行了。
或者用“自动操作”做一个shell脚本，内容是 `/opt/homebrew/bin/wine xxx`，存为应用程序

## 检查校验码

MD5 验证码
```sh
# MD5 内置
md5 file
# MD5sum 安装
md5sum file
# crc32
crc32 /path/to/file
# 批量
for filename in `ls`; do md5 $filename; done
md5 -r *
# 过滤文件
find -s /path/to/folder -type f -exec md5sum {} \;
find -s /path/to/folder -type f -exec md5 {} \;
# sha1
shasum /path/to/file
# sha256
sha256 /path/to/file
# md5sha1sum
brew install md5sha1sum
# openssl
openssl md5 /path/to/file
openssl sha1 /path/to/file
openssl sha256 /path/to/file

```

## macOS 26 Tahoe

Tahoe 里面 Apple 去掉了原来的启动台 Launchpad，替换为 Spotlight，恢复的方法：

- 官方的讨论：[How do I restore the old Launchpad in macOS Tahoe](https://discussions.apple.com/thread/256146250?sortBy=rank)
- [命令行恢复方式（可能已失效）](https://www.reddit.com/r/MacOSBeta/comments/1lk8j5r/get_launchpad_back_macos_26/)
- 开源替代品：[kristof12345/Launchpad](https://github.com/kristof12345/Launchpad)
- [Semnykcze/MacOS-26-Launchpad](https://github.com/Semnykcze/MacOS-26-Launchpad) - 恢复脚本（可能已失效）
- NovaPadGo - AppStore 上的第三方 Launchpad，收费
- [LaunchBoard – App Launcher](https://apps.apple.com/us/app/launchboard-app-launcher/id6753108141)
- [Quick App Launcher (QAL) Pro](https://apps.apple.com/us/app/quick-app-launcher-qal-pro/id6740396517) - 收费

## 处理 Mac .DS_Store 文件

[知乎文章：.DS_Store文件彻底删除+禁用生成2025最全攻略](https://zhuanlan.zhihu.com/p/1926963355161190495)

```
# 打开显示隐藏文件
defaults write com.apple.finder AppleShowAllFiles TRUE ; killall Finder
# 查找
find /path/where/is -name .DS_Store
# 删除
find /path/where/is -name .DS_Store -delete
# 批量删除
find . -name '.DS_Store' -type f -delete
# 另外还有图片预览缓存
find . -name '._.*' -type f -delete
# 另一个几个版本：删除 ._.DS_Store 、跳过输出
find . -type f \( -name ".DS_Store" -o -name "._.DS_Store" \) -delete -print 2>&1 | grep -v "Permission denied"
sudo find / -name “.DS_Store” -depth -exec rm {} \
rm -v **/.DS_Store

# 禁止在网络共享目录生成，重启生效
defaults write com.apple.desktopservices DSDontWriteNetworkStores -bool TRUE
# 禁止在移动磁盘生成，重启生效
defaults write com.apple.desktopservices DSDontWriteUSBStores -bool TRUE
# 查看设置
defaults read com.apple.desktopservices DSDontWriteNetworkStores
defaults read com.apple.desktopservices DSDontWriteUSBStores
# 恢复
defaults write com.apple.finder AppleShowAllFiles FALSE ; killall Finder
defaults write com.apple.desktopservices DSDontWriteNetworkStores -bool FALSE
defaults write com.apple.desktopservices DSDontWriteUSBStores -bool FALSE
# 另一个禁用特定目录生成 .DS_Store 的方法，只能单个目录设置
sudo cp -af /dev/null ~/Documents/.DS_Store && sudo chmod a=rw ~/Documents/.DS_Store

```

- [CleanMyMac](https://macpaw.com/cleanmymac) 默认批量删除 .DS_Store 文件
- [Asepsis](https://asepsis.binaryage.com/) - 禁用 .DS_Store，但是只支持旧版 MacOS 10.8 - 10.10
- [BlueHarvest](https://www.zeroonetwenty.com/blueharvest/) - 自动删除 .DS_Store，支持 macOS 10.15 至 macOS 15，收费
- [DS_Store Cleaner](https://apps.apple.com/us/app/ds-store-cleaner/id6748859939?mt=12) - 手动清除 DS_Store 文件，免费，2025年，v1.2，[官网](https://www.pcffm.de/macos-app-delete-ds_store-files-in-seconds/)需要梯子

## 启用未知来源软件

Mac 提示「未打开“XXX.app”」Apple 无法验证“Sketch.app”是否包含可能危害Mac安全或泄露隐私的恶意软件。

是因为：macOS 15.0 系统开始，Mac 改动了保护机制，默认不允许安装未知来源的软件（即自己下载的 APP 且没有授权开发证书签名）。

临时授权：「系统偏好设置」-「隐私与安全性」-「安全性」，点击「仍要打开」

或者使用单一签名：执行：`sudo xattr -rd com.apple.quarantine /Applications/XXX.app`

永久授权：终端执行：`sudo spctl --master-disable`，此为之安全性来源里增加了选项“任何来源”，然后去安全性里设置为允许“任何来源”

## 其他

- [is Apple Silicon Ready](https://isapplesiliconready.com/)
- [屏蔽设置提示升级的小红点](https://zhuanlan.zhihu.com/p/1951680001368917919)
- 关于 SIP (System Integrity Protection) - 禁用：在恢复模式下运行 `csrutil disable`，恢复：`csrutil enable`（强烈不建议关闭）