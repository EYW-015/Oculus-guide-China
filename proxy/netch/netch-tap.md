# Netch TAP模式

## Netch TAP/TUN

{% hint style="info" %}
对于不遵循系统代理的软件，开启 TUN/TAP 模式将在电脑设置一个虚拟网卡，接管其流量并交由 Netch 处理，此模式可以代理大部分应用流量
{% endhint %}

在模式中选择列表最底部的**`[TUN/TAP]绕过局域网和中国大陆`**模式即可启用TAP设备

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/img/netch/netch_mode.png)

打开**`控制面板` &gt; `网络和 Internet` &gt; `网络和共享中心` &gt; 左侧`更改适配器设置`**，找到名称描述为**`TAP-Windows Adapter V9`**的适配器，如果显示已启用，说明TAP模式成功开启

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/img/netch/netch4.png)

{% hint style="info" %}
如果TAP设备无法正常使用，先停用加速，在**`选项`**中**`卸载TUN/TAP驱动`**，再重新启用
{% endhint %}

