# Quest联网&激活

此方案需使用电脑的**无线网卡**，如台式机没有无线网卡，**就去TB花20买一个USB WIFI**，如果**不支持开启系统原生热点**，可以使用网上搜索的免费热点软件进行共享

激活头显需要你的**梯子线路支持UDP转发**，否则头显无法更新固件‌

{% hint style="success" %}
不仅限于激活，也可以作为日常联网使用
{% endhint %}

## 热点共享 <a href="#re-dian-gong-xiang" id="re-dian-gong-xiang"></a>

先打开Clash的TUN模式

{% content-ref url="../network/cfw/clash-tun.md" %}
[clash-tun.md](../network/cfw/clash-tun.md)
{% endcontent-ref %}

然后开启你的WIFI热点，然后会在你的网络适配器中多出一个**`本地连接* <数字>`**且描述为**`Microsoft Wi-Fi ...`**的适配器，这是你的**`WIFI热点网络适配器`**

​![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/img/clash/clash9.png)‌

右键**`clash TUN设备`** **>** **`属性`** **>** **`共享`**，勾选**`允许其他网络用户...`**，在下拉菜单中选择之前开启的名称为 **`本地连接* <数字>`** 的**`WIFI热点适配器`**，如果没有下拉菜单，先取消**`允许共享`**，保存关闭之后再回来打开​

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/img/clash/clash10.png)‌

设置完成，将你的头显连接至你的电脑WIFI热点，即可正常连接网络
