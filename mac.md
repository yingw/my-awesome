# Mac 软件

> 记录我在 MacOS 上使用的工具和配置
> 2025年更新，MacBookPro 2021 M1 Pro

目录

<!-- TOC -->

- [Mac 软件](#mac-软件)
  - [系统工具](#系统工具)
    - [终端工具](#终端工具)
    - [虚拟机](#虚拟机)
    - [输入法](#输入法)
    - [系统清理](#系统清理)
    - [截屏工具](#截屏工具)
    - [压缩解压](#压缩解压)
    - [剪贴板管理](#剪贴板管理)
    - [浏览器](#浏览器)
    - [性能测试](#性能测试)
    - [远程控制](#远程控制)
    - [协同工具](#协同工具)
    - [办公套件](#办公套件)
    - [邮件客户端](#邮件客户端)
    - [文档编辑](#文档编辑)
    - [笔记管理](#笔记管理)
    - [翻译软件](#翻译软件)
    - [开发工具](#开发工具)
    - [图像处理](#图像处理)
    - [下载工具](#下载工具)
    - [媒体播放](#媒体播放)
    - [磁盘工具](#磁盘工具)
    - [系统设置](#系统设置)
    - [系统监控](#系统监控)
    - [VPN](#vpn)
    - [镜像工具](#镜像工具)
    - [网盘](#网盘)
    - [账号管理](#账号管理)
    - [壁纸屏保](#壁纸屏保)
    - [预览增强](#预览增强)
    - [文件管理](#文件管理)
    - [其他](#其他)
  - [命令行工具](#命令行工具)
  - [网站](#网站)

<!-- /TOC -->

## 系统工具

- [Homebrew](https://brew.sh/) - 软件管理，安装命令 `/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`，或者下载预编译好的 [release](https://github.com/Homebrew/brew/releases) v4.5.2
- [Cakebrew](https://www.cakebrew.com/) - Homebrew 图形界面管理，`brew install --cask cakebrew`，v1.3 最后更新：2021年，支持 Silicon（可能被弃用了）
- [Cork](https://github.com/buresdv/Cork) - Homebrew 快速 GUI，Cakebrew 的替代，`brew install --cask cork`，v1.5.5，2025年。`brew install --cask cork`，收费的，但是开源可以自己编译
- [Latest](https://max.codes/latest/) - 版本检查更新，还支持非 brew 安装的应用
- [Applite](https://aerolite.dev/applite) - 也是 brew 的应用管理，有推荐，就是比较慢，要这设置里设置一下代理用 sock 协议，`brew install --cask applite`
- [MacPorts](https://www.macports.org/) - 另一个软件管理工具。v2.10.7
- [Alfred](https://apps.apple.com/cn/app/alfred/id405843582?mt=12) - 搜索、快速启动工具，很多功能，`brew install --cask alfred`，v1.2 最后更新：2012年
- [uTools](https://www.u-tools.cn/index.html) - Alfred 平替，还有 Windows 版，v7.1.1
- [CheetSheet](https://www.mediaatelier.com/CheatSheet/) - 快捷键提示，长按 Command，`brew install --cask cheatsheet`，其他 Mac 的快捷键提示，[参考](https://sspai.com/post/45338)，[官方](https://support.apple.com/zh-cn/102650)，2025年官网已失效，可以切换到 keyClu
- [KeyClu](https://github.com/Anze/KeyCluCask/) - 快捷键提示，按 `⌘, ⌘` 呼出，`brew install --cask keyclu`，v0.30.1
- [CustomShortcuts](https://www.houdah.com/customShortcuts/) - CustomShortcuts 与 KeyClu 一起使用。单击菜单按钮可直接从备忘单中自定义键盘快捷键。`brew install --cask customshortcuts`。v1.2.1
- [Mactracker](https://apps.apple.com/cn/app/mactracker/id430255202?mt=12) - 提供苹果全系列产品的所有信息，v7.13.5，最后更新：2025年
- [HandShaker](https://www.smartisan.com/apps/#/handshaker) - 锤子科技的文件管理软件，用于在 Mac 电脑上管理 Android 手机内容，通过手机端 APP 链接配对，v2.5.6，最后更新：2018年
- [MacDroid](https://www.macdroid.app/) - 和 Android 设备传输文件，免费版只有只读模式，`brew install --cask macdroid`
- [OpenMTP](https://openmtp.ganeshrvel.com/) - Mac 上的 Android 手机文件管理，可 MTP 文件传输，`brew install --cask openmtp`
- [LocalSend](https://localsend.org/zh-CN) - 将文件分享到附近的设备，基于本地网络。`brew install --cask localsend`
- [LaunchRocket](https://github.com/jimbojsb/launchrocket) - 自动启动服务管理，`brew install --cask launchrocket`，v0.7，最后更新：2014年
- [GamePad Companion](https://apps.apple.com/us/app/gamepad-companion/id428799479?mt=12) - 手柄驱动，收费，v3.3.1，最后更新：2014年
- [超级右键](https://apps.apple.com/cn/app/%E8%B6%85%E7%BA%A7%E5%8F%B3%E9%94%AE-irightmouse/id1497428978?mt=12) - 右键菜单管理软件，v2.3.2，最后更新：2024年
- [Better And Better](https://www.better365.cn/bab2.html) - 触控板、鼠标、键盘的手势等。v2.6.7，最后更新：2025年，安装包是pkg格式
- [AdGrard](https://adguard.com/zh_cn/welcome.html) - 拦截多个浏览器、系统的广告，收费，试用期14天
- [Vanilla](https://matthewpalmer.net/vanilla/) - 免费版隐藏任务栏图标，基本够用；收费额外功能
- [Dozer](https://github.com/Mortennn/Dozer) - 隐藏任务栏图标，可以替换 Vanilla `brew install --cask dozer`。v4.0.0，最后更新：2019年
- [Hidden Bar](https://github.com/dwarvesf/hidden/) - 同 Dozer，隐藏任务栏图标，更新点 `brew install --cask hiddenbar`。v1.9，最后更新：2022年
- [Ice](https://icemenubar.app/) - 菜单栏管理，免费；0.11.12，2024年；`brew install jordanbaird-ice`
- [Bartender](https://www.macbartender.com/) - 管理菜单栏图标，收费
- [iBar](https://www.better365.cn/ibar.html) - 菜单栏管理，可以聚合模式向下扩展，聚合模式收费
- [OnlySwitch](https://github.com/jacklandrin/OnlySwitch) - 一键切换各种开关，还可以隐藏刘海（Notch），`brew install only-switch`，v2.5.6，2025年
- [Itsycal](https://www.mowglii.com/itsycal/) - 菜单栏日历，最后更新：2025年
- [QuickRes](https://thnkdev.com/QuickRes/) - 快速切换分辨率，收费，支持M1。v4.9，最后更新：2021年
- [Ethernet Status](https://apps.apple.com/cn/app/ethernet-status/id1186187538?mt=12) - 显示有线网络连接状态。v4.5，最后更新：2023年
- [Scroll Reverser](https://pilotmoon.com/scrollreverser/) - 分离触摸板和鼠标的自然滚动设置，正常情况下，Mac只允许同时设置触控板和外部鼠标的滚动方向，不能独立设置，明显不自然，这个可以分开独立设置。v1.9，最后更新：2024年，`brew install scroll-reverser`
- [Mos](https://mos.caldis.me/) - 控制鼠标滚动方向，可以设置应用模式 `brew install --cask mos`。v3.5.0，最后更新：2025年
- [InsomniaX](https://insomniax.en.softonic.com/mac) - 控制 Mac 在合上盖子和闲置超时后是否进入休眠状态，比较老了，有点问题。主页已失效
- [Monitor Control](https://github.com/MonitorControl/MonitorControl) - 控制扩展视频输出的显示亮度和设备音量 `brew install --cask monitorcontrol`。v4.3.3，2024年
- [Gas Mask](https://github.com/2ndalpha/gasmask) - Hosts 管理 `brew install --cask gas-mask`。v0.8.6，2020年
- [SwitchHosts](https://github.com/oldj/SwitchHosts) - Hosts 模板，快速切换 `brew install --cask switchhosts`。v4.2.0，2024年
- [iHosts](https://toolinbox.net/iHosts/) - v1.4.0，2018年
- [MacOS小助手](https://www.macwk.com/soft/macos-assistant-macwk) - 工具集，含禁用 macOS 更新提示
- [Spectacle](https://www.spectacleapp.com/) - 分隔屏幕窗口布局 `brew install --cask spectacle`
- [Rectangle](https://rectangleapp.com/) - 分隔屏幕窗口布局，支持拖动 `brew install --cask rectangle`，v0.87，最后更新：2025年
- [Multipass](https://multipass.run/) - Ubuntu 公司官方的虚拟机 `brew install --cask multipass`
- [Caffeine](https://intelliscapesolutions.com/apps/caffeine) - 阻止Mac进入休眠，可改用 KeepingYouAwake `brew install --cask caffeine`，v1.1.3，最后更新：2020年
- [Amphetamine](https://apps.apple.com/us/app/amphetamine/id937984704?mt=12) -  App Store 上的另一款阻止休眠，免费。v5.3.2，2023年
- [KeepingYouAwake](https://keepingyouawake.app/) - 同 Caffeine，更新更频繁 `brew install --cask keepingyouawake`。v1.6.6，2024年
- [iHash](https://apps.apple.com/cn/app/ihash/id763902043?mt=12) - 比较文件、文件夹 Hash 值（找不到了）。替代品：[Hash/Check](https://apps.apple.com/us/app/hash-check/id1550525767?mt=12)，免费，v2.1，2023年
- [Suspicious Package](https://www.mothersruin.com/software/SuspiciousPackage/) - 查看包安装内部信息 `brew install --cask suspicious-package`。v4.5，2024年
- [AltTab](https://github.com/lwouis/alt-tab-macos) - 可以用 Alt+Tab 切换窗口 `brew install --cask alt-tab`。v7.24.0，2025年
- [Barrier](https://github.com/debauchee/barrier/) - 允许跨系统操作键鼠控制多台PC `brew install --cask barrier`。v2.4.0，2021年
- [Wine](https://wiki.winehq.org/MacOS) - Windows 环境模拟，依赖 [XQuartz](https://www.xquartz.org/)（X窗口系统），要先安装 `brew install --cask xquartz`，`brew install --cask --no-quarantine wine-stable`，版本 v10.0_2，2025年，目前还只支持 Intel，需要 Rosetta2 兼容；卸载：`brew uninstall --cask wine-stable`。[解决中文乱码方块](https://app.techweb.com.cn/ios/2017-05-05/2520364.shtml)
- [Lulu](https://objective-see.org/products/lulu.html) - 网络防火墙 `brew install --cask lulu`。v3.1.5，2025年
- [Logi Options+](https://www.logitech.com/en-us/software/logi-options-plus.html) - 罗技鼠标驱动
- [BetterDisplay](https://github.com/waydabber/BetterDisplay) - 控制外接屏，在投屏时可以关闭主屏幕（免费），GitHub上就一个Readme，不开源，有部分专业版功能收费，v3.5.6，`brew install --cask betterdisplay`
- [赤友右键超人](https://aibotech.cn/right-click-menu/) - 右键菜单增强型应用

### 终端工具

- [iTerm2](https://iterm2.com/) - 好用的终端工具。`brew install --cask iterm2`。v3.5.14，2025年
- [oh-my-zsh](https://ohmyz.sh/) - 用脚本安装，[参考](https://sspai.com/post/55176)。[Oh My Posh](https://ohmyposh.dev/) - `brew install oh-my-posh`
  - 修改主题 `～/.zshrc`，agnoster
  - 安装 [字体](https://github.com/powerline/fonts.git) ，用 `DejaVu Sans Mono for Powerline`
  - [Sleep Aid](https://ohanaware.com/sleepaid/) - 记录分析是哪个进程中休眠时唤醒Mac，十四天试用。作者 sam 在[这里](https://www.reddit.com/r/macbookpro/comments/qqo4v2/my_m1_max_keeps_switching_between_sleep_and/)声称`NUB.SPMISw3IRQ nub-spmi0.0x02 rtc/SleepService`这个进程是正常的，可以尝试切换 `"Wake for Maintenance"`

### 虚拟机

- [Parallels Desktop](https://www.parallels.com/) - 虚拟机，收费
- [Virtualbox](https://www.virtualbox.org/) - 虚拟机，`brew install --cask virtualbox`。v7.1.8
- VM VirtualBox Extension Pack - VirtualBox 的扩展包，用于支持 USB3.0 等 `brew install --cask virtualbox-extension-pack`
- [VMWare Fusion Player/Pro](https://www.vmware.com/products/fusion/fusion-evaluation.html)
- [BlueStacks](https://www.bluestacks.com/) - 蓝叠安卓模拟器
- [Qemu](http://www.qemu.org/) - QEMU is a generic and open source machine & userspace emulator and virtualizer. 开源的托管虚拟机，通过纯软件来实现虚拟化模拟器

### 输入法

- [搜狗输入法](https://pinyin.sogou.com/mac/) - 现在没有 brew 安装，需要手动下载。v6.18.0 2025年6月
- [自动切换输入法](https://apps.apple.com/cn/app/%E8%87%AA%E5%8A%A8%E5%88%87%E6%8D%A2%E8%BE%93%E5%85%A5%E6%B3%95/id1470350547?mt=12) - v2.2.7，2025年

### 系统清理

- [腾讯柠檬清理](https://lemon.qq.com/) - 腾讯的系统清理软件，有工具栏提示 `brew install --cask tencent-lemon`，不要使用 App Store 的版本，功能少。v5.1.14
- [Dr.Cleaner](https://dr-cleaner.en.softonic.com/mac) - 系统清理工具，免费
- [CleanMyMac X](https://macpaw.com/cleanmymac) - 系统清理工具，收费 `brew install --cask cleanmymac`
- [AppCleaner](http://freemacsoft.net/appcleaner/) - 卸载应用，`brew install --cask appcleaner`。v3.6.8，2023年

### 截屏工具

- [iPic](https://toolinbox.net/iPic/) - 图床，[AppStore地址](https://apps.apple.com/cn/app/ipic-image-file-upload-tool/id1101244278?mt=12)。v1.8.4，2024年
- [Annotate](https://itunes.apple.com/us/app/annotate-capture-screenshot/id918207447?mt=12) - 截屏工具
- [Snipaste](https://www.snipaste.com/download.html) - 截图软件，免费 `brew install --cask snipaste`。v2.10.6，2025年
- [iShot](https://apps.apple.com/cn/app/ishot-%E6%88%AA%E5%9B%BE-%E5%BD%95%E5%B1%8F-2020%E5%85%A8%E6%96%B0%E9%AB%98%E5%BA%A6/id1485844094?mt=12) - 截图工具，支持长截图。v2.5.9，2024年
- [Kap](https://getkap.co/)，[GitHub](https://github.com/wulkano/kap)： `brew install --cask kap` 可以截屏，可以录屏为 GIF 或者 MP4，比较大。v3.6.0，2022年
- [LICEcap](https://www.cockos.com/licecap/) - 区域录屏为 GIF `brew install --cask licecap`。v1.32，2022年

### 压缩解压

- [Keka](https://www.keka.io/en/) - 免费下载，AppStore 上收费，也是 [7zip](https://www.7-zip.org/download.html) 的非官方 Mac 版 `brew install --cask keka`，7z官方有Mac的控制台版本。v1.5.0，2025年
- [Betterzip](https://www.betterzip.net/) - 收费，可试用，有类似7z的主界面，$25，v5.3.4，2023年 `brew install --cask betterzip`
- [The Unarchiver](https://www.theunarchiver.com/) - 免费，`brew install --cask the-unarchiver`。v4.3.9，2025年
- [MacZip](https://ezip.awehunt.com/) - 原名`eZip`，国产解压缩工具，免费 `brew install --cask maczip`。v2.4，2024年
- [Bandizip](http://www.bandisoft.com/bandizip.mac/) - 收费

### 剪贴板管理

- [CopyLess 2](https://apps.apple.com/cn/app/copyless-2/id993841014?mt=12) - 剪贴板管理，免费版可以记录 100 个历史和 5 个收藏
- [Paste](https://pasteapp.io/) - 剪贴板工具，收费

### 浏览器

- [Chrome](https://www.google.com/chrome/) - `brew install --cask google-chrome`，Chrome 上的插件参考：[Chrome 插件](./chrome.md)

### 性能测试

- [Geekbench](https://www.geekbench.com/) - 系统检测评分，收费，试用 `brew install --cask geekbench`。v6.4.0
- [Blackmagic Disk Speed Test](https://apps.apple.com/us/app/blackmagic-disk-speed-test/id425264550?mt=12) - 磁盘性能测试
- [Cinebench](https://www.maxon.net/en/products/cinebench-r20-overview/) - GPU 图形性能测试，收费，十四天试用 `brew install --cask cinebench`，官网版本是2025，Homebrew下载的是2024，要用 [R23](https://www.techspot.com/downloads/7579-cinebench-r23.html)，下载试用需要注册等人 v2025.4.0

### 远程控制

- [TeamViewer](https://www.teamviewer.cn/cn/) - 远程控制
- [VNC Viewer](https://www.realvnc.com/en/connect/download/viewer/) - VNC 客户端 `brew install --cask vnc-viewer`
- [向日葵](https://sunlogin.oray.com/download/) - 远程控制
- 开启远程控制 - `共享 - 开启 “远程登录”、“远程管理”`
- [蒲公英](https://apps.apple.com/cn/app/id1305707014) - 异地组网
- [Remote Desktop Manager](https://remotedesktopmanager.com/) - 有 Free 和 Enterprise 版本，免费版不能记录密码，支持 Windows 和 Mac `brew install --cask remote-desktop-manager-free`。Version: 2025.1.16.3
- [CyberDuck](https://cyberduck.io/) - 连接各种远程文件库，支持 FTP、OneDriver、Google Driver、Amazon S3，免费，Store上收费 `brew install --cask cyberduck`。v9.1.4，2025年
- [FileZilla](https://filezilla-project.org/) - FTP 客户端，v3.69.1
- Screen Sharing.APP（屏幕共享） - Mac 自带的 VNC 客户端
- [AnyDesk](https://anydesk.com/zhs) 远程桌面，需要对方也安装，用 ID 链接
- [windows-app](https://adoption.microsoft.com/windows-app/) - `brew install --cask windows-app`，v11.1.9，之前叫：[Microsoft Remote Desktop](https://apps.apple.com/us/app/microsoft-remote-desktop/id715768417)，最新版 8.0.44，应用商店里锁国区，可以到 [外面](https://rink.hockeyapp.net/apps/5e0c144289a51fca2d3bfa39ce7f2b06/) 下 Version 10.2.13 (1593)，或者从 brew 安装
- [Tabby](https://tabby.sh/) - SSH 客户端，有连接管理，[GitHub](https://github.com/eugeny/tabby)，v1.0.223，`brew install --cask tabby`

### 协同工具

- [微信](https://mac.weixin.qq.com/?t=mac&lang=zh_CN) - 官网版本比 AppStore 上高
- [企业微信](https://work.weixin.qq.com/) - 腾讯
- [Zoom](https://zoom.us/) - Web 端 & 桌面端，免费用户 3 人以上 40 分钟会议，只要有一个收费用户即无限制
- [Teams](https://teams.microsoft.com/) - Web 端 + 桌面端
- [钉钉](https://www.dingtalk.com/) - 阿里的协同工具，[AppStore](https://apps.apple.com/cn/app/%E9%92%89%E9%92%89/id1435447041?mt=12)
- [阿里旺旺](https://wangwang.taobao.com/)
- Telegram - `brew install telegram/telegram-desktop`

### 办公套件

- [Office365](https://www.microsoft.com/zh-cn/microsoft-365?rtc=1) - 微软 Office，可从 [AppStore](https://itunes.apple.com/cn/app-bundle/microsoft-office-365/id1450038993?mt=12) 下载，按年授权；`brew install --cask microsoft-office`
- [iWork](https://www.apple.com/iwork/) - 苹果的办公套件，Pages、Numbers、Keynote，免费，AppStore 下载
- [WPS Office MAC 版](https://www.wps.cn/) 或 [2](https://www.wps.com/zh-hant/office/mac/) - 金山的 WPS，不要用 brew 里的 wpsoffice，是国际版，要用 `brew install --cask wpsoffice-cn`。网站上下载很乱，各种版本，也只有在线安装包，找不到离线安装包。v7.4.1
- [ProjectLibre](http://www.projectlibre.com/) - 项目管理软件，Office Project 的替代，前身是 OpenProj
- [OpenOffice](https://www.openoffice.org/) - 开源 Office 套件，`brew install --cask openoffice`
- [draw.io](https://www.draw.io/) - 有 Web 版和 [桌面版](https://github.com/jgraph/drawio-desktop/releases)，`brew install --cask drawio`。v27.0.5
- [PDF Expert](https://www.pdfexpert.cn/) - PDF 阅读器、编辑工具，收费
- OmniGraffle - 可以查看 Visio 文档
- [edrawmax](https://www.edrawsoft.cn/edrawmax/) - 亿图图示，收费

### 邮件客户端

- [Spark](https://sparkmailapp.com/) - 邮件客户端
- [网易邮箱大师](https://mail.163.com/dashi/) - 网易邮件客户端

### 文档编辑

- [NotepadNext](https://github.com/dail8859/NotepadNext) - Notepad++ 的 Mac 替代，v0.11，2025年，homebrew 要设置 [tap](https://github.com/dail8859/homebrew-notepadnext)
- [Typora](https://www.typora.io/) - Markdown 格式编辑器 `brew install --cask typora`，最后的[免费版 v0.11.18](https://github.com/wyf9661/typora-free)
- [VNote](https://app.vnote.fun/) -  Markdown编辑器，支持Windows/Mac/Linux，[GitHub](https://github.com/vnotex/vnote)，`brew install --cask vnote`，v3.19.2
- [MacDown](https://macdown.uranusjr.com/) - Markdown 格式编辑器 `brew install --cask macdown`
- [Sublime Text](https://www.sublimetext.com/3) - 文本编辑器 `brew install --cask sublime-text`
- [OmniGraffle 7](https://www.omnigroup.com/omnigraffle/) - 专业绘图，类 Visio，收费
- [MacVim](https://macvim.org/) - Vim 编辑器，`brew install --cask macvim`
- [MindNote](https://apps.apple.com/cn/app/mindnode-6/id1289197285?mt=12) - 思维导图，收费
- [Xmind](https://xmind.cn/) - 思维导图，收费，有免费版，v25.04
- [Meld](https://yousseb.github.io/meld/) - 差异比对合并工具，`rew install --cask meld`，[Github](https://github.com/yousseb/meld/releases/)上的版本更新，v3.21.0 (r4)，2023年，
- [DiffMerge](https://www.sourcegear.com/diffmerge/) - 比对合并工具 `brew install --cask diffmerge`
- [Beyond Compare](https://www.scootersoftware.com/) - 收费 `brew install --cask beyond-compare` v5.0.7
- [Obsidian](https://obsidian.md/download) - 免费，笔记软件，支持 Markdown。v1.8.10
- [BBEdit](https://www.barebones.com/products/bbedit/) - 文本编辑器，收费，有30天试用，`brew install --cask bbedit`
- [CotEditor](https://coteditor.com/) - 简单的文本编辑工具，`brew install --cask coteditor`
- [PlistEdit Pro](https://www.fatcatsoftware.com/plisteditpro/) - 编辑 plist 文件，Xcode 也可以，试用版
- [Xplist](https://github.com/ic005k/Xplist) - 免费的 plist 编辑器，v1.2.47 2022年

### 笔记管理

- [有道云笔记](https://note.youdao.com/index.html) - 网易的笔记工具，可以和 Windows 同步；[AppStore](https://itunes.apple.com/cn/app/%E6%9C%89%E9%81%93%E4%BA%91%E7%AC%94%E8%AE%B0/id1121484812?mt=12)；[Web 端](https://note.youdao.com/)；`brew install --cask youdaonote`
- [印象笔记](https://yinxiang.com/)，国际版 [Evernote](https://evernote.com/intl/zh-cn/) - `brew install --cask evernote`
- [Trello](https://trello.com/)  - 任务看板，[商店](https://itunes.apple.com/cn/app/trello/id1278508951?mt=12)

### 翻译软件

- [有道词典](http://cidian.youdao.com/multi.html) - 网易的翻译软件，`brew install --cask youdaodict`
- [Eudic 欧路词典](https://www.eudic.net/v4/en/app/eudic) ,or [AppStore](https://apps.apple.com/cn/app/eudic-%E6%AC%A7%E8%B7%AF%E8%AF%8D%E5%85%B8/id434350458?mt=12) - Lite 版不支持第三方词库，基本够用 `brew install --cask eudic`
- [DeepL](https://www.deepl.com/translator) - 可以翻译整篇文档，在线版或离线版 `brew install --cask deepl`
- [Bob](https://github.com/ripperhe/Bob) - 翻译软件，支持划词翻译、截屏翻译

### 开发工具

- Java SDK - 有多个选择 `adoptopenjdk8` `adoptopenjdk11` `corretto`，举例安装 adoptopenjdk11：

```s
brew tap AdoptOpenJDK/openjdk
brew install —cask adoptopenjdk11
```

- [Visual Studio Code](https://code.visualstudio.com/) - 微软的集成开发环境，`brew install --cask visual-studio-code`
- [Xcode](https://itunes.apple.com/cn/app/xcode/id497799835?mt=12) - 苹果的集成开发环境
- [XCode Command Line Toolss](https://developer.apple.com/download/more/)
- [GitKraken](https://www.gitkraken.com/) - Git 客户端，`brew install --cask gitkraken`
- [Dash](https://kapeli.com/dash) - 管理语言框架的 api 文档，收费，但可以一直免费用，低版本也是免费的，AppStore 上还有移动端，免费，或者用另一个网页版：[https://devdocs.io/](https://devdocs.io/) 还不需要下周很大的文件 `brew install --cask dash`
- [Postman](https://www.postman.com/) - `brew install postman`
- [MySQL Workbench](https://www.mysql.com/products/workbench/) - MySQL 管理工具，支持建模 `brew install --cask mysqlworkbench`
- [Another Redis Desktop Manager](https://github.com/qishibo/AnotherRedisDesktopManager/) - Redis 客户端 `brew install --cask another-redis-desktop-manager`
- [Sequel Pro](https://sequelpro.com/) - MySQL/MariaDB 数据库管理工具 `brew install --cask sequel-pro`
- [Unity Hub](https://unity3d.com/get-unity/download) - Unity Hub，默认装的是国际版 `brew install --cask unity-hub`
- [Unity](https://unity.com/products) - Unity 开发工具 `brew install --cask unity`，一定要 Hub
- [Krita](https://krita.org/zh/) - 免费绘画软件
- [JD-GUI](http://jd.benow.ca/) - 反编译工具 `brew install --cask jd-gui`

### 图像处理

- [GIMP](https://www.gimp.org/) - 免费的图像处理工具，`brew install --cask gimp`
- [PicGo](https://picgo.github.io/PicGo-Doc/zh/) - 图床，`brew install --cask picgo`
- Adobe 全家桶

### 下载工具

- [迅雷](http://mac.xunlei.com/) - 下载工具 `brew install --cask thunder`
- [Folx](https://mac.eltima.com/cn/torrent-client.html) - 下载工具，免费 + 收费
- [Downie 4](https://software.charliemonroe.net/downie/) - 视频下载，可以下载 YouTube 视频，收费 `brew install --cask downie`
- [qBittorrent](https://www.qbittorrent.org/) - BT 客户端 `brew install --cask qbittorrent`
- [Transmission](https://transmissionbt.com/) - BT 客户端 `brew install --cask transmission`
- [Free Download Manager](https://www.freedownloadmanager.org/) - 下载工具，有 Chrome 插件集成，`brew install --cask free-download-manager`，v6.28
- [Motrix](https://motrix.app/) - 基于 Aria2 的下载工具，[GitHub](https://github.com/agalwood/Motrix)，v1.8.19，2023年
- [speedtest-cli](https://github.com/sivel/speedtest-cli) - 命令行测试工具，[网站](https://speedtest.net)，安装 `brew install speedtest-cli`，运行：`speedtest-cli --simple`

### 媒体播放

- [IINA](https://www.iina.io/) - 视频播放，开源免费，`brew install --cask iina`。v1.3.5，2024年。
- VLC - `brew install --cask vlc`
- [网易云音乐](https://music.163.com/) - 网易，`brew install --cask neteasemusic`
- [Listen 1](https://listen1.github.io/listen1/)：搜索和播放来自网易云音乐，虾米，QQ 音乐，酷狗音乐，酷我音乐网站的歌曲，`brew install --cask listen1`。v2.32.0，2024年
- [OBS Studio](https://obsproject.com/) - 截取视频采集卡视频流 `brew install --cask obs`，v31.0.3，2025年
- [HandBrake](https://handbrake.fr/) - 视频转码工具 `brew install --cask handbrake`
- [Plex](https://www.plex.tv/) - 家庭影院 `brew install --cask plex`
- [XnViewMP](https://www.xnview.com/) - 看图软件 `brew install --cask xnviewmp`
- [VidHub](https://www.freedidi.com/12241.html) - 免费的视频播放器，支持iOS、Mac、ipad、Apple TV
- [foobar2000](https://www.foobar2000.org/mac) - 有 Mac 版，v2.24.5，2025年，`brew install --cask foobar2000`

### 磁盘工具

- [Paragon NTFS](https://www.paragon-software.com/home/ntfs-mac/) - 读写 Windows NTFS 分区，收费 `brew install --cask paragon-ntfs`，其他几个都有点问题，加载不了
- [Mounty for NTFS](https://mounty.app/) - 读写 Windows NTFS 分区，免费，没找到开源，可能是闭源的，`brew install --cask mounty`，2023年，v2.4，支持 MacOS 15
- [NTFSTool](https://ntfstool.com/)- 读写 Windows NTFS 分区，免费 `brew install --cask ntfstool`，[GitHub](https://github.com/ntfstool/ntfstool)，最后更新：2024年，v3.5.1，支持 M1～M3，第一次需要安装 NTFS 驱动，见 [Help](https://ntfstool.com/help.html)，需要关闭 SIP/重启安装。谨慎使用！非开源，issue上都在骂，收费了。卸载方法见：[issue](https://github.com/ntfstool/ntfstool/issues/105)
- [Tuxera NTFS](https://ntfsformac.tuxera.com/download/) - 读写 NTFS，收费
- [DaisyDisk](https://daisydiskapp.com/) - 显示磁盘占用情况，收费，使用邮箱激活试用，`brew install --cask daisydisk`
- [Disk Inventory X](http://www.derlien.com/) - 磁盘信息情况统计，类似 WinDirStat `brew install --cask disk-inventory-x`，v1.3，非原生，依赖 Rosetta，新版本有点问题：读不出外部磁盘文件的大小
- [GrandPerspectiv](https://grandperspectiv.sourceforge.net/) - 图形显示磁盘文件大小分析，sourceforge 下载免费，AppStore 上下载收费，v3.5.3-L1，2025年。不怎么好看，但是能用
- [SquirrelDisk](https://www.squirreldisk.com/) - 磁盘空间可视化，环形显示不是很直观，v0.3.4，2023年，[Github](https://github.com/adileo/squirreldisk)
- [CalHash](https://www.titanium-software.fr/en/calhash.html) - 一个带GUI的Hash计算工具，`brew install --cask calhash`
- [Disk Space Analyzer: Inspector](https://apps.apple.com/us/app/disk-space-analyzer-inspector/id446243721?mt=12)
- [baobab](https://apps.gnome.org/zh-CN/Baobab/) - 图形化磁盘，是基于 Gnome 开发的？所以安装一堆依赖。`brew install baobab`，v48，2025年
- [ncdu](https://dev.yorhel.nl/ncdu) - 命令行模式下的磁盘分析，`brew install ncdu`

### 系统设置

- [TinkerTool](https://www.bresink.com/osx/TinkerTool.html) - 系统工具集，注意下载对应系统版本
- [Deeper](https://www.titanium-software.fr/en/deeper.html) - 配置程序，`brew install --cask deeper`
- [OnyX](https://www.titanium-software.fr/en/onyx.html) - 系统维护和配置程序，`brew install --cask onyx`
- [TopNorch](https://topnotch.app/) - 隐藏 Mac 顶部刘海，就是设置任务栏黑色，还可以设置底部圆角，`brew install --cask topnorch`

### 系统监控

- [Stat](https://github.com/exelban/stats) -  系统监控，免费且能看进程 `brew install --cask stats`。v2.11.43，2025年
- [iStat Menu](https://bjango.com/mac/istatmenus/) - 菜单栏里的系统监控工具，收费 `brew install --cask istat-menus`。v7.10.2
- [Glances](https://github.com/nicolargo/glances) - 命令行查看系统运行状态。`brew install glances`
- [iGlance](https://github.com/iglance/iGlance) - 菜单栏里的系统监控工具，多了个风扇转速（已终止开发） `brew install --cask iglance`，
- [Better Menubar](https://apps.apple.com/cn/app/better-menubar/id1472818562?mt=12) - 实时监测显示电脑内存、CPU、蓝牙设备及电量，突然检测不出了
- [MenuMeters](https://member.ipmu.jp/yuji.tachikawa/MenuMetersElCapitan/) - `brew install --cask menumeters`，[GitHub](https://github.com/yujitach/MenuMeters) ，[原版](http://www.ragingmenace.com/software/menumeters/) 不支持 10.11 以上 OSX，这个是 fork
- [BitBar](https://github.com/matryer/bitbar), [Plugins](https://github.com/matryer/bitbar-plugins) - 支持用各种插件在菜单栏显示信息 `brew install --cask bitbar`
- [Eul](https://github.com/gao-sun/eul) - 支持 Big Sur 桌面组件 `brew install --cask eul`
- [Intel® Power Gadget](https://software.intel.com/content/www/us/en/develop/articles/intel-power-gadget.html) - `brew install --cask intel-power-gadget`
- [Turbo Boost Switcher](http://tbswitcher.rugarciap.com/) - `brew install --cask turbo-boost-switcher` 睿频开关
- [coconutBattery](https://www.coconut-flavour.com/coconutbattery/) - 显示电池详细信息 `brew install --cask coconutbattery`

### VPN

- ShadowSocks - 代理服务器管理
  - [ShadowsocksX](https://github.com/shadowsocks/shadowsocks-iOS) - `brew install --cask shadowsocksx`，安装的是官方 port，GitHub 主页留了一句 “Removed according to regulations.”（被和谐）
  - [ShadowSocks-NG](https://github.com/shadowsocks/ShadowsocksX-NG) - Mac 客户端，`brew install --cask shadowsocksx-ng`
  - [ShadowSocks-NG-X](https://github.com/qinyuhang/ShadowsocksX-NG-R/) - 要看 dev 分支，`brew install --cask shadowsocksx-ng-r`
  - 不能用 windows 的 gui-config.json 配置文件，只能手动添加配置或者官网扫二维码
  - 最后在 Mac 网络设置里设置 socks 代理：127.0.0.1:1080
- [V2Ray](https://www.v2ray.com/)- 构建基础通信网络，支持 Socks、HTTP、Shadowsocks、VMess 等协议，客户端参考 [查看](https://www.v2ray.com/awesome/tools.html)
  - [V2rayU](https://github.com/yanue/V2rayU/tree/master) - Mac 客户端，`brew install --cask v2rayu`，可以设置规则。v4.2.5，2024年
  - [V2RayX](https://github.com/Cenmrev/V2RayX)- Mac 客户端，已被禁用！`brew install --cask v2rayx`，依赖 Rosetta 2，但是卸除有问题，谨慎使用。v1.5.1，2019年
  - [HollyTech](https://store.holytech.tech/clientarea.php) - 服务 + 客户端
  - [Qv2ray](https://github.com/Qv2ray/Qv2ray) - 跨平台的客户端，`brew install --cask qv2ray`
- [FortiClient](https://forticlient.com/) - 安装的是在线安装包，还要执行 FortiClientUpdate.app 完成安装 `brew install forticlient-vpn`，但是下载完整安装包很慢
- [Proxifier](https://www.proxifier.com/) - 管理应用的代理路径，收费
- [ClashX](https://github.com/yichengchen/clashX) - 类似 V2RayU
- [Clash Verge](https://github.com/clash-verge-rev/clash-verge-rev) - 原版的 Clash Verge 移除了，这个是延续。v2.2.3，2025年

### 镜像工具

- [Etcher](https://etcher.balena.io/) - 烧镜像到 U 盘 `brew install --cask balenaetcher`，v2.1.2，要用 arm64 版本
- [UNetbootin](https://unetbootin.github.io/) - 制作 Linux 安装盘 `brew install --cask unetbootin`
- [Raspberry Pi Imager](https://www.raspberrypi.com/software/) - 烧录镜像，原本是树莓派专用， `brew install --cask raspberry-pi-imager`，v1.9.0，2024年，[Github地址](https://github.com/raspberrypi/rpi-imager)

### 网盘

- [百度云盘](http://pan.baidu.com/download#pan) - `brew install --cask baidunetdisk`
- [OneDrive](https://apps.apple.com/cn/app/onedrive/id823766827?mt=12) - 微软网盘 `brew install --cask onedrive`

### 账号管理

- [KeePass](https://keepass.info/) - 密码管理
  - [KeepassXC](https://keepassxc.org/) - 跨平台 [Github](https://github.com/keepassxreboot/keepassxc/) `brew install --cask keepassxc`。v2.7.10，2025年
  - [MacPass](https://macpassapp.org) - Mac 客户端，[GitHub](https://github.com/MacPass/MacPass) `brew install --cask macpass`。v0.8.1，2022年
  - [KeePass for Mac](https://keepass.info/download/p_macosx/index.html) - 很老了，最后更新 2013 年
  - [KeeWeb](https://keeweb.info/) - Web 端和桌面端， [Github](https://github.com/keeweb/keeweb) `brew install --cask keeweb`
- LastPass - Google 插件
- [1Password](https://1password.com/) - 密码管理 `brew install --cask 1password`

### 壁纸屏保

- [Wallpaper Wizard](https://wallwiz.com/) - 收费，摄影作品
- [fliqlo](https://fliqlo.com/) - 时钟屏幕保护 `brew install --cask fliqlo` v1.9.4，2024年
- Dynamic Wallpaper Engine - 收费，免费版叫花见
- 壁纸精灵 - 收费
- [Unsplash Wallpapers](https://unsplash.com/wallpapers) - 免费，自然
- [Pap.er](http://paper.meiyuan.in/)

### 预览增强

```bash
#Quick Look 系列
brew install --cask qlcolorcode    #预览脚本时自动代码配色
brew install --cask qlstephen      #预览未知拓展名的纯文本文件
brew install --cask qlmarkdown     #预览 Markdown 文件
brew install --cask quicklook-json #预览 JSON 文件
brew install --cask quicklook-csv  #预览 CSV 文件
brew install --cask qlimagesize    #预览图片大小
brew install --cask qlvideo        #预览视频
brew install --cask provisionql    #预览 mobileprovision、provisionprofile、ipa 文件

```

### 文件管理

- [transnomino](https://www.transnomino.com/) - 文件批量改名，支持正则表达式，v9.3，2025年
- [FileBot](https://www.filebot.net/) - 视频文件名批量处理
- [ABetterFinderRename](https://www.publicspace.net/ABetterFinderRename/index.html)

### 其他

- [Steam](https://store.steampowered.com/about/) - 游戏平台，Steam 的 Mac 版本，v4.0，`brew install --cask steam`
- [RetroArch](https://www.retroarch.com/) - v1.21.0，`brew install --cask retroarch`

## 命令行工具

一些好用的第三方命令行工具（待整理）

- autojump - `brew install autojump`
- thefuck - `brew install thefuck`
- screenfetch - 显示系统信息，`brew install screenfetch`
- [mackup](https://github.com/lra/mackup) - 备份配置，我的配置：[my-mac-mackup-backup](https://github.com/yingw/my-mac-mackup-backup)，`brew install mackup`
- [diskutil](https://www.jianshu.com/p/6a1f365617ad)
- [Karabiner-Elements](https://karabiner-elements.pqrs.org/) - 键盘映射，但是会覆盖系统自动的修饰键映射，要重新映射一下，但是不能映射组合键 `brew install --cask karabiner-elements`

## 网站

- [Dynamic Wallpaper Club](https://dynamicwallpaper.club/) - 动态壁纸俱乐部，手动下载动态壁纸
- [MacWk](https://www.macwk.com/soft/all/p1) - Mac 软件网站
