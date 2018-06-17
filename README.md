[Security Monkey 部署指南](https://github.com/Netflix/security_monkey/)
===============

<img align="right" alt="Security Monkey Logo 2017" src="docs/images/Security_Monkey.png" width="50%">

Security Monkey 可以帮助您有效的监控 [AWS 账户](https://medium.com/@Netflix_Techblog/netflix-security-monkey-on-google-cloud-platform-gcp-f221604c0cc7) ，了解在使用AWS 过程中，产生不安全的策略配置，或者不恰当的更改，而且还可以根据不同的级别进行邮件警报。 

Security Monkey 提供了一个简洁的用户界面来浏览和搜索您在AWS上所有区域的帐户。 Security Monkey会记住以前的账号配置状态，并且可以告诉您到底发生了什么变化，以及何时发生了变化。

Security Monkey 可以高度自定义扩展 [用户账号类型](docs/plugins.md), [AWS 账号监控行为](docs/development.md#adding-a-watcher), [账户审计](docs/development.md#adding-an-auditor)和 [警报](docs/misc.md#custom-alerters).

Security Monkey　目前可以运行在　Ubuntu Linux或者OS X，运行环境：CPython 2.7

[![Gitter chat](https://badges.gitter.im/gitterHQ/gitter.png)](https://gitter.im/Netflix/security_monkey)

| Develop Branch  | Master Branch |
| ------------- | ------------- |
| [![Build Status](https://travis-ci.org/Netflix/security_monkey.svg?branch=develop)](https://travis-ci.org/Netflix/security_monkey)  | [![Build Status](https://travis-ci.org/Netflix/security_monkey.svg?branch=master)](https://travis-ci.org/Netflix/security_monkey)  |
| [![Coverage Status](https://coveralls.io/repos/github/Netflix/security_monkey/badge.svg?branch=develop)](https://coveralls.io/github/Netflix/security_monkey?branch=develop)  | [![Coverage Status](https://coveralls.io/repos/github/Netflix/security_monkey/badge.svg?branch=master)](https://coveralls.io/github/Netflix/security_monkey?branch=master) |

🚨⚠️🥁🎺　请注意: 重要更新 1.0 🎺🥁⚠️🚨
--------------
如果您是首次部署Security Monkey可以忽略这一段。
如果您是第一次升级到1.0，请查看[快速入门](docs/quickstart.md)和[自动启动文档](docs/autostarting.md)，因为Security Monkey有一个新的部署模式。 此外，新增了IAM权限。

项目资源
-----------------

- [Security Monkey 架构概述](docs/architecture.md)
- [快速部署](docs/quickstart.md)
- [User Guide](docs/userguide.md)
- [Upgrading](docs/update.md)
- [Changelog](docs/changelog.md)
- [Source code](https://github.com/netflix/security_monkey)
- [Issue tracker](https://github.com/netflix/security_monkey/issues)
- [Gitter.im Chat Room](https://gitter.im/Netflix/security_monkey)
- [CloudAux](https://github.com/Netflix-Skunkworks/cloudaux)
- [PolicyUniverse](https://github.com/Netflix-Skunkworks/policyuniverse)
- [Troubleshooting](docs/troubleshooting.md)

实例图解
---------------
Security Monkey的组件如下:
![diagram](docs/images/sm_instance_diagram.png)


权限获取图解
------------
Security Monkey 通过使用 AWS IAM STS 服务的 Assume Role 提供凭证进行AWS账户扫描
![diagram](docs/images/sm_iam_diagram.png)

贡献
----------

本项目是由Netflix 公司开源的一个安全审计软件，本人只是针对 AWS 审计一部分做了翻译，以及说明一些需要注意的部署要点。如果你想使用Security Monkey 部署在 GCP或者其他地方，请查看源项目。如果您有更好的建议，欢迎随时提issue。如需最新功能请查看[security monkey](https://github.com/Netflix/security_monkey/)项目源站。除非特别声明，本开源项目所有领域内容均只代表所参与贡献的技术人员个人立场，与其公司背景无关。本项目出发点旨在抛砖引玉，有任何不同意见和反馈，请提交 Issue 讨论，或发送邮件至 romennts@gmail.com .