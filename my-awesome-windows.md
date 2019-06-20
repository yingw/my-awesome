# My Awesome Windows

> 记录我的Windows工具和设置

## 开发工具
- [Git](https://git-scm.com/) git客户端，证书
- [Oracle Java SDK](https://www.oracle.com/technetwork/java/javase/downloads/index.html)：Java SE 8u212
- OpenJDK
- [Maven](https://maven.apache.org/)
- [Visual Studio Code](https://code.visualstudio.com/)：安装后用Sync插件同步其他所有插件。（[我的插件](.\my-awesome-vscode)）
- [Notepad++](https://notepad-plus-plus.org/)：老牌的文本编辑工具，处理大文件比较慢
- BeyondCompare：授权
- DBeaver
- MySQL
- [IDEA intellij](http://www.jetbrains.com/idea/)：[注册码](http://idea.lanyus.com/)
- Redis 客户端
    - [Redisplus](https://gitee.com/MaxBill/RedisPlus)：国人开发，跨平台
    - [Redis Desktop Managerment](https://redisdesktop.com/)：开源，新版本需要付费或自己编译下载（[编译说明](http://docs.redisdesktop.com/en/latest/install/)），Windows上可以用国人编译的[Windows版本](https://github.com/necan/RedisDesktopManager-Windows)
- [Node.js](https://nodejs.org/zh-cn/)
- [Ruby](https://rubyinstaller.org/)，Jekyll
- VueCLI
- XShell 终端管理
- Xming 给不支持桌面连接的Linux开放桌面接入
- FileZilla Server/Client
- SoapUI
- WinSCP
- UltraEdit/EmEditor

## 系统工具
- [Chrome](https://www.google.com/intl/zh-CN/chrome/)：谷歌浏览器，官网下载。初始登入同步需要全局代理。（[我的插件](.\my-awesome-chrome)）
- [Shadowsocks](https://github.com/shadowsocks/shadowsocks-windows)：直接替换 `gui-config.json`
- 驱动管理：建议Windows更新即可；[驱动人生](https://www.160.com/)；不要用驱动精灵，偷偷安装金山毒霸，优化后windows更新失败
- [Office365](https://portal.office.com/account#installs)：用公司的账号激活，Outlook要用应用密码，在线生成密码后要关闭窗口才能生效
    - Word
    - Excel：安装插件
    - PowerPoint
    - Outlook：导入备份
    - Evernote：个人账号
    - Skype for Business
- [金山词霸](http://www.iciba.com/)：或者用[有道词典](http://cidian.youdao.com/)
- [KeePass2](https://keepass.info)
- [Draw.io](https://about.draw.io/integrations/#integrations_offline) 开源绘图工具，可替换visio
- [百度网盘](https://pan.baidu.com/)
- [QQ](https://im.qq.com/)
- [微信](https://pc.weixin.qq.com/)
- [企业微信](https://work.weixin.qq.com/)
- 淘宝旺旺：可以不安装一直用手机版或web版
- [迅雷X](https://www.xunlei.com/)：下载工具，mini版本迅雷已经不太好用了
- [迅雷影音](http://video.xunlei.com/pc.html)，或[完美解码](http://jm.wmzhe.com/)，或[POTPlayer](http://potplayer.daum.net/?lang=zh_CN)，KMPlayer；[人人影视播放器](http://app.rrys.tv/)：用来下载[人人](http://www.zmz2019.com/)的视频( )
- [foobar2000](https://www.foobar2000.org/)，[网易云音乐](https://music.163.com/)
- [7-Zip](https://www.7-zip.org/)、[360压缩](http://yasuo.360.cn/)
- [搜狗输入法](https://pinyin.sogou.com/) 同步
- [福昕阅读器](https://www.foxitsoftware.cn/products/reader/)（FoxitReader）阅读PDF文档
- globalprotected 公司VPN
- SAPGUI
- [有道云笔记](http://note.youdao.com)
- [金山词霸](http://cp.iciba.com/)
- [DiskGenius](http://www.diskgenius.cn/DiskGenius)
- TeamViewer
- 启动盘制作
    - ETCher
    - 老毛桃
    - 大白菜
- Evernote 笔记工具，中国区印象笔记，用的全球区
- FSCapture 截屏工具，免费版
- Windows MKLINK：符号链接，一些需要重新设置位置、需要备份管理的目录建议做链接，如：

```
mklink /j c:\Users\yinguowei\AppData\Local\Yarn d:\Temp\Yarn
mklink /j c:\Users\yinguowei\.dbeaver4 d:\yinguowei\Documents\.dbeaver4
```

## 其他设置

- [删除**“3D对象”**文件夹](https://jingyan.baidu.com/article/3f16e0031cdd5c2591c103e6.html)