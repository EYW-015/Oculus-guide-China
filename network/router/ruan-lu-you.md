# 软路由

{% hint style="success" %}
**爬梯上网终极解决方案，最强大的路由器开源平台之一**
{% endhint %}

{% hint style="warning" %}
软路由需要较强动手能力与学习能力，电脑小白请绕道

如果您选择使用软路由科学上网，则默认您有足够的动手能力与学习能力，网上有大量相关教程，请自行谷歌寻找，本文尾部友链中也有诸多YouTuber大神的频道链接，您可以观看他们的视频学习相关知识
{% endhint %}

## ARM平台

ARM型号推荐

* Nanopi R2S ￥200
  * 入门级软路由首选推荐
* Nanopi R4S ￥380起
* 树莓派4B ￥300起

## X86平台

只要是台电脑就行，不限于Intel / AMD

**可以用家里的旧电脑改装，0成本**\
也可以到TB/闲鱼淘二手矿渣小主机，基本在200-600之间\
要么直接TB买成品软路由，600起价，配置高的例如搭载I7 CPU的成品软路由可以打上2500\
或者捡垃圾收拆机件自己组电脑，组全新电脑也没有问题\
你拿十年前的赛扬也能用，装一台3990X也可以，全看个人需求

{% hint style="warning" %}
此坑深不见底，前期投入不一定大，后期需求增长导致的开销增长极高，慎入
{% endhint %}

## 固件下载

* [恩山论坛X64 / 树莓派固件](https://www.right.com.cn/forum/thread-3777668-1-1.html)
* [各类开发板固件](https://github.com/ruoyizhou/OpenWRT-For-Pi)
* 作者编译的 X64 & R2S 固件下载
  * [openwrt-x64实体机](https://github.com/EYW-015/Oculus-guide-China/releases/download/openwrt-x64/openwrt-x86-64-generic-squashfs-combined-efi.img.gz)&#x20;
    * [openwrt-x64虚拟机](https://github.com/EYW-015/Oculus-guide-China/releases/download/openwrt-x64/openwrt-x86-64-generic-squashfs-combined-efi.vmdk)
  * [openwrt-r2s](https://github.com/EYW-015/Oculus-guide-China/releases/download/openwrt-r2s/openwrt-rockchip-armv8-friendlyarm\_nanopi-r2s-squashfs-sysupgrade.img.gz)

### 自行编译

* [Lean's OpenWrt](https://github.com/coolsnowwolf/lede)

## 电脑临时软路由

找一个空U盘，有1G容量就可以

下载 **x64实体机固件**，解压(打不开去安装 [**Bandizip**](https://cn.bandisoft.com/bandizip/) **** )\
下载刷机工具 [**Win32diskimager**](https://sourceforge.net/projects/win32diskimager/)，打开刷机工具，把解压好的固件拖进去，右边选择你的U盘，点击**`Write`**

刷写完成之后重启电脑，进入bios选择U盘启动\
启动完成之后去把软路由IP改成你自己家的网段\
改IP教程 [https://zhuanlan.zhihu.com/p/55140921](https://zhuanlan.zhihu.com/p/55140921)\
重启电脑，并再次选择U盘启动

打开手机浏览器，进入刚刚设置的IP\
输入密码，进入**`网络` > `接口` > `修改`**\
将**`网关`**和**`DNS`**改成你的主路由IP\
保存应用

进入**`服务` > `SSRP`**，订阅你的节点并启用即可

需要使用软路由的设备\
手动将**`WIFI` / `以太网`**的**`IP设置`**改为**`静态`**，**`网关`**和**`DNS`**设置为软路由的IP\
不用软路由的时候就把IP设置改回**`DHCP`**
