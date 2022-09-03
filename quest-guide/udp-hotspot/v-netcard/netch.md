# Netch

## 简介

* [项目主页](https://github.com/NetchX/Netch)

Netch 是一款 Windows 平台的开源游戏加速工具

{% hint style="warning" %}
关于程序无法安装/启动的问题，建议您安装 .NET 5.0 Desktop Runtime x64 之后再尝试使用。请注意，您需要安装的是 64 位的版本

Download link - 下载链接 [https://dotnet.microsoft.com/download/dotnet/thank-you/runtime-desktop-5.0.7-windows-x64-installer](https://dotnet.microsoft.com/download/dotnet/thank-you/runtime-desktop-5.0.7-windows-x64-installer)
{% endhint %}

## 下载使用

* [最新版本发布页](https://github.com/NetchX/Netch/releases/latest/)

{% hint style="info" %}
请去GitHub发布页下载最新版本，如遇版本设置选项与本教程不一致的情况，请自行机智
{% endhint %}

下载最新版本的压缩包之后，解压至**桌面以外的任意目录**，运行Netch客户端会看到如下界面

![](https://fastly.jsdelivr.net/gh/EYW-015/Oculus-guide-China/img/netch/netch1.png)

## 配置导入

先在机场找到你的可订阅地址，复制你的订阅地址

{% hint style="info" %}
Netch支持以下协议：SS / VMess / Socks5 / SSR / Trojan
{% endhint %}

在Netch主界面点击**`订阅` > `管理订阅链接`**，打开如下界面

![](https://fastly.jsdelivr.net/gh/EYW-015/Oculus-guide-China/img/netch/netch2.png)

**`备注`**栏填写任意名称，链接栏将你的订阅地址粘贴进去，点击**`添加`**\
****点击**`订阅` > `从订阅链接更新服务器`**，如Windows提示更新成功即可

## 启动加速

在模式中选择列表中的**`[3] Bypass Lan and China`**模式即可启用TUN模式

![](https://fastly.jsdelivr.net/gh/EYW-015/Oculus-guide-China/img/netch/netch\_mode2.png)

打开**`控制面板` > `网络和 Internet` > `网络和共享中心` > 左侧`更改适配器设置`**，找到名称为**`aioCloud(WireGuard Tunnel)`**的适配器，如果已启用，说明TUN模式成功开启

![](https://fastly.jsdelivr.net/gh/EYW-015/Oculus-guide-China/img/netch/netch\_adp.png)

{% hint style="info" %}
如果TUN设备无法正常使用，先停用加速，在**`选项`**中**`卸载 NF 服务`**，再重新启用
{% endhint %}

{% hint style="info" %}
更加详细的使用说明，请查看[**官方说明文档**](https://github.com/NetchX/Netch/blob/master/docs/Quickstart.zh-CN.md)
{% endhint %}
