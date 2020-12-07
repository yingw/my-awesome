# Mac 软件

> 记录我在 MacOS 上使用的工具和配置

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
    - [下载工具](#下载工具)
    - [媒体播放](#媒体播放)
    - [磁盘工具](#磁盘工具)
    - [系统设置](#系统设置)
    - [系统监控](#系统监控)
    - [VPN](#vpn)
    - [镜像工具](#镜像工具)
    - [网盘](#网盘)
    - [账号管理](#账号管理)
    - [预览增强](#预览增强)
  - [命令行工具](#命令行工具)

<!-- /TOC -->

## 系统工具

- [Homebrew](https://brew.sh/) - 软件管理
- [Cakebrew](https://www.cakebrew.com/) - Homebrew 图形界面管理，`brew cask install cakebrew`
- [Alfred](https://apps.apple.com/cn/app/alfred/id405843582?mt=12) - 搜索、快速启动工具，很多功能，`brew cask install alfred`
- [CheetSheet](https://www.mediaatelier.com/CheatSheet/) - 快捷键提示，长按 Command，`brew cask install cheatsheet`，其他 Mac 的快捷键提示，[参考](https://sspai.com/post/45338)，[官方](https://support.apple.com/zh-cn/HT201236)
- [Mactracker](https://apps.apple.com/cn/app/mactracker/id430255202?mt=12) - 提供苹果全系列产品的所有信息
- [HandShaker](https://www.smartisan.com/apps/#/handshaker) - 锤子科技的文件管理软件，用于在 Mac 电脑上管理 Android 手机内容
- [LaunchRocket](https://github.com/jimbojsb/launchrocket) - 管理服务，`brew cask install launchrocket`
- [GamePad Companion](https://apps.apple.com/us/app/gamepad-companion/id428799479?mt=12) - 手柄驱动，收费
- [超级右键](https://apps.apple.com/cn/app/%E8%B6%85%E7%BA%A7%E5%8F%B3%E9%94%AE-irightmouse/id1497428978?mt=12) - 右键菜单管理软件
- [Better And Better](https://www.better365.cn/bab2.html) - 触控板、鼠标、键盘的手势等
- [AdGrard](https://adguard.com/zh_cn/welcome.html) - 拦截多个浏览器、系统的广告，收费
- [Vanilla](https://matthewpalmer.net/vanilla/) - 免费版可以隐藏任菜单栏图标，Pro 有更多功能
- [Bartender](https://www.macbartender.com/) - 管理菜单栏图标，收费
- [Itsycal](https://www.mowglii.com/itsycal/) - 菜单栏日历
- [QuickRes](https://thnkdev.com/QuickRes/) - 快速切换分辨率，收费
- [Ethernet Status](https://apps.apple.com/cn/app/ethernet-status/id1186187538?mt=12) - 显示有线网络连接状态
- [Scroll Reverser](https://pilotmoon.com/scrollreverser/) - 分离触摸板和鼠标的自然滚动设置
- [InsomniaX](https://insomniax.en.softonic.com/mac) - 控制 Mac 在合上盖子和闲置超时后是否进入休眠状态
- [Monitor Control](https://github.com/MonitorControl/MonitorControl) - 控制扩展视频输出的显示亮度和设备音量 `brew cask install monitorcontrol`
- [Gas Mask](https://github.com/2ndalpha/gasmask) - Hosts 管理 `brew cask install gas-mask`
- [SwitchHosts](https://github.com/oldj/SwitchHosts) - Hosts 模板，快速切换 `brew cask install switchhosts`
- [MacOS小助手](https://www.macwk.com/soft/macos-assistant-macwk) - 工具集，含禁用 macOS 更新提示

### 终端工具

- [iTerm2](https://www.iterm2.com/) - 好用的终端工具，`brew cask install iterm2`
- [oh-my-zsh](https://ohmyz.sh/) - [参考](https://sspai.com/post/55176)
  - 修改主题 `～/.zshrc`，agnoster
  - 安装 [字体](https://github.com/powerline/fonts.git) ，用 `DejaVu Sans Mono for Powerline`

### 虚拟机

- [Parallels Desktop](https://www.parallels.com/) - 虚拟机，收费
- [Virtualbox](https://www.virtualbox.org/) - 虚拟机，`brew cask install virtualbox`
- [VMWare Fusion Player/Pro](https://www.vmware.com/products/fusion/fusion-evaluation.html)

### 输入法

- [搜狗输入法](https://pinyin.sogou.com/mac/) - `brew cask install sogouinput`
- [自动切换输入法](https://apps.apple.com/cn/app/%E8%87%AA%E5%8A%A8%E5%88%87%E6%8D%A2%E8%BE%93%E5%85%A5%E6%B3%95/id1470350547?mt=12)

### 系统清理

- [腾讯柠檬清理](https://lemon.qq.com/) - 腾讯的系统清理软件，有工具栏提示 `brew cask install tencent-lemon`
- [Dr.Cleaner](https://dr-cleaner.en.softonic.com/mac) - 系统清理工具，免费
- [CleanMyMac X](https://macpaw.com/cleanmymac) - 系统清理工具，收费 `brew cask install cleanmymac`
- [AppCleaner](http://freemacsoft.net/appcleaner/) - 卸载应用，`brew cask install appcleaner`

### 截屏工具

- [iPic](https://toolinbox.net/iPic/) - 图床
- [Annotate](https://itunes.apple.com/us/app/annotate-capture-screenshot/id918207447?mt=12) - 截屏工具
- [Snipaste](https://www.snipaste.com/download.html) - 截图软件，免费 `brew cask install snipaste`
- [iShot](https://apps.apple.com/cn/app/ishot-%E6%88%AA%E5%9B%BE-%E5%BD%95%E5%B1%8F-2020%E5%85%A8%E6%96%B0%E9%AB%98%E5%BA%A6/id1485844094?mt=12) - 截图工具，支持长截图
- [Kap](https://getkap.co/)，[GitHub](https://github.com/wulkano/kap)： `brew cask install kap` 可以截屏，可以录屏为 GIF 或者 MP4

### 压缩解压

- [Keka](https://www.keka.io/en/) - 免费下载，AppStore 上收费，也是 [7zip](https://www.7-zip.org/download.html) 的非官方 Mac 版 `brew cask install keka`
- [Betterzip](https://www.betterzip.net/) - 收费 `brew cask install betterzip`
- [The Unarchiver](https://www.theunarchiver.com/) - 免费，`brew cask install the-unarchiver`
- [eZip](https://ezip.awehunt.com/) - 国产解压缩工具，免费 `brew cask install ezip`
- [Bandizip](http://www.bandisoft.com/bandizip.mac/) - 收费

### 剪贴板管理

- [CopyLess 2](https://apps.apple.com/cn/app/copyless-2/id993841014?mt=12) - 剪贴板管理，免费版可以记录 100 个历史和 5 个收藏
- [Paste](https://pasteapp.io/) - 剪贴板工具，收费

### 浏览器

- [Chrome](https://www.google.com/chrome/) - `brew cask install google-chrome`，Chrome 上的插件参考：[Chrome 插件](./chrome.md)

### 性能测试

- [Geekbench](https://www.geekbench.com/) - 系统检测评分，收费 `brew cask install geekbench`
- [Blackmagic Disk Speed Test](https://apps.apple.com/us/app/blackmagic-disk-speed-test/id425264550?mt=12) - 磁盘性能测试
- [Cinebench](https://www.maxon.net/en/products/cinebench-r20-overview/) - GPU 图形性能测试 `brew cask install cinebench`

### 远程控制

- [TeamViewer](https://www.teamviewer.cn/cn/) - 远程控制
- [VNC Viewer](https://www.realvnc.com/en/connect/download/viewer/) - VNC 客户端
- [向日葵](https://sunlogin.oray.com/download/) - 远程控制
- 开启远程控制 - `共享 - 开启 “远程登录”、“远程管理”`
- [蒲公英](https://apps.apple.com/cn/app/id1305707014) - 异地组网
- [Remote Desktop Manager](https://remotedesktopmanager.com/) - 有 Free 和 Enterprise 版本，支持 Windows 和 Mac
- Screen Sharing.APP（屏幕共享） - Mac 自带的 VNC 客户端
- [AnyDesk](https://anydesk.com/zhs) 远程桌面，需要对方也安装，用 ID 链接
- [Microsoft Remote Desktop](https://apps.apple.com/us/app/microsoft-remote-desktop/id715768417)，最新版 8.0.44，应用商店里锁国区，可以到 [外面](https://rink.hockeyapp.net/apps/5e0c144289a51fca2d3bfa39ce7f2b06/) 下 Version 10.2.13 (1593)，或者从 brew 安装

### 协同工具

- [企业微信](https://work.weixin.qq.com/) - 腾讯
- [Zoom](https://zoom.us/) - Web 端 & 桌面端，免费用户 3 人以上 40 分钟会议，只要有一个收费用户即无限制
- [Teams](https://teams.microsoft.com/) - Web 端 + 桌面端
- [钉钉](https://www.dingtalk.com/) - 阿里的协同工具，[AppStore](https://apps.apple.com/cn/app/%E9%92%89%E9%92%89/id1435447041?mt=12)
- [阿里旺旺](https://wangwang.taobao.com/)

### 办公套件

- [Office365](https://www.microsoft.com/zh-cn/microsoft-365?rtc=1) - 微软 Office，可从 [AppStore](https://itunes.apple.com/cn/app-bundle/microsoft-office-365/id1450038993?mt=12) 下载，按年授权；`brew cask install microsoft-office`
- [iWork](https://www.apple.com/iwork/) - 苹果的办公套件，Pages、Numbers、Keynote，免费，AppStore 下载
- [WPS Office MAC 版](https://www.wps.cn/) 或 [2](https://www.wps.com/mac/) - 金山的 WPS，免费 `brew cask install wpsoffice`
- [ProjectLibre](http://www.projectlibre.com/) - 项目管理软件，Office Project 的替代，前身是 OpenProj
- [OpenOffice](https://www.openoffice.org/) - 开源 Office 套件，`brew cask install openoffice`
- [draw.io](https://www.draw.io/) - 有 Web 版和 [桌面版](https://github.com/jgraph/drawio-desktop/releases)，`brew cask install drawio`
- [PDF Expert](https://www.pdfexpert.cn/) - PDF 阅读器、编辑工具，收费

### 邮件客户端

- [Spark](https://sparkmailapp.com/) - 邮件客户端
- [网易邮箱大师](https://mail.163.com/dashi/) - 网易邮件客户端

### 文档编辑

- [Typora](https://www.typora.io/) - Markdown 格式编辑器，`brew cask install typora`
- [Sublime Text](https://www.sublimetext.com/3) - 文本编辑器，`brew cask install sublime-text`
- [OmniGraffle 7](https://www.omnigroup.com/omnigraffle/) - 专业绘图，类 Visio，收费
- [MacVim](https://github.com/macvim-dev/macvim) - Vim 编辑器，`brew cask install macvim`
- [MindNote](https://apps.apple.com/cn/app/mindnode-6/id1289197285?mt=12) - 思维导图，收费

### 笔记管理

- [有道云笔记](https://note.youdao.com/index.html) - 网易的笔记工具，可以和 Windows 同步；[AppStore](https://itunes.apple.com/cn/app/%E6%9C%89%E9%81%93%E4%BA%91%E7%AC%94%E8%AE%B0/id1121484812?mt=12)；[Web 端](https://note.youdao.com/)；`brew cask install youdaonote`
- [印象笔记](https://yinxiang.com/)，国际版 [Evernote](https://evernote.com/intl/zh-cn/) - `brew cask install evernote`
- [Trello](https://trello.com/)  - 任务看板，[商店](https://itunes.apple.com/cn/app/trello/id1278508951?mt=12)

### 翻译软件

- [有道词典](http://cidian.youdao.com/multi.html) - 网易的翻译软件，`brew cask install youdaodict`
- [Eudic 欧路词典](https://www.eudic.net/v4/en/app/eudic) ,or [AppStore](https://apps.apple.com/cn/app/eudic-%E6%AC%A7%E8%B7%AF%E8%AF%8D%E5%85%B8/id434350458?mt=12) - Lite 版不支持第三方词库，基本够用 `brew cask install eudic`

### 开发工具

- [Visual Studio Code](https://code.visualstudio.com/) - 微软的集成开发环境，`brew cask install visual-studio-code`
- [Xcode](https://itunes.apple.com/cn/app/xcode/id497799835?mt=12) - 苹果的集成开发环境
- [XCode Command Line Toolss](https://developer.apple.com/download/more/)
- [GitKraken](https://www.gitkraken.com/) - Git 客户端，`brew cask install gitkraken`
- [Dash](https://kapeli.com/dash) - 管理语言框架的 api 文档，收费，但可以一直免费用，低版本也是免费的，AppStore 上还有移动端，免费，或者用另一个网页版：[https://devdocs.io/](https://devdocs.io/) 还不需要下周很大的文件 `brew cask install dash`

### 下载工具

- [迅雷](http://mac.xunlei.com/) - 下载工具 `brew cask install thunder`
- [Folx](https://mac.eltima.com/cn/torrent-client.html) - 下载工具，免费 + 收费
- [Downie 4](https://software.charliemonroe.net/downie/) - 视频下载，可以下载 YouTube 视频，收费 `brew cask install downie`

### 媒体播放

- [IINA](https://www.iina.io/) - 视频播放，开源免费
- VLC - `brew cask install vlc`
- [网易云音乐](https://music.163.com/) - 网易，`brew cask install neteasemusic`
- [Listen 1](https://listen1.github.io/listen1/)：搜索和播放来自网易云音乐，虾米，QQ 音乐，酷狗音乐，酷我音乐网站的歌曲，`brew cask install listen1`

### 磁盘工具

- [DaisyDisk](https://daisydiskapp.com/) - 显示磁盘占用情况，收费 `brew cask install daisydisk`
- [Paragon NTFS](https://www.paragon-software.com/home/ntfs-mac/) - 读写 Windows NTFS 分区，收费 `brew cask install paragon-ntfs`
- [Mounty for NTFS](https://mounty.app/) - 读写 Windows NTFS 分区，免费，`brew cask install mounty`
- [NTFSTool](https://ntfstool.com/)- 读写 Windows NTFS 分区，免费 `brew cask install ntfstool`
- [Disk Inventory X](http://www.derlien.com/) - 磁盘信息情况统计，类似 WinDirStat `brew cask install disk-inventory-x`

### 系统设置

- [TinkerTool](https://www.bresink.com/osx/TinkerTool.html) - 工具集
- [Deeper](https://www.titanium-software.fr/en/deeper.html) - 配置程序，`brew cask install deeper`
- [OnyX](https://www.titanium-software.fr/en/onyx.html) - 系统维护和配置程序，`brew cask install onyx`

### 系统监控

- [Glances](https://github.com/nicolargo/glances) - 命令行查看系统运行状态。`brew cask install glances`
- [iStat Menu](https://bjango.com/mac/istatmenus/) - 菜单栏里的系统监控工具，收费 `brew cask install istat-menus`
- [iGlance](https://github.com/iglance/iGlance) - 菜单栏里的系统监控工具，多了个风扇转速 `brew cask install iglance`
- [Better Menubar](https://apps.apple.com/cn/app/better-menubar/id1472818562?mt=12) - 实时监测显示电脑内存、CPU、蓝牙设备及电量
- [MenuMeters](https://member.ipmu.jp/yuji.tachikawa/MenuMetersElCapitan/) - `brew cask install menumeters`，[GitHub](https://github.com/yujitach/MenuMeters) ，[原版](http://www.ragingmenace.com/software/menumeters/) 不支持 10.11 以上 OSX，这个是 fork
- [BitBar](https://github.com/matryer/bitbar), [Plugins](https://github.com/matryer/bitbar-plugins) - 支持用各种插件在菜单栏显示信息 `brew cask install bitbar`

### VPN

- ShadowSocks - 代理服务器管理
  - [ShadowsocksX](https://github.com/shadowsocks/shadowsocks-iOS) - `brew cask install shadowsocksx`，安装的是官方 port，GitHub 主页留了一句 “Removed according to regulations.”（被和谐）
  - [ShadowSocks-NG](https://github.com/shadowsocks/ShadowsocksX-NG) - Mac 客户端，`brew cask install shadowsocksx-ng`
  - [ShadowSocks-NG-X](https://github.com/qinyuhang/ShadowsocksX-NG-R/) - 要看 dev 分支，`brew cask install shadowsocksx-ng-r`
  - 不能用 windows 的 gui-config.json 配置文件，只能手动添加配置或者官网扫二维码
  - 最后在 Mac 网络设置里设置 socks 代理：127.0.0.1:1080
- [V2Ray](https://www.v2ray.com/)- 构建基础通信网络，支持 Socks、HTTP、Shadowsocks、VMess 等协议，客户端参考 [查看](https://www.v2ray.com/awesome/tools.html)
  - [V2rayU](https://github.com/yanue/V2rayU/tree/master) - Mac 客户端，`brew cask install v2rayu`
  - [V2RayX](https://github.com/Cenmrev/V2RayX)- Mac 客户端，`brew cask install v2rayx`
  - [HollyTech](https://store.holytech.tech/clientarea.php) - 服务 + 客户端
  - [Qv2ray](https://github.com/Qv2ray/Qv2ray) - 跨平台的客户端，`brew cask install qv2ray`

### 镜像工具

- [Etcher](https://www.balena.io/etcher/) - 烧镜像到 U 盘 `brew cask install balenaetcher`

### 网盘

- [百度云盘](http://pan.baidu.com/download#pan) - `brew cask install baidunetdisk`
- [OneDrive](https://apps.apple.com/cn/app/onedrive/id823766827?mt=12) - 微软网盘 `brew cask install onedrive`

### 账号管理

- [KeePass](https://keepass.info/) - 密码管理
  - [KeepassXC](https://keepassxc.org/) - 跨平台 [Github](https://github.com/keepassxreboot/keepassxc/) `brew cask install keepassxc`
  - [MacPass](https://macpassapp.org) - Mac 客户端，[GitHub](https://github.com/MacPass/MacPass) `brew cask install macpass`
  - [KeePass for Mac](https://keepass.info/download/p_macosx/index.html) - 很老了，最后更新 2013 年
  - [KeeWeb](https://keeweb.info/) - Web 端和桌面端， [Github](https://github.com/keeweb/keeweb) `brew cask install keeweb`
- LastPass - Google 插件
- [1Password](https://1password.com/) - 密码管理 `brew cask install 1password`

### 预览增强

```bash
#Quick Look 系列
brew cask install qlcolorcode    #预览脚本时自动代码配色
brew cask install qlstephen      #预览未知拓展名的纯文本文件
brew cask install qlmarkdown     #预览 Markdown 文件
brew cask install quicklook-json #预览 JSON 文件
brew cask install quicklook-csv  #预览 CSV 文件
```

## 命令行工具

一些好用的第三方命令行工具（待整理）

- autojump - `brew install autojump`
- thefuck - `brew install thefuck`
- screenfetch - 显示系统信息，`brew install screenfetch`
- [mackup](https://github.com/lra/mackup) - 备份配置，我的配置：[my-mac-mackup-backup](https://github.com/yingw/my-mac-mackup-backup)，`brew install mackup`
- [diskutil](https://www.jianshu.com/p/6a1f365617ad)
