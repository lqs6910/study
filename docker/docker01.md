# 基于Ubuntu安装
## 1. 更新atp索引
> $ sudo apt-get update

## 2. 安装最新版本的Docker CE和containerd，或者转到下一步安装特定版本
> $ sudo apt-get install docker-ce docker-ce-cli containerd.io

## 3. 要安装特定版本的Docker CE，请在repo中列出可用版本，然后选择并安装
> $ apt-cache madison docker-ce \
> $ sudo apt-get install docker-ce=<VERSION_STRING> docker-ce-cli=<VERSION_STRING containerd.io

## 4. 如果您想将Docker用作非root用户，您现在应该考虑将您的用户添加到“docker”组
> $sudo usermod -aG docker your-user