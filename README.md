## Introduction

因为 github.com 的访问速度较慢，Openpilot 源码较大（~600M），一些分支版本甚至超过1G，这让 Openpilot 的下载安装变得非常痛苦，基于以上原因，需要把 openpilot 相关的项目同步到 gitee，这个脚本，是用于自动登录 gitee 并触发强制同步的。


项目地址：https://doc.sdut.me/mirror.html

## Usage

### 异地登陆验证

gitee **异地登录**需要输入验证码，先关注公众号 giteecom 绑定账号后可以 **跳过验证**。

### 安装依赖

#### 安装 python 依赖

```bash
pip install -r requirements.txt
```

### 修改配置

```bash
# 根据样例复制一份
cp .env.example .env 

# 编辑用户名密码，更新成自己的
vi .env
```

### 运行

```bash
# 使用 root 权限运行
sudo python SyncOpenpilot.py
```
