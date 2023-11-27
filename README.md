# 容器与架构

总结了架构设计中需要思考的一些问题，同时引入容器技术完善架构的弹性，也涉及到部分安全问题。

详细的计算机安全问题请参考专业文档资料


<!-- PROJECT SHIELDS -->

[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]
<!-- [![LinkedIn][linkedin-shield]][linkedin-url] -->

<!-- PROJECT LOGO -->

--------------------

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


--------------------

## 目录

[目录](index.md)

## 架构设计

### 参考文档
[架构设计要点](架构设计要点/架构设计.md)


## SpringCloud

### 参考文档

[SpringCloud官方文档](https://www.springcloud.cc/spring-reference.html)

[SpringCloudAlibaba官方文档](https://github.com/alibaba/spring-cloud-alibaba/wiki)

[SpringCloud组件示例代码](https://github.com/espmihacker/cloud2020)

[SpringCloud脚手架](https://github.com/zhoutaoo/SpringCloud)


## 文件服务

### 参考文档

[文件服务比较](https://blog.csdn.net/u011436427/article/details/98198935)

[FastDFS](FastDFS/FastDFS.md)

[OSS阿里云](https://help.aliyun.com/zh/oss/product-overview/what-is-oss)


## 容器技术

### 参考文档

#### Docker

[Docker自用笔记](Docker/Docker.md)

[Docker中文手册](https://docker-practice.github.io/zh-cn/)

#### Kubernetes:

[Kubernetes自用笔记](Kubernetes/Kubernetes.md)

[Kubernetes详细部署笔记](Kubernetes/follow-me-install-kubernetes-cluster/SUMMARY.md)


## 监控与性能分析

### 参考文档

[Zabbix使用手册](https://www.zabbix.com/documentation/current/zh/manual)

[Zabbix模板案例](https://github.com/zhujinhe/collection-of-zabbix-templates)

[Perf性能分析](https://www.brendangregg.com/perf.html)


## 贡献者

请阅读**CONTRIBUTING.md** 查阅为该项目做出贡献的开发者。

#### 如何参与开源项目

贡献使开源社区成为一个学习、激励和创造的绝佳场所。你所作的任何贡献都是**非常感谢**的。


1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request


## 版本控制

该项目使用Git进行版本管理。您可以在repository参看当前可用版本。

<!-- ## 作者 -->
<!--  -->
<!-- [小昊子](https://github.com/worst001) -->
<!--  -->
<!-- 制做不易，如果有帮到你就请作者喝杯咖啡吧! -->
<!--  -->
<!-- ![支付宝加微信](https://xiyou-oss.oss-cn-shanghai.aliyuncs.com/%E5%85%AC%E4%BC%97%E5%8F%B7%E4%B8%8E%E6%94%AF%E4%BB%98/%E6%94%AF%E4%BB%98%E5%AE%9D%E5%8A%A0%E5%BE%AE%E4%BF%A1.jpg) -->
<!--  -->
<!-- 作者无聊时做的测试游戏，完全免费哦！ -->
<!--  -->
<!-- ![公众号](https://xiyou-oss.oss-cn-shanghai.aliyuncs.com/%E5%85%AC%E4%BC%97%E5%8F%B7%E4%B8%8E%E6%94%AF%E4%BB%98/%E5%85%AC%E4%BC%97%E5%8F%B7%E5%B0%8F.jpg) -->

## 参考资料

[https://github.com/zhoutaoo/SpringCloud](https://github.com/zhoutaoo/SpringCloud)

[https://github.com/hegphegp/docker-learning](https://github.com/hegphegp/docker-learning)

[https://github.com/opsnull/follow-me-install-kubernetes-cluster](https://github.com/opsnull/follow-me-install-kubernetes-cluster)

[尚硅谷系列教程资料](http://www.atguigu.com/opensource.shtml)

<!-- links -->
[your-project-path]:shaojintian/Best_README_template
[contributors-shield]: https://img.shields.io/github/contributors/worst001/mkdocs_middleware.svg?style=flat-square
[contributors-url]: https://github.com/worst001/mkdocs_middleware/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/worst001/mkdocs_middleware.svg?style=flat-square
[forks-url]: https://github.com/worst001/mkdocs_middleware/network/members
[stars-shield]: https://img.shields.io/github/stars/worst001/mkdocs_middleware.svg?style=flat-square
[stars-url]: https://github.com/worst001/mkdocs_middleware/stargazers
[issues-shield]: https://img.shields.io/github/issues/worst001/mkdocs_middleware.svg?style=flat-square
[issues-url]: https://img.shields.io/github/issues/worst001/mkdocs_middleware.svg
[license-shield]: https://img.shields.io/github/license/worst001/mkdocs_middleware.svg?style=flat-square
[license-url]: https://github.com/worst001/mkdocs_middleware/blob/main/LICENSE.txt
<!-- [linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=flat-square&logo=linkedin&colorB=555 -->
<!-- [linkedin-url]: https://linkedin.com/in/shaojintian -->
