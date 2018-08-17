---
copyright:
  years: 2018
lastupdated: "2018-04-20"
---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# 安装 IBM Cloud Monitoring Service for IaaS Bare Metal Agent (Beta)

要在现有 {{site.data.keyword.baremetal_short}} 上运行高级监视，请执行以下步骤以在您的裸机设备上安装 {{site.data.keyword.BluSoftlayer_full}} Monitoring Service for IaaS Bare Metal Agent。

## 先决条件
必须连接到您的裸机设备来下载并运行安装程序。

## 在 Windows 中安装

1. 下载 Windows IBM Cloud Monitoring Agent 安装程序。[下载](http://downloads.service.softlayer.com/ibm-monitoring-baremetal-agent/latest/baremetal-monitoring-agent-windows-amd64.msi)
2. 在目标机器上运行该安装程序。 

## 在 Linux 中安装

1. 下载 Linux IBM Cloud Monitoring Agent 安装程序。[下载](http://downloads.service.softlayer.com/ibm-monitoring-baremetal-agent/latest/baremetal-monitoring-agent-linux-amd64.tgz)
2. 在目标机器上解压缩该安装程序。`tar –vxf baremetal-monitoring-agent-linux-amd64.tgz`
3. 运行 linux_install.sh 脚本。

        
## 在 FreeBSD 中安装
1. 下载 FreeBSD IBM Cloud Monitoring Agent 安装程序。[下载](http://downloads.service.softlayer.com/ibm-monitoring-baremetal-agent/latest/baremetal-monitoring-agent-freebsd-amd64.tgz)
2. 在目标机器上解压缩该安装程序。`tar -xvf baremetal-monitoring-agent-freebsd-amd64.tgz`
3. 运行 freebsd_install.sh 脚本。 

## 后续步骤

在您运行安装后，系统会自动完成安装过程。在 Windows 中，会显示一条消息，其中包含安装成功的确认信息，或有关所发生错误的信息。

如果使用防火墙，那么可能需要允许 IBM Cloud Monitoring Agent 通过防火墙传递数据。该代理程序使用端口 8090 进行出站 HTTPS 通信。有关可能需要允许的 IP 地址的更多信息，请参阅[负载均衡器 IP 范围](https://console.bluemix.net/docs/infrastructure/hardware-firewall-dedicated/ips.html#load-balancer-ips)。
