# 电脑热点激活

{% hint style="info" %}
此方案需使用电脑的无线网卡开启热点，如您的电脑没有无线网卡，请使用其他方案
{% endhint %}

{% hint style="warning" %}
使用此方案前需要先开启梯子的TAP模式，并需要你的梯子线路支持UDP转发，否则头显无法更新固件
{% endhint %}

## 热点共享

首先开启你的WIFI热点，然后会在你的网络适配器中多出一个**`本地连接* <数字>`**且描述为**`Microsoft Wi-Fi ...`**的适配器，这是你的**`WIFI热点网络适配器`**

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/clash/clash9.png)

双击**`cfw-tap`**设备\(或者是你的**`Netch适配器`**\)，进入**`共享`**页面，勾选**`允许其他网络用户...`**，在下拉菜单中选择之前开启的名称为 **`本地连接* <数字>`** 的**`WIFI热点适配器`**，如果没有下拉菜单，手动将适配器名称 **`本地连接* <数字>`** 填写进框内，保存确定

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/clash/clash10.png)

{% hint style="info" %}
如果WIFI自动关闭了，再打开就可以了
{% endhint %}

设置完成，将你的头显连接至你的电脑WIFI热点，即可正常连接网络

