# 启用TAP模式

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

在Netch的**模式**选项中，拉到最底下，选择**`[TUN/TAP]绕过局域网`**，启动加速

打开**`控制面板` &gt; `网络和 Internet` &gt; `网络和共享中心` &gt; 左侧`更改适配器设置`**，找到名称为**`以太网 <数字>`**且描述为**`TAP-Windows ...`**的适配器，如果显示已启用，说明tap模式成功开启

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/netch/netch4.png)

