
## Mac


## 1.2. 开发工具

- [Medis](https://github.com/luin/medis) Redis 客户端，打包收费，需要自己编译
- [Sequel Pro](https://github.com/sequelpro/sequelpro) MySQL 客户端，好久不更新了。如果只连 MySQL 可以用这个
- [DBeaver](http://dbeaver.io/) - `brew cask install dbeaver-community`
- 加环境变量
- Intellij
- [Spring Tools (STS)](https://spring.io/tools/)
brew cask install springtoolsuite
- Nodejs `brew install node`

用 Homebrew 安装 Java，[参考](https://blog.csdn.net/u013310075/article/details/81024790)，(但是下载的是 Oracle 版本，看看怎么下载 openjdk)

```bash
brew tap caskroom/versions
brew search java
brew cask install java8
```

- Ansible
- docker
- maven
- jdk


- [SDKMAN](https://sdkman.io/) - 也是 SDK 管理

```bash
curl -s "https://get.sdkman.io" | bash
source "$HOME/.sdkman/bin/sdkman-init.sh"
sdk version
sdk ls java
sdk install
```


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
brew install python    #安装 python3
```

- Charles 网络抓包工具
- FileZilla
- sourceTree
- Postman
