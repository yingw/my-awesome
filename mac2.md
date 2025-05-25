# MacOS 命令

## 1.3. MacOS 恢复功能

[官方文档](https://support.apple.com/zh-cn/HT201314)，关机状态下按住 `Command (⌘)-R`，再按电源键开机，进入恢复，可以：

1. Restore From Time Machine Backup
2. Reinstall Mac OS X
3. Disk Utility （分区）

注：重装需要联网下载整个 OS 镜像

或者 [制作使用引导安装器](https://support.apple.com/zh-cn/HT201372)

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

然后 `source .bash_profile`

curl 连不上，设置代理

```s
export http_proxy=socket5://127.0.0.1:20090
export https_proxy=socket5://127.0.0.1:20090
```

curl 可能不直接使用系统设置的代理，可以

```sh
alias curl="curl -x <proxy_host>:<proxy_port>"
```

或者在  ~/.curlrc 中添加：

```sh
proxy = <proxy_host>:<proxy_port>
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

1. 设置代理
使用 curl，wget，brew 等 http 应用程序会调用 http_proxy 和 https_proxy 这两环境变量进行代理，通过下面方式设置：

方式 1

```sh
export http_proxy=http://127.0.0.1:20091
export https_proxy=$http_proxy
```

方式 2

```sh
export http_proxy=http://127.0.0.1:20091 https_proxy=http://127.0.0.1:20091
```

2. 取消设置代理

```sh
unset http_proxy https_proxy
```

3. 快速切换代理
可以在 ~/.zshrc 或者 ~/.bash_profile 中添加这样的 alias：

```sh
alias goproxy='export http_proxy=http://127.0.0.1:20091 https_proxy=http://127.0.0.1:20091'
alias disproxy='unset http_proxy https_proxy'
```

后续通过 goproxy / disproxy 进行切换

## 快捷键

- Shift + Ctrl + Opt + 关机: 瞬间关机
- Ctrl + Opt + 关机: 正常关机
- F11
- Ctrl + Command + F 全屏
- Optional + Command + D 隐藏任务栏
