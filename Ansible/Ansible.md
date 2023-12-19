# Ansible

## 批量发送公钥

事先安装了 `sshpass` 这个工具来非交互式输入密码。

```bash
#!/bin/bash

# 获取待发送公钥的文件路径，默认使用当前用户的公钥
PUBLIC_KEY_PATH="${HOME}/.ssh/id_rsa.pub"

# 确保提供了至少一个IP地址作为参数
if [ "$#" -lt 1 ]; then
  echo "Usage: $0 IP_ADDRESS [IP_ADDRESS...]"
  exit 1
fi

# 获取 SSH 用户名和密码
read -p "Enter SSH Username: " SSH_USER
read -s -p "Enter SSH Password: " SSH_PASS
echo

# 循环遍历所有提供的 IP 地址
for HOST_IP in "$@"
do
  # 使用 sshpass 和 ssh-copy-id 将公钥复制到对应的托管节点
  sshpass -p "$SSH_PASS" ssh-copy-id -i "$PUBLIC_KEY_PATH" -o StrictHostKeyChecking=no "${SSH_USER}@${HOST_IP}"
done

echo "Public key has been copied to all the provided hosts."


```

将这个脚本保存成一个文件，比如 `send-ssh-keys.sh`，赋予它执行权限：

```bash
chmod +x send-ssh-keys.sh

```

然后，可以这样执行脚本：

```bash
./send-ssh-keys.sh 192.168.1.1 192.168.1.2 192.168.1.3

```

