# 电脑热点激活

Oculus Quest 2可以直接通过微信从亚马逊官方小程序购买，海外直邮，没有中间商赚差价，方便又实惠，微信扫码即可进入：

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/quest/amz1.png)![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/quest/amz2.png)

如果缺货可以多关注一下，最近是隔几天有货隔几天没货，若价格离谱说明缺货

{% hint style="info" %}
此方案需使用电脑的无线网卡开启热点，并使用 CFW / SStap / Netch 开启TAP模式进行网络共享，如您的电脑没有无线网卡，或无法使用TAP设备，请使用其他方案
{% endhint %}

## 开启TAP模式

{% hint style="info" %}
如果你使用的是 SStap / Netch，你可以直接跳过此步骤
{% endhint %}

首先参照前面的教程设置好你的CFW客户端，在**`General`**菜单中找到**`TAP Device`**选项，点击**`Manage` &gt; `Install`**

进入**Profile**菜单，找到你的配置，点击最左边的按钮

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/clash/clash5.png)

此时会提示选择打开方式，在**`更多应用`**中选择**`记事本`**

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/clash/clash6.png)

找到一行`proxies:`在它上方加一个空行，复制下面的代码，将其粘贴进去，保存退出

{% hint style="info" %}
找不到请按 **Ctrl + F** 寻找
{% endhint %}

```text
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

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/clash/clash7.png)

打开**`控制面板` &gt; `网络和 Internet` &gt; `网络和共享中心` &gt; 左侧`更改适配器设置`**，找到名称为**`cfw-tap`**的适配器，如果显示已启用，说明tap模式成功开启

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/clash/clash8.png)

## 热点共享

首先开启你的WIFI热点，然后会在你的网络适配器中多出一个**`本地连接* <数字>`**，这是你的**`WIFI热点网络适配器`**

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/clash/clash9.png)

双击**`cfw-tap`**设备\(或者是你的SStap适配器\)，进入**`共享`**页面，勾选**`允许其他网络用户XXX`**，在下拉菜单中选择之前开启的名称为 **`本地连接* <数字>`** 的**`WIFI热点适配器`**，如果没有下拉菜单，手动将适配器名称 **`本地连接* <数字>`** 填写进框内，保存确定

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/clash/clash10.png)

{% hint style="info" %}
如果WIFI自动关闭了，再打开就可以了
{% endhint %}

设置完成，将你的头显连接至你的WIFI热点，即可正常连接网络

