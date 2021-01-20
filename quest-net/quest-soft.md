# 软件激活

{% hint style="info" %}
请先参阅前方**梯子客户端**页面
{% endhint %}

{% hint style="warning" %}
SS客户端不支持UDP转发，不一定适用于Quest激活，如激活失败请尝试其他方案
{% endhint %}

{% page-ref page="../proxy-client/" %}

## 查看电脑IP

首先确认你的VR设备与你的电脑连接至同一个WIFI

然后查看你电脑的IP，系统托盘点击**网络 &gt; 属性**  
如果你的电脑使用的是**有线连接**，那么进入以太网详细信息寻找IP

\*\*\*\*![wifi1](https://cdn.jsdelivr.net/gh/eyw015/Oculus-guide-China/wifi/wifi1.png)

下拉至详细属性，寻找你的**IPv4 地址**

![](https://cdn.jsdelivr.net/gh/eyw015/Oculus-guide-China/wifi/wifi2.png)

## Quest联网

连接上WIFI之后**修改**WIFI

![wifi1](https://cdn.jsdelivr.net/gh/eyw015/Oculus-guide-China/quest/Qwifi1.jpg)

将**代理**设置为**手动**

![wifi2](https://cdn.jsdelivr.net/gh/eyw015/Oculus-guide-China/quest/Qwifi2.jpg)

将主机名设置为你的**电脑IP地址**，代理服务器端口设置为你的**梯子客户端端口**，然后保存即可正常使用

{% hint style="info" %}
端口为你梯子客户端开启的**局域网\(LAN\)代理端口**，Clash默认7890，SS默认1080
{% endhint %}

