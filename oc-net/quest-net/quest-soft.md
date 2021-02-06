# 软件激活

{% hint style="warning" %}
使用此方案前需要先开启梯子的TAP模式，并需要你的梯子线路支持UDP转发，否则头显无法更新固件
{% endhint %}

## 查看电脑IP

首先确认你的VR设备与你的电脑连接至同一个WIFI

然后查看你电脑的IP，系统托盘点击**`网络` &gt; `属性`**  
如果你的电脑使用的是**有线连接**，那么进入以太网详细信息寻找IP

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/wifi/wifi1.png)

下拉至详细属性，寻找你的**`电脑 IPv4 地址`**

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/wifi/wifi2.png)

记住你的**`电脑IP地址`**

## Quest联网

连接WIFI**输入密码的时候**打开下方**`高级设置`**

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/quest/wifi1.jpg)

将**`IP设置`**改为**`静态`**  
将**`IP地址`**的**`前3段`**填写为与你的**`电脑IP地址前3段`**一致，**`第4段`**改一个数，例如**`235`**  
例如我电脑是**`192.168.60.199`**，这里就填写**`192.168.60.235`**

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/quest/wifi2.jpg)

将**`网关`**设置为你的**`电脑IP地址`**  
**`DNS1`**设置为**`电脑IP地址前3段`**，**第4段**设置为**`1`**  
例如我的是**`192.168.60.1`**  
剩余不变

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/quest/wifi3.jpg)

连接至WIFI，即可正常激活更新

