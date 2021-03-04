# 电脑热点激活

## 上一步

{% page-ref page="../../proxy/netch.md" %}

{% page-ref page="../../proxy/cfw.md" %}

{% hint style="info" %}
此方案需使用电脑的**无线网卡**，如台式机没有无线网卡，**就去TB花20买一个USB WIFI**，如果**不支持开启系统原生热点**，可以使用网上搜索的免费热点软件进行共享
{% endhint %}

{% hint style="warning" %}
激活头显需要你的**梯子线路支持UDP转发**，否则头显无法更新固件
{% endhint %}

## Netch开启TAP模式

点击**`设置` &gt; `TUN/TAP` &gt; `使用自定义DNS`打钩 &gt; DNS填写`119.29.29.29` &gt; `保存`**

在Netch的**模式栏**中，拉到最底下，选择**`[TUN/TAP]绕过局域网`**，启动加速

打开**`控制面板` &gt; `网络和 Internet` &gt; `网络和共享中心` &gt; 左侧`更改适配器设置`**，找到名称描述为**`TAP-Windows Adapter V9`**的适配器，如果显示已启用，说明TAP模式成功开启

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/img/netch/netch4.png)

{% hint style="info" %}
如果网络一直显示**正在识别**，那关闭加速，在**`选项`**中**`卸载TUN/TAP驱动`**并重新开启加速
{% endhint %}

## CFW开启TUN模式

首先参照前面的教程设置好你的CFW客户端  
然后在**`General`**菜单中找到**`Service Mode`**选项，点击**`Manage` &gt; `Install`**

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/img/clash/clash_tun_install.png)

进入**`Settings页面` &gt; `Profile Mixin` &gt; `YAML` &gt; `Edit`**

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/img/clash/clash61.png)

将下面的代码粘贴进去

```yaml
mixin: # object
  dns:
    enable: true
    enhanced-mode: redir-host
    nameserver:
    - 119.29.29.29
    - 223.5.5.5
    - 223.6.6.6
  tun:
    enable: true
    stack: gvisor
    dns-hijack:
    - 198.18.0.2:53
    macOS-auto-route: true
    macOS-auto-detect-interface: true
```

修改好的配置文件应类似下图格式

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/img/clash/clash_mixin.png)

点击右下角保存，回到**`General`**页面，将**`Mixin`**开关打开

打开**`控制面板` &gt; `网络和 Internet` &gt; `网络和共享中心` &gt; 左侧`更改适配器设置`**，找到名称为**`Clash`**且描述为**`Clash Tunnel`**的适配器，如果显示已启用，说明tap模式成功开启

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/img/clash/clash_tun_adp.png)

## 热点共享

首先开启你的WIFI热点，然后会在你的网络适配器中多出一个**`本地连接* <数字>`**且描述为**`Microsoft Wi-Fi ...`**的适配器，这是你的**`WIFI热点网络适配器`**

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/img/clash/clash9.png)

右键**`Netch适配器`**\(或者是你的**`clash TUN设备`**\) **&gt; `属性` &gt; `共享`**，勾选**`允许其他网络用户...`**，在下拉菜单中选择之前开启的名称为 **`本地连接* <数字>`** 的**`WIFI热点适配器`**，如果没有下拉菜单，先取消**`允许共享`**，保存关闭之后再回来打开

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/img/clash/clash10.png)

设置完成，将你的头显连接至你的电脑WIFI热点，即可正常连接网络

