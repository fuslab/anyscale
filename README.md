# JDataFlow Platfrom

**JDP是企业级Core Data & Core AI 流分析平台， JDP全称`JDataFlow Platfrom`**，分析流动中的数据。JDP并不是一个框架，而是一套完整的解决方案，主要包括：

- 基础理念：`JDP` 基于Streaming Analytics Visualization架构。
- 开发工具：`Ambari`，基于Ambari源码扩展，JDP更好的融合Ambari。
- 基础构成：`JDP`核心基于高性能的分布式关系型数据库构建，支撑万亿数据秒级响应能力。
- 核心功能：`JDP`核心Core Data & Core AI：
    + Core Data提供高度可视化的流数据分析，Streaming Analytics to Visualization。
    + Core AI提供分布式系统上的AI能力，Smart Application。

- 基础运维：开箱即用，可视化运维管理系统`Ambari Manager`：
    + 提供核心的服务管理与配置中心功能，保障集群的稳定可靠。
    + 简单高效的管理大规模分布式系统，仅需专注业务应用。

![JDataFlow](http://www.fusionlab.cn/zh-cn/docs/intro/img/JDataFlow-Pratfrom.png)

## 设计原则

- Internet of Things (IoT)，连接一切的时代，数据在流动中被处理。
- JDP流分析平台，简单高性能的数据分析，Core Data遵循分布式系统设计原则。
- 遵循企业现有服务体系。无缝融入现有企业数据中心系统，可直接交互数据。

## 特性

- One-stop solution：开箱即用 & 简单 & 易用。
- 高性能：万亿数据秒级响应，提供PB级数据存储。
- 扩展性：规模化部署，可达几百台集群规模。
- 可视化：可视化的数据收集、数据存储、数据分析、数据报表。
- 可靠性：集群提供副本容错机制，硬件故障不会造成数据丢失。
- 简单运维：日志、监控、报警、配置、服务一栈式管理。
- 简单易用：提供标准SQL，拖拽式数据分析。

## JDP Development plan for 3.0.0.0 

* 研发计划

![](https://github.com/fusionlabcn/jdp/raw/master/img/jdp-3-0-0-0-develop-plan.png)

* 测试计划

![](https://github.com/fusionlabcn/jdp/raw/master/img/jdp-3-0-0-0-testing.png)

地址：http://www.fusionlab.cn

* 项目列表

| 名称 | 说明 | 地址 |  状态 | 备注 | 
| :--- | :----: | :----: | :----: | :----: |
| jdp-package | JDP Ecosystem Package Management Tools | [Github](https://github.com/fusionlabcn/jdp-package) | ok |  :seedling: |
| jdp | JDP for roadmap | [Github](https://github.com/fusionlabcn/jdp) | ok |  :seedling: |
| jdp-select | JDP Ecosystem Package Core Tools | [Github](https://github.com/fusionlabcn/jdp-select) | ok |  :seedling: |
| jdp-ambari-mpack | JDP Ecosystem Management Platform | [Github](https://github.com/fusionlabcn/jdp-ambari-mpack) | ok |  :seedling: |
| Ambari | JDP Stack in Ambari | [Github](https://github.com/fusionlabcn/ambari) | ok |  :seedling: |

## JDP Development plan for 3.1.0.0 

* 研发计划

![](https://github.com/fusionlabcn/jdp/raw/master/img/jdp-3-1-0-0-develop-plan.png)

* 测试计划

![](https://github.com/fusionlabcn/jdp/raw/master/img/jdp-3-1-0-0-testing.png)

* 项目列表

| 名称 | 说明 | 地址 |  状态 | 备注 | 
| :--- | :----: | :----: | :----: | :----: |
| jdp-package | JDP Ecosystem Package Management Tools | [Github](https://github.com/fusionlabcn/jdp-package) | ok |  :seedling: |
| jdp-select | JDP Ecosystem Package Core Tools | [Github](https://github.com/fusionlabcn/jdp-select) | ok |  :seedling: |
| Ambari | JDP Stack in Ambari | [Github](https://github.com/fusionlabcn/ambari) | ok |  :seedling: |

注：jdp-ambari-mpack 和 jdp-ambari 项目在`3.1.0.0`中会融合，未来只会存在一个项目。

* 开发约束

项目列表，涉及的相关项目版本，全都统一为`branch-3.1.0.0`，jdp-package和labs-docs除外，拥有相关prefix，suffix需保持一致。
比如：jdp-3.1.0.0需具备版本一致性。

需要开启统称为`branch-3.1.0.0`分支以此为基础进行开发。最终release版本之前，可通`branch-3.1.0.0`分支发布带rc后缀的版本，比如rc1,rc2等。

新特性开发，可开启带develop关键字的分支，每个roadmap特性都会以pr的形式提到`branch-3.1.0.0`中，最终版本合并到master，并且打进行tag发布。

- {project_name}-number(unique)-feature-{describe}

bugfix开发，相关问题修复，需开启带有bugfix-{describe}关键字的分支，测试通过以pr的形式提给`branch-3.1.0.0`。

- {project_name}-number(unique)-bugfix-{describe}

commit信息，开发新特性和问题修复，严格以全英文方式提交信息，尽量让每一个pr都能清楚描述解决的问题或新特性。

文档编写

> 1. 新特性的开发，需在文档项目中，编写详细的设计文档，设计文档评审通过，开始实现功能。
> 2. 每个新特性开发合并`branch-3.1.0.0`，需要编写相关使用文档，每次提交CI持续集成会自动部署为一个静态网站，只需专注编写文档。整个文档严格遵守markdown语法规范，文档内容描述需通俗易懂，易于理解。

。。。。
