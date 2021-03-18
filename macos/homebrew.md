## Homebrew

安装Homebrew：

```bash
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"

# 或
ruby -e "$(curl -fsSL https://raw.github.com/Homebrew/homebrew/go/install)"
```

[Cask](https://github.com/Homebrew/homebrew-cask) - 现在好像不用 brew cask 了，直接 brew + install/uninstall

常用命令：

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

## 安装cask

```sh
brew tap homebrew/cask
brew install brew-cask
```
