# My Awesome Windows

> 记录我的Windows工具和设置

## 系统工具

- [Chrome](https://www.google.com/intl/zh-CN/chrome/)：谷歌浏览器，官网下载。初始登入同步需要全局代理。（[我的插件](./chrome.md)）
- [Shadowsocks](https://github.com/shadowsocks/shadowsocks-windows)：直接替换 `gui-config.json`
- 驱动管理：建议Windows更新即可；[驱动人生](https://www.160.com/)；不要用驱动精灵，偷偷安装金山毒霸，优化后windows更新失败
- [Office365](https://portal.office.com/account#installs)：用公司的账号激活，Outlook要用应用密码，在线生成密码后要关闭窗口才能生效

  - Word
  - Excel：安装插件
  - PowerPoint
  - Outlook：导入备份
  - Evernote：@me 个人账号
  - Skype for Business
  - OneDrive：@me 个人账号
- [金山词霸](http://www.iciba.com/)：或者用[有道词典](http://cidian.youdao.com/)
- [KeePass2](https://keepass.info)
- [Draw.io](https://about.draw.io/integrations/#integrations_offline) 开源绘图工具，可替换visio
- [百度网盘](https://pan.baidu.com/)
- [QQ](https://im.qq.com/)
- [微信](https://pc.weixin.qq.com/)
- [企业微信](https://work.weixin.qq.com/)
- 淘宝旺旺：可以不安装一直用手机版或web版
- [迅雷X](https://www.xunlei.com/)：下载工具，mini版本迅雷已经不太好用了
- [迅雷影音](http://video.xunlei.com/pc.html)，或[完美解码](http://jm.wmzhe.com/)，或[POTPlayer](http://potplayer.daum.net/?lang=zh_CN)，KMPlayer；[人人影视播放器](http://app.rrys.tv/)：用来下载[人人](http://www.zmz2019.com/)的视频
- [foobar2000](https://www.foobar2000.org/)，[网易云音乐](https://music.163.com/)
- [7-Zip](https://www.7-zip.org/)、[360压缩](http://yasuo.360.cn/)
- [搜狗输入法](https://pinyin.sogou.com/) 同步
- [福昕阅读器](https://www.foxitsoftware.cn/products/reader/)（FoxitReader）阅读PDF文档
- globalprotected 公司VPN
- SAPGUI
- [有道云笔记](http://note.youdao.com)
- [金山词霸](http://cp.iciba.com/)
- [DiskGenius](http://www.diskgenius.cn/DiskGenius)：分区修改，慎用
- TeamViewer
- 启动盘制作
  - [Etcher](https://www.balena.io/etcher/)：现在改名叫balenaEtcher了，烧录ISO镜像到U盘
  - 老毛桃：PE启动盘
  - 大白菜：PE
- Evernote 笔记工具，中国区印象笔记，用的全球区
- FSCapture 截屏工具，免费版
- [CamStudio](https://camstudio.org/)：桌面录像，免费
- WinDirStat：磁盘状态查看

### 其他设置

- [删除**“3D对象”**文件夹](https://jingyan.baidu.com/article/3f16e0031cdd5c2591c103e6.html)
- Stick Notes 同步：备份目录`C:\Users\yingu\AppData\Local\Packages\Microsoft.MicrosoftStickyNotes_8wekyb3d8bbwe`
- mklink：符号链接，一些需要重新设置位置、需要备份管理的目录建议做链接，如：
    ```
    mklink /j c:\Users\yinguowei\AppData\Local\Yarn d:\Temp\Yarn
    mklink /j c:\Users\yinguowei\.dbeaver4 d:\yinguowei\Documents\.dbeaver4
    ```

## 开发工具

- [Git](https://git-scm.com/) git客户端，证书
- [SourceTree](https://www.sourcetreeapp.com/)
- [GitKraken](https://www.gitkraken.com/)
- [Oracle Java SDK](https://www.oracle.com/technetwork/java/javase/downloads/index.html)：Java SE 8u212
- OpenJDK
- [Maven](https://maven.apache.org/)
- [Visual Studio Code](https://code.visualstudio.com/)：安装后用Sync插件同步其他所有插件。（[我的插件](./vscode.md)）
- [Notepad++](https://notepad-plus-plus.org/)：老牌的文本编辑工具，处理大文件比较慢
- [BeyondCompare](http://www.beyondcompare.cc/xiazai.html)：￥249.00永久授权
- [DBeaver](https://dbeaver.io/)：分社区版和企业版，关系型数据库管理免费
- MySQL
- Java IDE
    - [IDEA intellij](http://www.jetbrains.com/idea/)：Java IDE，Ultimate版本，$499.00/user 1st year
    - [Spring Tools](https://spring.io/tools)：之前叫STS，Spring Tool Suits，可替代 IDEA、Eclipse
    - Android Studio
    - Eclipse for Java EE
- Redis 客户端
    - [Redisplus](https://gitee.com/MaxBill/RedisPlus)：国人开发，跨平台
    - [Redis Desktop Managerment](https://redisdesktop.com/)：开源，新版本需要付费或自己编译下载（[编译说明](http://docs.redisdesktop.com/en/latest/install/)），Windows上可以用国人编译的[Windows版本](https://github.com/necan/RedisDesktopManager-Windows)
- [Node.js](https://nodejs.org/zh-cn/)
- [Ruby](https://rubyinstaller.org/)，Jekyll
- VueCLI
- [XShell，Xftp](https://www.netsarang.com/zh/xshell-download/)：终端管理，家庭/学校用户免费
- Windows Terminal：新的官方终端，商店下载安装
- Xming 给不支持桌面连接的Linux开放桌面接入
- FileZilla Server/Client
- SoapUI
- WinSCP
- UltraEdit/EmEditor
- [Oracle VirtualBox](https://www.virtualbox.org/)：虚拟机
- [Docker for Windows](https://www.docker.com/products/docker-desktop)：现在叫 Docker Desktop，[下载地址](https://download.docker.com/win/stable/Docker%20for%20Windows%20Installer.exe)

