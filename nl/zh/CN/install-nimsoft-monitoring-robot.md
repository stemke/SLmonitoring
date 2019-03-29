---

copyright:
  years: 2014, 2019
lastupdated: "2019-02-11"

keywords:

subcollection: slmonitoring

---

{:shortdesc: .shortdesc}
{:new_window: target="_blank"}

# 安装和管理 Nimsoft Monitoring Robot
{: #installing-and-managing-the-nimsoft-monitoring-robot}

要在现有 {{site.data.keyword.baremetal_short}} 或 {{site.data.keyword.BluVirtServers_short}} 上运行高级监视，请安装 Nimsoft Monitoring Robot。Nimsoft Monitoring Robot 允许监视管理系统与专用网络上的裸机服务器或虚拟服务器进行通信。安装 Nimsoft Monitoring Robot 之后，大约需要 5-10 分钟才能在 {{site.data.keyword.slportal_full}} 上使用该应用程序。要在 Windows 或 Linux 中安装 Nimsoft Monitoring Robot，请执行以下步骤。

## 先决条件

安装之前，必须在专用网络上打开以下端口：

* tcp/48000
* tcp/48001
* tcp/48002

此外，还需要为专用网络打开端口 tcp/48003 到 tcp/50000，以允许 API 所使用的完整功能。如果未打开这些端口，某些监视代理程序会受到影响。如果在配置期间遇到错误，请先确保这些端口已打开，然后再开具凭单来上报问题。

* 对于某些监视代理程序，**openjdk** 是必需的，例如 Tomcat Monitoring Agent。
* 某些 64 位 Linux 分发版需要 **glibc.i686** 和 **nss-softtokn-freebl.i686**。
* **FreeBSD** 中不支持监视系统。

如果由于与 Nimsoft Robot 的通信错误而导致配置监视服务时出错，那么配置过程可能会由于连接受限而暂停。连接受限通常是由防火墙或其他安全软件造成的，因为此类软件会阻止从 Nimsoft 管理服务器访问系统。要重新供应监视服务，请执行以下步骤：

## 重新供应监视代理程序

1. 转至**设备**菜单，然后选择**监视**。
* 找到要为其配置监视服务的系统。
* 在右侧列的**高级**下拉菜单下，选择**“重新部署所有代理程序”**。
* 在**弹出窗口**页面上选择监视模板。
* 单击**重新部署**。

## 在 Windows 中安装
{: #install-windows}

1. 要将最新版本的 Windows 安装程序下载到设备上以便进行安装，请访问 http://downloads.service.softlayer.com/nimsoft/（您必须已连接到客户 VPN）。
* 以管理员身份运行 Nimsoft Monitoring Robot 文件。

## 在 Linux 中安装
{: #install-linux}

1. 通过客户 VPN 连接到专用网络。
* 将 [32 位 ![外部链接图标](../../icons/launch-glyph.svg "外部链接图标")](http://downloads.service.softlayer.com/nimsoft/NIMSOFT_LINUX_32.tar.gz){: new_window} 或 [64 位 ![外部链接图标](../../icons/launch-glyph.svg "外部链接图标")](http://downloads.service.softlayer.com/nimsoft/NIMSOFT_LINUX_64.tar.gz){: new_window} Linux 安装程序下载到设备上以便进行安装。[Nimsoft 安装程序 ![外部链接图标](../../icons/launch-glyph.svg "外部链接图标")](http://downloads.service.softlayer.com/nimsoft/){: new_window} 上还有 Debian 和 Ubuntu 版本。
* 运行以下命令来完成安装，如果运行 64 位安装，需要将 32 替换为 64：

        $ tar –xzvf NIMSOFT_LINUX_32.tar.gz
        $ cd NIMSOFT_LINUX_32
        $ ./install.sh

## 后续步骤

在您运行安装后，系统会自动完成安装过程。在 Windows 中，会显示一条消息，其中包含安装成功的确认信息，或有关所发生错误的信息。
