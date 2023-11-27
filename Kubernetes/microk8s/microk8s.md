# 常用命令速查

--------------------------------------

## SNAP

```bash

#重启服务
systemctl restart snapd

# 安装microk8s本
snap install microk8s --classic --channel=latest/stable

# 安装microk8s指定版本
snap install microk8s --classic --channel=1.11/stable

# 切换microk8s到指定版本
snap refresh --channel=latest/stable microk8s

# 卸载microk8s
snap remove microk8s

# 查看microk8s信息
snap info microk8s
```

-----------------------------------------------------------------

## microk8s

```bash

# 查看状态
microk8s status --wait-ready

# 启动
microk8s start

# 停止，会停止关联的服务
microk8s stop

# 附加插件
microk8s.enable dns dashboard ingress

# 去除插件
microk8s.disable dns dashboard ingress

# 状态检查
microk8s.inspect

```

-----------------------------------------------------------------
## kubectl

```bash

# 配置文件，修改后重启mirok8s后生效
vi /var/snap/microk8s/current/args/containerd.template.toml

# 设置别名
snap alias microk8s.kubectl kubectl

# 获取节点列表
kubectl get nodes

# 查看所有信息pod、service
kubectl get all -A

# 查看pod信息
kubectl get pods --all-namespaces 

# 查看pod的IP端口列表
kubectl get svc -A

# 查看指定pod的详细信息，包括IP、端口、错误等信息
kubectl describe --namespace kube-system pod/kubernetes-dashboard-6fd7f9c494-dgxlj

# 查看所有pod情
kubectl describe pod --all-namespaces

# 映射指定pod的指定端口到本地
kubectl port-forward --namespace=kube-system --address=0.0.0.0 pod/kubernetes-dashboard-6fd7f9c494-dgxlj 8443:8443

# 解释含义
kubectl explain pods
kubectl explain pods.spec.containers
```

-----------------------------------------------------------------
## containers

```bash

# 查看镜像
microk8s.ctr images ls

# 查看容器
microk8s.ctr containers ls

# 导入镜像
microk8s.ctr i import importImage.tarc

```

