<a name="readme-top"></a>
<!-- PROJECT SHIELDS -->

[![Contributors][contributors-shield]][contributors-url]
[![Forks][forks-shield]][forks-url]
[![Stargazers][stars-shield]][stars-url]
[![Issues][issues-shield]][issues-url]
[![MIT License][license-shield]][license-url]
<!-- [![LinkedIn][linkedin-shield]][linkedin-url] -->

<!-- PROJECT LOGO -->

<!-- 项目LOGO -->
<br />
<div align="center">
  <!-- <a href="http://note.grft.top"> -->
  <!--   <img src="https://xiyou-oss.oss-cn-shanghai.aliyuncs.com/mkdocs/logo.png" alt="Logo" width="480" height="270"> -->
  <!-- </a> -->

  <h3 align="center">容器与架构</h3>

  <p align="center">
    <br />
    <a href="http://note.grft.top/容器与架构/"><strong>探索文档 »</strong></a>
    <br />
  </p>
</div>

<!-- 目录 -->
<details>
  <summary>目录</summary>
  <ol>
    <li><a href="#关于项目">关于项目</a></li>
    <li><a href="#什么是架构设计">什么是架构设计</a></li>
    <li><a href="#什么是容器技术">什么是容器技术</a></li>
    <li><a href="#技术目录">技术目录</a></li>
    <li><a href="#贡献">贡献</a></li>
    <li><a href="#许可证">许可证</a></li>
    <li><a href="#联系方式">联系方式</a></li>
    <li><a href="#鸣谢">鸣谢</a></li>
  </ol>
</details>

## 关于项目

总结了架构设计中需要思考的一些问题，同时引入容器技术完善架构的弹性，也涉及到部分安全问题。

详细的计算机安全问题请参考专业文档资料

公网资料、笔记地址请访问这里 主入口可访问这里

- 文档地址: [http://note.grft.top/容器与架构/](http://note.grft.top/容器与架构/)

其他相关技术可以访问我的博客，主页地址请访问这里

- 访问入口：[http://note.grft.top](http://note.grft.top)

互联网中的架构设计和容器技术分别涵盖了软件开发和部署的关键方面。

<p align="right">(<a href="#readme-top">返回顶部</a>)</p>

## 什么是架构设计
互联网架构设计是指根据业务需求，系统特性，以及预期的用户负载来规划和设计软件系统的结构。
一个良好的架构设计能支持软件系统的伸缩性、可用性、性能和安全性。在互联网公司，架构通常需要设计得能够处理高并发访问、数据一致性问题、分布式系统的复杂性等等。

### 架构设计可以分为几个层次(包括但不限于)
+ 单体架构 - 一个单一的应用包含了所有的业务逻辑。它简单易部署，但难以扩展。
+ 分层架构 - 应用被分为不同层（如表示层、业务逻辑层、数据访问层），使得代码更加组织化和模块化。
+ 微服务架构 - 一个复杂的应用被拆分成一组小的、松耦合的服务，它们可以独立地开发、部署和缩放。
+ 服务导向架构(SOA) - 强调服务组合和复用，使用消息传递等机制实现不同服务之间的通信。
+ 事件驱动架构 - 中心化在事件的产生、探测、响应的机制，非常适合于高度异步的系统。
+ 云原生架构 - 设计用于利用云计算优势的架构，包括微服务、容器化、DevOps、持续交付和可观测性。

<p align="right">(<a href="#readme-top">返回顶部</a>)</p>

## 什么是容器技术
容器技术是一种轻量级、可移植、自给自足的软件打包机制，能让应用程序在几乎任何环境中无缝运行。容器为应用程序提供了一个隔离的执行环境，称为容器，该环境包括应用程序及其所有依赖，从而避免了在不同环境之间迁移时出现的“在我的机器上可以运行”问题。
Docker是一个广泛使用的容器平台，它使得创建、部署和运行容器变得简单。Kubernetes是一个容器编排系统，用于自动化容器部署、扩展和管理。

### 容器技术带来的主要优势包括
+ 一致性 - 开发、测试和生产环境可以保持一致性，降低了部署复杂性。
+ 快速部署 - 容器可以迅速启动和停止，加快了开发和发布的过程。
+ 微服务友好 - 微服务架构与容器化相辅相成，每个服务可以打包在自己的容器中。
+ 资源效率 - 容器在操作系统层面共享资源，使得它们比虚拟机更加资源高效。
+ 可移植性 - 容器可以在任何支持容器技术的环境中运行，包括各种云服务平台。
+ 伸缩性和自动化 - 容器可以利用Kubernetes等工具进行自动化扩缩和负载管理。

### 两者的关系
结合架构设计和容器技术可以创建出高度可扩展的、有弹性的互联网应用。架构设计提供了一个总体蓝图，而容器技术则为这些建筑的每个独立部分提供了一种高效和一致性的运行和管理方式。这样的结合通常被称为云原生架构，在云环境中发挥着越来越重要的作用。

<p align="right">(<a href="#readme-top">返回顶部</a>)</p>

## 技术目录

[目录与大纲](index.md)

### 架构设计

+ [架构设计要点](架构设计要点/架构设计.md)

### SpringCloud

+ [SpringCloud官方文档](https://www.springcloud.cc/spring-reference.html)
+ [SpringCloudAlibaba官方文档](https://github.com/alibaba/spring-cloud-alibaba/wiki)
+ [SpringCloud组件示例代码](https://github.com/espmihacker/cloud2020)
+ [SpringCloud脚手架](https://github.com/zhoutaoo/SpringCloud)


### 文件服务

+ [文件服务比较](https://blog.csdn.net/u011436427/article/details/98198935)
+ [FastDFS](https://cloud.tencent.com/developer/article/1915740)
+ [OSS阿里云](https://help.aliyun.com/zh/oss/product-overview/what-is-oss)

### 容器技术

#### Docker

+ [Docker自用笔记](Docker/Docker.md)
+ [Docker详细笔记](https://github.com/jaywcjlove/docker-tutorial)
+ [Docker中文手册](https://docker-practice.github.io/zh-cn/)

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

#### 详细文档资料
+ [1、组件介绍](Kubernetes/文档/1、Kubernetes%20-%20组件介绍/1、笔记/Kubernetes%20组件介绍.pdf)
+ [2、基础概念](Kubernetes/文档/2、Kubernetes%20-%20基础概念/1、笔记/Kubernetes%20基础概念.pdf)
+ [3、集群安装](Kubernetes/文档/3、Kubernetes%20-%20集群安装/1、笔记/Kubernetes%20集群安装.pdf)
+ [4、资源清单](Kubernetes/文档/4、Kubernetes%20-%20资源清单/1、笔记/Kubernetes%20资源清单.pdf)
+ 5、资源控制器:
    - [Pod 控制器](Kubernetes/文档/5、Kubernetes%20-%20资源控制器/1、笔记/1、Kubernetes%20Pod%20控制器.pdf)
    - [Deployment 控制器](Kubernetes/文档/5、Kubernetes%20-%20资源控制器/1、笔记/2、Kubernetes%20Deployment%20控制器.pdf)
    - [DaemonSet 控制器](Kubernetes/文档/5、Kubernetes%20-%20资源控制器/1、笔记/3、Kubernetes%20DaemonSet%20控制器.pdf)
    - [JobCronJob 控制器](Kubernetes/文档/5、Kubernetes%20-%20资源控制器/1、笔记/4、Kubernetes%20JobCronJob%20控制器.pdf)
+ 6、Service:
    - [Service](Kubernetes/文档/6、Kubernetes%20-%20Service/1、笔记/1、Kubernetes%20Service.pdf)
    - [Ingress](Kubernetes/文档/6、Kubernetes%20-%20Service/1、笔记/2、Kubernetes%20Ingress.pdf)
+ 7、存储:
    - [configMap](Kubernetes/文档/7、Kubernetes%20-%20存储/1、笔记/1、Kubernetes%20-%20configMap.pdf)
    - [Secret](Kubernetes/文档/7、Kubernetes%20-%20存储/1、笔记/2、Kubernetes%20-%20Secret.pdf)
    - [volume](Kubernetes/文档/7、Kubernetes%20-%20存储/1、笔记/3、Kubernetes%20-%20volume.pdf)
    - [Persistent](Kubernetes/文档/7、Kubernetes%20-%20存储/1、笔记/4、Kubernetes%20-%20Persistent%20Volume.pdf)
+ 8、集群调度:
    - [调度说明](Kubernetes/文档/8、Kubernetes%20-%20集群调度/1、笔记/1、Kubernetes%20调度器%20-%20调度说明.pdf)
    - [调度亲和性](Kubernetes/文档/8、Kubernetes%20-%20集群调度/1、笔记/2、Kubernetes%20调度器%20-%20调度亲和性.pdf)
    - [污点](Kubernetes/文档/8、Kubernetes%20-%20集群调度/1、笔记/3、Kubernetes%20调度器%20-%20污点.pdf)
    - [固定节点](Kubernetes/文档/8、Kubernetes%20-%20集群调度/1、笔记/4、Kubernetes%20调度器%20-%20固定节点.pdf)
+ 9、安全:
    - [机制说明](Kubernetes/文档/9、Kubernetes%20-%20安全/1、笔记/1、Kubernetes%20集群安全%20-%20机制说明.pdf)
    - [认证](Kubernetes/文档/9、Kubernetes%20-%20安全/1、笔记/2、Kubernetes%20集群安全%20-%20认证.pdf)
    - [鉴权](Kubernetes/文档/9、Kubernetes%20-%20安全/1、笔记/3、Kubernetes%20集群安全%20-%20鉴权.pdf)
    - [准入控制](Kubernetes/文档/9、Kubernetes%20-%20安全/1、笔记/4、Kubernetes%20集群安全%20-%20准入控制.pdf)
+ 10、Helm 及其它功能性组件:
    - [部署 Helm](Kubernetes/文档/10、Kubernetes%20-%20Helm%20及其它功能性组件/1、笔记/1、部署%20Helm.pdf)
    - [使用 Helm 部署 dashboard](Kubernetes/文档/10、Kubernetes%20-%20Helm%20及其它功能性组件/1、笔记/2、使用%20Helm%20部署%20dashboard%20.pdf)
    - [使用 Helm 部署 metrics-server](Kubernetes/文档/10、Kubernetes%20-%20Helm%20及其它功能性组件/1、笔记/3、使用%20Helm%20部署%20metrics-server.pdf)
    - [部署 prometheus](Kubernetes/文档/10、Kubernetes%20-%20Helm%20及其它功能性组件/1、笔记/4、部署%20prometheus.pdf)
    - [部署 EFK 平台](Kubernetes/文档/10、Kubernetes%20-%20Helm%20及其它功能性组件/1、笔记/5、部署%20EFK%20平台.pdf)
+ 11、证书可用时间修改:
  - [证书有效期修改](Kubernetes/文档/11、Kubernetes%20-%20证书可用时间修改/1、笔记/证书有效期修改.pdf)
+ 12、高可用的 K8S 集群构建:
  - [系统初始化](Kubernetes/文档/11、Kubernetes%20-%20证书可用时间修改/1、笔记/证书有效期修改.pdf)
  - [Kubeadm 部署安装改](Kubernetes/文档/11、Kubernetes%20-%20证书可用时间修改/1、笔记/证书有效期修改.pdf)


### Ansible

+ [详细笔记](Ansible/运维自动化之ANSIBLE.md)
+ [Ansible](https://cn-ansibledoc.readthedocs.io/zh-cn/latest/)
+ [Ansible-Galaxy](https://galaxy.ansible.com/ui/)


### 监控与性能分析

+ [Zabbix使用手册](https://www.zabbix.com/documentation/current/zh/manual)
+ [Zabbix模板案例](https://github.com/zhujinhe/collection-of-zabbix-templates)
+ [Perf性能分析](https://www.brendangregg.com/perf.html)

<p align="right">(<a href="#readme-top">返回顶部</a>)</p>

<!-- 贡献 -->

## 贡献

贡献是使开源社区成为一个如此令人惊叹的地方，以学习、激励和创造。您所做的任何贡献都将非常感谢。

如果您对使这个项目变得更好有建议，请 fork 该仓库并创建 pull request。您也可以打开一个带有“enhancement”标签的问题。不要忘记给这个项目点个星！再次感谢！

<p align="right">(<a href="#readme-top">返回顶部</a>)</p>


<!-- 许可证 -->
## 许可证

根据 MIT 许可证进行分发。更多信息请参见 [LICENSE.txt](LICENSE)。

<p align="right">(<a href="#readme-top">返回顶部</a>)</p>

<!-- 联系方式 -->
## 联系方式

关注我: [小昊子](https://github.com/worst001)

博客地址: [http://note.grft.top](http://note.grft.top)

项目链接: [https://github.com/worst001/note_container_architecture](https://github.com/worst001/note_container_architecture)

<p align="right">(<a href="#readme-top">返回顶部</a>)</p>

## 鸣谢

因为仓库与文档的数量比较大，有些借鉴资料忘了在`参考文档`部分提及原作者与原仓库，若有疏漏请告诉，我及时补上。

所有引用的原资料都确认是开源认证，若有侵权请告知。

[https://github.com/zhoutaoo/SpringCloud](https://github.com/zhoutaoo/SpringCloud)

[https://github.com/hegphegp/docker-learning](https://github.com/hegphegp/docker-learning)

[https://github.com/opsnull/follow-me-install-kubernetes-cluster](https://github.com/opsnull/follow-me-install-kubernetes-cluster)

[https://github.com/ansible/ansible-examples](https://github.com/ansible/ansible-examples)

[https://www.yuque.com/qiuyi1992/blog/upib2e](https://www.yuque.com/qiuyi1992/blog/upib2e)

[尚硅谷系列教程资料](http://www.atguigu.com/opensource.shtml)

[https://openai.com/chatgpt](https://openai.com/chatgpt)

<p align="right">(<a href="#readme-top">返回顶部</a>)</p>

<!-- links -->
[your-project-path]:shaojintian/Best_README_template
[contributors-shield]: https://img.shields.io/github/contributors/worst001/note_container_architecture.svg?style=flat-square
[contributors-url]: https://github.com/worst001/note_container_architecture/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/worst001/note_container_architecture.svg?style=flat-square
[forks-url]: https://github.com/worst001/note_container_architecture/network/members
[stars-shield]: https://img.shields.io/github/stars/worst001/note_container_architecture.svg?style=flat-square
[stars-url]: https://github.com/worst001/note_container_architecture/stargazers
[issues-shield]: https://img.shields.io/github/issues/worst001/note_container_architecture.svg?style=flat-square
[issues-url]: https://img.shields.io/github/issues/worst001/note_container_architecture.svg
[license-shield]: https://img.shields.io/github/license/worst001/note_container_architecture.svg?style=flat-square
[license-url]: https://github.com/worst001/note_container_architecture/blob/main/LICENSE.txt
<!-- [linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=flat-square&logo=linkedin&colorB=555 -->
<!-- [linkedin-url]: https://linkedin.com/in/shaojintian -->
