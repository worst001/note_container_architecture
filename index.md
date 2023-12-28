<!-- PROJECT SHIELDS -->

[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]
[![Stargazers][stars-shield]][stars-url]
<!-- [![LinkedIn][linkedin-shield]][linkedin-url] -->

<!-- PROJECT LOGO -->

# 容器与架构

互联网中的架构设计和容器技术分别涵盖了软件开发和部署的关键方面。

## 架构设计
互联网架构设计是指根据业务需求，系统特性，以及预期的用户负载来规划和设计软件系统的结构。
一个良好的架构设计能支持软件系统的伸缩性、可用性、性能和安全性。在互联网公司，架构通常需要设计得能够处理高并发访问、数据一致性问题、分布式系统的复杂性等等。

### 架构设计可以分为几个层次(包括但不限于)
+ 单体架构 - 一个单一的应用包含了所有的业务逻辑。它简单易部署，但难以扩展。
+ 分层架构 - 应用被分为不同层（如表示层、业务逻辑层、数据访问层），使得代码更加组织化和模块化。
+ 微服务架构 - 一个复杂的应用被拆分成一组小的、松耦合的服务，它们可以独立地开发、部署和缩放。
+ 服务导向架构(SOA) - 强调服务组合和复用，使用消息传递等机制实现不同服务之间的通信。
+ 事件驱动架构 - 中心化在事件的产生、探测、响应的机制，非常适合于高度异步的系统。
+ 云原生架构 - 设计用于利用云计算优势的架构，包括微服务、容器化、DevOps、持续交付和可观测性。

## 容器技术
容器技术是一种轻量级、可移植、自给自足的软件打包机制，能让应用程序在几乎任何环境中无缝运行。容器为应用程序提供了一个隔离的执行环境，称为容器，该环境包括应用程序及其所有依赖，从而避免了在不同环境之间迁移时出现的“在我的机器上可以运行”问题。
Docker是一个广泛使用的容器平台，它使得创建、部署和运行容器变得简单。Kubernetes是一个容器编排系统，用于自动化容器部署、扩展和管理。

### 容器技术带来的主要优势包括
+ 一致性 - 开发、测试和生产环境可以保持一致性，降低了部署复杂性。
+ 快速部署 - 容器可以迅速启动和停止，加快了开发和发布的过程。
+ 微服务友好 - 微服务架构与容器化相辅相成，每个服务可以打包在自己的容器中。
+ 资源效率 - 容器在操作系统层面共享资源，使得它们比虚拟机更加资源高效。
+ 可移植性 - 容器可以在任何支持容器技术的环境中运行，包括各种云服务平台。
+ 伸缩性和自动化 - 容器可以利用Kubernetes等工具进行自动化扩缩和负载管理。

## 两者的关系
结合架构设计和容器技术可以创建出高度可扩展的、有弹性的互联网应用。架构设计提供了一个总体蓝图，而容器技术则为这些建筑的每个独立部分提供了一种高效和一致性的运行和管理方式。这样的结合通常被称为云原生架构，在云环境中发挥着越来越重要的作用。

-----------------------


## 架构设计

### 参考文档
[架构设计要点](架构设计要点/架构设计.md)

### 基本介绍
架构设计是软件开发过程中至关重要的一步，它关乎到系统的质量、性能、可维护性、可扩展性和安全性。

+ 需求理解
    + 明确项目的业务需求，例如性能需求、数据一致性需求、可用性要求等。了解预期的用户量、数据增长、请求量、数据读写比率等指标。
+ 模块化与分层
    + 将系统从逻辑上分解为独立的模块和层次，以便于管理和扩展。使用服务化或微服务架构(SpringCloud)，将不同的服务职责划分明确。
+ 数据设计
    + 根据数据量、数据模型设计合适的数据库架构，选择合适的数据库类型（关系型/非关系型）。针对数据的访问模式和一致性需求选择适合的数据复制和分片策略。
+ 可扩展性与弹性
    + 设计可横向扩展的架构，以对应业务增长和高峰期流量。实现自动扩展功能，让系统能够根据负载自动增减资源。
+ 高可用性与容错性
    + 采用冗余设计，如多副本、多活跨地域集群来提高系统的可用性。设计故障切换机制和灾难恢复策略，保证系统的持续运行。
+ 性能优化
    + 使用高效的通信协议和数据序列化方法。合理设置缓存层，减轻数据库层的压力。依据性能测试结果对系统进行调优。
+ 网络设计
    + 优化网络拓扑，尽可能减少延迟和带宽限制。根据流量模式配置合理的负载均衡策略。
+ 安全性
    + 实施网络层和应用层的安全策略，如防火墙、入侵检测系统等。确保数据传输的加密和敏感数据的安全存储。
+ 监控和日志
    + 实施实时监控系统，以获取系统的健康状态和性能指标。收集和分析日志，便于故障排查和性能调优。
+ 成本效益
    + 评估与预算项目的成本，并根据需要在性能和成本之间权衡。考虑使用云服务能带来的经济效益，如按需付费等。
+ 灵活性与未来证明
    + 架构设计应有助于未来技术的整合，避免落入技术陷阱。考虑系统未来可能的扩展方向，如新功能的添加和技术栈的迭代。


## SpringCloud

### 参考文档

[SpringCloud官方文档](https://www.springcloud.cc/spring-reference.html)

[SpringCloudAlibaba官方文档](https://github.com/alibaba/spring-cloud-alibaba/wiki)

[SpringCloud组件示例代码](https://github.com/espmihacker/cloud2020)

[SpringCloud脚手架](https://github.com/zhoutaoo/SpringCloud)

### 基本介绍
Spring Cloud是一个用于构建分布式系统的开发工具包（framework）。
它基于Spring框架，提供了一系列的组件和库，用于简化开发、部署和管理分布式系统中的常见模式和功能。
Spring Cloud的设计目标是帮助开发人员快速构建具有弹性、可伸缩性和高可用性的分布式应用。
它提供了多个子项目，每个子项目都专注于解决分布式系统中的不同问题。

#### Spring Cloud 相关组件包括
+ 服务注册与发现（Service Discovery）
    + 通过使用Eureka、Consul或Zookeeper等注册中心，可以实现服务的自动注册和发现。服务提供者在启动时将自己注册到注册中心，服务消费者可以从注册中心获取可用的服务地址，实现服务之间的动态调用。
+ 负载均衡（Load Balancing）
    + 通过Ribbon组件，Spring Cloud可以实现负载均衡，将请求分发到多个服务实例上，提高系统的可扩展性和容错性。
+ 配置管理（Configuration Management）
    + 使用Spring Cloud Config，可以集中管理分布式系统的配置信息，并支持配置文件的动态刷新，减少配置变更对系统的影响。
+ 熔断器（Circuit Breaker）
    + 通过Hystrix组件，Spring Cloud可以实现熔断器模式，当某个服务发生故障或超时时，熔断器可以快速响应并提供默认的降级策略，防止故障扩散。
+ 分布式消息传递（Messaging）
    + 通过使用Spring Cloud Stream，可以实现分布式系统中的异步消息传递。它支持多种消息中间件，如Kafka、RabbitMQ等，并提供了统一的编程模型。
+ 链路追踪（Tracing）
    + 通过使用Spring Cloud Sleuth和Zipkin，可以实现对分布式系统请求的链路追踪和监控，帮助开发人员分析和解决系统中的性能问题。
+ API 网关（API Gateway）
    + 通过Spring Cloud Gateway或Zuul，可以构建一个统一的入口来管理和保护后端的微服务，并提供路由、鉴权、限流等功能。

#### Spring Cloud Alibaba相关组件包括
+ Nacos
    + 一个动态服务发现、配置管理和服务管理平台。Nacos支持服务的注册与发现，提供了动态配置服务，其配置管理能力可以动态调整微服务配置，而无须重启服务。
+ Sentinel
    + 一种流量控制组件，其提供高效的流量防护和监控功能。Sentinel主要负责微服务的容错管理，它可以处理诸如熔断限流、降级和系统负载保护等功能。
+ RocketMQ
    + 用于消息传递的中间件。它提供了可靠的消息发布和订阅机制，并且保证了强一致性。RocketMQ适用于复杂的分布式系统中的异步通信和解耦。
+ Seata
    + 一种分布式事务协调组件。Seata 执行全局事务管理，通过控制分布式事务的提交或回滚，以保持数据的最终一致性。
+ Alibaba Cloud OSS
    + 集成了阿里云的对象存储服务（OSS），是一个海量、安全、低成本、高可靠的云存储服务，用于存放和处理各类文件。
+ Alibaba Cloud SchedulerX
    + 一种分布式任务调度组件，其提供了秒级、精准、高可靠、高可用的定时（基于CRON）任务调度服务。
+ Alibaba Cloud SMS
    + 集成了阿里云的短信服务，用于发送短信通知和验证码等。


## 文件服务

### 参考文档

[文件服务比较](https://blog.csdn.net/u011436427/article/details/98198935)

[FastDFS](https://cloud.tencent.com/developer/article/1915740)

[OSS阿里云](https://help.aliyun.com/zh/oss/product-overview/what-is-oss)

### 基本介绍
架构设计是软件开发过程中至关重要的一步，它关乎到系统的质量、性能、可维护性、可扩展性和安全性。
文件服务是指提供对文件的存储、管理和访问的一种服务。
在分布式系统中，文件服务通常被用于存储和共享各种类型的文件，如图片、文档、视频等。

+ 存储
    + 文件服务提供了可靠的存储介质，用于保存用户上传的文件。这些文件可以被长期保留，并根据需要进行读取、写入和删除操作。
+ 访问控制
    + 文件服务通常支持对文件的访问控制，以确保只有经过授权的用户或应用程序能够访问特定的文件。这可以通过基于角色的权限控制、访问令牌或访问密钥来实现。
+ 文件管理
    + 文件服务提供了对文件的元数据管理，允许用户为文件添加标签、描述、分类等信息，方便文件的组织和检索。
+ 文件传输
    + 文件服务支持文件的上传和下载操作，以便用户可以方便地将文件从本地设备上传到服务器，或者从服务器下载到本地设备。
+ 文件共享
    + 文件服务通常提供共享文件的功能，使多个用户或应用程序能够同时访问和编辑同一个文件。这可以通过共享链接、访问权限控制等方式实现。
+ 备份与恢复
    + 文件服务通常具备数据备份和恢复机制，以保护文件免受数据丢失或损坏的影响。备份可以定期进行，以确保文件数据的安全性和可恢复性。

常见的文件服务包括云存储服务（如阿里OSS、Amazon S3、Google Cloud Storage）、分布式文件系统（如Hadoop HDFS、Ceph）以及基于对象存储的文件服务（如MinIO、OpenStack Swift）。
这些文件服务提供了高可用性、可伸缩性和数据持久性等特性，适用于各种规模和需求的应用场景。


## 容器技术

### 参考文档

#### Docker

[Docker自用笔记](Docker/Docker.md)

[Docker详细笔记](https://github.com/jaywcjlove/docker-tutorial)

[Docker中文手册](https://docker-practice.github.io/zh-cn/)

#### Kubernetes

+ [Kubernetes自用笔记](Kubernetes/Kubernetes.md)

#### Kubernetes详细部署笔记
+ [目录](Kubernetes/follow-me-install-kubernetes-cluster/SUMMARY.md)
+ [00.组件版本和配置策略](Kubernetes/follow-me-install-kubernetes-cluster/00.组件版本和配置策略.md)
+ [01.初始化系统和全局变量](Kubernetes/follow-me-install-kubernetes-cluster/01.初始化系统和全局变量.md)
+ [02.创建CA根证书和秘钥](Kubernetes/follow-me-install-kubernetes-cluster/02.创建CA根证书和秘钥.md)
+ [03.kubectl](Kubernetes/follow-me-install-kubernetes-cluster/03.kubectl.md)
+ [04.etcd集群](Kubernetes/follow-me-install-kubernetes-cluster/04.etcd集群.md)
+ 05.部署master:
  - [05-1.master节点](Kubernetes/follow-me-install-kubernetes-cluster/05-1.master节点.md)
  - [05-2.apiserver集群](Kubernetes/follow-me-install-kubernetes-cluster/05-2.apiserver集群.md)
  - [05-3.controller-manager集群](Kubernetes/follow-me-install-kubernetes-cluster/05-3.controller-manager集群.md)
  - [05-4.scheduler集群](Kubernetes/follow-me-install-kubernetes-cluster/05-4.scheduler集群.md)
+ 06.部署worker:
  - [06-1.worker节点](Kubernetes/follow-me-install-kubernetes-cluster/06-1.worker节点.md)
  - [06-2.apiserver高可用](Kubernetes/follow-me-install-kubernetes-cluster/06-2.apiserver高可用.md)
  - [06-3.containerd](Kubernetes/follow-me-install-kubernetes-cluster/06-3.containerd.md)
  - [06-4.kubelet](Kubernetes/follow-me-install-kubernetes-cluster/06-4.kubelet.md)
  - [06-5.kube-proxy](Kubernetes/follow-me-install-kubernetes-cluster/06-5.kube-proxy.md)
  - [06-6.calico](Kubernetes/follow-me-install-kubernetes-cluster/06-6.calico.md)
+ [07.验证集群功能](Kubernetes/follow-me-install-kubernetes-cluster/07.验证集群功能.md)
+ 08.部署插件:
  - [08-1.部署集群插件](Kubernetes/follow-me-install-kubernetes-cluster/08-1.部署集群插件.md)
  - [08-2.coredns插件](Kubernetes/follow-me-install-kubernetes-cluster/08-2.coredns插件.md)
  - [08-3.dashboard插件](Kubernetes/follow-me-install-kubernetes-cluster/08-3.dashboard插件.md)
  - [08-4.kube-prometheus插件](Kubernetes/follow-me-install-kubernetes-cluster/08-4.kube-prometheus插件.md)
  - [08-5.EFK插件](Kubernetes/follow-me-install-kubernetes-cluster/08-5.EFK插件.md)
+ [09.Registry](Kubernetes/follow-me-install-kubernetes-cluster/09.Registry.md)
+ [10.清理集群](Kubernetes/follow-me-install-kubernetes-cluster/10.清理集群.md)
+ [A.浏览器访问kube-apiserver安全端口](Kubernetes/follow-me-install-kubernetes-cluster/A.浏览器访问kube-apiserver安全端口.md)
+ [B.校验TLS证书](Kubernetes/follow-me-install-kubernetes-cluster/B.校验TLS证书.md)
+ [C.metrics-server插件](Kubernetes/follow-me-install-kubernetes-cluster/C.metrics-server插件.md)
+ [D.部署Harbor-Registry](Kubernetes/follow-me-install-kubernetes-cluster/D.部署Harbor-Registry.md)
+ [E.部署flannel网络](Kubernetes/follow-me-install-kubernetes-cluster/E.部署flannel网络.md)
+ [F.部署docker](Kubernetes/follow-me-install-kubernetes-cluster/F.部署docker.md)

##### 详细文档资料
+ [Kubernetes详细文档资料](Kubernetes/Direction.md)

### 基本介绍
容器技术是一种用于虚拟化和隔离应用程序的轻量级虚拟化技术。它将应用程序及其所有依赖项（例如库、配置文件等）打包到一个独立的运行环境中，称为容器。每个容器都是相互隔离且具有自己的文件系统、进程空间和网络接口。

+ 隔离性
    + 容器提供了应用程序之间的强隔离，使它们在同一主机上运行时相互不受干扰。这种隔离性可以防止应用程序之间的冲突和干扰，提高系统的安全性和可靠性。
+ 轻量级
    + 相比于传统的虚拟机技术，容器技术更加轻量级。容器共享主机的操作系统内核，并在其上运行应用程序，因此容器的启动速度更快，资源占用更少。
+ 可移植性
    + 容器可以在不同的平台和环境中进行移植，包括物理机、虚拟机、云平台等。由于容器打包了所有的依赖项，所以应用程序可以在各种环境中以相同的方式运行，减少了部署和配置的复杂性。
+ 弹性伸缩
    + 容器技术使得应用程序的弹性伸缩变得更加容易。通过在需要时快速启动或停止容器实例，可以根据负载情况进行动态调整，以满足不同的需求。
+ 简化部署和管理
    + 容器技术提供了统一的部署和管理模型。通过使用容器编排工具（如Kubernetes、Docker Swarm等），可以自动化地部署、扩展和管理容器集群，简化了应用程序的运维工作。

容器技术的发展主要得益于Docker这样的开源项目的推动。Docker为容器技术提供了一个流行的标准和工具生态系统，使得容器的使用变得更加简单和普及。此外，还有其他的容器技术和平台，如LXC、rkt、Podman等，它们提供了不同的特性和适用场景。


## Ansible

### 参考资料

[详细笔记](Ansible/运维自动化之ANSIBLE.md)

[Ansible](https://cn-ansibledoc.readthedocs.io/zh-cn/latest/)

[Ansible-Galaxy](https://galaxy.ansible.com/ui/)

### 基本介绍

Ansible是一种开源的自动化工具，用于配置管理、应用程序部署和编排任务。它采用简单易懂的语法和模块化的设计，使得系统管理人员可以轻松地自动化各种IT任务。

#### 以下是关于Ansible的一些要点

+ 基于SSH协议：
    + Ansible使用SSH协议与远程主机通信，无需在远程主机上安装任何代理或软件。这使得部署和管理任务更加简单和安全。
+ 声明性语法：
    + Ansible使用声明性的YAML语法来描述系统配置和任务。通过编写易读的Playbooks，可以定义所需的状态和操作，而无需关心底层执行细节。
+ 模块化设计：
    + Ansible提供了大量的模块，用于执行各种系统管理任务，如文件操作、包管理、服务管理等。这些模块可以根据需要组合，以实现复杂的自动化流程。
+ 剧本（Playbooks）：
    + 剧本是Ansible的核心概念，它是一个文本文件，包含了一系列任务和配置。通过编写剧本，可以定义整个自动化过程，并按顺序执行其中的任务。
+ 主控节点（Control Node）：
    + Ansible的控制节点是运行Ansible命令和Playbooks的主机。控制节点上的Ansible命令会通过SSH连接到远程主机执行任务。
+ 库与社区支持：
    + Ansible拥有丰富的模块库和活跃的社区支持。官方提供了大量的核心模块，同时社区也贡献了许多自定义模块和Playbooks，可以满足各种不同场景的需求。
+ 可扩展性：
    + Ansible具有良好的可扩展性，可以轻松地扩展到数千台远程主机。它支持分组、变量和条件控制等功能，使得管理大规模基础架构变得更加简单。


## 监控与性能分析

### 参考文档

[Zabbix使用手册](https://www.zabbix.com/documentation/current/zh/manual)

[Zabbix模板案例](https://github.com/zhujinhe/collection-of-zabbix-templates)

[Perf性能分析](https://www.brendangregg.com/perf.html)

### 基本介绍

#### Zabbix
+ Zabbix是一个开源的企业级监控解决方案，用于监测各种IT基础设施组件的性能和可用性。
+ 它提供了丰富的功能，包括数据收集、报警、可视化和自动化等。
+ Zabbix使用代理程序或SNMP来收集各种指标，如CPU利用率、内存使用情况、网络流量、磁盘空间等。
+ 它支持多种通信协议和监控方式，并提供Web界面和API来进行配置和管理。
+ Zabbix还提供了灵活的报警机制，可以在指标达到预设阈值时发送通知，以及生成图表和报告等。

#### Perf
+ Perf是Linux操作系统上的性能分析工具，用于深入了解系统的性能特征和瓶颈。
+ Perf可以对CPU、内存、磁盘IO、网络等方面的性能指标进行采集和分析。
+ 它通过使用Linux内核提供的性能事件计数器（PMU）和性能事件采集子系统，实时监测和分析各个组件的性能。
+ Perf提供了一系列的命令行工具，可以进行事件采集、数据分析和报告生成等操作。
+ Perf还支持可视化工具，如perf report、perf top等，用于更直观地展示性能数据。


<!-- links -->
[your-project-path]:shaojintian/Best_README_template
[contributors-shield]: https://img.shields.io/github/contributors/worst001/note_container_architecture.svg?style=flat-square
[contributors-url]: https://github.com/worst001/note_container_architecture/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/worst001/note_container_architecture.svg?style=flat-square
[forks-url]: https://github.com/worst001/note_container_architecture/network/members
[stars-shield]: https://img.shields.io/github/stars/worst001/note_container_architecture.svg?style=social
[stars-url]: https://github.com/worst001/note_container_architecture/stargazers
[issues-shield]: https://img.shields.io/github/issues/worst001/note_container_architecture.svg?style=flat-square
[issues-url]: https://img.shields.io/github/issues/worst001/note_container_architecture.svg
[license-shield]: https://img.shields.io/github/license/worst001/note_container_architecture.svg?style=flat-square
[license-url]: https://github.com/worst001/note_container_architecture/blob/main/LICENSE.txt
