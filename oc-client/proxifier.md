# Proxifier+梯子客户端

## 梯子开启LAN连接

### Clash

在General菜单中，将Allow LAN选项调至开启状态

### SS

右键托盘区图标，**允许来自LAN的链接**，确认其为开启状态

## 简介

* [Proxifier官网](https://www.proxifier.com/)

先至官网下载Proxifier并安装，首次运行会出现激活提示，可以选择31天试用或自行激活，运行之后会出现如下界面，并且托盘区会出现一个新的灰色方框图标，那就是Proxifier

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/proxifier/px1.png)

## Proxifier设置

首先下载这个[**配置文件**](https://cdn.jsdelivr.net/gh/eyw015/Oculus-guide-China/proxifier/OculusConfig.ppx)，双击打开它，在弹出窗口中点击OK

然后点击菜单栏的第一个按钮

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/proxifier/px2.png)

双击第一个条目

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/proxifier/px3.png)

将你的代理软件端口输入到**Port**栏中，点击**OK &gt; OK**

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/proxifier/px4.png)

{% hint style="info" %}
代理软件端口为**允许局域网链接的端口**，Clash默认为7890，SS默认为1080
{% endhint %}

PX设置完毕，运行OC客户端，PX界面应如下图出现大量OC链接，说明OC成功联网

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/proxifier/px5.png)

{% hint style="info" %}
如PX中未出现OC链接，请尝试在**任务管理器 &gt; 服务**中，找到并**重启OVRService**
{% endhint %}

