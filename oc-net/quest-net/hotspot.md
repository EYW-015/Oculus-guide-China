# 电脑热点激活

{% hint style="info" %}
此方案需使用电脑的**无线网卡**，如台式机没有无线网卡，就去TB花20买一个USB WIFI
{% endhint %}

{% hint style="warning" %}
激活头显需要你的梯子线路支持UDP转发，否则头显无法更新固件
{% endhint %}

## CFW开启TAP模式

{% hint style="info" %}
如果你使用的是Netch，请跳到下方的**Netch部分**
{% endhint %}

首先参照前面的教程设置好你的CFW客户端  
然后在**`General`**菜单中找到**`TAP Device`**选项，点击**`Manage` &gt; `Install`**

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/clash/clash51.png)

进入**`Settings页面` &gt; `Profile Mixin` &gt; `YAML` &gt; `Edit`**

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/clash/clash61.png)

将下面的代码粘贴进去

```yaml
mixin: #object
  dns:
    enable: true
    ipv6: false
    listen: 0.0.0.0:53
    enhanced-mode: redir-host
    nameserver:
    - 119.29.29.29
    - 223.5.5.5
    - 223.6.6.6
```

修改好的配置文件应类似下图格式

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/clash/clash71.png)

点击右下角保存，回到**`General`**页面，将**`Mixin`**开关打开

打开**`控制面板` &gt; `网络和 Internet` &gt; `网络和共享中心` &gt; 左侧`更改适配器设置`**，找到名称为**`cfw-tap`**的适配器，如果显示已启用，说明tap模式成功开启

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/clash/clash8.png)

## Netch开启TAP模式

在Netch的**模式栏**中，拉到最底下，选择**`[TUN/TAP]绕过局域网`**，启动加速

打开**`控制面板` &gt; `网络和 Internet` &gt; `网络和共享中心` &gt; 左侧`更改适配器设置`**，找到名称描述为**`TAP-Windows Adapter V9`**的适配器，如果显示已启用，说明TAP模式成功开启

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/netch/netch4.png)

## 热点共享

首先开启你的WIFI热点，然后会在你的网络适配器中多出一个**`本地连接* <数字>`**且描述为**`Microsoft Wi-Fi ...`**的适配器，这是你的**`WIFI热点网络适配器`**

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/clash/clash9.png)

双击**`cfw-tap`**设备\(或者是你的**`Netch适配器`**\)，进入**`共享`**页面，勾选**`允许其他网络用户...`**，在下拉菜单中选择之前开启的名称为 **`本地连接* <数字>`** 的**`WIFI热点适配器`**，如果没有下拉菜单，先取消**`允许共享`**，保存关闭之后再回来打开

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/clash/clash10.png)

设置完成，将你的头显连接至你的电脑WIFI热点，即可正常连接网络

