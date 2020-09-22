# My Awesome Mac

> 记录我在 MacOS 上使用的工具和配置

目录

<!-- TOC -->

- [My Awesome Mac](#my-awesome-mac)
  - [系统工具](#系统工具)
    - [协同工具](#协同工具)
    - [文档编辑](#文档编辑)
  - [VPN](#vpn)
  - [镜像](#镜像)
  - [1.2. 开发工具](#12-开发工具)
  - [1.3. MacOS 恢复功能](#13-macos-恢复功能)
  - [1.4. 初始化](#14-初始化)
  - [1.5. 安装 Windows](#15-安装-windows)
  - [2.1. 账号管理](#21-账号管理)
  - [2.2. Productive](#22-productive)
  - [2.3. System Software](#23-system-software)
  - [2.4. Development Software](#24-development-software)
    - [2.4.1. IDE](#241-ide)
  - [2.5. Game Development](#25-game-development)
  - [2.6. CheatSheet](#26-cheatsheet)
  - [2.7. 虚拟机](#27-虚拟机)
    - [2.7.1. parallels desktop](#271-parallels-desktop)
    - [2.7.2. VMWare Fusion ，VirtualBox](#272-vmware-fusion-virtualbox)
    - [环境变量](#环境变量)
    - [JDK](#jdk)
    - [压缩解压](#压缩解压)

<!-- /TOC -->

## 系统工具

- [Homebrew](https://brew.sh/)：用来软件管理。后面有很多软件都是用 Homebrew 安装。

### 协同工具

- [企业微信](https://work.weixin.qq.com/)：腾讯的，AppStore 下载。
- [Zoom](https://zoom.us/)：可以在 web 端使用，也有桌面端应用，免费用户 3 人以上 40 分钟会议，只要有一个收费用户即无限制。
- [Teams](https://teams.microsoft.com/)：微软的会议解决方案，web 端 + 桌面端。
- [钉钉](https://www.dingtalk.com/)：阿里旗下。

### 文档编辑

- [Typora](https://www.typora.io/)：Markdown 格式编辑器。
- [有道云笔记](https://note.youdao.com/index.html)：笔记，可以和 Windows 同步；[AppStore](https://itunes.apple.com/cn/app/%E6%9C%89%E9%81%93%E4%BA%91%E7%AC%94%E8%AE%B0/id1121484812?mt=12)；[在线版](https://note.youdao.com/)。
- 办公套件
  - Office：微软 Office，可以从 AppStore 下载，按年授权。
  - iWork：苹果的办公套件，AppStore 下载。
  - 邮箱：Outlook 或者 [Spark](https://sparkmailapp.com/) 免费版够用
  - [ProjectLibre](http://www.projectlibre.com/)：项目管理软件，Office Project 的替代，前身是免费的 OpenProj
  - [OpenOffice](https://www.openoffice.org/)：`brew cask install openoffice`
- iWorks 套件：苹果的办公三件套，现在免费了，系统默认安装。可以导出为 Office 格式
  - Pages
  - Numbers
  - Keynote

- [迅雷](http://mac.xunlei.com/)：下载工具
- SAP GUI Java 版
- 视频
- PDF 阅读器
- [mackup](https://github.com/lra/mackup)：备份配置，我的配置：[my-mac-mackup-backup](https://github.com/yingw/my-mac-mackup-backup)
- [iTerm2](https://www.iterm2.com/)：最好的终端，`brew cask install iterm2`
- zsh，[ohmyzsh](https://ohmyz.sh/)：[参考](https://sspai.com/post/55176)
  - 修改主题 `～/.zshrc`，agnoster
  - 安装 [字体](https://github.com/powerline/fonts.git) ，用 `DejaVu Sans Mono for Powerline`
- [Disk Inventory X 1.2](http://www.derlien.com/) 磁盘信息情况统计，类似 WinDirStat
- [Kap](https://getkap.co/)，[GitHub](https://github.com/wulkano/kap)： `brew cask install kap` 可以截屏，可以录屏为 GIF 或者 MP4
- [MenuMeters](https://member.ipmu.jp/yuji.tachikawa/MenuMetersElCapitan/)，[GitHub](https://github.com/yujitach/MenuMeters) `brew cask install menumeters`，[原版](http://www.ragingmenace.com/software/menumeters/) 不支持 10.11 以上 OSX，这个是 fork
- [AnyDesk](https://anydesk.com/zhs) 远程桌面，貌似需要对方也安装，用 ID 链接
- [Microsoft Remote Desktop](https://apps.apple.com/us/app/microsoft-remote-desktop/id715768417)，最新版 8.0.44，不知道为什么应用商店里锁国区，可以到 [外面](https://rink.hockeyapp.net/apps/5e0c144289a51fca2d3bfa39ce7f2b06/) 下着 Version 10.2.13 (1593)，或者从 brew 安装
- Windows 远程 Mac 可以用 VNC，在设置 - 共享 - 开启 “远程管理”- 允许 “VNC 用密码控制”，也可以只开 “屏幕共享”
- Mac 自带一个 VNC 客户端：屏幕共享（Screen Sharing.APP）
- screenfetch `brew install`
- [Xcode](https://itunes.apple.com/cn/app/xcode/id497799835?mt=12)
- [Trello](https://trello.com/) ：任务看板，[商店](https://itunes.apple.com/cn/app/trello/id1278508951?mt=12)
- [MindNote](https://apps.apple.com/cn/app/mindnode-6/id1289197285?mt=12) 思维导图，收费
- [Eudic 欧路词典](https://apps.apple.com/cn/app/eudic-%E6%AC%A7%E8%B7%AF%E8%AF%8D%E5%85%B8/id434350458?mt=12)：Lite 版不支持第三方词库，基本也够用
- [Alfred](https://apps.apple.com/cn/app/alfred/id405843582?mt=12)：搜索，很多功能
- [Zoom](https://www.zoom.us/download) 视频会议
- [钉钉](https://www.dingtalk.com/)：[应用商店](https://apps.apple.com/cn/app/%E9%92%89%E9%92%89/id1435447041?mt=12)
- [阿里旺旺](https://wangwang.taobao.com/)
- [CopyLess 2](https://apps.apple.com/cn/app/copyless-2/id993841014?mt=12)：剪贴板管理，免费版可以记录 100 个历史和 5 个收藏
- [Ethernet Status](https://apps.apple.com/cn/app/ethernet-status/id1186187538?mt=12) 能显示有线网络连接状态
- [Scroll Reverser](https://pilotmoon.com/scrollreverser/) 分离触摸板和鼠标的自然滚动设置
- InsomniaX 不行

## VPN

- ShadowSocks
翻墙工具，brew 上面有三个
  - [ShadowsocksX](https://github.com/shadowsocks/shadowsocks-iOS) 可以用
  - 安装: `brew cask install shadowsocksx` 安装的是官方 port，但是 github 主页留了一句 “Removed according to regulations.”（被和谐）
  - 不能用 windows 的 gui-config.json 配置文件，只能手动添加配置或者官网扫二维码
  - 最后在 Mac 网络设置里设置 socks 代理：127.0.0.1:1080
- [ShadowSocks-NG](https://github.com/shadowsocks/ShadowsocksX-NG)：用链接或二维码导出导入配置，版本 1.8.2
- [ShadowSocks-NG-X](https://github.com/qinyuhang/ShadowsocksX-NG-R/)：要看 dev 分支
- [HollyTech](https://store.holytech.tech/clientarea.php) - 客户端使用 [V2Ray](https://www.v2ray.com/)，各种客户端可以 [查看](https://www.v2ray.com/awesome/tools.html)，如 [Qv2ray](https://github.com/Qv2ray/Qv2ray) / [V2rayU](https://github.com/yanue/V2rayU/tree/master) / [V2RayX](https://github.com/Cenmrev/V2RayX)（订阅配置：https://subs.holytech.bid/osubscribe.php?sid=51886&token=wNiSdIyjw11z）

## 镜像

- [Etcher](https://www.balena.io/etcher/) - 烧镜像到 U 盘

## 1.2. 开发工具

- [Medis](https://github.com/luin/medis) Redis 客户端，打包收费，需要自己编译
- [Sequel Pro](https://github.com/sequelpro/sequelpro) MySQL 客户端，好久不更新了。如果只连 MySQL 可以用这个
- [DBeaver](http://dbeaver.io/)：`brew cask install dbeaver-community`

## 1.3. MacOS 恢复功能

[官方文档](https://support.apple.com/zh-cn/HT201314)，关机状态下按住 `Command (⌘)-R`，再按电源键开机，进入恢复，可以：

1. Restore From Time Machine Backup
2. Reinstall Mac OS X
3. Disk Utility （分区）

注：重装需要联网下载整个 OS 镜像

或者 [制作使用引导安装器](https://support.apple.com/zh-cn/HT201372)

## 1.4. 初始化

## 1.5. 安装 Windows

用 Mac 做 Windows 启动盘，需要 ISO 文件，[官方文档](https://support.apple.com/zh-cn/HT205016)
[在 Mac 上通过 “启动转换助理” 安装 Windows 10](https://support.apple.com/zh-cn/HT201468)

[参考](https://www.cnblogs.com/zhengxu/articles/6145651.html)

要用 Mac 的 Bootcamp 制作启动盘；（不需要）
重装后要在 U 盘里面执行

安装过程下周 2G 左右的驱动

切换：开机按着 Optional

## 2.1. 账号管理

- [百度云盘](http://pan.baidu.com/download#pan)
- [KeePass](https://keepass.info/) 密码管理  可能不支持 Mac；有个对应的 [Mac 版](https://keepass.info/download/p_macosx/index.html)，但是很老了 13 年
- [MacPass](https://macpassapp.org)；有个 web 在线版本 [KeeWeb](https://keeweb.info/) 也 [开源](https://github.com/keeweb/keeweb)7k star，也有对应用 Electron 封装的桌面版（太大）；
- [KeepassXC](https://keepassxc.org/) 跨平台  [Github](https://github.com/keepassxreboot/keepassxc/) 5k
- [OneDrive](https://apps.apple.com/cn/app/onedrive/id823766827?mt=12) 微软网盘
- Google 插件：LastPass
- Google 自己管理同步

## 2.2. Productive

- [Remote Desktop Manager](https://remotedesktopmanager.com/) 有 Free 和 Enterprise 版本，支持 Windows 和 Mac

## 2.3. System Software

- 1ting?
- Video player

## 2.4. Development Software

### 2.4.1. IDE

- [Visual Studio Code](https://code.visualstudio.com/) `brew cask install visual-studio-code`
- 加环境变量
- Intellij
- [Spring Tools (STS)](https://spring.io/tools/)
brew cask install springtoolsuite
- Nodejs `brew install node`

## 2.5. Game Development

- unity

要下载蛮多主键时间较长
(开启 ssl)

```bash
brew install wget
brew install curl
brew install openssl

brew install fish      #安装 fish shell
brew install git-flow  #安装 git-flow
brew install python    #安装 python
```

```bash
brew cask install launchrocket   #管理软件后台服务
brew cask install google-chrome  #安装 Chrome
brew cask install the-unarchiver #解压软件
brew cask install alfred         #效率软件
brew cask install qq             #腾讯 QQ
brew cask install evernote       #云笔记软件
brew cask install sublime-text   #文本编辑器
brew cask install skitch         #ervernote 配套的截图软件
brew cask install dropbox        #文件同步软件
brew cask install zotero         #网页收藏与文献管理软件
brew cask install anki           #记忆软件
brew cask install virtualbox     #虚拟机，可以装个 Windows
brew cask install self-control   #避免分心的软件
brew cask install vlc            #视频软件
brew cask install appcleaner     #应用清理
```

```bash
#Quick Look 系列
brew cask install qlcolorcode    #预览脚本时自动代码配色
brew cask install qlstephen      #预览未知拓展名的纯文本文件
brew cask install qlmarkdown     #预览 Markdown 文件
brew cask install quicklook-json #预览 JSON 文件
brew cask install quicklook-csv  #预览 CSV 文件
```

用 Homebrew 安装 Java，[参考](https://blog.csdn.net/u013310075/article/details/81024790)，(但是下载的是 Oracle 版本，看看怎么下载 openjdk)

```bash
brew tap caskroom/versions
brew search java
brew cask install java8
```

- [SDKMAN](https://sdkman.io/)：也是 SDK 管理

```bash
curl -s "https://get.sdkman.io" | bash
source "$HOME/.sdkman/bin/sdkman-init.sh"
sdk version
sdk ls java
sdk install
```

但是 sdk 安装的 java11 别的认不到

- [Dash](https://kapeli.com/dash)，管理各个语言框架的 api 文档，收费，但可以一直免费用，低版本也是免费的，AppStore 上还有移动端，免费，或者用另一个网页版：[https://devdocs.io/](https://devdocs.io/) 还不需要下周很大的文件
- Charles 网络抓包工具
- FileZilla
- Ansible
- docker
- maven
- jdk
- iTerm2 终端 `brew cask install iterm2` 主题 / 字体 / oh-my-zsh
- [oh-my-zsh](https://ohmyz.sh/)
- `sh -c "$(curl -fsSL https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"`
- [GitKraken](https://www.gitkraken.com/) Git 客户端，免费版够用 `brew cask install gitkraken`
- sourceTree 或 [GitKraken](https://www.gitkraken.com/)
- Postman
- CleanMymac
- Parallels Desktop 虚拟机
- [1Password](https://1password.com/) 密码管理
- [iPic](https://toolinbox.net/iPic/) 图床
- TextMate 算了，换 Sublime Text
- [Sublime Text](http://www.sublimetext.com)：主流有 2 和 3，默认下载版本 3
- [Annotate](https://itunes.apple.com/us/app/annotate-capture-screenshot/id918207447?mt=12) 截屏工具
- Microsoft Office 365 六件套（Word Excel PPT Outlook OneNote OneDrive）可以字节在 AppStore 下，用公司邮箱可以直接激活 ，[参考](https://itunes.apple.com/cn/app-bundle/microsoft-office-365/id1450038993?mt=12)
- 微信 / QQ / 企业微信 / 好压 9 试用 10 天）/The Unarchiver / 爱奇艺 / 网易云音乐，这些都可以在 AppStore 直接下
- 搜狗输入助手，可以和 windows 同步字库，账号：
- 网易云音乐
- [1ting](https://listen1.github.io/listen1/)：搜索和播放来自网易云音乐，虾米，QQ 音乐，酷狗音乐，酷我音乐网站的歌曲

如何卸载内置不用的应用：如股票 / 消息

- iPic 图床
- Mac 杀毒？

Mac 没有 Visio
visio 的替代品推荐 [OmniGraffle 7](https://www.omnigroup.com/omnigraffle/) 收费，

[破解版](https://www.zhinin.com/omnigraffle_pro-mac.html)

虚拟机 PD or VB

## 2.6. CheatSheet

Mac 的快捷键提示，[参考](https://sspai.com/post/45338)，[参考](https://www.mediaatelier.com/CheatSheet)（主页打得开，软件页 404 了），[官方](https://support.apple.com/zh-cn/HT201236)

## 2.7. 虚拟机

### 2.7.1. parallels desktop

### 2.7.2. VMWare Fusion ，VirtualBox

### 环境变量

给 Mac 设置环境变量，有很多配置可以，用户环境变量推荐 `.bash_profile`，如果是 zsh 修改 `.zshrc`, 或者推荐在. zshrc 文件加一行 source .bash_profile

[参考](https://blog.csdn.net/lilang66/article/details/81415990)
`/etc/profile /etc/paths ~/.bash_profile ~/.bash_login ~/.profile ~/.bashrc`

```bash
HOMEBREW_NO_AUTO_UPDATE=1
export HOMEBREW_NO_AUTO_UPDATE

export PATH=$PATH:<PATH 1>:<PATH 2>
```

然后 source .bash_profile

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

### 压缩解压

- [Keka](https://www.keka.io/en/) - 免费下载，AppStore 上收费，也是 [7zip](https://www.7-zip.org/download.html) 的非官方 Mac 版
- [Betterzip](https://www.betterzip.net/) - 收费
- [The Unarchiver](https://www.theunarchiver.com/) - 免费
- [eZip](https://ezip.awehunt.com/) - 免费
