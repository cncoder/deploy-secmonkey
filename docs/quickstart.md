快速部署指引
=================

在AWS 创建IAM 账号
-------------------------------

Security Monkey 可以运行在 [Amazon EC2 (AWS)](iam_aws.md) 实例

### Running Security Monkey in Production
快速入门指南非常适合学习Security Monkey并尝试使用它，但对于生产部署来说这不足够。 如果您按照Quickstart中的步骤操作，Security Monkey不会自动扫描您的环境，并且不会针对大型帐户进行扩展。 有关生产部署指南，请根据快速部署完之后，阅读 [自动启动](autostarting.md) and [Tuning the Watchers/Prioritizing](tuneworkers.md)

安装说明:
-------------------
1. [在 AWS 上创建IAM 角色和权限](iam_aws.md)
1. [启动 AWS EC2 服务器](installation/01-launch-instance.md)
2. [启动数据库服务器](installation/02-create-db.md)
3. [在您的 EC2 实例上安装Security Monkey](installation/03-install-sm.md)
4. [创建Security Monkey 账户](installation/04-accounts.md)
5. [创建SSL证书](installation/05-ssl.md)
6. [配置 Nginx](installation/06-nginx.md)
7. [登录Security Monkey & 加载AWS 账户数据](installation/07-load-data.md)
8. [为生产系统配置Security Monkey (自动启动)](autostarting.md)

用户手册
----------

更多请参阅 [用户指南](userguide.md) 了解Security Monkey的功能。

贡献
----------

本项目是由Netflix 公司开源的一个安全审计软件，本人只是针对 AWS 审计一部分做了翻译，以及说明一些需要注意的部署要点，如果您有更好的建议，欢迎随时提issue。如需最新功能请查看[security monkey](https://github.com/Netflix/security_monkey/) 项目源站。
