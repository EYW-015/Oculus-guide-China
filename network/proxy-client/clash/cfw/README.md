# Clash for Windows

## 简介

{% hint style="danger" %}
请**至GitHub**下载原作者发布的最新版本，请勿下载机场发布的旧版/中文版等来路不明的版本，所造成的风险与问题自行承担
{% endhint %}

* [项目主页](https://github.com/Fndroid/clash\_for\_windows\_pkg)

Clash for Windows (以下简称CFW) 是一个Windows平台的Clash图形界面客户端，支持多种代理协议，SS，VMess，Trojan，Socks5等

{% hint style="success" %}
Clash是最好的跨平台代理客户端之一，支持多种协议 / UDP转发 / TAP模式，以及高度自定义的策略组分流规则
{% endhint %}

{% hint style="info" %}
如果使用的机场支持Clash托管，您可以使用此客户端，如果不支持该格式托管仍想使用Clash，请自行寻找配置转换方式
{% endhint %}

## 下载使用

* [最新版本发布页](https://github.com/Fndroid/clash\_for\_windows\_pkg/releases)

下载对应版本之后安装运行，托盘区会出现一个深蓝色的小猫咪图标![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/img/clash/clash1.png)，这时Clash就启动成功了

{% hint style="info" %}
推荐使用exe安装包的方式使用该软件
{% endhint %}

## 界面介绍

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/img/clash/clash2.png)

## 托管订阅

在机场首页寻找Clash托管订阅地址，将其复制，选择左侧**`Profiles`**，在上部粘贴托管地址并点击**`Download`**，如果下部出现了新的配置选项，那么就订阅成功了

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/img/clash/clash3.png)

{% hint style="info" %}
如果订阅失败，请尝试手动下载并导入配置
{% endhint %}

## 开启系统代理

回到**`General`**页面，将**`System Proxy`**选项打开，托盘区图标变为黄色即可正常使用

### 选择线路

进入左侧**`Proxies`**页面，根据配置自行选择需要的线路

![](https://cdn.jsdelivr.net/gh/EYW-015/Oculus-guide-China/img/clash/clash4.png)

{% hint style="info" %}
由于各个机场使用的配置文件不一样，分流规则也不一样，详细的分流策略设置请咨询各家机场，阅读[**CFW说明文档**](https://docs.cfw.lbyczf.com)，或自行谷歌查询
{% endhint %}

## TUN模式

{% content-ref url="clash-tun.md" %}
[clash-tun.md](clash-tun.md)
{% endcontent-ref %}

{% hint style="info" %}
对于不遵循系统代理的软件，开启 TUN 模式将在电脑设置一个虚拟网卡，接管其流量并交由 CFW 处理，在 Windows 中，TUN 模式性能比 TAP 模式好
{% endhint %}

## **下一步**

### **Oculus PC 客户端联网**

{% content-ref url="../../../../quest-guide/oc-client/proxifier.md" %}
[proxifier.md](../../../../quest-guide/oc-client/proxifier.md)
{% endcontent-ref %}

### **Quest激活**

{% content-ref url="broken-reference" %}
[Broken link](broken-reference)
{% endcontent-ref %}
