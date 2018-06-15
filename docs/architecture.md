Security Monkey 系统架构概述
---------------
Security Monkey 运行在一个hub-spoke类型模型中，Security Monkey 部署在某个AWS账户中，然后通过 AWS　IAM　Assume　方式 “进入”其他账户，以获取其他账号的配置信息，统一在一个Web 界面处理。

有关这方面的更多详细信息，请参阅IAM部分中各个基础架构的详细信息。

组成Security Monkey的组件如下:
![diagram](images/sm_instance_diagram.png)

图表中的所有组件都应存在同一个帐户和区域内。

IAM 权限访问示意图：
------------
Security Monkey 通过  IAM STS 服务中的Assume Role方式获取临时权限扫描账号信息。
![diagram](images/sm_iam_diagram.png)
