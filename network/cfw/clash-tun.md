# CFW TUN 模式

{% hint style="danger" %}
请**至GitHub**下载原作者发布的最新版本，请勿下载机场发布的**旧版/中文版**等来路不明的版本，所造成的风险与问题自行承担
{% endhint %}

## CFW TUN模式

{% hint style="info" %}
对于不遵循系统代理的软件，开启 TUN 模式将在电脑设置一个虚拟网卡，接管其流量并交由 CFW 处理，在 Windows 中，TUN 模式性能比 TAP 模式好
{% endhint %}

### 安装TUN驱动

在**`General`**菜单中找到**`Service Mode`**选项，点击**`Manage` > `Install`**

安装成功后右侧**小地球应变为绿色**

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/img/clash/clash\_tun\_install.png)

### 设置并开启CFW TUN

点击**`TUN Mode` 旁边的齿轮 > `Reset` > `Save`**

![](../../.gitbook/assets/image.png)![](<../../.gitbook/assets/image (1).png>)

{% hint style="info" %}
图中的配置是作者改过的，**点完reset就别动了，不要照着改**
{% endhint %}

最后将**`TUN Mode`**选项右侧的开关打开即可

打开**`控制面板` > `网络和 Internet` > `网络和共享中心` > 左侧`更改适配器设置`**，找到名称为**`Clash`**且描述为**`Clash Tunnel`**的适配器，如果显示已启用，说明TUN模式成功开启

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/img/clash/clash\_tun\_adp.png)

## 热点共享网络

{% content-ref url="../../quest-guide/quest-net.md" %}
[quest-net.md](../../quest-guide/quest-net.md)
{% endcontent-ref %}
