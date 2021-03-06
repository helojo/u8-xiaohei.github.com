U8SDK
=====

U8SDK是一套技术开源的统一渠道SDK接入框架，能让手游开发商以最短的时间，一次性接入多家渠道SDK，让游戏快速上线。
手游开发商只需要化一两天时间接入U8SDK抽象层框架，然后通过本地一键打包工具，即可打出最终的各个渠道SDK的渠道包。
整个过程，方便快捷，安全可靠。同时，U8SDK整套框架的简单易扩展，使得手游开发商可以结合自己的业务需求，很方便地进行二次定制。


Note: U8SDK目前支持Android和iOS两个平台。U8Server目前已经开源([github地址](https://github.com/u8-xiaohei/U8Server))

U8SDK开发语言
--------

  * Android平台：抽象层框架采用java开发;
  * Android平台：打包工具采用python开发，同时支持python2.7和python3.4版本
  * Android平台：SDK接入工程采用java开发;
  * iOS平台：抽象层框架采用objective-c开发;
  * iOS平台：打包工具采用python开发，支持mac自带的python2.7版本
  * iOS平台：SDK接入工程采用objective-c开发;
  * U8Server: 采用J2EE框架(Struts2+Spring3+Hibernate3)开发
  * Demo：支持Unity3D、Cocos2dx、Flash平台，分别采用C#、C++和ActionScript开发


支持特性
------------

* 一次接入，多个游戏使用
* 本地批量打包，Android平台采用反编译动态资源整合方式；iOS平台基于母包整合配置和资源，动态出包。
* ICON角标自动处理(Android平台支持)
* 统一闪屏处理，采用巧妙的配置，决定当前采用的闪屏类型
* 渠道特殊逻辑支持
* 游戏特殊逻辑支持
* 插件集成(比如统计，分享，推送等)
* 便于和持续集成环境相整合(比如整合到jenkins持续集成环境中)

我们的宗旨
-----------------

U8SDK一直以来秉承开源的精神，U8SDK所有实现原理，都分享在我们的博客上，同时，我们还录制了完整介绍U8SDK原理的视频教程，目的只有一个，让所有使用U8SDK或者对统一渠道SDK接入解决方案感兴趣的童鞋，能够知其然知其所以然。

目前，U8Server我们已经开源了，也就是让所有使用U8SDK的同学，可以方便地基于U8Server来搭建一套统一用户认证中心和支付中心。U8SDK客户端也以最低的增值服务费用，来维持对U8SDK的技术支持和推广。因为，我们的目的很简单，就是让U8SDK一直坚持下去，并得到越来越多的游戏开发者的认可。

所以，U8SDK面对的不是企业，而是千千万万个游戏开发从业者，我们希望为广大游戏开发者，提供一个关于渠道SDK接入交流的地方。这就是为什么，我们花费这么多时间来讲解U8SDK的实现原理，以及开源U8Server等。

所以，如果你是一枚游戏开发者，那么，U8SDK肯定是适合你的！

- - - -

资料和交流
-----------

  * 欢迎加入U8SDK技术交流群: *207609068* (所有U8SDK的大哥大姐们，正在等着你呢)
  * 视频教程(Android)：[U8SDK Android部分视频教程](http://www.chuanke.com/2869716-122613.html)
  * 视频教程(iOS):[U8SDK iOS部分视频教程](http://www.chuanke.com/2869716-161991.html)
  * 视频教程(U8Server):[U8Server视频教程](http://www.chuanke.com/2869716-164072.html)
  * 官方网站：[www.u8sdk.com](http://www.u8sdk.com)
  * 官方博客：[www.uustory.com](http://www.uustory.com)
  * 问答社区：[U吧社区](http://www.uustory.com/sdk)
  * 增值服务：[U8SDK增值服务](http://www.u8sdk.com/plus/index.html)
  * U8Server开源地址：[github地址](https://github.com/u8-xiaohei/U8Server)
  * U8Server开源版本后台管理系统演示地址：[地址](http://121.42.144.254:8080/u8server_u/admin/index) （用户名和密码：u8sdk/u8sdk）
  * U8Server企业版后台管理系统演示地址：[地址](http://121.42.144.254:8080/u8server/admin/index) （用户名和密码：admin/u8sdk）

演示的渠道包
-------------

这里提供几个渠道包， 给大家演示下， 母包接入U8SDK之后，通过打包工具打出来的渠道包，所包含的一些功能。可以看下， 登录，登出，切换帐号，浮标显示，支付，以及SDK界面中切换帐号和登出等回调触发，退出游戏等功能


  * [360渠道包](http://pan.baidu.com/s/1geRJd5p)
  * [百度的包](http://pan.baidu.com/s/1gfoJFJ9)


诞生理由
-------

曾经的我们，被渠道SDK接入工作深深折磨着，那个时候经验不多，采用最简单粗暴的方式，最后为自己埋下了无数个苦果。后来，就有了现在的U8SDK，为的就是解脱自己，同时方便他人。

不为商业的目的，也不是极客的行为，仅仅因为我们自己需要，所以，就诞生了~

现有的第三方接入平台，部分渠道明确表示，不支持。所以，使用第三方接入平台，有点蛋蛋的忧伤。

为此，U8SDK的诞生，就义无反顾了。


1、客户端源码，需要通过[增值服务](http://www.u8sdk.com/plus/index.html)进行购买，不过也仅仅是白菜价，仅仅赚个维护推广费
2、U8Server，彻底[开源](https://github.com/u8-xiaohei/U8Server)，我们会不断对其进行升级和维护
3、不会被任意一家渠道拒绝，因为U8SDK就是你自己的~，技术开源透明，拥有源码，想怎么改就怎么改





