# Windows 工具箱

Windows 工具箱（Awesome Windows），记录我的 Windows 工具和设置

目录：

- [Windows 工具箱](#windows-工具箱)
  - [系统工具](#系统工具)
    - [系统安全](#系统安全)
    - [输入法](#输入法)
    - [密码管理](#密码管理)
    - [浏览器](#浏览器)
    - [VPN](#vpn)
    - [驱动管理](#驱动管理)
    - [磁盘管理](#磁盘管理)
    - [办公套件](#办公套件)
    - [下载工具](#下载工具)
    - [网盘](#网盘)
    - [即时通讯](#即时通讯)
    - [阅读工具](#阅读工具)
    - [看图工具](#看图工具)
    - [影音播放](#影音播放)
    - [翻译工具](#翻译工具)
    - [AI大模型](#ai大模型)
    - [远程控制](#远程控制)
    - [虚拟机](#虚拟机)
    - [终端工具](#终端工具)
    - [编辑工具](#编辑工具)
    - [压缩解压](#压缩解压)
    - [启动盘制作](#启动盘制作)
    - [截屏录屏](#截屏录屏)
    - [桌面美化](#桌面美化)
    - [其他](#其他)
  - [开发工具](#开发工具)
    - [源码管理](#源码管理)
    - [Java](#java)
    - [Python](#python)
    - [数据库工具](#数据库工具)
    - [IDE 集成开发环境](#ide-集成开发环境)
    - [其他工具](#其他工具)
    - [性能测试工具](#性能测试工具)
    - [其他运行环境](#其他运行环境)
    - [字体](#字体)
  - [Windows 自带工具](#windows-自带工具)
  - [CMD 常用命令](#cmd-常用命令)

## 系统工具

- [媒体创建工具 MediaCreationTool.exe](https://www.microsoft.com/zh-cn/software-download/windows10) - 微软官方 Windows 10 安装工具，制作 U 盘，得到名称为 ESD-USB 的 U 盘
- [QuickLook](https://github.com/QL-Win/QuickLook) - 文档快速预览工具 v3.7.3，应用商店安装，Office 文档预览还有装个 [插件](https://github.com/QL-Win/QuickLook.Plugin.OfficeViewer)
- 腾讯软件管理独立版 - 没有官网，在迅雷网盘里
- [HEU KMS Activator](https://github.com/zbezj/HEU_KMS_Activator) - v42.3.1 `HEU_KMS_Activator_v42.3.1.rar`，公众号：知彼而知己、小知彼而知己
- [图吧工具箱](https://www.tbtool.cn/) - 硬件检测工具合集，2024.09正式版

### 系统安全

用 Windows 10 自带的 Defender 和防火墙也够了

- [火绒安全软件(个人用户)](https://www.huorong.cn/) - 免费的个人安全防护、杀毒软件，个人版有5、6两个大版本，建议先用5，`sysdiag-all-5.0.76.7-2024.12.30.1.exe` `sysdiag-all-x64-6.0.4.5-2024.12.30.1.exe`
- [Autoruns](https://learn.microsoft.com/zh-cn/sysinternals/downloads/autoruns) - 微软官方的启动项管理工具 v14.11
- [Process Explorer](https://learn.microsoft.com/zh-cn/sysinternals/downloads/process-explorer) - 微软官方的进程管理工具 v17.06
- [Portmon](https://docs.microsoft.com/zh-cn/sysinternals/downloads/portmon) - 微软官方的进程监控，最后更新：2012年，可以看很多包括注册表，也可以用 `netstat` 查
- [DiskMon](https://learn.microsoft.com/zh-cn/sysinternals/downloads/diskmon) - 磁盘监控 v2.02，最后更新：2021年

### 输入法

- [搜狗输入法](https://shurufa.sogou.com/) - 同步账号的词库很方便，广告要设置关闭，已被腾讯并购 v14.12
- 微软拼音输入法
- 百度输入法

### 密码管理

- [KeePass](https://keepass.info) - 免费的密码管理工具 v2.57.1，还要下载[语言文件](https://keepass.info/translations.html)
- [LastPass](https://lastpass.com/) - Chrome 插件

### 浏览器

在特定的场合需要使用 Internet Explorer（IE 11），也可以用 Chrome 的插件 IE Tab；其他如 Edge 和 Firefox 用于测试应用的兼容性。

- [Chrome](https://www.google.com/intl/zh-CN/chrome/) - 谷歌浏览器，官网下载默认安装工具，可以下载[离线安装包](https://www.google.com/intl/en/chrome/?standalone=1)。初始登入同步需要全局代理，参考：[我的插件](./chrome.md)
- [Firefox](http://www.firefox.com.cn/) - Mozilla 的浏览器
- [Microsoft Edge](https://www.microsoft.com/en-us/edge) - 非 Windows 10 自带版本，已升级为 Chrome 内核
- [Safari](https://www.apple.com/cn/safari/) - 在 MacOSX 上测试兼容性
- [360浏览器](https://browser.360.cn/) - 15.3

### VPN

除了用来翻墙（需要购买账号），还有公司的 VPN 客户端。

- [v2rayN](https://github.com/2dust/v2rayN) - 7.4.2 版本需要 Microsoft .NET，可下载集成好的版本 `v2rayN-windows-64-SelfContained-With-Core.7z`，或者用 [QV2Ray](https://github.com/Qv2ray/Qv2ray) + [v2ray-core](https://github.com/v2fly/v2ray-core) 核心使用
- [Shadowsocks](https://github.com/shadowsocks/shadowsocks-windows) - 翻墙工具，结合 Chrome 的 SwithcyOmega 插件非常方便。初始化后，可以直接替换 `gui-config.json` 的配置。或者设置 PAC 模式
- [FortiClient](https://www.forticlient.com/) - 公司用的 VPN 客户端，也可以从 Windows 商店下载
- [EasyConnect](https://sslvpn.zjweu.edu.cn/com/installClient.html) - 深信服的 SSLVPN
- GlobalProtect - [Wilmar](https://wilmarvpn.wilmar.cn/global-protect/login.esp) 的 VPN，[下载地址](https://wilmarvpn.wilmar.cn/global-protect/msi/GlobalProtect64.msi)，[Mac 版](https://wilmarvpn.wilmar.cn/global-protect/msi/GlobalProtect.pkg)
- [SwitchHosts](https://github.com/oldj/SwitchHosts) - 切换 Hosts，再加入[地址](https://raw.hellogithub.com/hosts)更新 GitHub 地址
- [ZeroTier](https://www.zerotier.com/) - 1.10.6

### 驱动管理

建议 Windows 更新

- [驱动人生](https://qd.160.com/) - v8.16.XX，不要用驱动精灵，有标准版和集成了万能网卡驱动的网卡版，没有有线网络的环境建议用网卡版
- [鲁大师](https://www.ludashi.com/) - v6.X，有温控等，旧版鲁大师经典版v5.1
- [Splashtop Wired XDisplay](https://www.splashtop.com/wiredxdisplay) - 让 iPad 做扩展屏，收费
- [Logitech Options](https://www.logitech.com.cn/zh-cn/product/options?page=flow-multi-device-control) - 设置 Logitech Flow 多屏共享键鼠 M585 + M330，[下载地址](https://support.logi.com/hc/zh-cn/articles/360025297893)
- [Logitech G HUB](https://support.logi.com/hc/zh-cn/articles/360024361233) - 设置 G304

### 磁盘管理

- [DiskGenius](http://www.diskgenius.cn/DiskGenius) - V5.6.1 分区修改，慎用，海外版 PartitionGuru v4.9.5.508 专业版
- [WizTree](https://diskanalyzer.com/) - 磁盘使用情况可视化，类似 WinDirStat，超快，v4.23
- [WinDirStat](https://windirstat.net/) - 磁盘使用情况可视化 v1.1.2；新版本 v2.2.0 只是改了界面，还是慢
- [SpaceSniffer](http://www.uderzo.it/main_products/space_sniffer/) - 同 WinDirStat，v1.3.0.2 不更新
- [CCleaner](https://www.ccleaner.com/) - 清理工具，可以清除重复文件
- [Dism++](http://www.chuyu.me/) - 系统设置工具，可清理
- [Bootice](http://www.ipauly.com/) - 最后版本 16 年 v1.3.4.0，官网打不开，随便下载
- UltraISO - ISO 烧录，收费
- EasyBCD - 启动菜单修复工具，收费
- [EasyUEFI](https://www.easyuefi.com/index-us.html) - UEFI 信息编辑工具
- [TransMac](https://www.acutesystems.com/scrtm.htm) - 在 Windows 上打开 Mac 的 dmg 文件，收费
- [Everything](https://www.voidtools.com/zh-cn/) - 全盘检索 1.4.1.1026
- [Wox](https://github.com/Wox-launcher/Wox) - Windows 上 Everything 的启动器，类似 Alfred，打包版本，有点问题
- [Listary](https://www.listary.com/) - Everything 以外另一个搜索工具，v1.4.1196
- [PowerToys](https://github.com/microsoft/PowerToys) - 微软官方的效率工具，有快捷启动和批录重命名等 v0.87.1
- [Geek Uninstaller](https://geekuninstaller.com/) - 卸载工具 v1.5.2.165
- [PatchCleaner](https://sourceforge.net/projects/patchcleaner/) - 多余的补丁卸载工具 1.4.2.0，最后更新：2016年，Windows10 慎用，不更新
- Unlocker - 文件解除锁定工具，v1.9.2，也不更新了

### 办公套件

Office 有 2013、2016、Office365 等版本。

- [Office 2016](https://portal.office.com/account#installs) - 微软的办公套件：
  - Word
  - Excel - 安装插件
  - PowerPoint
  - Outlook - 邮箱。导入备份；登入要用应用密码，在线生成密码后要关闭窗口才能生效
  - Visio
  - Project
  - Skype for Business
  - OneDrive - 网盘个人账号，5G 免费空间
- [WPS Office](https://www.wps.cn/) - 免费，Office 替代；广告较多，有个 “配置工具” 关闭，12.1.0.18276，[旧版 WPS Office 2019](https://www.wps.cn/product/wps2019)：11.1.0.10314
- [Draw.io](https://about.draw.io/integrations/#integrations_offline) - 开源绘图工具，可替换 visio，新 [官网](https://app.diagrams.net/)，桌面版下载 [地址](https://github.com/jgraph/drawio-desktop/releases) v21.2.8
- [OpenProj](https://sourceforge.net/projects/openproj/) - 开源项目管理工具 v1.4，可替代 Project（openproj-1.4.msi），需要安装 JDK5，不更新
- [Processon](https://www.processon.com/) - 在线的作图、协作工具，免费一定额度
- [万彩办公大师](http://www.wofficebox.com/) - 好用免费的 DPF 工具套件 v3.1.2，还有个离线版推荐
- [Foxmail](https://www.foxmail.com/)

### 下载工具

- [迅雷](https://www.xunlei.com/) - 下载工具 v12.1
- [人人影视播放器](http://app.rrys.tv/) - 用来下载 [人人](http://www.zmz2019.com/) 的视频
- [FDM](https://www.freedownloadmanager.org/) - 插件支持下载 YouTube 视频

### 网盘

- [百度云](https://pan.baidu.com/download#win) - 免费 2T 空间，客户端支持 Mac、Linux 等
- [OneDrive](https://www.microsoft.com/zh-cn/microsoft-365/onedrive/download) - 微软的网盘，在 Office 套件里一起安装，[在线管理地址](https://skydrive.live.com/)
- Google Drive
- 坚果云
- [腾讯微云](https://www.weiyun.com/) - 10G
- 115、城通、夸克

### 即时通讯

- [QQ](https://im.qq.com/) - 现在也支持 [Linux 版本](https://im.qq.com/linuxqq/download.html) 了
- [微信](https://pc.weixin.qq.com/) - 个人微信，v3.9.12
- [企业微信](https://work.weixin.qq.com/) - 微信的企业版
- [阿里旺旺](https://wangwang.taobao.com/) - 也可以不安装一直用手机版或 Web 版
- [钉钉](https://www.dingtalk.com/) - 阿里旗下企业协同平台，企业用
- [Zoom](https://www.zoom.us/) - 国外用得多
- [Slack](https://slack.com/) - 国外用得多
- [Teams](https://teams.microsoft.com/) - 微软 Office 套件中
- [腾讯会议](https://meeting.tencent.com/) - v3.29.3.498

### 阅读工具

- [有道云笔记](https://note.youdao.com/note-download/) - 网易的笔记工具，支持 MarkDown 格式 v7.2.6
- [Evernote](https://evernote.com/) - 笔记工具，中国区印象笔记，用的全球区
- [福昕阅读器](https://www.foxitsoftware.cn/pdf-reader/)（FoxitReader） - PDF 文档阅读 v11
- [福昕智慧打印](https://www.foxitsoftware.cn/dayin/) - 远程调用打印机，和微信集成，方便
- [福昕 PDF 编辑器个人版](http://editor.foxitsoftware.cn/) - PDF 文档编辑工具，个人版会有水印，老版本 v9.2.3.42566，新版本 v13.3.119.26555
- SumatraPDF - 免费 PDF 浏览器

### 看图工具

- [XnView](https://www.xnview.com/en/) - 免费看图工具，有 MP 版本和 classic 版，Classic 2.52.0，MP 1.8.3
- [BandView](https://www.bandisoft.com/bandiview/) - v7.10，之前叫 [HoneyView](http://www.bandisoft.com/honeyview/) - 看图软件，与 BandZip 是一个开发商 最终版 v5.53
- [2345 看图王](http://pic.2345.cc/) - 和2345好压集成方便，v11.4
- [光影魔术手](http://www.neoimaging.cn/) - 图像编辑工具，比较老了，用习惯了 v4.4.1 不更新；24年新版本 v4.6.4
- [美图秀秀](https://xiuxiu.meitu.com/) - 图像编辑工具，有 [Linux 信创版](https://pc.meitu.com/pc?download=linux)
- [中望CAD 2024](https://www.zwcad.com/) - 国产的 CAD 工具
- [GIMP](https://www.gimp.org/downloads/) - 免费开源的PS平替 v2.10.38
- [inpaint-web](https://github.com/lxfater/inpaint-web) - 免费开源的画面修改（inpainting）、放大工具，[在线](https://inpaintweb.lxfater.com/)
- [Darktable](https://www.darktable.org/)
- [Photopea](https://www.photopea.com/) - 在线图片编辑 PS 软件
- [PhotoDemon](https://photodemon.org/) - 图片工具，可以打开PSD，v2024.12

### 影音播放

- [QQ 影音](https://player.qq.com/) - 好用，被下架了 最后版本 4.6.3.1104
- [迅雷影音](http://video.xunlei.com/pc.html) - 和迅雷集成方便，6.2.3.590
- [完美解码](http://jm.wmzhe.com/)
- [POTPlayer](http://potplayer.daum.net/?lang=zh_CN) - 播放器，也可以串流录屏 v24.12.16
- [KMPlayer](https://pc.qq.com/detail/0/detail_500.html)
- [foobar2000](https://www.foobar2000.org/) - v2.24.1
- [网易云音乐](https://music.163.com/) - 在线歌单、收藏 v2.10.5.200451
- [Listen1](https://github.com/listen1/listen1_desktop/releases) - 开源跨平台的多平台音乐播放器 v2.26.2
- [OBS Studio](https://obsproject.com/zh-cn) - 视频录制以及直播串流 v31.0.0
- [VLC media player](https://www.videolan.org/index.zh.html) - 视频播放，还支持网络流媒体播放以及捕获设备
- [Tiny Media Manager](https://www.tinymediamanager.org/) - 家庭影院视频库管理，用 v3.1.17 版，v4 收费

### 翻译工具

- [金山词霸](http://cp.iciba.com/) - 金山的桌面词典工具
- [网易有道词典](https://fanyi.youdao.com/download-Windows) - 网易、有道的桌面词典，v9.3.0 和 v11.0.0，新版本有 AI 翻译功能
- [谷歌翻译](https://translate.google.com/) - 在线
- [百度翻译](https://fanyi.baidu.com/) - 在线，支持AI翻译

### AI大模型

- [文心一言](https://yiyan.baidu.com/) - 百度
- [通义千问](https://tongyi.aliyun.com/qianwen/) - 阿里
- [讯飞星火](https://xinghuo.xfyun.cn/desk) - 科大讯飞
- [智谱清言](https://chatglm.cn/) - 清华
- [Kimi](https://kimi.moonshot.cn/) - 月之暗面
- [天工](https://www.tiangong.cn/)
- [腾讯云宝](https://yuanbao.tencent.com/) - 之前叫混元助手

国外的

- ChatGPT
- Bing
- Google Bard
- [Gemini](https://gemini.google.com/app)

### 远程控制

- [TeamViewer](https://www.teamviewer.cn/cn/) - 远程控制软件，注意漏洞
- [贝锐向日葵](https://sunlogin.oray.com/personal/) - 远程控制软件
- [贝锐蒲公英个人版](https://pgy.oray.com/download/personal)
- [Remote Desktop Manager](https://remotedesktopmanager.com/) - 多种协议的远程连接管理
- [Xming](https://sourceforge.net/projects/xming/) - 结合 ssh 工具可以远程打开 Linux 应用，给不支持桌面连接的服务器 Linux 开放桌面接入，不更新
- [FileZilla](https://filezilla-project.org/) - FTP 服务端和客户端工具 v3.62.0
- [SoapUI](https://www.soapui.org/) - SmartBear 公司的 Web Service 调试工具，有开源版和 Pro 版
- [Synergy](https://symless.com/?source=gui) - 多台电脑共享键盘和鼠标，需要服务端先添加设置客户端的主机名
- [Spacedesk](https://spacedesk.net/) - 投屏 Windows 桌面到 iPad

### 虚拟机

- [Oracle VirtualBox](https://www.virtualbox.org/) - 虚拟机
- [VMWare Workstation Pro](https://www.vmware.com/products/workstation-pro.html) - 虚拟机，个人免费
- [Windows Subsystems for Android](https://learn.microsoft.com/en-us/windows/android/wsa/) - 在 Windows Store 里下载，只支持 Windows 11
- [Windows Subsystem for Linux](https://www.microsoft.com/store/productId/9P9TQF7MRM4R) - [Ubuntu](https://www.microsoft.com/store/productId/9PDXGNCFSCZV) 或者 [22.04.2 LTS](https://www.microsoft.com/store/productId/9PN20MSR04DW)

### 终端工具

- [Windows Terminal](https://github.com/Microsoft/Terminal/) - 微软最新的终端工具，商店下载安装 v1.15.2874
- [Cmder](http://cmder.net/) - 打包了 ConEmu 等多个工具的终端
- [ConEmu](https://conemu.github.io/) - 终端工具，可以 [集成 WSL](https://conemu.github.io/en/BashOnWindows.html)
- [XShell，Xftp](https://www.netsarang.com/zh/xshell-download/) - 终端管理，家庭 / 学校用户免费
- [WinSCP](http://www.winscp.net/) - FTP 工具
- [SecureCRT](https://www.vandyke.com/products/securecrt/)
- [PuTTY](https://www.putty.org/) - 轻量级 SSH 和 Telnet 客户端

### 编辑工具

- [Typora](https://typora.io/) - Markdown 文档编辑工具，收费了，最后的免费版：
- [Notepad++](https://notepad-plus-plus.org/) - 文本编辑工具，处理大文件比较慢 v8.7.5
- [BeyondCompare](http://www.beyondcompare.cc/xiazai.html) - 文件比对工具，收费
- [UltraEdit](https://www.ultraedit.com/)
- [EmEditor](https://www.emeditor.com/) - 大文本处理比较方便
- [Xmind](https://www.xmind.cn/download/) - 思维导图，免费版导出 PDF 有水印 v22.09.3168
- [MobaXterm](https://mobaxterm.mobatek.net/) - 全能终端工具，免费版有些限制
- [Notepad3](https://github.com/rizonesoft/Notepad3) - v6.24.1221.1
- [Notepad--](https://gitee.com/cxasm/notepad--) - 有简单的比对功能，v3.0
- [Sublime Text](https://www.sublimetext.com/)
- [HBuilder](http://www.dcloud.io/) - HTML 编辑器
- [Atom](https://atom.io/) - GitHub 的编辑工具
- [Notepads](https://www.notepadsapp.com/) - 简洁的编辑器，应用商店安装
- [Notepad Next](https://github.com/dail8859/NotepadNext) - Notepad++的copy，支持Linux和Mac v0.9

### 压缩解压

- [7-Zip](https://www.7-zip.org/) - 免费开源跨平台 v24.09
- [Bandizip](http://www.bandisoft.com/bandizip/) - 无广告，支持 [Mac](https://apps.apple.com/cn/app/id1265704574)，注意 6.x 无广告，7.0 开始有广告和收费功能
- [360 压缩](http://yasuo.360.cn/) - 功能较多 v4.0.0.1540

### 启动盘制作

- [Etcher](https://etcher.balena.io/) - 现在改名叫 balenaEtcher 了，烧录 Linux ISO 镜像到 U 盘，v1.19.21
- [Rufus](http://rufus.ie/) - 制作 Windows 安装盘，v4.5
- [Win32 Disk Imager](https://sourceforge.net/projects/win32diskimager/files/Archive/) - v1.0 `win32diskimager-1.0.0-install.exe`
- FlashBoot - 需注册
- 老毛桃 - PE 启动盘
- [优启通](https://www.upe.net/) - 比较早期纯净的版本：[优启通 v3.3.2019.0605](https://www.itsk.com/thread-397875-1-1.html)
- [大白菜](https://www.dabaicai.com/)
- [微 PE](http://www.wepe.com.cn/) - 推荐，号称纯净，注意 2.1 版本可能有毒
- [微软 WinPE (Windows PE)](https://docs.microsoft.com/zh-cn/windows-hardware/manufacture/desktop/download-winpe--windows-pe)
- 其他 PE：深度、老毛桃、我心如水、云爱、天意、小马、装机员、深山红叶、完美者、无垠

### 截屏录屏

- [PicPick](https://picpick.app/zh/) - 截图工具，个人版免费 v6.3.2
- [FSCapture](https://www.faststone.org/FSCaptureDetail.htm) - 有个之前的版本免费
- [ScreenToGif](https://www.screentogif.com/?l=zh_cn) - 屏幕，摄像头和白板录像机与集成编辑器。可以录制视频或 GIF v2.37.1
- [CamStudio](https://camstudio.org/) - 桌面录像，免费 v2.7.4
- [Snipaste](https://zh.snipaste.com/download.html) - 免费，Mac

### 桌面美化

- [腾讯桌面整理](https://guanjia.qq.com/product/zmzl/) - 新版本已经和 Wallpaper Engine 兼容
- [Wallpaper Engine](https://store.steampowered.com/app/431960/Wallpaper_Engine/)
- [Fliplo](https://fliqlo.com/#/screensaver) - 时钟屏保，1.4 版本已经解决 Flash 禁用问题
- [Folder Painter v1.3](https://www.sordum.org/10124/folder-painter-v1-3/) - 给目录设置颜色
- [Drive Icon Manager](https://github.com/Return-Log/Drive-Icon-Manager) - 删除“我的电脑”里各种网盘的图标，v2.2

### 其他

- [Zamzar File Converter](https://file-converter.org/) - 本地文件格式转换
- [Shell](https://github.com/moudey/Shell) - 替换掉Windows的右键菜单，[下载地址](https://nilesoft.org/download) v1.9.18；没有设置界面，要改配置文件 *.nss；Notepad++ 的右键菜单和这个有冲突，[见](https://github.com/moudey/Shell/issues/347#issuecomment-1759312204)
- [Watt Toolkit](https://github.com/BeyondDimension/SteamTools) - 之前叫 Steam++，可以翻墙

## 开发工具

### 源码管理

- [Git](https://git-scm.com/) - git 客户端，证书 v2.47.1
- [SourceTree](https://www.sourcetreeapp.com/) - Git 图形客户端 v3.4.13
- [GitKraken](https://www.gitkraken.com/) - Git 图形客户端 9.4.0 有免费版
- [Easy XML Editor Pro](https://www.edit-xml.com/) - 表格化XML，可以试用很久，提示过期可以继续用可能没有编辑功能，有普通版 v1.7.8 和 Pro 版 v1.3，区别不大

### Java

- [Oracle Java SDK](https://www.oracle.com/technetwork/java/javase/downloads/index.html) - Java SE 8u231
- [OpenJDK](https://openjdk.java.net/)
- [Maven](https://maven.apache.org/)
- [阿里 Dragonwell8](https://github.com/dragonwell-project/dragonwell8/releases)
- [Adoptium/AdoptOpenJDK](https://adoptium.net/zh-CN/) - AdoptOpenJDK，现在称为Adoptium，8-LTS，11-LTS，17-LTS

### Python

- [Python](https://www.python.org/) - 3.8 ~ 3.13 按需下载，在环境变量 path 里标识 `C:\Users\yinguowei\AppData\Local\Programs\Python\Python311\Scripts\` 和 `C:\Users\yinguowei\AppData\Local\Programs\Python\Python311\`，目前使用 [3.10.11](https://www.python.org/downloads/release/python-31011/) 和 [3.11.9](https://www.python.org/downloads/release/python-3119/)
- [Anaconda](https://www.anaconda.com/download/success)
- [Miniconda](https://docs.anaconda.com/miniconda/)

### 数据库工具

- [MySQL Workbench](https://www.mysql.com/products/workbench/)
- [DBeaver](https://dbeaver.io/) - 分社区版和企业版，关系型数据库管理免费
- [Redisplus](https://gitee.com/MaxBill/RedisPlus) - Redis 客户端，国人开发，跨平台
- [Redis Desktop Managerment](https://redisdesktop.com/) - Redis 客户端，开源，新版本需要付费或自己编译下载（[编译说明](http://docs.redisdesktop.com/en/latest/install/)），Windows 上可以用国人编译的 [Windows 版本](https://github.com/necan/RedisDesktopManager/releases)

### IDE 集成开发环境

- [Visual Studio Code](https://code.visualstudio.com/) - 安装后用 Sync 插件同步其他所有插件（[我的插件](./vscode.md)） v1.96.2
- [Visual Studio 2022](https://visualstudio.microsoft.com/zh-hans/)
- [Visual Studio 2019/2017/2015/2013](https://visualstudio.microsoft.com/zh-hans/vs/older-downloads/)
- [IntelliJ IDEA](http://www.jetbrains.com/idea/) - Java IDE，Ultimate 版本，$499.00/user 1st year
- [Spring Tools](https://spring.io/tools) - 之前叫 STS，Spring Tool Suits，可替代 IDEA、Eclipse
- Android Studio
- [Eclipse for Java EE](https://www.eclipse.org/)

### 其他工具

- [Gisto](https://www.gistoapp.com/) - 代码片段管理
- [Zeal](https://zealdocs.org/) - 软件开发官方文档浏览器
- Hash.exe

### 性能测试工具

- [CPU-Z](https://www.cpuid.com/softwares/cpu-z.html) - 2.06
- [GPU-Z](https://www.techpowerup.com/gpuz/) - 查看 GPU 相关参数
- [3DMARK](https://www.3dmark.com/)
- [Cinebench](https://www.maxon.net/cn/%E4%BA%A7%E5%93%81/cinebench-r20-overview/)
- [AIDA64](https://www.aida64.com/) - 前身是 Evertest，收费
- 国际象棋（FritzChessBenchmark） - CPU 性能测试
- [HD Tune Pro](http://www.hdtune.com/download.html) - 磁盘健康状态，收费
- AS SSD Benchmark - 测试 SSD 性能
- [CrystalDiskMark](https://crystalmark.info/en/software/crystaldiskmark/) - 测试 U 盘读写速度
- [CrystalDiskInfo](https://crystalmark.info/en/software/crystaldiskinfo/)
- FlashBoot - 做 DOS 启动盘（刷 BIOS）
- Paragon ExtFS/NTFS
- [MSI Afterburner](https://cn.msi.com/page/afterburner) - 显卡超频工具，也可以显示游戏内 FPS
- [游戏加加](https://gamepp.com/) - 游戏内 FPS 显示
- [FurMark](http://www.geeks3d.com/furmark/) - 显卡拷机工具，甜甜圈
- 鲁大师 - 视频打分（娱乐大师）

### 其他运行环境

- [Node.js](https://nodejs.org/zh-cn/) - 18.16.0-LTS
- [Ruby](https://rubyinstaller.org/)，Jekyll
- VueCLI
- [Docker for Windows](https://www.docker.com/products/docker-desktop) - 现在叫 Docker Desktop，[下载地址](https://download.docker.com/win/stable/Docker%20for%20Windows%20Installer.exe)
- [.net runtime 6.x](https://dotnet.microsoft.com/zh-cn/download/dotnet) - .NET 6.0 Desktop Runtime (v6.0.16) - Windows x64 Installer!

### 字体

- [Powerline Fonts](https://github.com/powerline/fonts) - 额外的字体，用 "DejaVu Sans Mono for Powerline"

## Windows 自带工具

除了第三方工具，还有些 Windows 自带的工具也较常用

- gpedit.msc - 组策略编辑器
- msconfig - 系统配置
- service.msc - 服务
- diskmgmt.msc - 磁盘管理
- regedit
- msinfo32 - 系统信息
- mmc - 控制台
- mstsc - 远程桌面
- notepad
- cmd
- osk
- regedit / regedt32 - 注册表编辑器
- taskmgr
- control userpasswords2 / netplwiz - 可以在里面设置用户名、免密登入
- lusrmgr.msc - 本地用户和组管理
- [删除 “3D 对象” 文件夹](https://jingyan.baidu.com/article/3f16e0031cdd5c2591c103e6.html)
- Stick Notes 同步 - 备份目录 `C:\Users\yingu\AppData\Local\Packages\Microsoft.MicrosoftStickyNotes_8wekyb3d8bbwe`
- mklink - 符号链接，一些需要重新设置位置、需要备份管理的目录建议做链接，如：

```cmd
mklink /j c:\Users\yinguowei\AppData\Local\Yarn d:\Temp\Yarn
mklink /j c:\Users\yinguowei\.dbeaver4 d:\yinguowei\Documents\.dbeaver4
```

## CMD 常用命令

- shutdown
- copy
- tree
- xxcopy
- netstat
- taskkill
- | findstr "xxx"
  - 查端口：`netstat -aon|findstr "49157"`
  - 查进程：`tasklist|findstr "2720"`
- type
- taskkill - 结束进程：`taskkill /PID 1234`
- diskpart
  - 删除分区：`list disk / select disk x / clean`
  - 创建分区：`create partition primary / active / format fs=fat32/ntfs/exfat label="UDisk" quick`
