# Quest商店无链接

## 介绍

{% hint style="info" %}
Quest商店无法连接是由于没有**UDP转发**导致的
{% endhint %}

首先请检查你使用的**线路**是否支持**UDP转发**，如果线路支持，请检查你的梯子客户端是否支持，路由器用户检查是否开启了**游戏模式**

## NAT / UDP 测试工具

* [最新版本发布页](https://github.com/HMBSbige/NatTypeTester/releases/)

![](https://cdn.jsdelivr.net/gh/eyw015/Oculus-guide-China/quest/udp.png)

其中的Public end可以反映出你的UDP传输有没有经过加速器 / 梯子转发：  
Public end显示的是你当前连接到测试服务器使用的网络IP地址与端口，  
冒号前面（不包含冒号）的是IP地址，将IP地址复制到查询工具中查询，  
IP在线查询：[IPIP.NET](https://www.ipip.net/ip.html) / [ChinaZ站长之家](http://ip.tool.chinaz.com/) / [淘宝IP库](http://ip.taobao.com/)  
如果查询到的位置是你的本地宽带，那么说明UDP是直连，没有生效，  
如果查询到的位置是加速器 / 梯子服务器的所在地，那么说明经过了转发，加速生效  


