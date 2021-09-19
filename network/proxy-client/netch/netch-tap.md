# Netch TUN模式

## Netch TUN

{% hint style="info" %}
对于不遵循系统代理的软件，开启 TUN/TAP 模式将在电脑设置一个虚拟网卡，接管其流量并交由 Netch 处理，此模式可以代理大部分应用流量
{% endhint %}

在模式中选择列表中的**`[3] Bypass Lan and China`**模式即可启用TUN模式

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/img/netch/netch_mode2.png)

打开**`控制面板` &gt; `网络和 Internet` &gt; `网络和共享中心` &gt; 左侧`更改适配器设置`**，找到名称为**`aioCloud(WireGuard Tunnel)`**的适配器，如果已启用，说明TUN模式成功开启

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/img/netch/netch_adp.png)

{% hint style="info" %}
如果TUN设备无法正常使用，先停用加速，在**`选项`**中**`卸载 NF 服务`**，再重新启用
{% endhint %}

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/img/netch/netch_uninstall_nf.png)

## 热点共享网络

{% page-ref page="../../../quest-guide/quest-net.md" %}

