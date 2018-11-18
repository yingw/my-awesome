# My Awesome

此项目作为 [yingw](https://github.com/yingw) 的知识库记录。

使用 emoji 含义说明

- :heavy_dollar_sign: 商业软件
- :warning: 已终结
- :cloud: 在线工具
- ![GitHub stars](https://img.shields.io/github/stars/moby/moby.svg?label=Stars&style=social) 用 badge 显示在 GitHub 的 star 数

目录
[TOC]

## 操作系统

- [CentOS](https://www.centos.org/) Community Enterprise Operating System，RedHat 的开源编译版本，目前最常用的服务器操作系统
- [RHEL](https://www.redhat.com/en/technologies/linux-platforms/enterprise-linux) RedHat 的商用 Linux 发行版 💲
- [Ubuntu Server](https://www.ubuntu.com/server) Ubuntu 的服务器版本 
- [Windows Server](https://www.microsoft.com/en-us/cloud-platform/windows-server) Microsoft 的 Windows 服务器，有 03、08、12、16、19 版本 💲
- [AWS Linux](https://aws.amazon.com/cn/amazon-linux-ami/) Amazon AWS 的 Linux 操作系统 for EC2，基于 CentOS
- [Deepin 深度操作系统](https://www.deepin.org/) 国内的 Linux 发行版
- [Windows Subsystem for Linux](https://docs.microsoft.com/en-us/windows/wsl/install-win10) Win10 上的 Linux 子系统，可用于开发环境

## 设计

- [墨刀](https://free.modao.cc) 在线原型设计协作平台，有免费和收费版 ☁️ 💲
- [Axure RP](https://www.axure.com/) 老牌的原型设计工具 💲
- [Balsamiq](https://balsamiq.com/) Rapid wireframing tool 💲
- [Photopea](https://www.photopea.com/) 在线的免费图片编辑工具，类似 Photoshop ☁️

## 微服务

Java 的微服务开发平台主要有 Spring Cloud，Dubbo，也有新的无服务（Serverless）管理平台 Knative，服务网格（Service Mesh）架构 Istio

- **[Consul](https://www.consul.io/)** HashiCorp 的服务发现 [教程1](http://note.youdao.com/noteshare?id=260b576b89c46c712a66ff42af314404&sub=9D9D7FBBBA8F4DDCB4A5CE8D41708F61) [教程2](http://note.youdao.com/noteshare?id=cbb2af2fc18c218969fd2aecc6da2e6a&sub=42E5693611884D04A4B9C7318D33E678)
- **[Kong](https://getkong.org/)** 微服务 API 网关，有社区版和企业版 ，丰富的插件，基于 **[Nginx](http://nginx.org/)** 和 **[OpenResty](http://openresty.org/cn/)** [教程1](http://note.youdao.com/noteshare?id=d9faa3dcff2cb3200e61a7c9523b6ad7&sub=1B9691556D834F1F9041F69040A8B659)
- **[Spring Cloud](http://projects.spring.io/spring-cloud/)** Spring 的微服务解决方案 
- [**Spring Cloud Config**](https://cloud.spring.io/spring-cloud-config/) Spring Cloud 的配置服务
  - [**spring-cloud-config-admin**](https://github.com/dyc87112/spring-cloud-config-admin) Spring Cloud Config 的管理功能 by 翟永超
- **[Spring Cloud Sleuth](https://cloud.spring.io/spring-cloud-sleuth/)** 分布式追踪，借鉴 Dapper、Zipkin
- [**Apollo** ](https://github.com/ctripcorp/apollo) 携程的分布式配置中心
- **[Zipkin](https://zipkin.io/)** 链路追踪 
  - [**Zipkin4net** ](https://github.com/openzipkin/zipkin4net) Zipkin 的 .net 客户端 
- [**Hystrix** ](https://github.com/Netflix/Hystrix) 断路器 
- [**Ribbon** ](https://github.com/Netflix/ribbon) Netflix 的客户端负载均衡 
- **[JHipster UAA](https://www.jhipster.tech/using-uaa/)** or **[CloudFoundry UAA](https://github.com/cloudfoundry/uaa)**: 用户鉴权中心、单点登入
- [**Feign** ](https://github.com/OpenFeign/feign) Rest 客户端 
- **[Traefik](https://traefik.io/)** 现代化的代理服务器、负载均衡，使用微服务架构 
- **[Istio](https://istio.io)** 谷歌的微服务架构 
- [Dubbo](http://dubbo.io/) [:octocat:](https://github.com/dubbo) 阿里巴巴的微服务框架 :triangular_flag_on_post:
- [Dubbox](http://dangdangdotcom.github.io/dubbox/) [:octocat:](https://github.com/dangdangdotcom/dubbox) 当当的 Dubbo 扩展 :triangular_flag_on_post:
- Eureka [:octocat:](https://github.com/Netflix/eureka) 服务注册发现 
- Netflix OSS 
- Zuul [:octocat:](https://github.com/Netflix/zuul) API 网关 
- Apollo [:octocat:](https://github.com/ctripcorp/apollo) 携程的分布式配置中心 :triangular_flag_on_post:
- [etcd](https://coreos.com/etcd/) CoreOS 的分布式键值存储，可用于服务发现 
- [ServiceComb](http://servicecomb.incubator.apache.org/) 华为的微服务框架 :triangular_flag_on_post:
- [Micrometer](http://micrometer.io/) 服务监控 
- [Steeltoe](https://steeltoe.io/) Pivotal 提供的 .net 和 Sprig cloud 体系整合方案

## 容器

- [Docker](https://www.docker.com/) 容器 
  - Machine
  - Compose
  - [Docker Registry](https://docs.docker.com/registry/) 被 Distribution 替代 
  - [Docker Distribution](https://docs.docker.com/registry/) 替代了原来的 Registry 
- [Harbor](https://goharbor.io/) 容器镜像管理 by VMWare
- [Kubernetes](http://kubernetes.io/) Google 的容器编排 [![GitHub stars](https://img.shields.io/github/stars/kubernetes/kubernetes.svg?label=Stars&style=social)](https://github.com/kubernetes/kubernetes)
  - **[Helm](https://helm.sh/)** Kubernetes 的包管理 [![GitHub stars](https://img.shields.io/github/stars/helm/helm.svg?label=Stars&style=social)](https://github.com/helm/helm)
  - [kops](https://github.com/kubernetes/kops) Kubernetes Operations (kops) - Production Grade K8s Installation, Upgrades, and Management
- [Mesos](http://mesos.apache.org/) Apache 的开源分布式资源管理框架 [![GitHub stars](https://img.shields.io/github/stars/apache/mesos.svg?label=Stars&style=social)](https://github.com/apache/mesos)
- [Mesosphere](https://mesosphere.com/) 支持 Mesos 和 Kubernetes 的容器管理平台 💲
- [Moby](https://mobyproject.org/)  Docker 开源版 [![GitHub stars](https://img.shields.io/github/stars/moby/moby.svg?label=Stars&style=social)](https://github.com/moby/moby)
- [Swarm](https://docs.docker.com/engine/swarm/) [:octocat:](https://github.com/docker/swarm) Docker 的集群服务 
- [Alpine](https://alpinelinux.org/) 轻量级 Linux based on musl libc and busybox. Docker 用 
- [CoreOS](https://coreos.com/) 容器系统，已加入 RedHat 
- [Heapster](https://github.com/kubernetes/heapster/blob/master/docs/influxdb.md) [:octocat:](https://github.com/kubernetes/heapster) 容器的资源分析和监控 
- [Fluentd](http://www.fluentd.org) [:octocat:](https://github.com/fluent/fluentd) 日志收集，可用于管理Docker日志 
- cAdvisor [:octocat:](https://github.com/google/cadvisor) Google 的 docker 容器管理 
- Kitematic [:octocat:](https://github.com/docker/kitematic) Docker 桌面管理工具 
- [Portainer](https://portainer.io/) [:octocat:](https://github.com/portainer/portainer) Docker 管理 
- docker-gen [:octocat:](https://github.com/jwilder/docker-gen) 生成 docker nginx 的模板 
- [Clair](https://coreos.com/clair/) 容器镜像漏洞分析工具 by CoreOS
- [docker-maven-plugin](https://github.com/spotify/docker-maven-plugin) Docker 的 maven 插件 by spotify，官方已经推荐用下面新版的 dockerfile-maven
- [dockerfile-maven](https://github.com/spotify/dockerfile-maven) 新版插件 by spotfiy
- [Jib](https://github.com/GoogleContainerTools/jib) Google 的 java 应用容器化工具
- [Distroless](https://github.com/GoogleContainerTools/distroless) Google 的镜像，基于 Alpine
- [container-diff](https://github.com/GoogleContainerTools/container-diff) 查看镜像区别 by Google
- [gcr.io Google Container Registry](https://cloud.google.com/container-registry/)
- [docker-cn](https://www.docker-cn.com/registry-mirror) Docker 官方提供的 docker 中国镜像加速
- [DaoCloud](https://www.daocloud.io/mirror) DaoCloud 提供的  docker 中国镜像加速
- [mirror1](https://hub.docker.com/u/googlecontainer/)
- [mirror2](https://github.com/anjia0532/gcr.io_mirror)
### 推荐镜像
- [frolvlad/alpine-oraclejdk8](frolvlad/alpine-oraclejdk8)

## 运维

- [Ganglia](http://ganglia.info/) UC Berkeley发起的一个开源监控项目 
- **[Micrometer](http://micrometer.io/)** 服务监控  by Pivotal
- **[Ansible](https://www.ansible.com)** [:octocat:](https://github.com/ansible/ansible) 基于 Python 的自动化运维工具  by RedHat
  - [Tower](https://www.ansible.com/products/tower) :heavy_dollar_sign: by RedHat 
- [Puppet](https://puppet.com/) 集中配置管理系统 
- [SaltStack](https://saltstack.com/) 基础架构集中化管理平台 
- [Chef](https://www.chef.io/chef/) 管理基础设施运行时环境和应用的自动化平台 
- **[Elastic Stack](https://www.elastic.co/products)** ELK 平台 
  - [ElasticSearch](https://www.elastic.co/products/elasticsearch) 分布式搜索服务 
  - [Kibana](https://www.elastic.co/products/kibana) ELK 的前端展示中心 
  - [Logstash](https://www.elastic.co/products/logstash) Log 收集组件 
  - [Beats](https://www.elastic.co/products/beats) 新一代的数据采集组件，有 Filebeat, Metricbeat, Packetbeat, Winlogbeat, Auditbeat, Heartbeat
- [logz.io](https://logz.io/) ELK as a Service 有免费版 :cloud:
- **[Grafana](https://grafana.com/)** [:octocat:](https://github.com/grafana/grafana) 非常漂亮的分析和监控平台可视化面板 
- **[Prometheus](https://prometheus.io/)** [:octocat:](https://github.com/prometheus/prometheus/) 监控报警系统和时序列数据库 
- **[蓝绿发布](http://www.tuicool.com/articles/2Iji2ue)** 两个相同的环境的测试切换 
- [灰度发布（金丝雀发布）](https://www.v2ex.com/t/344341) 部分发布测试 
- [ArcSight](https://software.microfocus.com/en-us/home) 有很多产品，日志跟踪，商业 
- [Oneops](http://oneops.com/) [:octocat:](https://github.com/oneops/oneops) 沃尔玛的 DevOps 平台 
- [Terraform](https://www.terraform.io/) by HashiCorp  IT 基础架构自动化编排工具 

## 安全
- [OAuth 2.0](https://oauth.net/) 
- [Ralasafe](http://www.oschina.net/p/ralasafe) 权限管理中间件，已不更新 :warning:
- [Shiro](http://shiro.apache.org/) [:octocat:](https://github.com/apache/shiro) Apache 的权限管理框架 
- [Spring Security](https://spring.io/projects/spring-security) [:octocat:](https://github.com/spring-projects/spring-security) Spring 的安全框架，之前是 Acegi Security 
- [Vault](https://www.vaultproject.io/) [:octocat:](https://github.com/hashicorp/vault) HashiCorp 的密码、证书管理 
- [Auth0](https://auth0.com/) 认证服务 :cloud:
- [Authing](https://authing.cn/) 国产的认证云 :cloud:
## 安全 单点登入
- [StormPath](https://stormpath.com/) Security，已被 okta 收购 
- [Okta](https://www.okta.com/) 认证解决方案，Matt 所在的公司 :heavy_dollar_sign::cloud:
- **[Keycloak](https://www.keycloak.org/)** [:octocat:](https://github.com/keycloak/keycloak) Redhat 的单点登入解决方案 
- [CAS](https://www.apereo.org/projects/cas) [:octocat:](https://github.com/apereo/cas) Apereo 的单点登录产品，之前也叫 Jasiq CAS 
## 报表
- [UReport](http://www.bstek.com/products/ureport) [:octocat:](https://github.com/youseries/ureport) 锐道的纯 Java 报表引擎 
- [FineReport](http://www.finereport.com/) 帆软的报表 :heavy_dollar_sign::triangular_flag_on_post:
## 编译
- [Ant](http://ant.apache.org/) Apache 老牌的编译打包工具 
- [Gradle](https://gradle.org/) [:octocat:](https://github.com/gradle/gradle) 编译工具 
- [Grunt](https://gruntjs.com/) [:octocat:](https://github.com/gruntjs/grunt) JavaScript Task Runner 
- [Gulp](https://gulpjs.com/) [:octocat:](https://github.com/gulpjs/gulp) Automating painful or time-consuming tasks 
- [Maven](http://maven.apache.org/) [:octocat:](https://github.com/apache/maven) Apache Maven 打包编译工具 
- [Nexus](http://www.sonatype.org/nexus/) Nexus Repository OSS，maven 等的私有仓库
- [MSBuild](https://github.com/Microsoft/msbuild) 微软的 .net / .net core 编译工具
- [Bazle](https://bazel.build/) 谷歌的 java 编译工具
## 测试
- [Badboy](http://www.badboy.com.au/) 导出 Jmeter 测试脚本 
- [BlazeMeter](https://www.blazemeter.com/) 兼容 Jmeter 商业测试工具 :cloud: 免费50用户，有 chrome 插件录制
- [Browsersync](http://www.browsersync.cn/) 浏览器同步兼容性测试工具 
- [GA](https://www.ibm.com/developerworks/community/groups/service/html/communityview?communityUuid=22d56091-3a7b-4497-b36e-634b51838e11) IBM 提供的 Java GC 和堆观察程序 
- [Gatling](https://gatling.io/) [:octocat:](https://github.com/gatling/gatling) 压力和性能测试工具 
- [Protractor](http://www.protractortest.org/) [:octocat:](https://github.com/angular/protractor) Angular 的 e2e 测试 
- [HA](http://www.ibm.com/developerworks/cn/java/j-lo-javacore/) IBM Heap Analyzer 
- [Jasmine](https://jasmine.github.io/) [:octocat:](https://github.com/jasmine/jasmine) Behavior-Driven JavaScript 
- [JCA](https://www.ibm.com/developerworks/community/groups/service/html/communityview?communityUuid=2245aa39-fa5c-4475-b891-14c205f7333c) IBM 提供的 Java 进程和 Dump 分析 
- [JMeter](https://jmeter.apache.org/) Apache 的自动测试工具 
- [JMeterPlugins](https://jmeter-plugins.org/) Custom Plugins for Apache Jmeter 
- [JProfiler](http://www.ej-technologies.com/products/jprofiler/overview.html) :heavy_dollar_sign:
- [JUnit](http://junit.org/junit4/) Java 单元测试工具 
- [Karma](https://karma-runner.github.io/) [:octocat:](https://github.com/karma-runner/karma) JavaScript 的 测试运行器 
- [LoadRunner](http://www8.hp.com/us/en/software-solutions/loadrunner-load-testing/index.html) HP 商用的压力测试工具 :heavy_dollar_sign:
- [Newman](https://www.getpostman.com/docs/v6/postman/collection_runs/command_line_integration_with_newman) [:octocat:](https://github.com/postmanlabs/newman) Postman 命令行工具 
- [Postman](https://www.getpostman.com/) API 测试工具，Chrome 插件 
- QTP HP 的自动测试工具，Quick Test Professional :heavy_dollar_sign:
- [Seleniumhq](https://www.seleniumhq.org/) [:octocat:](https://github.com/SeleniumHQ/selenium) 自动测试框架。组件有 WebDriver、IDE 
- [SonarQube](http://www.sonarqube.org/) [:octocat:](https://github.com/SonarSource/sonarqube) 开源的代码质量检测平台 
  - [sonarcloud](https://sonarcloud.io/about) :cloud: 在线 sonar 服务，开源免费，需要翻墙
- [EasyMock](http://easymock.org) [:octocat:](https://github.com/easymock/easymock) Mock 测试环境 
- [Easy Mock](https://www.easy-mock.com) [:octocat:](https://github.com/easy-mock/easy-mock) 大搜车的 Mock Server :cloud::triangular_flag_on_post:
- [SoapUI](https://www.soapui.org/) WebService、API 测试工具，有开源版和专业版 
- [Gerrit](https://www.gerritcodereview.com/) 代码检查 
- [Puppeteer](https://pptr.dev/) [:octocat:](https://github.com/GoogleChrome/puppeteer) Chrome 的无头浏览器 Node API 
- [Headless Chrome](https://developers.google.com/web/updates/2017/04/headless-chrome) Google 的 Chrome 无头浏览器 
- [try-puppeteer](https://try-puppeteer.appspot.com/) [:octocat:](https://github.com/ebidel/try-puppeteer) Puppeteer 在线运行测试 
- [Zephyr](https://www.getzephyr.com/) 测试管理工具，已经被 smartbear（SoapUI）收购 :heavy_dollar_sign:
- [Katalon](https://www.katalon.com/) 自动化测试工具
## 持续集成
- [Jenkins](https://jenkins.io) 老牌的 CI CD 工具 
  - [Jenkins X](https://jenkins.io/projects/jenkins-x/) Native CI/CD for Kubernetes 
  - [BlueOcean](https://jenkins.io/projects/blueocean/) Jenkins 优化配置方式
- [Spinnaker](http://www.spinnaker.io/) [:octocat:](https://github.com/spinnaker/spinnaker) Netflix 的持续交付平台 
- [CircleCI](http://circleci.com/) 持续集成 
- [Drone](https://drone.io/) [:octocat:](https://github.com/drone/drone) 持续集成和持续部署平台 
- [Travis CI](https://travis-ci.org/) 同步 GitHub 项目的持续集成和部署平台，有 pro 版 
- **[Azure DevOps (VSTS)](https://azure.microsoft.com/zh-cn/services/devops/)** 微软的 DevOps 服务，5个用户免费 :cloud:

## 代码仓库
- CVS 
- [Git-SCM](https://git-scm.com/) [:octocat:](https://github.com/git/git) Git 
- [GitHub Desktop](https://desktop.github.com/) GitHub 开发的 Git 桌面端 
- [GitLab](https://about.gitlab.com/) 可私有部署的代码托管平台 
- [GitLab CI](https://docs.gitlab.com/ce/ci/) GitLab 的持续集成 
- [Subversion](http://subversion.tigris.org/) 
- [SourceTree](https://www.sourcetreeapp.com/) Git 的客户端 
- [TortoiseCVS](http://www.tortoisecvs.org/) CVS 的客户端 
- [TortoiseSVN](https://tortoisesvn.net/) SVN 的客户端 
- VSS Microsoft 的 CVS 管理工具 Visual SourceSafe 
- [Gogs](https://gogs.io/) [:octocat:](https://github.com/gogs/gogs) 自助 Git 托管服务 
- [Subclipse](http://marketplace.eclipse.org/content/subclipse) Eclipse 的 SVN 支持插件 
## 分布式存储
- [GlusterFS](https://www.gluster.org/) 分布式存储 
- FastDFS [:octocat:](https://github.com/happyfish100/fastdfs) 分布式文件系统 
- [HDFS](http://hadoop.apache.org/docs/stable/hadoop-project-dist/hadoop-hdfs/HdfsUserGuide.html) 基于 Java 的 Hadoop 分布式文件系统 
## 管理模板
- [AdminLTE](https://adminlte.io/) [:octocat:](https://github.com/almasaeed2010/AdminLTE) 免费的 Html 管理模板 
- [H+](http://www.zi-han.net/theme/hplus/) 基于 Inspina 的后台模板 :heavy_dollar_sign::triangular_flag_on_post:
- [Inspinia 2.7.1](https://wrapbootstrap.com/theme/inspinia-responsive-admin-theme-WB0R5L90S) 收费的后台模板，有 AngularJS 版本，官网说要 retire 了 :heavy_dollar_sign:
- [LarryMS](http://www.larrycms.com/tpl/) :triangular_flag_on_post:
- [SB Admin 2](https://startbootstrap.com/template-overviews/sb-admin-2/) [:octocat:](https://github.com/blackrockdigital/startbootstrap-sb-admin-2/) Bootstrap 的页面模板 
- [Gentelella Admin](https://colorlib.com/polygon/gentelella/index.html) [:octocat:](https://github.com/puikinsh/gentelella) 
- [CoreUI](https://coreui.io/) Bootstrap 管理模板，有免费版和收费版，支持多个语言
## 监控
- [Nagios](https://www.nagios.com/products/nagios-core/) 监控服务和主机 
- [Observium Community](http://www.observium.org/) 网络监控 
- [Oracle RUEI](http://www.oracle.com/technetwork/oem/uxinsight/realuserexperienceinsight-085193.html) Oracle 的用户体验监控，可以通过路由器截取数据包报错网页内容 :heavy_dollar_sign:
- [SolarWinds](http://www.solarwinds.com/) 公司用的监控工具 :heavy_dollar_sign:
- [Zabbix](http://www.zabbix.com/) 监控平台，组件有 DPA:Database Performance Analyzer; SAM: Server & Application Performance Monitoring; WMP: Website Monitoring & Performance Software 
- [Dynatrace](https://www.dynatrace.com/) Gartner 上排名第一的 APM 
- [听云](https://www.tingyun.com/) 国内的应用性能监控平台（APM） :heavy_dollar_sign::cloud::triangular_flag_on_post:
- [Elastalert](https://elastalert.readthedocs.io/) [:octocat:](https://github.com/Yelp/elastalert) Yelp 美国的点评网的告警 for ElasticSearch 
- [Pinpoint](http://naver.github.io/pinpoint/) [:octocat:](https://github.com/naver/pinpoint) Java 写的 APM 
## 浏览器
- [Chrome](https://www.google.com/chrome/) Google 浏览器 
- [Edge](https://www.microsoft.com/en-us/windows/microsoft-edge) Microsoft 最新浏览器 
- [Firefox](http://www.firefox.com.cn/firefox/) 火狐浏览器 
- [IE](https://www.microsoft.com/zh-cn/download/internet-explorer.aspx) Microsoft Internet Explorer 
## 流程引擎
- [Activiti](https://www.activiti.org/) [:octocat:](https://github.com/Activiti/Activiti) Java 的工作流和 BPM 平台 
- [Drools](http://www.drools.org/) [:octocat:](https://github.com/kiegroup/drools) JBoss 的规则引擎 
- [jBPM](http://www.jbpm.org/) [:octocat:](https://github.com/kiegroup/jbpm) JBoss 的工作流引擎，已经改名为 Kiegroups 
- [URule](http://www.bstek.com/products/urule) [:octocat:](https://github.com/youseries/urule) 国内锐道的基于RETE算法的规则引擎 
- [Flowable](https://www.flowable.org/) 从 Activiti 团队分离出去的核心主创新构建的流程引擎
## 模板引擎
- [Freemarker](https://freemarker.apache.org/) Java template engine 
- [Velocity](http://velocity.apache.org/) Apache 的 Java 模板引擎 
- [Sitemesh](http://wiki.sitemesh.org/wiki/display/sitemesh/Home) OpenSymphony 的 Java Web 模板 
- [Thymeleaf](http://www.thymeleaf.org/) [:octocat:](https://github.com/thymeleaf/thymeleaf) Java 模板引擎 
- [Thymeleaf Layout Dialect](https://ultraq.github.io/thymeleaf-layout-dialect/) [:octocat:](https://github.com/ultraq/thymeleaf-layout-dialect) Thymeleaf 的 Layout 
- [Tiles](http://tiles.apache.org/) Apache 的 Java 模板引擎 
## 前端模板
- [Amaze UI](http://amazeui.org/) [:octocat:](https://github.com/amazeui/amazeui) HTML5 跨屏前端框架 
- [Ant Design](https://ant.design/) [:octocat:](https://github.com/ant-design/ant-design/) 蚂蚁金服的企业级前端设计语言和基于 React 的前端框架实现 
- [Ant Design Pro](https://pro.ant.design/) [:octocat:](https://github.com/ant-design/ant-design-pro/) 中台前端/设计解决方案 
- [Ant Design Mobile](https://mobile.ant.design/index-cn) [:octocat:](https://github.com/ant-design/ant-design-mobile/) 基于 Preact / React / React Native 的 UI 组件库 
- [AntV](https://antv.alipay.com/zh-cn/index.html) [:octocat:](https://github.com/antvis/g2/) G2 图表，G6 流程图，F2 移动 
- [Bootstrap](https://getbootstrap.com/) [:octocat:](https://github.com/twbs/bootstrap) 
- [Bootstrap 中文网](http://www.bootcss.com/) :triangular_flag_on_post:
- [DWZ](http://jui.org/) 国产jQuery UI框架 (jUI) :triangular_flag_on_post:
- [EasyUI](http://www.jeasyui.com/) 
- [Element](http://element-cn.eleme.io/) [:octocat:](https://github.com/ElemeFE/element) 基于 Vue 2.0 的组件库 
- [vue-element-admin](http://panjiachen.github.io/vue-element-admin/) [:octocat:](https://github.com/PanJiaChen/vue-element-admin) 基于 Vue.js 和 element 的后台集成方案 
- [Material Design Lite](https://getmdl.io/) [:octocat:](https://github.com/google/material-design-lite) Google 的 Material Design 实现 
- [GWT](http://www.gwtproject.org/) Google Web Toolkit，Google 的前端 JavaScript 应用程序工具集 
- [JQuery UI](http://jqueryui.com/) [:octocat:](https://github.com/jquery/jquery-ui) 
- [Layer](http://layer.layui.com/) [:octocat:](https://github.com/sentsin/layer/) web弹层组件 :triangular_flag_on_post:
- [Layui](http://www.layui.com/) [:octocat:](https://github.com/sentsin/layui/) layui 是一款采用自身模块规范编写的情怀型前端UI框架 :triangular_flag_on_post:
- [Material Design](https://material.io/) 
- [YUI](http://yuilibrary.com/) Yahoo 的 JavaScript CSS 库，已终止 :warning:
- [zui](http://zui.sexy/) [:octocat:](https://github.com/easysoft/zui) 
- CSS3 
- [Primefaces](https://www.primefaces.org/) JSF、Angular 解决方案 
- [Material-UI](https://material-ui.com) [:octocat:](https://github.com/mui-org/material-ui) Material Design 的 React 实现 
## 数据库

### 关系型数据库

- [MySQL](http://www.mysql.com/) 有 Community、Cluster、Enterprise 版，目前使用最多的开源数据库
- [Oracle](https://www.oracle.com/database/index.html) Oracle 数据库 💲
- [PostgreSQL](https://www.postgresql.org/) 
- [MSSQL](https://www.microsoft.com/en-us/cloud-platform/sql-server) Microsoft SQL Server 数据库，有 Express、Developer、Enterprise 版 💲
- [Aurora](https://aws.amazon.com/cn/rds/aurora/) AWS 的兼容 MySQL 和 PostgreSQL 的关系数据库，号称性能和 Oracle 相当
- [H2](http://h2database.com/html/main.html) 轻量级可嵌入数据库，用于开发环境  

### 非关系型数据库

- [Memcached](http://memcached.org/) 分布式内存对象缓存系统 
- [Redis](http://redis.io/) [:octocat:](https://github.com/antirez/redis) Redis is an open source (BSD licensed), in-memory data structure store, used as database, cache and message broker. 
  - [Redsmin](https://www.redsmin.com/) Redis 在线服务 ☁️
  - 哨兵
- [MongoDB](https://www.mongodb.com/) [:octocat:](https://github.com/mongodb/mongo) 基于分布式文件存储的数据库 
- [HBase](http://hbase.apache.org/) Apahce 的分布式的、面向列的 Hadoop 数据库 
- [Cassandra](http://cassandra.apache.org/) Apache 的分布式NoSQL数据库 
- [Hadoop](http://hadoop.apache.org/) Apache 的分布式系统基础架构 
- [Spark](http://spark.apache.org/) Apache 的基于内存计算的集群计算系统 
- [IndexedDB](https://developer.mozilla.org/zh-CN/docs/Web/API/IndexedDB_API) 浏览器本地数据库，操作 API，非关系型，JSON 格式

### 其他数据库

- [Amoeba](http://wiki.hexnova.com/display/amoeba/Home) [​:rainbow:​](https://sourceforge.net/projects/amoeba/files/) 支持数据分片的分布式关系型数据库 
- Corba [:octocat:](https://github.com/alibaba/cobar) 基于MySQL的分布式数据库服务中间件 
- [DB2](https://www.ibm.com/analytics/us/en/technology/db2/db2-linux-unix-windows.html) IBM DB2 数据库 :heavy_dollar_sign:
- [Derby](https://db.apache.org/derby/) [:rainbow:](https://svn.apache.org/repos/asf/db/derby/code/branches/) Apache 的轻量级可嵌入应用服务器数据库 
- [HSQLDB](http://hsqldb.org) Java 写的数据库 
- [InfluxDB](https://www.influxdata.com) 时序数据库 
- [MariaDB](https://mariadb.org/) [:octocat:](https://github.com/MariaDB/server) MySQL 的分支数据库 
- [SQLLite](http://sqlite.org/) 
- [TiDB](https://pingcap.com) 开源分布式 NewSQL 关系型数据库 
- Netflix Atlas [:octocat:](https://github.com/Netflix/atlas) 时序数据库 
- [Couchbase](https://www.couchbase.com/) NoSQL 数据库，组件有 Lite，Server，SyncGateway，Connector 
- [OpenTSDB](http://opentsdb.net/) [:octocat:](https://github.com/OpenTSDB/opentsdb) 时序数据库
### 数据库管理工具
- [DB Visualizer](http://www.dbvis.com/) :heavy_dollar_sign:
- [DBeaver](http://dbeaver.jkiss.org/) [:octocat:](https://github.com/serge-rider/dbeaver/) 
- [Navicat](https://www.navicat.com/) :heavy_dollar_sign:
- [PHPMyAdmin](https://www.phpmyadmin.net/) PHP 的 MySQL 管理端 
- [SQL Developer](http://www.oracle.com/technetwork/developer-tools/sql-developer/overview/index.html) Oracle 的数据库管理工具 
- [SQLyog](https://www.webyog.com/product/sqlyog) 
- [Kettle](https://community.hitachivantara.com/docs/DOC-1009855) Java 编写的 ETL 工具 ，也叫 PDI (Pentaho Data Integration)
- [Database.net](http://fishcodelib.com/Database.htm) .net 写的数据库管理工具 
- [LiquiBase](https://www.liquibase.org/) [:octocat:](https://github.com/liquibase/liquibase) 数据库版本 
- [Flyway](https://flywaydb.org/) [:octocat:](https://github.com/flyway/flyway) 数据库版本、迁移工具
- [Mycat](http://www.mycat.io/) [:octocat:](https://github.com/MyCATApache/MyCAT-Server/) 数据库分库分表中间件 🚩
- [Sharding-JDBC](http://shardingjdbc.io/) [:octocat:](https://github.com/shardingjdbc/sharding-jdbc) Distributed database middleware 
- [Talend](https://www.talend.com/products/data-integration/) ETL 工具  
- [Druid](http://druid.io/) [:octocat:](https://github.com/druid-io/druid/) 面向海量数据的、用于实时查询与分析的OLAP存储系统 
- [JPQL](https://en.wikipedia.org/wiki/Java_Persistence_Query_Language) Java Persistence Query Language 
- [QueryDSL](http://www.querydsl.com/) [:octocat:](https://github.com/querydsl/querydsl) 简化JPA操作DSL
## 搜索引擎
- [ElasticSearch](https://www.elastic.co/products/elasticsearch) [:octocat:](https://github.com/elastic/elasticsearch) 分布式搜索服务 
- [Lucene](http://lucene.apache.org/) Apache 的全文检索引擎工具包 
- [Solr](http://lucene.apache.org/solr/) Apache 的基于 Lucene 的企业级搜索应用服务器 
## 图标
- [Font Awesome](http://fontawesome.io/icons/) [:octocat:](https://github.com/FortAwesome/Font-Awesome) 图标库 
- [Github Octicons](https://octicons.github.com/) GitHub 的图标 
- [Iconfont](http://www.iconfont.cn/) 阿里妈妈的矢量图标库 :triangular_flag_on_post:
## 图表
- [D3](https://d3js.org/) [:octocat:](https://github.com/d3/d3) D3.js(Data-Driven Documents) JavaScript 可视化库 
- [Echarts](http://echarts.baidu.com/) [:octocat:](https://github.com/ecomfe/echarts) 百度的数据可视化图表 
- ECharts-Java [:octocat:](https://github.com/abel533/ECharts) 针对ECharts2.x版本的Java类库，实现了所有ECharts中的Json结构对应的Java对象 
- [HighCharts](https://www.highcharts.com/) [:octocat:](https://github.com/highcharts/highcharts) 
- [JFreeChart](http://www.jfree.org/jfreechart/index.html) [:octocat:](https://github.com/jfree/jfreechart)  
## 项目管理
- [禅道](http://www.zentao.net/) 青岛易软天创的项目管理软件 :triangular_flag_on_post:
- [Redmine](https://www.redmine.org/) 项目管理软件 :cloud:
## 消息队列
- [ActiveMQ](http://activemq.apache.org/) Apache 的消息队列 
- [IBM MQ](https://www.ibm.com/products/mq) IBM 的消息队列产品 :heavy_dollar_sign:
- [JMS](http://docs.oracle.com/javaee/6/tutorial/doc/bncdq.html) Java 消息服务规范 
- [Kafka](http://kafka.apache.org/) Apache 的高性能分布式消息服务 
- [RabbitMQ](http://www.rabbitmq.com/) Pivotal 的消息队列 
## 虚拟机
- [Vagrant](https://www.vagrantup.com/) HashiCorp 的虚拟开发环境平台 
- [VirtualBox](https://www.virtualbox.org/) Oracle 的虚拟机 
- [Workstation Player (VMPlayer)](https://www.vmware.com/products/workstation-player.html) VMWare 的虚拟机播放工具，免费 
- [VMWare vSphere Hypervisor (ESXi)](https://www.vmware.com/cn/products/vsphere-hypervisor.html) VMWare 的免费裸机 hypervisor 
- [VMWare Workstation Pro](https://www.vmware.com/cn/products/workstation-pro.html) VMWare 的虚拟机工作站 :heavy_dollar_sign:
## 移动开发
- [Android SDK](https://developer.android.com/studio/) Android 开发集成环境，基于 IDEA 
- [Apahce Cordova](http://cordova.apache.org/) Apache 的移动跨平台 H5 开发框架 
- [Ionic](https://ionicframework.com/) [:octocat:](https://github.com/ionic-team/ionic) 跨平台移动 PWA 开发 SDK 
- [JQuery Mobile](http://jquerymobile.com/) JQuery 的移动框架 
- [OutSystems Now](https://labs.outsystems.net/OutSystemsNowDocs/WebSite.OutSystemsNow.aspx) OutSystems 的移动平台 
- [PhoneGap](http://phonegap.com/) 跨平台移动开发框架 
- [Sencha Touch](https://www.sencha.com/products/touch/) 
- [Worklight](https://www.ibm.com/support/knowledgecenter/en/SSZH4A_6.0.0/com.ibm.worklight.getstart.doc/topics/c_overview.html) IBM 收购的移动开发平台 :heavy_dollar_sign:
- [Ignite](https://infinite.red/ignite) [:octocat:](https://github.com/infinitered/ignite) 开发 React Native 移动应用的 CLI 
- Swift
## 应用服务器
- [GlassFish](https://javaee.github.io/glassfish/) [:octocat:](https://github.com/javaee/glassfish) Java EE 实现的应用服务器 
- [Jetty](http://www.eclipse.org/jetty/) [:octocat:](https://github.com/eclipse/jetty.project) 
- [JBoss EAP](https://developers.redhat.com/products/eap/overview/) JBoss Enterprise Application Platform 
- Redis Session Manager for Apache Tomcat [:octocat:](https://github.com/jcoleman/tomcat-redis-session-manager) Tomcat Session共享插件 
- [Resin](http://caucho.com/) 轻量级应用服务器，用于泛微 
- [Tomcat](http://tomcat.apache.org/) [:octocat:](https://github.com/apache/tomcat) Apache Tomcat Java 应用服务器 
- [TomEE](http://tomee.apache.org/) [:octocat:](https://github.com/apache/tomee) Tomcat 的 EE 版本 
- [Weblogic](http://www.oracle.com/technetwork/middleware/weblogic/overview/index.html) BEA 的应用服务器，被 Oracle 收购 :heavy_dollar_sign:
- [WebSphere](http://www-03.ibm.com/software/products/en/appserv-was) IBM 的 JEE 应用服务器 :heavy_dollar_sign:
- [WebSphere CE](http://publib.boulder.ibm.com/wasce/Front_en.html) Websphere 的社区免费版 
- [WildFly](http://wildfly.org/) [:octocat:](https://github.com/wildfly/wildfly) 之前是 JBoss AS 
- [Netty](http://netty.io/) 要和 Spring Boot 2.0 的 WebFlux、WebSocket 结合使用
- Reactive 响应式、非堵塞的函数式 Reactive Web 框架 
- [ReactiveX](http://reactivex.io/) ：[RxJava](https://github.com/ReactiveX/RxJava) 响应式编程框架，链式、异步、观察者模式
- [Reactor](https://projectreactor.io/) 非阻塞应用编程框架，响应式编程，by Pivotal

## 云服务
- [AliYun 阿里云](https://www.aliyun.com/) 云服务器 ECS、数据库 RDS、万网域名 :heavy_dollar_sign::cloud::triangular_flag_on_post:
- [腾讯云](https://cloud.tencent.com/) :heavy_dollar_sign::cloud::triangular_flag_on_post:
- [AWS](https://aws.amazon.com/) 亚马逊云 :heavy_dollar_sign::cloud:
  - [AWS CloudFront](https://aws.amazon.com/cn/cloudfront/) CDN 
  - [AWS EC2](https://aws.amazon.com/cn/ec2/) 弹性计算 
  - [AWS ECS](https://aws.amazon.com/cn/ecs/) 容器 
  - [AWS Elastic BeansTalk](https://aws.amazon.com/cn/elasticbeanstalk/) PaaS 应用服务器 
  - [AWS ELB](https://aws.amazon.com/cn/elasticloadbalancing/) Elastic Load Balancing 
  - [AWS Lambda](https://aws.amazon.com/cn/lambda/) FaaS 
  - [AWS RDS](https://aws.amazon.com/cn/rds/) PaaS 数据库 
  - [AWS Redshift](https://aws.amazon.com/cn/redshift/) 数据仓库 
  - [AWS S3](https://aws.amazon.com/cn/s3/) 存储 Simple Storage Service
  - EKS
- [Azure](https://www.azure.cn/zh-cn/) 微软的云服务平台 :heavy_dollar_sign::cloud:
  - [Azure SQL](https://www.azure.cn/zh-cn/home/features/sql-database/) 有 vCore 和 DTU 计算方式
- [Cloud Foundry](https://www.cloudfoundry.org/) Pivotal 云 :heavy_dollar_sign::cloud:
- [DigitalOcean](https://www.digitalocean.com/) 云服务 :heavy_dollar_sign::cloud:
- [Heroku](https://www.heroku.com/) 云服务 :heavy_dollar_sign::cloud:

## 在线文档
- [readme](https://readme.io/) 在线文档平台，商业，14 天试用 :cloud:
- [ReadMe Build](https://readme.build) 在线文档平台，有免费和收费版 :cloud:
- [Read the Docs](https://readthedocs.io/) 创建、托管和浏览文档 :cloud:
## API
- [RAML](https://raml.org/) Mule 支持的 YAML格式定义的 RESTful API 建模语言 
- [OpenAPI](https://openapis.org/) [:octocat:](https://github.com/OAI/OpenAPI-Specification) API 规范，Mule 已加入 
- **[Swagger](https://swagger.io/)** API
  - **swagger2markup** [:octocat:](https://github.com/Swagger2Markup/swagger2markup) Swagger 转 AsciiDoc 或者 Markdown
  - **[asciidockor](https://asciidoctor.org/)** [:octocat:](https://github.com/asciidoctor/asciidoctor-maven-plugin) AsciiDoc 转 HTML 或者 PDF
  - **[Swagger UI](https://swagger.io/tools/swagger-ui/)** Swagger 的 Web UI 
  - [Swagger Codegen](https://swagger.io/tools/swagger-codegen/) 生成 OpenAPI 规范的客户端服务端代码 
## CSS
- [Less](http://lesscss.org) [:octocat:](https://github.com/less/less.js) Dynamic stylesheet language 
## CSS 模板
- [Material Design for Bootstrap](https://fezvrasta.github.io/bootstrap-material-design/) [:octocat:](https://github.com/FezVrasta/bootstrap-material-design) 
- [Materialize](https://materializecss.com/) [:octocat:](https://github.com/Dogfalo/materialize) 
## ESB
- [Mule ESB](https://www.mulesoft.com) 社区和商用的 ESB，有 Runtime、API Gateway、Designer、RAML :heavy_dollar_sign:
- [AnyPoint Studio](https://www.mulesoft.com/platform/studio) Mule 的 IDE 
## HTML 模板
- Freelancer [:octocat:](https://github.com/blackrockdigital/startbootstrap-freelancer/) Bootstrap 的页面模板 
- [Semantic UI](https://semantic-ui.com/) [:octocat:](https://github.com/semantic-org/semantic-ui/) 支持 React、Angular 
- [Semantic UI React](https://react.semantic-ui.com/) Semantic UI 的 React 分支 
- [Start Bootstrap](https://startbootstrap.com/) 免费的 Bootstrap 模板和主题 
## HTML 组件
- [bootstrap-datepicker](https://uxsolutions.github.io/bootstrap-datepicker/) [:octocat:](https://github.com/uxsolutions/bootstrap-datepicker) Bootstrap 的日期选择控件 
- [layDate](http://www.layui.com/laydate/) [:octocat:](https://github.com/sentsin/laydate/) Layui 的日期选择控件 :triangular_flag_on_post:
- [jstree](https://www.jstree.com) js 树控件 
- [Masonry](https://masonry.desandro.com/) [:octocat:](https://github.com/desandro/masonry) jQuery 瀑布流插件 
## HTTP 服务器
- [Apache ab](https://httpd.apache.org/docs/2.4/programs/ab.html) Apache HTTP服务器压力测试工具 
- [OpenResty](http://openresty.org/) [:octocat:](https://github.com/openresty/openresty) 基于 NGINX 和 LuaJIT 的 Web 平台 
- [Tengine](http://tengine.taobao.org/) [:octocat:](https://github.com/alibaba/tengine) 淘宝网发起的Web服务器 
- [Apache HTTP Server](http://httpd.apache.org/) [:rainbow:](https://svn.apache.org/repos/asf/httpd/httpd/branches/) Apache 的 HTTP 服务器 
- [HAProxy](http://www.haproxy.org/) 可用性、负载均衡的代理软件 
- [IBM HTTP Server](http://www-03.ibm.com/software/products/en/http-servers) IBM 的 HTTP 服务器，基于 Apache :heavy_dollar_sign:
- [Nginx](http://nginx.org/) HTTP 和反向代理服务器 
- [Apache AJP](https://httpd.apache.org/docs/2.4/mod/mod_proxy_ajp.html) Apache 的 mod_proxy_ajp 负载均衡组件 
- [Squid](http://www.squid-cache.org/) 反向代理服务器，代理缓存服务器 
## IDE
- [M2Eclipse](https://www.eclipse.org/m2e/) Eclipse 的 Maven 支持插件 
- [MAT](http://www.eclipse.org/mat/) Eclipse Memory Analyzer 
- [Atom](https://atom.io/) [:octocat:](https://github.com/atom/atom) GitHub 的编辑工具 
- [Eclipse](http://www.eclipse.org/) Java 集成开发环境 
- [IntelliJ IDEA](https://www.jetbrains.com/idea/) Jetbrain 的 Java 开发集成环境 :heavy_dollar_sign:
- [MyEclipse](https://www.genuitec.com/products/myeclipse/) :heavy_dollar_sign:
- [NetBeans](https://netbeans.org) 
- [Notepad++](https://notepad-plus-plus.org/) 
- [OEPE](http://www.oracle.com/technetwork/developer-tools/eclipse/overview/index.html) Oracle 的 Java 集成开发环境，基于 Eclipse 
- [RAD](http://www.ibm.com/software/products/en/application/) IBM Rational Application Developer :heavy_dollar_sign:
- [Spring Tool Suite](https://spring.io/tools/sts) Spring 提供的 Java 集成开发环境 
- [Sublime](https://www.sublimetext.com/) 
- [Visual Studio Code](https://code.visualstudio.com/) 微软的跨语言开发环境 
- [HBuilder](http://www.dcloud.io/) HTML 编辑器 
- [JBoss Tools](http://tools.jboss.org) JBoss 的 Eclipse 插件，支持 Hibernate 等 
- JRebel [:rainbow:](https://zeroturnaround.com/software/jrebel/) 商用的 Eclipse Tomcat 热部署插件 
## Java
- [Spring Framework](https://spring.io/projects/spring-framework) [:octocat:](https://github.com/spring-projects/spring-framework) Spring 框架，依赖注入、切面、控制反转 
- Google Guice [:octocat:](https://github.com/google/guice/) Google 的依赖注入框架 
- [Apache POI](http://poi.apache.org/index.html) Apache 的 Java Excel 工具，有 Excel workbooks (SS=HSSF+XSSF), 和 SXSSF (Streaming Usermodel API) (Evant Model) 
- Appfuse [:octocat:](https://github.com/appfuse/appfuse) Matt Raible开发的一个指导性的入门级J2EE框架 
- CAT [:octocat:](https://github.com/dianping/cat) 大众点评的 Java 实时应用监控平台 
- [JD-GUI](http://jd.benow.ca/) [:octocat:](https://github.com/java-decompiler/jd-gui) Java 的反编译工具 
- [JavaFX](http://www.oracle.com/technetwork/java/javafx/overview/index.html) Java 桌面设计工具包，已变成 OpenJDK 的 OpenJFX 
- [Scene Builder](http://gluonhq.com/labs/scene-builder/) JavaFX 设计工具 
- [JavaSDK](http://www.oracle.com/technetwork/java/javase/downloads/index-jsp-138363.html) JDK 
- [JSF](http://www.oracle.com/technetwork/java/javaee/javaserverfaces-139869.html) JavaServer Faces 
- [JSP](http://www.runoob.com/jsp/jsp-tutorial.html) 
- [OpenJDK](http://openjdk.java.net/) JDK 的开源分支 
- [Quartz](http://www.quartz-scheduler.org/) [:octocat:](https://github.com/quartz-scheduler/quartz) OpenSymphony 的定时任务框架 
- [dom4j](http://dom4j.github.io/) 
- [fastjson](https://github.com/alibaba/fastjson/wiki/Quick-Start-CN) [:octocat:](https://github.com/alibaba/fastjson) 阿里巴巴的 Java 语言实现的 JSON 解析器和生成器 :triangular_flag_on_post:
- [gRPC](http://www.grpc.io/) [:octocat:](https://github.com/grpc/grpc-java) Google 的 RPC 框架 
- Guava [:octocat:](https://github.com/google/guava) Google 的 Java 开发库 
- [Jackson](https://github.com/alibaba/fastjson/wiki/Quick-Start-CN) [:octocat:](https://github.com/FasterXML/jackson) Java JSON 库 
- [JBoss Cache](http://jbosscache.jboss.org/) JBoss 的分布式缓存 
- [JBoss Forge](http://forge.jboss.org) JBoss 的快速开发平台，之前叫 Jboss Seam 
- JCaptcha [:rainbow:](http://jcaptcha.sourceforge.net/) Java 的验证码
- [reCAPTCHA](https://www.google.com/recaptcha/) Google 的验证码，国内用 recaptcha.net [说明](https://developers.google.com/recaptcha/docs/faq)
- Joda-Time [:octocat:](https://github.com/JodaOrg/joda-time) [:rainbow:](http://www.joda.org/joda-time/) Java 的日期时间操作，Java8 后就建议用 java.time 
- [OSCache](https://mvnrepository.com/artifact/opensymphony/oscache) OpenSymphony 的缓存 
- [Spark Java](http://sparkjava.com/) 轻量级的 Java Web 开发框架，支持 Java8 和 Kotlin 
- [Spring Batch](https://spring.io/projects/spring-batch) [:octocat:](https://github.com/perwendel/spark) Spring 的批处理框架 
- [Spring IO platform](http://platform.spring.io/platform/) Spring 的依赖管理 
- [UnboundID LDAP SDK for Java](https://www.ldap.com/unboundid-ldap-sdk-for-java) [:octocat:](https://github.com/pingidentity/ldapsdk) Java 的 LDAP 工具包 
- [Wro4j](http://wro4j.github.io/wro4j/) [:octocat:](https://github.com/wro4j/wro4j) Java Web 资源优化工具包 
- [Webjars](http://www.webjars.org/) Web Libraries in Jars 
- [J2Objc](https://developers.google.com/j2objc/) [:octocat:](https://github.com/google/j2objc) Google 的 Java 转 Objective-C 工具 
- ZXing [:octocat:](https://github.com/zxing/zxing) Java, Android 的扫码工具包 
- [pac4j](http://www.pac4j.org/) [:octocat:](https://github.com/pac4j/pac4j) Java 安全引擎，多种集成 
- [OpenJPA](http://openjpa.apache.org/) Apache 的 JPA 实现 
- [Caching Data with Spring](https://spring.io/guides/gs/caching/) Spring 的缓存接口，集成多种实现
- [MapStruct](http://mapstruct.org/) Java 对象转换
- [p3c](https://github.com/alibaba/p3c) 阿里巴巴的 Java 开发规范，有 IDEA 和 Eclipse 插件
## Java 脚手架
- [Dropwizard](https://www.dropwizard.io/) Java 轻量级 Web 开发框架 
- [JEECG](http://www.jeecg.org/) 基于代码生成器的J2EE快速开发平台 :triangular_flag_on_post:
- [JeeWx 捷微](http://www.jeewx.com/) 微信管家系统 :triangular_flag_on_post:
- [JFinal](http://www.jfinal.com/) 基于 Java 语言的极速 WEB + ORM 框架 :triangular_flag_on_post:
- [JHipster](http://www.jhipster.tech/) [:octocat:](https://github.com/jhipster/generator-jhipster) Spring Boot + AngularJS 的 Java 快速开发脚手架 
  - JHipster Registry
  - JHipster UAA
  - [JDL Studio](https://start.jhipster.tech/jdl-studio/)
- [Play Framework](https://www.playframework.com/) Java & Scala.的快速 Web 开发框架 
- [Spring Boot](https://spring.io/projects/spring-boot) [:octocat:](https://github.com/spring-projects/spring-boot) Spring 基础开发平台 
- [spring-boot-admin](https://github.com/codecentric/spring-boot-admin) Spring Boot 应用的管理程序
- [Spring Roo](http://projects.spring.io/spring-roo/) [:octocat:](https://github.com/spring-projects/spring-roo) Java 快速开发脚手架 
- [Spring Side](http://springside.github.io/) [:octocat:](https://github.com/springside/springside4) 国内江南白衣大神的快速 SSH Java 开发框架，目前在唯品会 
- [enhancer.io](https://enhancer.io) 一站式信息系统开发云平台 :triangular_flag_on_post:
## Java MVC
- [Spring MVC](http://projects.spring.io/spring-framework/) Spring 的 MVC 框架 
- [Struts2](http://struts.apache.org/) Apache 的 MVC 框架，基于之前的 OpenSymphony Webwork 
## Java ORM
- [Hibernate](http://hibernate.org/orm/) [:octocat:](https://github.com/hibernate/hibernate-orm) JBoss 的 ORM 工具 
- [JPA](http://www.oracle.com/technetwork/java/javaee/tech/persistence-jsp-140049.html) Java Persistence API Java 的持久化 API，JSR-220 标准 
- [MyBatis](http://www.mybatis.org/mybatis-3/) [:octocat:](https://github.com/mybatis/mybatis-3) 持久层框架 
- [Spring Data JPA](https://projects.spring.io/spring-data-jpa/) [:octocat:](https://github.com/spring-projects/spring-data-jpa) Spring 的数据访问、JPA 接口 
## Javascript
- [Angular](https://angular.io/) [:octocat:](https://github.com/angular/angular.js) Google 的 JavaScript 框架 
- [AngularJS](https://angularjs.org/) [:octocat:](https://github.com/angular/angular.js) Google 的 JavaScript 框架，1.0 版本已废弃 
- [Backbone](http://backbonejs.org/) [:octocat:](https://github.com/jashkenas/backbone) 
- [Bower](https://bower.io/) [:octocat:](https://github.com/bower/bower) Web 开发包管理工具 
- [Dojo](http://dojotoolkit.org/) 
- [ECMAScript 6](http://es6-features.org/) [:octocat:](https://github.com/lukehoban/es6features) 
- [ESLint](https://eslint.org/) [:octocat:](https://github.com/eslint/eslint) JavaScript 代码检查 
- [ExtJS](https://www.sencha.com/products/extjs/) :heavy_dollar_sign:
- [JQuery](http://jquery.com/) [:octocat:](https://github.com/jquery/jquery) 
- [jQWidgets](http://www.jqwidgets.com/) :heavy_dollar_sign:
- [JSX](https://reactjs.org/docs/introducing-jsx.html) React 用混合 Html 和 JavaScript 的语法 
- [Node.JS](https://nodejs.org/en/) V8 JavaScript 运行时 
  - [frontend-maven-plugin](https://github.com/eirslett/frontend-maven-plugin)
- [npm](https://www.npmjs.com/) [:octocat:](https://github.com/npm/npm) Node 包管理器 
- [Promises/A+](https://promisesaplus.com/) [:octocat:](https://github.com/promises-aplus/promises-spec) JavaScript 回调规范 
- [React](https://reactjs.org/) [:octocat:](https://github.com/facebook/react/) Facebook 的 JavaScript 库 
- [React Native](https://facebook.github.io/react-native/) [:octocat:](https://github.com/facebook/react-native) React 写原生移动应用 
- dva [:octocat:](https://github.com/dvajs/dva) 基于 redux、redux-saga 和 react-router 的轻量级前端框架 
- [Select2](https://select2.org/) [:octocat:](https://github.com/select2/select2) The jQuery replacement for select boxes 
- [Vue.js](http://cn.vuejs.org/) [:octocat:](https://github.com/vuejs/vue) 渐进式JavaScript框架 
- [Ztree](http://www.treejs.cn/v3/main.php#_zTreeInfo) JQuery 核心的 Tree 插件 
- [Dandelion-Datatables](http://dandelion.github.io/components/datatables/) 基于 DataTables jQuery 插件的表格控件，最新版15年 :warning:
- [DataTables](https://datatables.net/) HTML 表格控件 
- [My97DataPicker](http://www.my97.net/) 国产的 JS 日期控件 :triangular_flag_on_post:
- [Ajax](http://www.w3school.com.cn/ajax/index.asp) 
- [Webpack](https://webpack.js.org/) [:octocat:](https://github.com/webpack/webpack) Module bundler 
- [Prettier](https://prettier.io/) [:octocat:](https://github.com/prettier/prettier) JavaScript 的代码优化 
- [JSLint](http://www.jslint.com/) [:octocat:](https://github.com/douglascrockford/JSLint) JavaScript 的代码优化 
## JDBC
- C3P0 [:rainbow:](https://sourceforge.net/projects/c3p0/) 
- [DBCP](http://commons.apache.org/proper/commons-dbcp/) Apache 的数据连接池 
- Druid [:octocat:](https://github.com/alibaba/druid) 阿里巴巴的数据库监控和缓存 
- [Druid Spring Boot Starter](https://github.com/alibaba/druid/tree/master/druid-spring-boot-starter) Druid 和 String Boot 集成的 starter 
- [Ehcache](http://www.ehcache.org/) [:octocat:](https://github.com/ehcache/ehcache3) Java 的缓存 
- [Tomcat JDBC pool](https://tomcat.apache.org/tomcat-7.0-doc/jdbc-pool.html) Apache Tomcat JDBC 池 
## PaaS
- [OutSystems](http://www.outsystems.com/) 国外的低代码快速开发平台，有移动版，基于 .net，组件有：Service Studio, Integration Studio, Platform Service :heavy_dollar_sign:
## Spring Boot
- [Guns](https://gitee.com/naan1993/guns) [:octocat:](https://github.com/stylefeng/Guns) 基于 SpringBoot 的后台管理系统，整合 Springmvc + Shiro + MyBatis-plus + Beetl + Flowable 
- [SPPanAdmin](https://gitee.com/whoismy8023/SPPanAdmin) [:octocat:](https://github.com/whoismy8023/SPPanAdmin) 基于 SpringBoot 的管理系统模板，已经闭源 
- ybg-plus [:rainbow:](https://gitee.com/SYDeament/ybg_plus) 云报告 ybg3.0极速版 :triangular_flag_on_post:
- ybg-spring-fast [:rainbow:](https://gitee.com/YYDeament/88ybg) 云报告 :triangular_flag_on_post:
## Tools
- [蝉知](http://www.chanzhi.org/) 易软天创的企业门户软件 :triangular_flag_on_post:
- [Apache Commons](http://commons.apache.org/) Apache 的 Java 开发工具包，有 Utils，IO，File，HttpClient 等 
- Cloc [:octocat:](https://github.com/AlDanial/cloc) 命令行统计代码量共计 
- [ConEmu](https://conemu.github.io/) Windows 下的 cmd 工具 
- [Cygwin](http://www.cygwin.com/) Windows 上 Linux 环境模拟 
- [FileZilla](https://filezilla-project.org/) FTP 客户端 & 服务端 
- [Hyperledger](https://www.hyperledger.org/) 被 IBM 采用的区块链平台 
- [IBM Blockchain](https://www.ibm.com/blockchain/) IBM 的区块链，基于 Hyperledger 
- Jira [:rainbow:](https://www.atlassian.com/software/jira) Atlassian 商用的问题跟踪系统 :heavy_dollar_sign:
- Confluence
- XWiki
- JSON 
- JSONView [:rainbow:](https://chrome.google.com/webstore/detail/jsonview/chklaanhfefbnpoihckbnefhakgolnmc) Chrome 插件 JSON 工具 
- JSONLint [:rainbow:](https://jsonlint.com/) 在线 JSON 工具 
- KindEditor [:rainbow:](http://kindeditor.net) 可视化 HTML 编辑器 
- Limesurvey [:rainbow:](https://www.limesurvey.org/) 开源的 PHP 调查问卷系统 
- Mantis [:rainbow:](http://www.mantisbt.org/) 问题跟踪系统 
- MingGW [:rainbow:](http://www.mingw.org/) Windows 上 Linux 命令模拟环境 
- ModSecurity [:rainbow:](http://www.modsecurity.org/) Web 应用防火墙 
- Netty [:rainbow:](http://netty.io/) NIO（非阻塞I/O）框架 
- OpenShift [:rainbow:](https://www.openshift.com/) RedHat 的 Kubernetes 和私有云平台 
- OpenProj [:rainbow:](https://sourceforge.net/projects/openproj/) 项目管理软件，代替Office Project，已终结 :warning:
- [OpenSNS](http://www.opensns.cn/) 开源社交系统 
- [PatchCleaner](http://www.homedev.com.au/Free/PatchCleaner) Windows 的 Installers 清理工具 
- [Pencil](http://pencil.evolus.vn/) 原型绘制工具 
- [ProjectLibre](http://www.projectlibre.com/product/projectlibre-open-source) 基于OpenProj 
- [RAID](https://zh.wikipedia.org/wiki/RAID) 磁盘阵列技术 
- [RubyInstaller](https://rubyinstaller.org/) Widnows 上安装 Ruby 环境 
- [Seafile](http://seafile.com/) 企业云盘 :triangular_flag_on_post:
- [Slack](https://slack.com/) 国外的即时通信 & 协同平台 
- [Storm](http://storm.apache.org/) Apache 的实时计算框架 
- [SuperScan](https://superscan.en.softonic.com/) Windows 上的免费端口扫描工具 
- [TFS](http://tfs.taobao.org/) 淘宝针对海量非结构化数据存储设计的分布式系统 :warning::triangular_flag_on_post:
- [Thrift](http://thrift.apache.org/) Facebook 实现的一种高效的、支持多种编程语言的远程服务调用的框架 
- [Trac](https://trac.edgewall.org/) 问题跟踪系统 
- [Typora](https://typora.io/) Markdown 文档编辑工具 
- [Video Download Capture](https://video-download-capture.en.softonic.com/) 可以从 SafariBooks 网站下载视频 :cloud:
- [Xshell](http://www.netsarang.com/products/xsh_overview.html) 终端工具 
- [XXL-JOB](http://www.xuxueli.com/xxl-job/) [:octocat:](https://github.com/xuxueli/xxl-job/) 轻量级分布式任务调度框架 大众点评 许雪里 :triangular_flag_on_post:
- [zeplin](https://app.zeplin.io/) UI 设计协同工具 :cloud:
- [Zookeeper](https://zookeeper.apache.org/) Apache 分布式应用程序协调服务 
- [ArchiMate](https://www.archimatetool.com/) 架构建模工具

## Web 工具
- [Google Trends](https://www.google.com/trends) Google 趋势查询 :cloud:

## WebService
- [Axis2](http://axis.apache.org/axis2/java/core/) Apache 的 Web Services / SOAP / WSDL 引擎 
- [CXF](http://cxf.apache.org/) Apache 的服务框架，支持 SOAP, XML/HTTP, RESTful HTTP, or CORBA 协议，HTTP, JMS or JBI 传输，JAX-WS and JAX-RS 前端 API 
- [SOAP](http://www.w3school.com.cn/soap/) 基于 XML 的 SOAP 协议 
- [WSDL](http://www.w3school.com.cn/wsdl/) WSDL（网络服务描述语言，Web Services Description Language）基于 XML 的语言，用于描述和访问 Web Services 

##  其他

- [Apache Kylin](http://kylin.apache.org/cn/) Apache 分布式分析引擎 
- [Apache Camel](http://camel.apache.org) Apache 的企业应用集成（EAI）Java 实现 
- [FileNet](http://www-01.ibm.com/support/docview.wss?uid=swg27042122) IBM 的文件、流程管理平台，P8 5.2.1，已不更新 :heavy_dollar_sign:
- [HTML5](http://www.w3school.com.cn/html5/index.asp) 
- [Softerra LDAP Browser](https://www.ldapadministrator.com/softerra-ldap-browser.htm) LDAP 客户端工具 
- [Firebase](https://firebase.google.com) Google 的后台服务 BaaS :cloud:
- [LeanCloud](https://leancloud.cn/) 移动开发后端 BaaS :cloud:
- [Akka](https://akka.io/) Scale 写的实时处理 
- [Gemfire](https://pivotal.io/pivotal-gemfire) 基于 Apache Geode 的内存分布式数据平台 
- [ProcessOn](https://www.processon.com/) 在线流程图设计 :cloud::triangular_flag_on_post:
- [Trello](https://trello.com) 看板工具，免费、收费版 :cloud:
- [SkyWalking](http://skywalking.apache.org/) [:octocat:](https://github.com/apache/incubator-skywalking) 国内大神吴晟创作的 APM，捐献 Apache :triangular_flag_on_post:
- [Open-Falcon](http://open-falcon.org/) [:octocat:](https://github.com/open-falcon/falcon-plus/) 小米的监控平台 :triangular_flag_on_post:
- [ShieldsIO](http://shields.io/) 在线制作 Badge :cloud:
- [云收藏](http://favorites.ren/) [:octocat:](https://github.com/cloudfavorites/favorites-web) 在线收藏夹，Spring Boot 示例 :cloud::triangular_flag_on_post:
- [Let’s Encrypt](https://letsencrypt.org/) 免费 Https 证书 
- [站酷 (ZCOOL)](https://www.zcool.com.cn/) 设计师平台 :cloud::triangular_flag_on_post:
- [Jekyll](https://jekyllrb.com/) 免费的 Blog 生成工具，和 GitHub Pages 集成 
- [Etcher](https://etcher.io/) 烧 Linux 工具
- [Algolia](https://www.algolia.com/) 为网站与移动应用提供托管式搜索API，开源项目免费 :cloud:
- [Typeform](https://www.typeform.com/) 在线表单服务
- Raft 算法，Consul
- paxos 算法，Zookeeper
- [Protocal Buffers](https://developers.google.com/protocol-buffers/) (简称 Protobuf) 是 Google 公司内部的混合语言数据标准 
- [WSO2](https://wso2.com/) 企业基础平台，有 IAM、API、集成
- [blackduck](https://www.blackducksoftware.com/) 开源安全管理
- [Kanbanize](https://kanbanize.com/) :heavy_dollar_sign: 个人版免费，但实际只是个 email 分类工具 [flow-e](https://flow-e.com/)
- [Hygieia](https://github.com/Hygieia/Hygieia) DevOps Dashboard，多个 DevOps 工具的统一面板，能集成 Jira、Jenkins 等多个 Collector