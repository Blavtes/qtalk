由于公司战略调整，您可能需要看看[这里](https://github.com/startalkIM)


Startalk是世界上最好的开源im系统级解决方案!

* [English Version](https://github.com/qunarcorp/qtalk/blob/master/README.md)
* [Startalk是啥](#Startalk(星语)——通用通信解决方案)
* [我们的使用场景](#我们的使用场景)
* [系统特性](#系统特性)
* [系统独有特性](#系统自有特点)
* [如何使用？](#如何使用？)
  * [部署环境要求](#部署环境要求)
  * [快速开始](#快速开始)
  * [如何在startalk内集成自己的应用](#如何在startalk内集成自己的应用)
  * 官方网站
  * [系统特性](#系统特性)
  * [技术支持](#技术支持)
  * [去中心化设计及部署方式](#去中心化设计及部署方式)  
* [常见使用问题](#常见使用问题)
* [已有用户](#已有用户)

**********************************************
***让部署更简单！***

***Startalk一键部署包已开放，请您到以下地址下载：[一键部署](https://im.qunar.com/#/download_easy)***
**********************************************

# Startalk(星语)——通用通信解决方案

沟通是人类最基础的需求——《人类简史》

Startalk 的目标是成为一款通用的，高性能的企业级im套件。也在努力改变当前大型im系统无完整开源解决方案的现状。

Startalk 前身是去哪儿的Qtalk，已在Qunar稳定运行3年多。

其内核也在去哪儿旅行和去哪儿网站上扮演着着客服服务工具的角色。

也就是说，一套内核同时为去哪儿网提供了内部企业办公和商家tob业务的支撑。


# 我们的使用场景
* 办公自动化OA
* 商业企业客服系统
* 各种im场景的SDK级嵌入

# 系统自有特点
* 开放源代码

```comment
我们正在逐步把工作重心从公司git转移到github上，希望可以为大家提供更稳定持久的服务。
```
* 只推荐私有化部署

```comment
企业有私有化部署的理由和需求，我们是希望帮助企业甚至团体在满足高效沟通和足够的扩展性上提供尽可能多的帮助。
```

# 如何使用？

Startalk专注于基于私有化部署。
这导致了startalk的登录过程略显复杂。
但是没关系，Startalk团队致力于把im系统设计门槛降低到很低的同时，也致力于降低首次接入时的成本。

通常，我们使用一款自有软件时，常见的接入方式分三步：
* 下载app
* 根据官方要求做一些设定
* 注册账号&登录

Startalk因为是私有化部署，服务器也需要部署在自己公司，这使得接入步骤变成了四步：
* 下载app
* 部署后台系统(新增)
* 通过后台配置，给客户端做一些设定
* 倒入账号&登录

如果您真的很希望做私有化接入，但是又不想在前期有一些投入和成本，可以考虑在公共环境中做试用或暂住：

* 加入公共域.

当您已经决定加入私有化部署，或者决定从公共环境中将数据迁移到私有环境：

* 开始[私有化部署!](https://github.com/qunarcorp/ejabberd-open#startalk-ejabberd).


## 部署环境要求
-   [后端](https://github.com/qunarcorp/ejabberd-open)服务器centos 7(未来会支持ubuntu,以及各种私有云)
-   [ios SDK](https://github.com/qunarcorp/imsdk-ios)  最低支持iOS9系统
-   最低[Android SDK](https://github.com/qunarcorp/imsdk-android)：
SDK要求最低API级别为16
-   编译[Android SDK](https://github.com/qunarcorp/imsdk-android)： SDK要求您针对API 26或更高版本进行编译
-   [Windows 1.0](https://github.com/qunarcorp/open_source_startalk)： 要求window vs2012 qt 5.2.1
-   [PC 2.0](https://github.com/qunarcorp/startalk_pc_v2) 含Windows，MAC，linux三个平台，要求qt5.9以上，cmake3.12及以上
-   [Web](https://github.com/qunarcorp/startalk_web)： 推荐部署环境node 8.6.0 npm 5.3.0（node@>=7.6.0；npm@>=3.0.0；pm2@>=2.0.0）
-   其他平台均可使用C++14进行编译。界面是[qt](https://qt.io/)

### 看到这里，您现在可能已经希望测试一番了。。。

## 快速开始
* [ejabberd](https://github.com/qunarcorp/ejabberd-open)  后端源码及介绍

* [imsdk-android](https://github.com/qunarcorp/imsdk-android) 安卓源码及介绍

* [imsdk-iOS](https://github.com/qunarcorp/imsdk-ios) iOS 源码及介绍

* [Windows1.0](https://github.com/qunarcorp/open_source_startalk) Windows 源码及介绍

* [PC2.0](https://github.com/qunarcorp/startalk_pc_v2) PC2.0 源码及介绍

* [Web](https://github.com/qunarcorp/startalk_web) web 源码及介绍

如果您不想费事，或者希望可以快速开始，那么可以进入我们的官方网站注册公共域账号进行测试。

## 如何在startalk内集成自己的应用
Startalk支持用户进行二次扩展，我们提供上传应用的后台，您可通过后台配置的方式嵌入自己的应用，满足企业定制化需求。[点击了解详情](application.md)

## 官方网站
我们针对不同层次的客户提供了不同层次的支持方式。
如果您感兴趣但是担心各种使用上的问题，可以移步官网，百度搜索“星语”

## 系统特性
* 注重您的使用体验和信息安全
* 支持端到端加密方式。默认使用TLS连接，纯二进制协议
* 支持所有的消息类型，文本、表情、文件、音视频、图片、位置、红包、代码……；
* 支持全平台接入；
* 采用去中心化设计。支持私有云或公有云部署

### 包括以下扩展功能
-   单聊及群聊
-   搜索
-   push
-   音视频
-   红包&AA收款
-   会话加密
-   组织架构
-   企业OA

## 技术支持（QQ交流群）
![QQ](image/erweima.png)


## 去中心化设计及部署方式
![architecture](image/arch.png)

Startalk 采用去中心化设计，将非状态服务合并到了Public中，状态服务进入了Domain中。Domain横向扩展，相互之间隔离

![architecture](image/deploy.png)

去中心化部署，只要有服务器，自己家里都能部署一套im服务


### 后端模块

![architecture](image/arch_ejab.png)

+ [ejabberd](https://github.com/qunarcorp/ejabberd-open)

IM核心组件，负责维持与客户端的长连接和消息路由

+ [or](https://github.com/qunarcorp/or_open)

IM负载均衡组件，负责验证客户端身份，以及转发http请求到对应的后台服务
+ [im_http_service](https://github.com/qunarcorp/im_http_service_open)

IM HTTP接口服务，负责IM相关数据的查询、设置以及历史消息同步

+ [qtalk_cowboy](https://github.com/qunarcorp/qtalk_cowboy_open)(后面所有的接口都会迁移到im_http_service，这个服务会废弃)

IM HTTP接口服务，负责IM相关数据的查询、设置以及历史消息同步，后面会全部迁移到im_http_service上

+ [qfproxy](https://github.com/qunarcorp/qfproxy_open)

IM文件服务，负责文件的上传和下载

+ [qtalk_search](https://github.com/qunarcorp/qtalk_search)

提供远程搜索人员和群的服务

+ redis

IM缓存服务

+ postgresql

IM数据库服务

### 客户端模块

#### android端
+ [imsdk-android](https://github.com/qunarcorp/imsdk-android)
安卓SDK

#### ios端
+ [imsdk-iOS](https://github.com/qunarcorp/imsdk-ios)
ios SDK

+ [libqimkit-ios-cook ](https://github.com/qunarcorp/libqimkit-ios-cook)
各个组件Pod库

+ [libqimcommoncategories](https://github.com/qunarcorp/libqimcommoncategories-ios)
扩展工具组件库

+ [libqimdatabase](https://github.com/qunarcorp/libqimdatabase-ios)
数据库组件库

+ [libqimopenssl](https://github.com/qunarcorp/libqimopenssl-ios)
适用于iOS/Mac的OpenSSL库

#### Windows端1.0版本
+ [Windows1.0](https://github.com/qunarcorp/open_source_startalk)源码

#### PC2.0（含window、mac、Linux端）
+ [PC 2.0](https://github.com/qunarcorp/startalk_pc_v2)源码

#### Web端
+ [Web](https://github.com/qunarcorp/startalk_web)源码

#### Emacs
+ [Emacs](https://github.com/qunarcorp/qim-emacs)源码


# 常见使用问题
+ [查看常见使用问题](https://github.com/qunarcorp/qtalk/issues)

# 已有用户

目前已广泛使用的主要厂商，如去哪儿、北工大、便利蜂、新晨航空、爱云动、OpenResty

![architecture](image/qunar.png)![architecture](image/blf.png)![architecture](image/sports.png)![architecture](image/bjgydx.png)![architecture](image/xchk.png)![architecture](image/or.png)![architecture](image/yakang.png)![architecture](image/weichai.png)![architecture](image/qichezhijia.png)
