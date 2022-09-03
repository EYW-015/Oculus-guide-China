---
description: 科学上网&翻墙
---

# 热点设置

此方案需使用电脑的**无线网卡**，如台式机没有无线网卡，**就去TB花20买一个USB WIFI**，如果**不支持开启系统原生热点**，可以使用网上搜索的免费热点软件进行共享

激活头显需要你的**梯子线路**<mark style="color:red;">**支持UDP转发**</mark>，否则头显无法更新固件‌

{% hint style="success" %}
<mark style="color:red;">**########################**</mark>

远程激活请联系QQ：<mark style="color:blue;">**3030217730**</mark>

<mark style="color:red;">**########################**</mark>
{% endhint %}

## 热点共享 <a href="#re-dian-gong-xiang" id="re-dian-gong-xiang"></a>

首先启用梯子软件的虚拟网卡

然后开启你的WIFI热点，然后会在你的网络适配器中多出一个**`本地连接* <数字>`**且描述为**`Microsoft Wi-Fi ...`**的适配器，这是你的**`WIFI热点网络适配器`**

![](https://fastly.jsdelivr.net/gh/EYW-015/Oculus-guide-China/img/clash/clash9.png)

右键**`虚拟网卡设备`** **>** **`属性`** **>** **`共享`**，勾选**`允许其他网络用户...`**，在下拉菜单中选择之前开启的名称为 **`本地连接* <数字>`** 的**`WIFI热点适配器`**，如果没有下拉菜单，先取消**`允许共享`**，保存关闭之后再回来打开​

![](https://fastly.jsdelivr.net/gh/EYW-015/Oculus-guide-China/img/clash/clash10.png)

设置完成，将你的头显连接至你的电脑WIFI热点，即可正常连接网络

### USB热点

如果你用的USB WiFi已经自带了IP，共享时提示改为自动获取，那就打开热点适配器的**属性 > Internet协议版本4 > 改为自动获取**，再进行共享
