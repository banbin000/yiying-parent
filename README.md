# 在线电影
 在线电影基于springboot2.2.1-RELEASE,nacos,SpringCloud Hoxton.SR1,spring-cloud-alibaba-2.1.0-RELEASE,Sentinel,Seata,dubbo来构建的微服务项目
 
在线电影，实现在线观看电影以及在线购买电影票的主要功能等
技术架构，spring boot spring cloud、nacos、dubbo、mybatis-plus,采用前后端分离方式，前端主要由vue开发工具开发，分为前台门户页面和后台管理页面，后台主要由Java的一些架构开发

应用架构图

![../技术架构图](1)

# 项目用到的技术
项目采用前后端分离开发，前端需要独立部署。目前核心的技术栈采用的是SpringBoot2.1.5.RELEASE+Dubbo2.7.2,

# 前端使用的技术
nodejs
axios
es6
vue
sass
Element UI
webpack
vue router

前端页面链接
````https://github.com/qitianfeng/````

# 后端使用的技术
后端的主要架构是基于springboot+dubbo+mybatis-plus.

SpringBoot2.1.6
Mybatis
Dubbo2.7.3
nacos
Mysql
Redis
Elasticsearch
druid
Docker
mybatis generator
Sentinel
Seata

# 后台项目模块说明及规划
|                              |                 |                                                              |
| ---------------------------- | --------------- | ------------------------------------------------------------ |
| db_script 本项目的数据库脚本 | 使用mysql数据库 | 暂时未做分表处理，不过有考虑到分表的情况                     |
| yiying-parent                | pom文件         | 父控文件，对服务统一jar包管理                                |
| yiying-common                | jar             | 公共组件，各个服务需要引用                                   |
| service-user                 | dubbo服务       | 采用sso单点登录，实现用户的登录与注册，用户信息的查询与修改，集成第三方登录(微博登录) |
| service-movie                | dubbo服务       | 实现堆电影的上传，修改，展示，删除等功能                     |
| service-oss                  | dubbo服务       | 实现文件的上传                                               |
| service-vod                  | dubbo服务       | 实现视频的上传，以及视频的点播                               |
| service-search               | dubbo服务       | 采用elasticsearch搜索引擎，实现对电影的条件检索              |
| service-order                | dubbo服务       | 创建订单，删除订单                                           |
| service-pay                  | dubbo服务       | 支付                                                         |
| service-banner               | dubbo服务       | 广告的申请，展示，计费等功能                                 |
| yiying-service-api           | jar包           | 各个服务创建各自的api工程                                    |




# 前台项目整体的规划有
首页渲染，轮播、自定义展示板块
商品查询、商品展示、商品详情
个人中心、用户注册、个人信息修改、收获地址维护
购物车、订单查询、下单、支付
促销活动
![../前端架构](2)



需要配置文件信息的发送邮件  ---> qitiancode@163.com 
