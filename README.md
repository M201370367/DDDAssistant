# DDDAssistant

## 介绍

Android常用MVC，MVP，MVVM，MVI设计模式简单，对于庞大且复杂的系统没明确设计方案。

DDD（Domain-Driven Design领域驱动设计）思想非常适用于大型的应用架构设计。

DDDAssistant是一款协助开发基于DDD思想的大型应用的工具，能够自动生成DDD Class，检索各领域服务。开发一个新功能时，往往需要查询已有实现，方便复用，该工具可直接过滤查看各领域的领域服务、实体、聚合和基础设施，使用起来非常方便。

理解DDD思想，可先理解其分层架构。

分层架构：
![img](https://img-blog.csdnimg.cn/460dcf13f63b4c1e93c4f77b54c4ec84.png?x-oss-process=image/watermark,type_d3F5LXplbmhlaQ,shadow_50,text_Q1NETiBASGFyb2xkX1RpaGFu,size_20,color_FFFFFF,t_70,g_se,x_16#pic_center)


表现/展现层（UI Layer）：图中的用户界面层，对应于MVP中的V（View）。

应用层（Application Layer）：应用层定义系统的业务功能，并指挥领域层中的领域对象实现这些功能，对应于MVP中的P（Presenter）。

领域层（Domain Layer）：核心层，实现所有业务逻辑。领域层包含实体，值对象，领域服务。一个领域只能处理自身范围内逻辑，涉及多个领域业务用领域服务。

基础设施层（Infrastructure Layer）：提供整个业务系统的基础服务。

DDD各层的主要职责和怎么分工协作如下图(微服务应用):
![img](https://img-blog.csdnimg.cn/a6bbac3f0d0140049e44d2dca76fd788.png?x-oss-process=image/watermark,type_d3F5LXplbmhlaQ,shadow_50,text_Q1NETiBASGFyb2xkX1RpaGFu,size_20,color_FFFFFF,t_70,g_se,x_16#pic_center)


## 如何使用

### 步骤一 安装 DDDAssistant plugin
将DDDAssistant.jar下载到本地

打开Android Studio，File-Settings-Plugins-Install Plugin From Disk-选中DDDAssistant.jar进行安装

安装后restart

### 步骤二 移植DDD 基础组件
将AndroidDemo中的dddcommon模块移植自己工程中

### 步骤三 创建DDD Class
可根据需要，使用DDD工具创建各种DDD Class

DDD工具创建入口：
![img](https://img-blog.csdnimg.cn/20bbadfc7e2c4212bf5ed0d170a5bbe8.png?x-oss-process=image/watermark,type_d3F5LXplbmhlaQ,shadow_50,text_Q1NETiBASGFyb2xkX1RpaGFu,size_20,color_FFFFFF,t_70,g_se,x_16#pic_center)

### 步骤四 查看DDD实现
在文本编辑处按下快捷键：ctrl + d，会弹出如下结果：
![img](https://img-blog.csdnimg.cn/39e2822faf3343f5baed836690c5e007.png?x-oss-process=image/watermark,type_d3F5LXplbmhlaQ,shadow_50,text_Q1NETiBASGFyb2xkX1RpaGFu,size_20,color_FFFFFF,t_70,g_se,x_16#pic_center)

------------------------------------------------------------------
------------------------------------------------------------------
欢迎提issue一起交流！
