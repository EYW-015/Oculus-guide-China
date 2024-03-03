# Proxifier+代理客户端

## 梯子开启LAN连接

### CFW

在**`General`**页面中将**`Allow LAN`**选项打开，默认端口为**`7890`**

## 简介

* [Proxifier官网](https://www.proxifier.com/)

Proxifier是一款代理软件，支持自定义规则分流，可以使用进程代理，地址代理\
配合无分流 / 低级分流功能的梯子客户端，也可以实现类似 Clash / Netch 那样的高级分流策略

先至官网下载Proxifier并安装，首次运行会出现激活提示，可以选择31天试用或自行激活(懂得都懂)

运行之后会出现如下界面，并且托盘区会出现一个新的灰色方框图标，那就是Proxifier

![](https://fastly.jsdelivr.net/gh/EYW-015/Oculus-guide-China/img/proxifier/px1.png)

## Proxifier设置

首先下载这个<mark style="color:purple;">**配置文件**</mark>，双击打开它，在弹出窗口中点击**`OK`**

{% file src="../../.gitbook/assets/Oculus_conf.ppx" %}

然后点击菜单栏的第一个按钮

![](https://fastly.jsdelivr.net/gh/EYW-015/Oculus-guide-China/img/proxifier/px2.png)

双击第一个条目

![](https://fastly.jsdelivr.net/gh/EYW-015/Oculus-guide-China/img/proxifier/px3.png)

将你的代理软件端口输入到**`Port`**栏中，点击**`OK` > `OK`**

![](https://fastly.jsdelivr.net/gh/EYW-015/Oculus-guide-China/img/proxifier/px4.png)

{% hint style="info" %}
代理软件端口为**允许局域网链接的端口**，Clash默认为**`7890`**，SS默认为**`1080`**
{% endhint %}

PX设置完毕，运行OC客户端，PX界面应如下图出现大量OC链接，说明OC成功联网

![](https://fastly.jsdelivr.net/gh/EYW-015/Oculus-guide-China/img/proxifier/px5.png)

{% hint style="info" %}
如PX中未出现OC链接，请尝试在**`任务管理器` > `服务`**中，找到并**重启`OVRService`**
{% endhint %}
