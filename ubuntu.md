# Ubuntu

记录在 [Ubuntu Desktop](https://ubuntu.com/download/desktop) 18.04.3 LTS (Bionic Beaver) 上安装和配置的应用。文档 [GitHub 地址](https://github.com/yingw/my-awesome/blob/master/ubuntu.md)。

[TOC]

## 安装 Ubuntu

从[官网](https://ubuntu.com/download/desktop)下载 ISO 镜像后，做成 DVD，或者用 [Rufus](https://rufus.ie/) 或 [Etcher](https://www.balena.io/etcher/) 制作启动盘，注意传统模式或 UEFI 模式。

参考：[How to burn a DVD on Windows](https://tutorials.ubuntu.com/tutorial/tutorial-burn-a-dvd-on-windows)，以及 [How to create a bootable USB stick on Windows](https://tutorials.ubuntu.com/tutorial/tutorial-create-a-usb-stick-on-windows)

启动后选择全盘安装或者和 Windows 共存。

注意：

- 建议安装选英文，后面改中文。或者看怎么改目录名称。也可以 ln 目录。
- 建议安装断网或选择不要更新，之后切换源了再更新。

## 基础设置

安装后的一些基础设置项。

### 更新国内源

在安装过程或启动后的更新前，建议使用国内源进行更新，速度快。启动“软件更新器”，或者命令方式：

```sh
sudo update-manager --no-update
```

在 `Settings`，可以测试速度或者直接用默认的 `China` 源，如：`http://ftp.sjtu.edu.cn/ubuntu`（上海交大）；或者编辑 `/etc/apt/sources.list` 手动添加新的的源地址。

### 系统更新

设置好源之后就尽快更新，最好设置自动更新或手动配置自动更新任务：

```sh
sudo apt-get -y update && sudo apt-get -y upgrade
```

### 卸载默认应用

卸载一些不用的初始自带的应用：


```sh
# 卸载 Thunderbird 邮件软件，后面用 Evolution
sudo apt-get remove -y thunderbird

# 卸载系统自带的视频播放器 Totem
sudo apt-get remove -y totem

# 卸载系统自带的音频播放器 Rhythmbo
sudo apt-get remove -y rhythmbox

# 卸载自带的游戏
dpkg -l | grep game
sudo apt-get remove -y gnome-mines gnome-mahjongg gnome-sudoku aisleriot

# 删除没用的 Amazon 链接
sudo apt-get remove -y ubuntu-web-launchers
```

### 安装常用工具

```sh
# 安装 vim、wget、zsh 等
sudo apt-get install -y vim curl wget lsb git zsh zip unzip lrzsz screen bash-completion telnet net-tools openssl
```

如果是在虚拟机里运行，还需要安装vmtools，需要安装编译套件，cpp gcc make 等，需要安装增强工具包：

```sh
sudo apt-get install -y build-essential
```

## 系统美化

### Gnome Tweak Tools

启用了 “universe” 发行版组件（universe main security 等的含义）

```
sudo add-apt-repository universe
```

安装 Tweak Tools

```
sudo apt install -y gnome-tweak-tool
```



### 主题

官方主题网站：https://www.gnome-look.org/，[参考](https://linuxconfig.org/the-10-best-ubuntu-themes-18-04-bionic-beaver-linux)。

- 应用：仿 Mac 的 [Mojave-dark](https://github.com/vinceliuice/Mojave-gtk-theme)

- 光标：[Pop](https://github.com/pop-os/gtk-theme)

-  Shell：[Vimix-dark-laptop-doder](https://github.com/vinceliuice/vimix-gtk-themes)

- 图标：[McMojave-circle-dark](https://github.com/vinceliuice/McMojave-circle)




## 系统工具

终端、输入法、视频播放、网盘等。


### Zsh

1. 安装 zsh

```sh
sudo apt-get install -y zsh
```

安装后 zsh 进入，bash 进入

2. 安装 [oh-my-zsh](http://ohmyz.sh/)

```sh
$ sh -c "$(curl -fsSL https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"
# Or
$ sh -c "$(wget https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh -O -)"
```

3. 修改默认的 shell

```sh
# 查看默认的 zsh
which zsh
# 修改默认的 sh 为当前 zsh，重启生效
chsh -s $(which zsh)
# 显示当前的 sh
echo $SHELL
# 显示所有的 sh
cat /etc/shells
# 显示 zsh 的版本
zsh --version
# 改回 bash
chsh -s $(which bash)
```

4. 安装 zsh 插件

插件目录：`~/.oh-my-zsh/plugins/`，启用设置在 `~/.zshrc`，如：

```
plugins=(
  git docker zsh-completions
)
```

自定义插件可以放在 `~/.oh-my-zsh/custom/plugins/`，如：安装 [JHipster 的插件](https://jhipster.github.io/oh-my-zsh/)

```
git clone https://github.com/jhipster/jhipster-oh-my-zsh-plugin.git  ~/.oh-my-zsh/custom/plugins/jhipster \
  && cd \
  && . ~/.zshrc
```

[zsh-completion](https://github.com/zsh-users/zsh-completions)，clone 或下载，拷贝到 custom 插件目录，然后配置 `~/.zshrc`

```sh
  plugins=(… zsh-completions)
  autoload -U compinit && compinit
```

装好再装其他语言的代码补全，如 docker-compose

5. 配置 oh-my-zsh 主题

参考[说明](https://note.youdao.com/)，修改配置文件 `.zshrc`，如：

```
ZSH_THEME="agnoster"
```

安装 [powerline 字体](https://github.com/powerline/fonts)以支持特殊字符的显示，下载 fonts-master.zip 解压安装 `./install.sh`

```sh
sudo apt-get install -y fonts-powerline
```

在终端工具的选型里选用等宽字体 `DejaVu Sans Mono Book`（还有些特殊字符显示不了， ，用 powerline 字体可以）

语法高亮插件： [zsh-syntax-highlighting](https://github.com/zsh-users/zsh-syntax-highlighting)

```sh
git clone https://github.com/zsh-users/zsh-syntax-highlighting.git 
echo "source ${(q-)PWD}/zsh-syntax-highlighting/zsh-syntax-highlighting.zsh" >> ${ZDOTDIR:-$HOME}/.zshrc
```

使之生效 `source ~/.zshrc`，或重进入 zsh

https://github.com/zsh-users/zsh-completions

```sh
autoload -U compinit && compinit
echo "autoload -U promptinit" > ~/.zshrc
```


### 搜狗拼音

卸载 ibus)（可以不用，好像会自动安装），安装 fcitx：

```sh
sudo apt-get purge ibus
sudo apt-get install -y fcitx
```

修改中文在安装语言中把汉语拖到最上面

[搜狗拼音输入法](https://pinyin.sogou.com/linux/) - 安装 deb 包后，“区域语言”->“管理已安装的语言”，键盘输入法系统选择 “fcitx”，注销重新进入

重启后要在 fcitx 配置应用里面添加输入法。如果没看到输入法，根据提示删掉 ~/.config/SogouPY 目录重启

进入个人中心同步设置

在终端和 gedit不能输入中文
在fcitx配置里面去掉两个'自动英文模式'

### 网盘

- [Dropbox](https://www.dropbox.com/) - 免费才 2G，国内使用需要设置代理。
- [百度网盘](https://pan.baidu.com/download) - 百度官方支持 Linux 版本客户端。也可以用 deepin-wine 版本。
- OneDrive - 可以用 GitHub 上的 [onedrive](https://github.com/skilion/onedrive)，[配置方法参考](https://zhuanlan.zhihu.com/p/55622552)。
```
# 初始化，默认在 ~/onedrive 创建仓库，根据链接用浏览器登入输入返回 url 绑定。（目前只能全部下载）
onedrive
# 设置自启动服务
sudo systemctl --user enable onedrive
sudo systemctl --user start onedrive
# 检查配置
onedrive --display-config
# 查看日志
journalctl --user-unit onedrive.service
```
- 坚果云 - 按流量限制，免费版上传流量 1G / 月，下载流量 3G / 月，支持所有终端客户端。

### Keepass

密码管理工具。可以直接仓库安装 `sudo apt-get install keepass2`，当前版本（2.43）和官网已经保持一致了。

汉化，[下载](https://keepass.info/translations.html)中文语言包 `Chinese_Simplified.lngx` ，放到 `/usr/lib/keepass2/Languages` 新建目录里面

乱码问题，在字体文件：`/etc/fonts/conf.avail/65-nonlatin.conf` 里面加入

```xml
<alias>
    <family>Ubuntu</family>
    <prefer>
        <family>sans-serif</family>
    </prefer>
</alias>
```

### Autojump

命令行快速跳转的工具，[官网](https://github.com/wting/autojump)。安装：

```
sudo apt-get install -y autojump
```

配置在 .bashrc 和 .zshrc 里面加上：

```sh
echo ". /usr/share/autojump/autojump.sh" >> ~/.bashrc
echo ". /usr/share/autojump/autojump.sh" >> ~/.zshrc
```

用法：

```
j
```

### 其他

```
sudo apt-get install -y screenfetch
```

---

### 谷歌浏览器 Chrome

```sh
# 更新 Chrome 国内源
sudo wget https://repo.fdzh.org/chrome/google-chrome.list -P /etc/apt/sources.list.d/
# 或
sudo sh -c 'echo "deb http://dl.google.com/linux/chrome/deb/ stable main" >> /etc/apt/sources.list.d/google-chrome.list'

# 添加chrome 秘钥
wget -q -O - https://dl.google.com/linux/linux_signing_key.pub  | sudo apt-key add -

# 安装 Chrome
sudo apt-get update
sudo apt-get install google-chrome-stable
```

卸载 Firefox，如果用于测试目的可以不要卸载

```sh
sudo apt-get purge firefox ubufox
```

### remove / purge / autoremove 的区别

## GNOME 插件

https://extensions.gnome.org/

1. 先要安装 shell 扩展支持，安装好要注销重进生效

```sh
sudo apt install -y gnome-shell-extensions
```

重新启动 GNOME Shell。 按 `Alt+F2` 并输入 `r`，提交。

安装 Ubuntu 的插件集：

```sh
sudo apt-get install -y gnome-shell-extensions
```

在 Chrome 里启用 GNOME 插件监控，需要

1. 安装 Chrome 插件：[GNOME Shell integration](https://chrome.google.com/webstore/detail/gnome-shell-integration/gphhapmejobijbbhgpjhcjognlahblep)

2. 安装本地连接器：

   ```sh
   sudo apt-get install -y chrome-gnome-shell
   ```

安装托盘icon栏，Topicons plus

从 https://extensions.gnome.org/ 找插件，可以通过浏览器安装，有些已经在仓库里的可以用命令找：`apt search gnome-shell-extension-`，用命令安装：

- [Bing Wallpaper Changer](https://extensions.gnome.org/extension/1262/bing-wallpaper-changer/)：使用 Bing 壁纸
- [Dash To Dock](https://note.youdao.com/)：定制 GNOME 的侧边栏
- [Remove Dropdown Arrows](https://extensions.gnome.org/extension/800/remove-dropdown-arrows/)：移除菜单上图标的下拉箭头
- [Removable Drive Menu](https://extensions.gnome.org/extension/7/removable-drive-menu/)：可移除设备的按钮
- [OpenWeather](https://extensions.gnome.org/extension/750/openweather/)：天气插件
- [Internet speed meter](https://extensions.gnome.org/extension/1461/internet-speed-meter/)：显示网速的插件
- [Impatience](https://extensions.gnome.org/extension/277/impatience/)：加快桌面动画效果的速度
- [Extension Update Notifier](https://extensions.gnome.org/extension/1166/extension-update-notifier/)：插件更新提醒
- [Screenshot Tool](https://extensions.gnome.org/extension/1112/screenshot-tool/)：截屏工具，比自带的好用
- [Caffeine](https://extensions.gnome.org/extension/517/caffeine/)：禁用屏保和休眠
- [Appfolders Management extension](https://extensions.gnome.org/extension/1217/appfolders-manager/)：启动菜单里增加目录的管理
- [Apt Update Indicator](https://extensions.gnome.org/extension/1139/apt-update-indicator/)：系统升级的提示
- [CPU Power Management](https://extensions.gnome.org/extension/945/cpu-power-manager/)：电源管理，只支持 Intel CPU
- [Hide Activities Button](https://extensions.gnome.org/extension/744/hide-activities-button/)：隐藏活动菜单
- [Refresh Wifi Connections](https://extensions.gnome.org/extension/905/refresh-wifi-connections/)：增加刷新 Wifi 热点的按钮
- [Gno-Menu](https://extensions.gnome.org/extension/608/gnomenu/)：功能强大的开始菜单，但是我用会死机
- [Status Area Horizontal Spacing](https://extensions.gnome.org/extension/355/status-area-horizontal-spacing/)：调整顶部菜单图标的间距，默认6太大，调整到4
- [Media Player Indicator](https://extensions.gnome.org/extension/55/media-player-indicator/)：媒体播放器的桌面菜单
- [NoAnnoyance](https://extensions.gnome.org/extension/1236/noannoyance/)：消除那个烦人的“Window is ready”，直接前台
- Place Status Indicator：左上角增加位置菜单
- Application Menu：应用菜单，注意要打开“活动热区预览”
- TopIcons Plus：任务栏的图标
- User Themes：自定义主题
- Better Volume indicator：音量图标的一些额外操作
- Native Window Placement：预览窗口的时候更好的排列
- Proxy Switcher：在网络设置菜单里切换代理
- Random Wallpaper：多个桌面背景来源的自动设置，用了 Unsplash
- Trash：回收站图标

## Deepin Wine

Deepin Wine 是深度科技定制的 Wine，wszqkqk 移植到 Ubuntu，可以装微信、迅雷、QQ等。参考[《2019年wine QQ最完美解决方案》]( https://www.lulinux.com/archives/1319) ，从 GitHub 或Gitee clone 安装：

```sh
git clone https://gitee.com/wszqkzqk/deepin-wine-for-ubuntu.git --depth=1
cd deepin-wine-for-ubuntu
sudo ./install.sh
```


再从 http://mirrors.aliyun.com/deepin/pool/non-free/d/ 下载各个 deb 包安装：

```
depk -i *.deb
```

### 微信

```sh
wget http://mirrors.aliyun.com/deepin/pool/non-free/d/deepin.com.wechat/deepin.com.wechat_2.6.8.65deepin0_i386.deb
sudo dpkg -i deepin.com.wechat_2.6.8.65deepin0_i386.deb
```
有可能随着微信的更新，这个容器没有升级，可以在安装好了以后从 https://pc.weixin.qq.com/  下载 Widnows 的最新版安装：

```sh
export WINEPREFIX=~/.deepinwine/Deepin-WeChat
deepin-wine xxx.exe
```

- 微信无法发送图片：`sudo apt install libjpeg62:i386`

- 如果中间有个黑框是表情包，输入 666 有新图就刷掉了

### 迅雷

```bash
wget http://mirrors.aliyun.com/deepin/pool/non-free/d/deepin.com.thunderspeed/deepin.com.thunderspeed_7.10.35.366deepin18_i386.deb
sudo dpkg -i deepin.com.thunderspeed_7.10.35.366deepin18_i386.deb
```
在设置里选微软雅黑。
桌面左上角可能有个黑框，可能是广告，双击就没了。

另外，还有个用electron的版本 https://www.cnblogs.com/dunitian/p/9124806.html

### 字体修复

[参考1](https://blog.csdn.net/qq_37624415/article/details/82228572) [参考2](https://blog.csdn.net/ysy950803/article/details/80326832)
一些软件容器安装后都没有比较好的字体，可以使用 Windows 的微软雅黑：

1. 拷贝三个 Windows 字体文件 *.ttc 到应用的 `driver_c/windows/fonts` 目录

2. 创建 `font.reg` 文件，然后注册：

```properties
REGEDIT4

[HKEY_LOCAL_MACHINE\Software\Microsoft\Windows NT\CurrentVersion\FontLink\SystemLink]
"Lucida Sans Unicode"="msyh.ttc"
"Microsoft Sans Serif"="msyh.ttc"
"MS Sans Serif"="msyh.ttc"
"Tahoma"="msyh.ttc"
"Tahoma Bold"="msyhbd.ttc"
"msyh"="msyh.ttc"
"Arial"="msyh.ttc"
"Arial Black"="msyh.ttc"
```

```sh
env WINEPREFIX=~/.deepinwine/Deepin-ThunderSpeed deepin-wine regedit ~/Downloads/font.reg 
```

3. 编辑系统注册表文件 `system.reg` ，在 `FontSubstitutes` 下修改：`"MS Shell Dlg"="msyh"`：

```
"MS Shell Dlg" = "msyh"
```



### 创建容器

```sh
WINEPREFIX=~/.deepinwine/Deepin-YNote deepin-wine winecfg
# 或者设置环境变量
export WINEPREFIX=~/.deepinwine/Deepin-YNote
```

下载安装文件 *.exe

```sh
WINEPREFIX=~/.deepinwine/Deepin-YNote deepin-wine ~/Downloads/YNote.exe
```

按上面修复字体。

字体对不齐，等宽？

创建快捷键？

在目录：/opt/deepinwine/apps/Deepin-ThunderSpeed 下面
创建 run.sh

在 /usr/share/applications 创建*.desktop 文件,，内容是：


```
#!/usr/bin/env xdg-open

[Desktop Entry]
Encoding=UTF-8
Type=Application
X-Created-By=Deepin WINE Team
Categories=internet;
Icon=deepin.com.baidu.pan
Exec="/opt/deepinwine/apps/Deepin-BaiduNetDisk/run.sh" -u %u
Name=BaiduNetDisk
Name[zh_CN]=百度网盘
Comment=Baidu net disk client on Deepin Wine
StartupWMClass=baidunetdisk.exe
MimeType=

```

或者安装工具 gnome-panel

```
sudo apt-get install gnome-panel
sudo gnome-desktop-item-edit /usr/share/applications/ --create-new
```


### ttf-mscorefonts-installer 问题

安装微软的 TrueType 核心字库

```
sudo apt-get installubuntu-restricted-extras
或
sudo apt-get installttf-mscorefonts-installer
```

方法2

```sh
wget http://httpredir.debian.org/debian/pool/contrib/m/msttcorefonts/ttf-mscorefonts-installer_3.6_all.deb
sudo dpkg -i ttf-mscorefonts-installer_3.6_all.deb
```




### 有道云笔记


```
# 设置环境变量
export WINEPREFIX=~/.deepinwine/Deepin-YNote
# 初始容器：配置用 Windows XP 模式
deepin-wine winecfg
# 修复字体：拷贝字体文件、注册关联、修改字体 system.reg
# 安装应用：要下载 XP 版本支持的 5.8 版
deepin-wine ~/Downloads/YNote5.8.exe
# 修复字体后，启动
deepin-wine ~/.deepinwine/Deepin-YouDaoYun/drive_c/Program\ Files/Youdao/YoudaoNote/YoudaoNote.exe
```

创建应用连接

查看 /opt/deepinwine/tools/run.sh，原来支持有道云，名字需要是 Deepin-YNote

新建 /opt/deepinwine/apps/Deepin-YNote/run.sh
(从隔壁微信拷过来)

```sh
#!/bin/sh

#   Copyright (C) 2016 Deepin, Inc.
#
#   Author:     Yin Guo Wei <yinguowei@gmail.com>

BOTTLENAME="Deepin-YNote"
APPVER="2.6.2.31deepin0"

/opt/deepinwine/tools/run.sh $BOTTLENAME $APPVER "$1" "$2" "$3"
```

在 /usr/share/applications 创建 YouDaoYun.desktop（或者用上面的 gnome-panel）

```properties
#!/usr/bin/env xdg-open
[Desktop Entry]
Version=1.0
Type=Application
Icon[zh_CN]=gnome-panel-launcher
Exec="/opt/deepinwine/apps/Deepin-YNote/run.sh" -u %u
Name[zh_CN]=YouDaoYun
Comment[zh_CN]=有道云笔记
Name=YouDaoYun
Comment=有道云笔记
Icon=gnome-panel-launcher
```
（图标待续）

### IE

一些场合需要用到 IE，用 deepin-wine 目前无法安装，可以用 chrome 的插件 ietab


### WPS

1. 卸载默认安装的 Libre Office：

```
sudo apt-get remove --purge libreoffice*
```

2. 安装 WPS，从 [WPS 官网](https://linux.wps.cn)下载 deb 包安装；缺失字体，去 [WPS 社区](http://wps-community.org/download.html?vl=fonts#download)下载字体包 `wps-office-fonts_1.0_all.deb` 安装，可能可以手动拷贝（好像没微软雅黑）

```
sudo mkdir /usr/share/fonts/wps-office
```

如果还提示有缺失，再补充windows 字体

可能还需要手动安装 libpng（不需要）

```sh
wget http://ftp.cn.debian.org/debian/pool/main/libp/libpng/libpng12-0_1.2.49-1+deb7u2_amd64.deb
```

清除更新字体缓存（手动需要）

```sh
sudo mkfontscale
sudo mkfontdir
sudo fc-cache
```

## VPN

PPA 安装方式

- [Shadowsocks-Qt5](https://github.com/shadowsocks/shadowsocks-qt5/releases)：下载 3.0.1 AppImage 格式，赋予执行权限 `chmod a+x Shadowsocks-Qt5-3.0.1-x86_64.AppImage`，就可以运行了。不能直接用 gui-config.json 导入服务器配置，可以用 URI 一个个导入。

（虚拟机中可以使用宿主机的 ShadowSocks，需要设置允许其他设备接入，Socks 代理模式：192.168.56.1 20090，主机开全局，建议 PAC）

- Wine
- Deeping container
- Flatpak https://blog.csdn.net/u011469138/article/details/82320761

## APT

APT、DPKG 相关软件管理命令

查看 Firefox 相关安装包

```
dpkg --get-selections | grep firefox
```

搜索
```
apt search chrome
```

查找已安装
```
apt list --installed | grep xxx
```

或 
```
dpkg -l
```

## 邮箱

- Thunderbird - 要先安装插件 `ExQuilla for Microsoft Exchange`，然后从菜单里：`工具 - ExQuilla - Add Microsoft Exchange Account`
- include Mailspring and Hiri. 、Nylas Mail  

```
sudo dpkg -i *.deb
```


```
sudo dpkg -I iptux.deb #查看 iptux.deb 软件包的详细信息，包括软件名称、版本以及大小等（其中 - I 等价于 --info）
sudo dpkg -c iptux.deb #查看 iptux.deb 软件包中包含的文件结构（其中 - c 等价于 --contents）
sudo dpkg -i iptux.deb #安装 iptux.deb 软件包（其中 - i 等价于 --install）
sudo dpkg -l iptux #查看 iptux 软件包的信息（软件名称可通过 dpkg -I 命令查看，其中 - l 等价于 --list）
sudo dpkg -L iptux #查看 iptux 软件包安装的所有文件（软件名称可通过 dpkg -I 命令查看，其中 - L 等价于 --listfiles）
sudo dpkg -s iptux #查看 iptux 软件包的详细信息（软件名称可通过 dpkg -I 命令查看，其中 - s 等价于 --status）
sudo dpkg -r iptux #卸载 iptux 软件包（软件名称可通过 dpkg -I 命令查看，其中 - r 等价于 --remove）

```

## 多媒体工具

### 视频播放

- [VLC media player](https://www.videolan.org/vlc/)：视频播放器，应用商店里版本比较乱，找最新版，也可以官网，或者用第三方仓库：

```
$ sudo add-apt-repository ppa:videolan/master-daily
$ sudo apt update
$ sudo apt-get install vlc qtwayland5
```

BBB 大雄兔视频

### 音频播放

GIMP 图片编辑

```
sudo apt-get install gimp
```

- [Listen1](https://github.com/listen1/listen1_desktop/releases)：开源跨平台的多平台音乐播放器
- [网易云音乐](https://music.163.com/#/download)：网易的音乐平台

### 编辑工具

Atom 可以当 notepad++ 用做通用编辑器

```
$ sudo add-apt-repository ppa:webupd8team/atom
$ sudo apt-get update
$ sudo apt-get install atom
```



安装 rpm 包

```
sudo apt-get install alien
sudo alien *.rpm
```

- Maven
- JDK

Markdown Editor

- [Typora](https://www.typora.io/) markdown编辑器 或 [CMD Markdown](https://www.zybuluo.com/mdeditor) 导出PDF收费

GitBook Editor
https://www.mdeditor.com/ 部分收费

新立得包管理器，不是应用商店

```
$ sudo apt-get install synaptic
```

VirtualBox 虚拟机

Ubuntu Cleaner，或者 BleachBit  https://www.bleachbit.org/download/linux

```
$ sudo add-apt-repository ppa:gerardpuig/ppa
$ sudo apt-get update
$ sudo apt-get install ubuntu-cleaner
```

- [Visual Studio Code](https://code.visualstudio.com/)  - 微软的编辑工具，
从官网下载 deb 包安装，安装sync插件，通过github同步配置及插件
- [IntelliJ IDEA](https://www.jetbrains.com/idea/) - 
最好用的 Java IDE，下载 C（免费）版或 U 版（收费，需注册激活）。导入 jar 同步配置。参考[我的插件](https://note.youdao.com/)。
- [CrossOver](http://www.crossoverchina.com/xiazai.html)：可以模拟 Windows 环境安装 Windows 软件，49元终身

mackup https://github.com/lra/mackup


- rdesktop：Windows 远程桌面，用法[参考](https://blog.csdn.net/u012472945/article/details/79447989)
```
sudo apt install -y rdesktop
rdesktop -f -a 16 -g 1440*900 -u wvradmin -p sta@0617 10.151.101.42
```
如果要用连接管理功能的客户端可以看[这里](https://www.ubuntupit.com/10-fast-and-secure-remote-desktop-client-software-for-linux/)

## 深度系列软件

有一堆深度系列软件体验较好，可以在应用市场里搜索“深度”选择安装：

- 深度软件包管理
- 深度看图
- 深度计算器
- 深度截图
- 深度终端
- 深度日历
- 深度影院
- 深度录音

## 参考文章

- [在 Ubuntu 16.04 中安装谷歌 Chrome 浏览器](https://jingyan.baidu.com/article/335530da98061b19cb41c31d.html)
- [26 Things To Do After Installing Ubuntu 18.04 Bionic Beaver Linux](https://linuxconfig.org/things-to-do-after-installing-ubuntu-18-04-bionic-beaver-linux)
- [Ubuntu16.04 安装 keepass 并汉化，解决乱码问题](https://blog.csdn.net/sfdst/article/details/78842478)
- [KeePass Password Safe 2.40 Released, How to Install in Ubuntu](https://www.linuxslaves.com/2018/09/keepass-password-safe-240-released-install-update-ubuntu-linux.html)
- [gnome 桌面环境拓展插件介绍](https://zhuanlan.zhihu.com/p/58729583)
- [Top 20 GNOME Extensions You Should Be Using Right Now](https://itsfoss.com/best-gnome-extensions/)

---

## Ubuntu Temp

wine 和 deepin-wine 并存，安装炉石

有道云笔记的字体问题

onedrive 测试

## 几个主题
/usr/share/themes，图标的目录是 /usr/share/icons
或 ~/.themes ~/.icons
[Sierra-gtk-theme](https://github.com/vinceliuice/Sierra-gtk-theme)
Mojave
[McMojave-circle](https://github.com/vinceliuice/McMojave-circle) 图标
https://www.gnome-look.org/p/1102582/ Cupertino 图标
Pop
Vimix

- [folder color](http://foldercolor.tuxfamily.org/)：给文件夹加颜色

Master PDF Editor，windows收费，linux免费，编辑PDF
https://code-industry.net/masterpdfeditor/


## Grub

Grub 也可以装主题
https://www.gnome-look.org/browse/cat/109/order/latest/
https://github.com/vinceliuice/grub2-themes `sudo ./install.sh -l`

三个文件
boot/grub/grub.cfg 是自动生成的，可以修改生成后的菜单名称，或隐藏菜单

etc/degault/grub 调整参数：分辨率，主题

conf.d 目录，修改10规则：lsb_release -d -s

> 找到 /boot/grub/grub.cfg 文件，找到这样一行： if background_color 44,0,30,0; 修改成 if background_color 0,0,0,0; 就会去除 grub 在选中 Ubuntu 系统之后出现的短暂的紫色。

## 自动挂载windows分区

blkid 查看uuid
编辑/etc/fstab,，加上

```
# Windows C:
UUID=3E98788D98784585 /media/Windows ntfs defaults 0 0
# Windows D:
UUID=C0EE70B8EE70A7F4 /media/Documents ntfs default 0 0

```
直接挂载或重启：sudo mount -a



## 字体

```
sudo apt-get install ttf-mscorefonts-installer
sudo apt-get install fontconfig
mkfontscale mkfontdir 和 fc-cache
```

把windows分区的字体挂载
sudo ln -s /media/Windows/Windows/Fonts /usr/share/fonts/WindowsFonts

## 快捷键

gnome-desktop-icon-edit 创建在 /usr/share/applications 里面 *.desktop
如果用应用“主菜单”编辑后，还会在： ~/.local/share/applications

任务栏名称还是：wine ？？

QQ 任务栏图标不对？？


假死重启
ctrl + alt + F1~7(1是桌面)

```
ps -t tty1
找 Xorg
kill -9 pid
或者重启桌面管理器gdm：sudo /etc/init.d/gdm3 restart
```

资源管理器
- hardinfo（图形）
- lshw(命令行)



- 钉钉：用 GitHub 上的 [Eelectron 版本](https://github.com/nashaofu/dingtalk)，建议关闭新消息托盘闪烁功能。
- [system-monitor](https://extensions.gnome.org/extension/120/system-monitor/)：CPU、内存等监控图。
- Keepass
- 系统代理切换
- Thunderbird：支持 Exchange Server 的插件：ExQuilla，收费
- Evolution：`sudo apt-get install evolution evolution-ews`这个支持免费
- Chrome https://www.google.cn/chrome/
- or
- `echo "deb [arch=amd64] http://dl.google.com/linux/chrome/deb/ stable main" > /etc/apt/sources.list.d/google-chrome.list`
- apt-get install -y google-chrome-stable
- 双系统时差，修改 `timedatectl set-local-rtc 1 --adjust-system-clock`，重启
- 修改 grub，改名字，改时间
- [VSCode](https://code.visualstudio.com/)
- [Sublime Text](https://www.sublimetext.com/)
- [Vim](https://www.vim.org/) Emacs
- Typora
- draw.io https://github.com/jgraph/drawio-desktop/releases
- https://www.jetbrains.com/idea/ 
- DBeaver https://dbeaver.io/


```
# IDEA IntelliJ
#0.0.0.0 account.jetbrains.com
#0.0.0.0 www.jetbrains.com
```

- JDK?
```

$ sudo apt-get purge openjdk*

安装jdk10
sudo add-apt-repository ppa:linuxuprising/java

sudo apt-get install oracle-java10-installer

sudo apt-get install oracle-java10-set-default

安装jdk8
sudo add-apt-repository ppa:webupd8team/java

sudo apt-get install oracle-java8-installer

sudo apt-get install oracle-java8-set-default

卸载
sudo apt-get remove --autoremove oracle-java8-installer oracle-java10-installer


#Openjdk
#:sudo apt-get install openjdk-8-jdk

#:update-alternatives --config java



```


VPN 

FortiClient: https://www.forticlient.com/repoinfo


修复安装时错误的

sudo apt --fix-broken install
--fix-missing?


用 sock 代理私用 ap，安装 tsocks
vi /etc/tsocks.conf

自定义软件类型，左上角菜单


Ubuntu 系统默认字体

/etc/fonts/conf.avail/64-language-selector-prefer.conf
修改里面 sc 的顺序