# Oculus PC客户端

## 更改安装路径

Oculus客户端默认安装路径是**C盘**，如果想安装到其他盘符，可按以下步骤操作

{% hint style="info" %}
确认目标硬盘有足够可用空间，且硬盘为NTFS格式分区，**不建议安装至机械硬盘内**
{% endhint %}

以**`管理员权限`**运行**`CMD`**，输入以下代码，回车

```
<你的OC安装包路径>\OculusSetup.exe /drive=<目标安装盘符>
```

#### 范例

```
C:\Users\USERNAME\Downloads\OculusSetup.exe /drive=D
```

## OC无法联网 / 登录

由于Oculus客户端的问题，**无法使用系统代理**，开了**全局模式**也无法使用梯子的流量

梯子只开系统代理的话就是个摆设，OC客户端仍然无法连网，便会出现诸如**卡在登录界面无限转圈**，或是**FB认证失败**等情况

于是就需要开启**Clash的TUN模式**给OC客户端联网，或用到**Proxifier**进行应用代理

{% content-ref url="../../network/cfw/clash-tun.md" %}
[clash-tun.md](../../network/cfw/clash-tun.md)
{% endcontent-ref %}

### Hosts

如果你baidu了Hosts方案，并且自行修改了Hosts文件，那么请将你的Hosts文件规则全部删除，可使用 火绒 或 Dism++ 工具箱清空Hosts文件内容，如果没改过，那就不用管了

{% hint style="info" %}
**花钱爬梯子 + 改Hosts = **<mark style="color:red;">**钱打水漂**</mark>

**就好比买了个3090回来，你把显示器插核显输出**
{% endhint %}

#### 原理讲解

国内会将Oculus相关域名解析至**美国/法国的Facebook CDN服务器**，无法进行直连，网上改hosts的方案是将此地址替换至**未被屏蔽的澳大利亚CDN服务器**进行链接

但是由于Oculus客户端**无法使用系统代理**，所以你<mark style="color:red;">**改了hosts也是直连，梯子在那看戏，钱打水漂！！！**</mark>
