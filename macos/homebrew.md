# Homebrew

## 安装 Homebrew

需要 XCode Command Line Tools，很大很慢，可以先手动安装

```sh
//安装依赖工具
xcode-select --install
```

```bash
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"

# 或
ruby -e "$(curl -fsSL https://raw.github.com/Homebrew/homebrew/go/install)"
```

[Cask](https://github.com/Homebrew/homebrew-cask) - 现在好像不用 brew cask 了，直接 brew + install/uninstall

## 常用命令

```sh
# 查找
brew search XXX
# 查看软件信息
brew info XXX
brew cask info XXX
# 安装软件
brew install XXX
brew cask install XXX
# 每次安装时都会检查更新很慢，可以跳过更新直接安装，见 https://github.com/Homebrew/brew/issues/1670
HOMEBREW_NO_AUTO_UPDATE=1 brew cask install XXX
# 卸载软件
brew uninstall XXX
# 查看当前已经安装的软件
brew list

```

官网说有些图形软件需要用cask安装

"To install, drag this icon..." no more. brew cask installs macOS apps, fonts and plugins and other non-open source software.

```sh
#Homebrew-Cask
brew tap caskroom/cask

# 安装 Cast:
brew tap phinze/homebrew-cask
brew install brew-cask
```

- 禁用自动升级

在每次命令前加环境变量

或者在 `~/.zshrc` 或 `~/.bash_profile` 里加上 `export HOMEBREW_NO_AUTO_UPDATE=true`

## 安装cask

```sh
brew tap homebrew/cask
brew install brew-cask
```

## 更换 Homebrew 源

一开始一直连接github失败，换中科院源

```sh
// 执行下面这句命令，更换为中科院的镜像：
git clone git://mirrors.ustc.edu.cn/homebrew-core.git/ /usr/local/Homebrew/Library/Taps/homebrew/homebrew-core --depth=1

// 把homebrew-core的镜像地址也设为中科院的国内镜像

cd "$(brew --repo)"

git remote set-url origin https://mirrors.ustc.edu.cn/brew.git

cd "$(brew --repo)/Library/Taps/homebrew/homebrew-core"

git remote set-url origin https://mirrors.ustc.edu.cn/homebrew-core.git

// 更新
brew update

// 使用
brew install node
```

或者改成socket代理，就好了

```sh
git config --global http.proxy http://127.0.0.1:1080
git config --global https.proxy https://127.0.0.1:1080

git config --global --unset http.proxy
git config --global --unset https.proxy

git config --global http.proxy 'socks5://127.0.0.1:20090'
git config --global https.proxy 'socks5://127.0.0.1:20090'
```

npm删除代理  `npm config delete proxy`

下载 sh 脚本，手动修改源

```sh
# HOMEBREW_CORE_DEFAULT_GIT_REMOTE="https://github.com/Homebrew/homebrew-core"
  HOMEBREW_CORE_DEFAULT_GIT_REMOTE="https://mirrors.ustc.edu.cn/homebrew-core.git"

# HOMEBREW_CORE_DEFAULT_GIT_REMOTE="https://github.com/Homebrew/linuxbrew-core"
  HOMEBREW_CORE_DEFAULT_GIT_REMOTE="https://mirrors.ustc.edu.cn/linuxbrew-core.git"

# HOMEBREW_BREW_DEFAULT_GIT_REMOTE="https://github.com/Homebrew/brew"
HOMEBREW_BREW_DEFAULT_GIT_REMOTE="https://mirrors.ustc.edu.cn/brew.git"

# 然后执行
/bin/bash -c ./install.sh

```

## 查看安装流行度、排名

https://formulae.brew.sh/analytics/cask-install/365d/

## 安装指定版本软件

1. 如果之前使用brew install node安装过node,需要先执行brew unlink node来'解绑'node
1. 查找可用的node版本 brew search node
1. 安装你需要的版本, 比如 brew install node@8
1. 然后 brew link node@8, 这一步可能会报错, 按照提示执行命令就ok了, 比如我最后执行的是brew link --overwrite --force node@8
1. node -v 不出意外, 就安装好了你想要的node版本

主仓库的可以直接 search node@，cask 的好像不行，要切换 git 版本，[参考](https://stackoverflow.com/questions/58373704/how-do-you-specify-a-version-using-brew-cask)

## 清除缓存

## 转移

brew list > a.txt
brew leaves > b.txt
for i in $(cat brew_leaves); do; brew install "$i"; done

## Logitech

logitech-options
logitech-gaming-software
