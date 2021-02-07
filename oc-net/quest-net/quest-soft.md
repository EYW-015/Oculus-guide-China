# 电脑代理联网

{% hint style="info" %}
此方案不可用于激活Quest设备，仅适合激活之后的联网使用
{% endhint %}

## 查看电脑IP

{% page-ref page="../../proxy/" %}

首先确认你的VR设备与你的电脑连接至同一个WIFI

然后查看你电脑的IP，系统托盘点击**`网络` &gt; `属性`**  
如果你的电脑使用的是**有线连接**，那么进入以太网详细信息寻找IP

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/wifi/wifi1.png)

下拉至详细属性，寻找你的**`IPv4 地址`**

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/wifi/wifi2.png)

## Quest联网

连接WIFI**输入密码的时候**打开下方**高级设置**

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/quest/wifi1.jpg)

将**代理**设置为**手动**

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/quest/Qwifi2.jpg)

将主机名设置为你的**`电脑IP地址`**，代理服务器端口设置为你的**`梯子客户端端口`**，然后保存即可正常使用

{% hint style="info" %}
端口为你梯子客户端开启的**局域网\(LAN\)代理端口**，Clash默认**`7890`**，SS默认**`1080`**
{% endhint %}

